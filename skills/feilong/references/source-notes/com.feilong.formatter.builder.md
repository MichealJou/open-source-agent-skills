# com.feilong.formatter.builder

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.formatter.builder.AbstractFormatterBuilder` | `List<FormatterColumnEntity> build(T bean,BeanFormatterConfig beanFormatterConfig)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.formatter.builder.BeanTypeFormatterBuilder` | `Object[] buildLineData(T bean,List<String> propertyNameList,BeanFormatterConfig beanFormatterConfig)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.formatter.builder.ColumnMaxWidthsBuilder` | `int[] build(List<Object[]> rows)` | 定位每列最大的宽度. |
| `com.feilong.formatter.builder.FormatterBuilder` | `List<FormatterColumnEntity> build(T bean,BeanFormatterConfig beanFormatterConfig)` | 构造 FormatterColumnEntity List. |
| `com.feilong.formatter.builder.FormatterBuilder` | `Object[] buildLineData(T bean,List<String> propertyNameList,BeanFormatterConfig beanFormatterConfig)` | 构造 数据. |
| `com.feilong.formatter.builder.FormatterBuilderFactory` | `FormatterBuilder create(T bean)` | 不同的bean类型,返回不同的创造器. 如果 bean 是 map 类型, 那么返回 MapTypeFormatterBuilder,否则返回 BeanTypeFormatterBuilder. |
| `com.feilong.formatter.builder.MapTypeFormatterBuilder` | `Object[] buildLineData(T bean,List<String> propertyNameList,BeanFormatterConfig beanFormatterConfig)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.formatter.builder.ValueHandler` | `String getValue(String propertyName,Object value,BeanFormatterConfig beanFormatterConfig)` | 【原文待译】Gets the value. |
