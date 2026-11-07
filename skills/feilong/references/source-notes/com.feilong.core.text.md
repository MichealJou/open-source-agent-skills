# com.feilong.core.text

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.core.text.MessageFormatUtil` | `String format(String pattern,Object... arguments)` | 调用 java.text.MessageFormat#format(String, Object...) 格式化. |
| `com.feilong.core.text.NumberFormatUtil` | `String format(Number value,String numberPattern,RoundingMode roundingMode)` | 将 Number 使用 RoundingMode numberPattern 格式化. |
