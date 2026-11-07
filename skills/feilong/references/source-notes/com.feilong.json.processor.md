# com.feilong.json.processor

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.json.processor.CapitalizePropertyNameProcessor` | `String processPropertyName(@SuppressWarnings("rawtypes")
Class beanClass,String currentPropertyName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.json.processor.SimpleMapPropertyNameProcessor` | `String processPropertyName(@SuppressWarnings("rawtypes")
Class beanClass,String currentPropertyName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.json.processor.StringOverLengthJsonValueProcessor` | `Object format(Object value,int maxLength)` | 【原文待译】Format. |
| `com.feilong.json.processor.StringOverLengthJsonValueProcessor` | `Object format(Object value,int maxLength,String overLengthMaskString)` | 【原文待译】Format. |
| `com.feilong.json.processor.StringOverLengthJsonValueProcessor` | `String getOverLengthMaskString()` | 获得 超长截取拼接的字符串. |
| `com.feilong.json.processor.StringOverLengthJsonValueProcessor` | `int getMaxLength()` | 获得 最大长度,默认 500. |
| `com.feilong.json.processor.StringOverLengthJsonValueProcessor` | `void setMaxLength(int maxLength)` | 设置 最大长度,默认 500. |
| `com.feilong.json.processor.StringOverLengthJsonValueProcessor` | `void setOverLengthMaskString(String overLengthMaskString)` | 设置 超长截取拼接的字符串. |
