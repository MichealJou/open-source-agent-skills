---
name: hutool
description: 使用或审查 Java Hutool 字符串、集合、日期、Bean 等能力，核对版本和边界并避免重复工具。
---

# Hutool

先核对实际依赖版本、团队工具选择约定和已有实现。选择方法前确认空值、异常、类型和数据语义；不要为工具复用绕过项目既有网络、安全、缓存或序列化链路。

- 字符串：查 `StrUtil` / `CharSequenceUtil`，区分 `isBlank` 与 `isEmpty` 的空白字符行为。
- 集合：查 `CollUtil` 等现有能力，确认 null、顺序、重复元素及返回集合的可变性；数据库过滤和分页仍应在正确的数据源完成。
- 日期：查 `DateUtil`；明确时区、格式、精度和跨天口径。5.8.46 的 `betweenDay(begin, end, true)` 会先归一到日期起始，不能未经验证替代其他时间计算。
- Bean：按项目约定优先既有映射方式；`BeanUtil.copyProperties` 使用前核对 null、覆盖范围、嵌套对象和 `CopyOptions`，不要假设深拷贝。
- 真实业务错误保留原异常契约；新增依赖或变更外部请求、加密配置需遵循当前项目及用户要求。

官方：[Hutool](https://github.com/chinabugotech/hutool)、[API 文档](https://plus.hutool.cn/apidocs/)。官网当前文档版本可能与项目不同。

## 与 Feilong、Guava 的选择顺序

先复用项目现有能力。模块已引入 Feilong 且语义满足时，判空、判零及内部必填断言先查 Feilong `Validator` / `Validate`；Feilong 不满足时再选 Hutool。要保留空格作为有效值时用 `StrUtil.isEmpty`，不能用会把空白当空的 Feilong 文本判空。其他字符串、集合、日期和文件操作优先核对已有 Hutool；Guava 不可变集合用于确需不可变语义的场景。不得为套用优先级改变业务行为或新增依赖。

## 什么时候用，怎么用

先查现有依赖和工具约定。以下按 5.8.46 核对，选择方法前确认空值和返回类型。

| 场景 | 选择 | 注意 |
| --- | --- | --- |
| 文本缺失或只有空白 | 先查 Feilong `Validator.isNullOrEmpty`；需要 Hutool 时 `StrUtil.isBlank(value)` | 先核对特殊空白字符语义；`isEmpty` 对空格返回 false。 |
| 集合为空时跳过处理 | 先查 Feilong `Validator.isNullOrEmpty(items)`；需要 Hutool 时 `CollUtil.isEmpty(items)` | null 也视为空；不应把空集合误认为查询失败。 |
| 按自然日计算间隔 | `DateUtil.betweenDay(start, end, true)` | 该版本先归一到日开始；核对时区、起止顺序及业务口径。 |
| 同名属性复制 | `BeanUtil.copyProperties(source, target)` | 检查覆盖和 null 策略；不要当深拷贝，也不要绕过项目已有 Mapper。 |

```java
if (StrUtil.isEmpty(name)) {
    return;
}
```

这里需要保留空格，因此使用 `StrUtil.isEmpty`；导入 `cn.hutool.core.util.StrUtil`。网络、加密、序列化先复用项目统一设施，不因库提供 API 而替换。

## 方法用途与优先级

按场景读取 [方法用途与选择](references/selection-guide.md) 和 [常用方法中文说明](references/usage-extended.md)，先核对已有项目能力、业务语义和当前依赖版本。未覆盖的方法继续查版本索引、源码与官方文档，不根据名称猜测。

## 查找全部方法

查看本技能的 [公开 API 索引](references/API-INDEX.md)，按包或名称定位方法与重载；调用前再查官方文档和项目实际版本。索引记录声明，不等于逐项解释、使用建议或兼容性保证；注意继承方法与索引范围。

## 源码方法说明

查看 [固定版本源码说明索引](references/source-notes/README.md) 按类和重载检索上游方法摘要；索引明确标记未翻译与无注释项，具体场景和优先级仍以本技能及项目规范为准。
