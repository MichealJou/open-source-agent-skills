# com.feilong.formatter.entity

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.formatter.entity.BeanFormatterConfig` | `Map<String, Transformer<Object, String>> getPropertyNameAndTransformerMap()` | 获得 指定属性类型转换. |
| `com.feilong.formatter.entity.BeanFormatterConfig` | `String[] getExcludePropertyNames()` | 获得 排除的属性名字, 会提取所有的属性, 然后剔除 exclude部分. |
| `com.feilong.formatter.entity.BeanFormatterConfig` | `String[] getIncludePropertyNames()` | 获得 包含的属性名字,会提取所有的属性,然后仅取 include部分. |
| `com.feilong.formatter.entity.BeanFormatterConfig` | `String[] getSorts()` | 获得 显示属性(列 )的顺序. |
| `com.feilong.formatter.entity.BeanFormatterConfig` | `void setExcludePropertyNames(String... excludePropertyNames)` | 设置 排除的属性名字, 会提取所有的属性, 然后剔除 exclude部分. |
| `com.feilong.formatter.entity.BeanFormatterConfig` | `void setIncludePropertyNames(String... includePropertyNames)` | 设置 包含的属性名字,会提取所有的属性,然后仅取 include部分. |
| `com.feilong.formatter.entity.BeanFormatterConfig` | `void setPropertyNameAndTransformerMap(Map<String, Transformer<Object, String>> propertyNameAndTransformerMap)` | 设置 指定属性类型转换. |
| `com.feilong.formatter.entity.BeanFormatterConfig` | `void setSorts(String... sorts)` | 设置 显示属性(列 )的顺序. |
| `com.feilong.formatter.entity.FormatterColumnEntity` | `String getName()` | 获得 显示的列的名称. |
| `com.feilong.formatter.entity.FormatterColumnEntity` | `String getPropertyName()` | 获得 属性名字. |
| `com.feilong.formatter.entity.FormatterColumnEntity` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.formatter.entity.FormatterColumnEntity` | `int getOrder()` | 获得 显示顺序. 数值从小到大排序 |
| `com.feilong.formatter.entity.FormatterColumnEntity` | `void setName(String name)` | 设置 显示的列的名称. |
| `com.feilong.formatter.entity.FormatterColumnEntity` | `void setOrder(int order)` | 设置 显示顺序. 数值从小到大排序 |
| `com.feilong.formatter.entity.FormatterColumnEntity` | `void setPropertyName(String propertyName)` | 设置 属性名字. |
