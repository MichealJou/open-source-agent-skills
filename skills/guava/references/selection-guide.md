# guava 方法用途与选择

核对版本：33.4.8-jre。本文只标明已核对的方法；同名重载的签名、空值与异常以该版本源码为准。

## 字符串：`Strings`

项目已引入 Feilong 且语义相同时，判空先用 Feilong；要求空格有效时先查 Hutool `StrUtil.isEmpty`。以下是 `Strings` 全部公开方法名。

| 方法 | 中文用途与场景 | 选择与边界 |
| --- | --- | --- |
| `isNullOrEmpty` | 判断 null 或空串 | 空格不是空串；本项目同语义先查 Hutool。 |
| `nullToEmpty` / `emptyToNull` | null 转空串 / 空串转 null | 保留接口值语义；未经要求不要修改原值。 |
| `padStart` / `padEnd` | 在字符串开头 / 末尾补指定字符以满足最小长度 | 核对长度口径；标识符、密钥和协议字段不能擅自补齐。 |
| `repeat` | 重复字符串指定次数 | 限制外部输入的次数，避免内存问题。 |
| `commonPrefix` / `commonSuffix` | 取两个字符序列的公共前缀 / 后缀 | 核对 Unicode 与边界行为；不等于路径安全校验。 |
| `lenientFormat` | 使用宽容格式化生成文本 | 格式与异常行为不是任意日志或 `String.format` 的等价替换。 |

## 其他常用能力

| 方法或类型 | 中文用途与场景 | 选择与边界 |
| --- | --- | --- |
| `Preconditions.checkArgument` | 检查内部参数条件 | 业务错误沿用业务异常；Feilong 已引入且适用时优先查 `Validate.isTrue`。 |
| `Preconditions.checkState` | 检查对象当前状态 | 先查 Feilong `Validate.validState`；异常契约需核对。 |
| `Preconditions.checkNotNull` | 检查内部引用非 null 并返回引用 | 先查 Feilong `Validate.notNull`；业务字段校验使用项目统一方式。 |
| `ImmutableList.copyOf` | 将输入复制为不可变列表 | null 元素不被接受；与需要原地修改的列表不是等价替换。 |

更多声明见 [base](api/com.google.common.base.md) 与 [collect](api/com.google.common.collect.md)。其他类尚未逐项编写中文解释。
