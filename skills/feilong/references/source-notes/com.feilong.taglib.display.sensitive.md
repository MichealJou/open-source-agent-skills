# com.feilong.taglib.display.sensitive

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.taglib.display.sensitive.SensitiveConfig` | `String getType()` | 获得 敏感词类型. |
| `com.feilong.taglib.display.sensitive.SensitiveConfig` | `char getMaskChar()` | 获得 掩码字符,比如*,#等,默认是*. |
| `com.feilong.taglib.display.sensitive.SensitiveConfig` | `void setMaskChar(char maskChar)` | 设置 掩码字符,比如*,#等,默认是*. |
| `com.feilong.taglib.display.sensitive.SensitiveConfig` | `void setType(String type)` | 设置 敏感词类型. |
| `com.feilong.taglib.display.sensitive.SensitivePropertiesConfig` | `Integer[] load(String type)` | 【原文待译】Load. |
| `com.feilong.taglib.display.sensitive.SensitiveTag` | `void setMaskChar(char maskChar)` | 设置 mask的字符,比如*,#等,默认是*. |
| `com.feilong.taglib.display.sensitive.SensitiveTag` | `void setType(String type)` | 设置 类型, 可以有 mobile , chinese name,address,email. |
| `com.feilong.taglib.display.sensitive.SensitiveTag` | `void setValue(String value)` | 设置 待mask字符串. |
| `com.feilong.taglib.display.sensitive.SensitiveType` | `SensitiveType toSensitiveType(String type)` | 【原文待译】Gets the sensitive type. |
| `com.feilong.taglib.display.sensitive.SensitiveType` | `String getType()` | 获得 type. |
| `com.feilong.taglib.display.sensitive.SensitiveUtil` | `String parse(String value,SensitiveConfig sensitiveConfig)` | 转换. |
| `com.feilong.taglib.display.sensitive.SensitiveUtil` | `String parse(String value,char maskChar,int leftNoMaskLength,int rightNoMaskLength)` | 【原文待译】Parses the. |
