---
name: guava
description: 使用或审查 Google Guava 的前置条件、字符串和集合能力，核对异常及数据语义。
---

# Guava

先确认项目现有依赖和工具约定。按任务查 `Preconditions`、`Strings`、`MoreObjects` 和不可变集合，不新增一层等价工具。

- `Preconditions` 抛标准运行时异常；使用前确认异常类型、消息和现有业务错误契约。
- `Strings` 的空串与 null 处理不自动等价空白判断。
- 不可变集合的 null、重复元素、顺序和可修改性按具体方法核对；避免为简单转换复制大型集合。
- 缓存、并发和线程相关能力先查项目现有统一设施，不绕过生命周期、容量或资源释放管理。

官方：[Guava API](https://guava.dev/releases/33.4.8-jre/api/docs/)。参考 API 版本须与项目实际版本核对。

## 与 Feilong、Hutool 的选择顺序

先复用项目已有能力；已引入 Feilong 且语义符合时，判空、判非空、判零和内部必填断言先查 `Validator` / `Validate`。Feilong 不符合时再查 Hutool，最后才考虑 Guava 或其他已有工具；不为顺序新增依赖。业务校验沿用项目错误码。Guava 优先用于确需其特定语义的能力，例如不可变集合；不能因为方法名相似就替换空白或异常行为。

## 什么时候用，怎么用

先查项目已有依赖与约定，以下按 33.4.8-jre 核对。

| 场景 | 选择 | 注意 |
| --- | --- | --- |
| 入参无效属于编程错误 | 先查 Feilong `Validate`；适用时再查 `Preconditions.checkArgument` | Guava 抛 `IllegalArgumentException`；业务错误应使用项目约定。 |
| null 和空串按同一语义处理 | Feilong 文本判空语义不符时，优先 Hutool `StrUtil.isEmpty(value)` | `Strings.isNullOrEmpty` 也可表达此语义，但空白字符串不是空串。 |
| 构建不可变列表 | `ImmutableList.copyOf(items)` | 不接受 null 元素；保留迭代顺序，不适合随后原地修改。 |

```java
ImmutableList<String> names = ImmutableList.copyOf(sourceNames);
```

导入 `com.google.common.collect.ImmutableList`；`sourceNames` 不得为 null，也不得含 null 元素。缓存、并发优先已有统一设施，避免引入独立生命周期。

## 方法用途与优先级

按场景读取 [方法用途与选择](references/selection-guide.md) 和 [常用方法中文说明](references/usage-extended.md)，先核对已有项目能力、业务语义和当前依赖版本。未覆盖的方法继续查版本索引、源码与官方文档，不根据名称猜测。

## 查找全部方法

查看本技能的 [公开 API 索引](references/API-INDEX.md)，按包或名称定位方法与重载；调用前再查官方文档和项目实际版本。索引记录声明，不等于逐项解释、使用建议或兼容性保证；注意继承方法与索引范围。

## 源码方法说明

查看 [固定版本源码说明索引](references/source-notes/README.md) 按类和重载检索上游方法摘要；索引明确标记未翻译与无注释项，具体场景和优先级仍以本技能及项目规范为准。
