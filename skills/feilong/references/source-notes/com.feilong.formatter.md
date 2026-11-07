# com.feilong.formatter

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.formatter.FormatterColumn` | `String name()` | 【原文待译】(Optional) The name of the column. Defaults to the property or field name. |
| `com.feilong.formatter.FormatterColumn` | `int order()` | (Optional) 排序,数值从小到大排序. |
| `com.feilong.formatter.FormatterUtil` | `String formatToSimpleTable(Iterable<T> iterable)` | 使用 SimpleTableFormatter来格式化. |
| `com.feilong.formatter.FormatterUtil` | `String formatToSimpleTable(Iterable<T> iterable,BeanFormatterConfig beanFormatterConfig)` | 使用 SimpleTableFormatter来格式化. |
| `com.feilong.formatter.FormatterUtil` | `String formatToSimpleTable(Iterable<T> iterable,String... sorts)` | 使用 SimpleTableFormatter以及指定特定的顺序字段来格式化. |
| `com.feilong.formatter.FormatterUtil` | `String formatToSimpleTable(Map<K, V> map)` | 格式化成简单的table格式. |
| `com.feilong.formatter.FormatterUtil` | `String formatToSimpleTable(T bean)` | 格式化成简单的table格式. |
| `com.feilong.formatter.SimpleTableFormatter` | `String format(String[] columnTitles,List<Object[]> dataList)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
