# com.feilong.csv.entity

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.csv.entity.BeanCsvConfig` | `Class<T> getBeanClass()` | 获得 迭代对象的类型. |
| `com.feilong.csv.entity.BeanCsvConfig` | `String[] getExcludePropertyNames()` | 获得 排除的属性名字, 会提取所有的属性, 然后剔除 exclude部分. |
| `com.feilong.csv.entity.BeanCsvConfig` | `String[] getIncludePropertyNames()` | 获得 包含的属性名字,会提取所有的属性,然后仅取 include部分. |
| `com.feilong.csv.entity.BeanCsvConfig` | `void setBeanClass(Class<T> beanClass)` | 设置 迭代对象的类型. |
| `com.feilong.csv.entity.BeanCsvConfig` | `void setExcludePropertyNames(String... excludePropertyNames)` | 设置 排除的属性名字, 会提取所有的属性, 然后剔除 exclude部分. |
| `com.feilong.csv.entity.BeanCsvConfig` | `void setIncludePropertyNames(String... includePropertyNames)` | 设置 包含的属性名字,会提取所有的属性,然后仅取 include部分. |
| `com.feilong.csv.entity.CsvColumn` | `String name()` | 【原文待译】(Optional) The name of the column. Defaults to the property or field name. |
| `com.feilong.csv.entity.CsvColumn` | `int order()` | (Optional) 排序 数值从小到大排序. |
| `com.feilong.csv.entity.CsvColumnEntity` | `String getName()` | 获得 the name. |
| `com.feilong.csv.entity.CsvColumnEntity` | `String getPropertyName()` | 获得 属性名字. |
| `com.feilong.csv.entity.CsvColumnEntity` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.csv.entity.CsvColumnEntity` | `int getOrder()` | 获得 the order. |
| `com.feilong.csv.entity.CsvColumnEntity` | `void setName(String name)` | 设置 the name. |
| `com.feilong.csv.entity.CsvColumnEntity` | `void setOrder(int order)` | 设置 the order. |
| `com.feilong.csv.entity.CsvColumnEntity` | `void setPropertyName(String propertyName)` | 设置 属性名字. |
| `com.feilong.csv.entity.CsvConfig` | `String getEncode()` | Gets the 编码. |
| `com.feilong.csv.entity.CsvConfig` | `boolean getIsPrintHeaderLine()` | 获得 是否输出 header line,如果是false,那么csv文件不会输出header line,默认是true. |
| `com.feilong.csv.entity.CsvConfig` | `char getSeparator()` | Gets the field 分隔符 默认,逗号. |
| `com.feilong.csv.entity.CsvConfig` | `void setEncode(String encode)` | Sets the 编码. |
| `com.feilong.csv.entity.CsvConfig` | `void setIsPrintHeaderLine(boolean isPrintHeaderLine)` | 设置 是否输出 header line,如果是false,那么csv文件不会输出header line,默认是true. |
| `com.feilong.csv.entity.CsvConfig` | `void setSeparator(char separator)` | Sets the field 分隔符 默认,逗号. |
