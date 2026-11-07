---
name: feilong
description: 使用或审查 Java Feilong 工具库，处理判空、判零、断言与集合边界，避免重复实现和语义改变。
---

# Feilong

先检查项目已有实现、依赖版本和团队约定，再选择工具；不要为了使用库添加重复抽象。适用范围以当前模块实际依赖和源码为准。

- `Validator.isNullOrEmpty` / `isNotNullOrEmpty` 可用于支持的对象判空。4.5.1 对字符序列会识别空白及特殊空格，其他普通对象不按内部属性判断。
- `isNullOrZero` / `isNotNullOrZero` 将 null 和零一起处理，使用前确认业务上可以合并；不要将负数视作零。
- `isAnyNullOrEmpty` / `isAllNullOrEmpty` 在 4.5.1 的空参数数组上分别返回 false / true；核对调用意图。
- `Validate.notNull`、`notEmpty`、`notBlank`、`isTrue` 用于断言。4.5.1 的 `notEmpty(CharSequence)` 判断长度，`notBlank` 还判断空白；null 与无效内容的异常类型不同，公开重载需要消息参数。
- 不把标准断言异常直接当成项目业务异常；保留现有错误码、国际化和调用契约。变更前核对源码、调用方和测试。

官方源码：[ifeilong/feilong](https://github.com/ifeilong/feilong)。版本差异以实际依赖源码为准。

## 与 Hutool、Guava 的选择顺序

先复用项目已有业务校验；在模块已引入且语义符合时，判空、判非空、判零和内部必填断言先查 Feilong `Validator` / `Validate`。Feilong 不满足所需语义时查 Hutool，再考虑现有其他工具或 JDK；不为执行顺序新增依赖，不以工具断言替代业务错误码。

| 业务意图 | 优先选择 | 关键区别 |
| --- | --- | --- |
| 文本的 null、空串、空白都算空 | `Validator.isNullOrEmpty(text)` | 4.5.1 按其空白字符规则判断；特殊字符先验证。 |
| 只把 null 和空串当空，空格有效 | Hutool `StrUtil.isEmpty(text)` | Feilong 文本判空会把空白当空，不能直接替代。 |
| 集合、Map 或数组为 null 或长度为零 | `Validator.isNullOrEmpty(value)` | 检查容器是否有元素，不递归检查元素。 |
| 仅判断普通对象是否为 null | `value == null` | Feilong 不检查普通对象内部属性；简单 null 判断保持直接。 |
| 数值为 null 或零都视为缺失 | `Validator.isNullOrZero(number)` | 只有业务明确合并 null 和零时才用。 |
| 所有或任一参数为空 | `isAllNullOrEmpty` / `isAnyNullOrEmpty` | 注意空参数分别返回 true / false。 |
| 参数无效属于内部编程错误 | `Validate.notNull` / `notEmpty` / `notBlank` / `isTrue` | 先核对空白规则、异常类型和消息。 |
| 业务参数校验失败 | 项目统一校验、业务异常和错误码 | 不直接替换成工具库的运行时异常。 |

其他字符串、集合、日期、文件操作先查项目已有能力和 Hutool；Guava 优先用于其不可变集合等实际适用能力。对象转换遵循项目已有 Mapper，查询遵循项目 Service 与数据库框架。优先级只在功能和行为等价时适用。

## 什么时候用，怎么用

先检查模块是否已有依赖。以下按 4.5.1 核对，其他版本查源码。

| 场景 | 选择 | 注意 |
| --- | --- | --- |
| 按库定义判断对象或文本是否为空 | `Validator.isNullOrEmpty(value)` | 字符序列的空白也算空；普通对象不会检查其字段。 |
| 多个参数中任一个为空 | `Validator.isAnyNullOrEmpty(a, b)` | 空参数数组返回 false；全部为空用 `isAllNullOrEmpty`，空数组返回 true。 |
| null 与数值零等价 | `Validator.isNullOrZero(number)` | null、0 被合并；负数不是零。 |
| 内部参数无效应立即失败 | `Validate.notBlank(value, "name is required")` | 有消息参数；null 和空白可能抛不同异常。业务异常、错误码沿用项目约定。 |

```java
if (Validator.isNullOrEmpty(name)) {
    return;
}
Validate.notBlank(name, "name must not be blank");
```

这里第一段适合空值无需处理的流程；第二段适合必须拒绝无效值的边界，不必在同一条路径重复使用。导入 `com.feilong.core.Validator` 和 `com.feilong.core.Validate`。断言消息格式按该版本的 `String.format` 风格使用 `%s`，不使用日志占位符 `{}`。

## 方法用途与优先级

按场景读取 [方法用途与选择](references/selection-guide.md) 和 [常用方法中文说明](references/usage-extended.md)，先核对已有项目能力、业务语义和当前依赖版本。未覆盖的方法继续查版本索引、源码与官方文档，不根据名称猜测。

## 查找全部方法

查看本技能的 [公开 API 索引](references/API-INDEX.md)，按包或名称定位方法与重载；调用前再查官方文档和项目实际版本。索引记录声明，不等于逐项解释、使用建议或兼容性保证；注意继承方法与索引范围。

## 源码方法说明

查看 [固定版本源码说明索引](references/source-notes/README.md) 按类和重载检索上游方法摘要；索引明确标记未翻译与无注释项，具体场景和优先级仍以本技能及项目规范为准。
