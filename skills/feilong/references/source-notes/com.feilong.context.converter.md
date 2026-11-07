# com.feilong.context.converter

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.context.converter.AbstractBeanClassStringToBeanConverter` | `Class<T> getBeanClass()` | 获得 需要被转换的bean对象类型. |
| `com.feilong.context.converter.AbstractBeanClassStringToBeanConverter` | `void setBeanClass(Class<T> beanClass)` | 设置 需要被转换的bean对象类型. |
| `com.feilong.context.converter.AbstractStringToBeanConverter` | `T convert(String value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.converter.IfStringToBeanConverter` | `void setFalseStringToBeanConverter(StringToBeanConverter<T> falseStringToBeanConverter)` | 设置 如果不满足条件,使用的对应的字符串转bean converter. |
| `com.feilong.context.converter.IfStringToBeanConverter` | `void setPredicate(Predicate<String> predicate)` | 设置 指定的判定条件. |
| `com.feilong.context.converter.IfStringToBeanConverter` | `void setTrueStringToBeanConverter(StringToBeanConverter<T> trueStringToBeanConverter)` | 设置 如果满足条件,使用的对应的字符串转bean converter. |
| `com.feilong.context.converter.JsonStringToBeanConverter` | `void setJsonToJavaConfig(JsonToJavaConfig jsonToJavaConfig)` | 【原文待译】Sets the json to java config. |
| `com.feilong.context.converter.JsonStringToListConverter` | `void setJsonToJavaConfig(JsonToJavaConfig jsonToJavaConfig)` | 【原文待译】Sets the json to java config. |
| `com.feilong.context.converter.MapBuilderStringToBeanConverter` | `BeanBuilder getBeanBuilder()` | 获得 构造对象. |
| `com.feilong.context.converter.MapBuilderStringToBeanConverter` | `NameAndValueMapBuilder getNameAndValueMapBuilder()` | 获得 名字和值的map 构造器. |
| `com.feilong.context.converter.MapBuilderStringToBeanConverter` | `void setBeanBuilder(BeanBuilder beanBuilder)` | 设置 构造对象. |
| `com.feilong.context.converter.MapBuilderStringToBeanConverter` | `void setNameAndValueMapBuilder(NameAndValueMapBuilder nameAndValueMapBuilder)` | 设置 名字和值的map 构造器. |
| `com.feilong.context.converter.StringToBeanConverter` | `T convert(String value)` | 转换. |
