# com.feilong.xml.xstream

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.xml.xstream.XStreamBuilder` | `XStream build(XStreamConfig xStreamConfig)` | 基于 XStreamConfig 构造 XStream. |
| `com.feilong.xml.xstream.XStreamConfig` | `Class<?>[] getProcessAnnotationsTypes()` | 哪个类的注解需要被激活. |
| `com.feilong.xml.xstream.XStreamConfig` | `List<Converter> getConverterList()` | 获得 转换器. |
| `com.feilong.xml.xstream.XStreamConfig` | `Map<Class<?>, Class<?>> getDefaultImplementationMap()` | 【原文待译】Associate a default implementation of a class with an object. Whenever XStream encounters an instance of this type, it will use the default implementation instead. For example, java.util.ArrayList is the default implementation of java.util.List. |
| `com.feilong.xml.xstream.XStreamConfig` | `Map<String, Class<?>> getAliasMap()` | 获得 别名. |
| `com.feilong.xml.xstream.XStreamConfig` | `Map<String, Class<?>> getImplicitCollectionMap()` | 获得 隐式集合 隐藏,隐藏,比如下面有list,泛型中的第二个参数 Class 是 ownerType. |
| `com.feilong.xml.xstream.XStreamConfig` | `boolean getIsPrettyPrint()` | 是否格式化输出. 默认 是true,使用 PrettyPrintWriter,如果设置成false ,将使用 CompactWriter |
| `com.feilong.xml.xstream.XStreamConfig` | `void setAliasMap(Map<String, Class<?>> aliasMap)` | 设置 别名. |
| `com.feilong.xml.xstream.XStreamConfig` | `void setConverterList(List<Converter> converterList)` | 设置 转换器. |
| `com.feilong.xml.xstream.XStreamConfig` | `void setDefaultImplementationMap(Map<Class<?>, Class<?>> defaultImplementationMap)` | 【原文待译】Associate a default implementation of a class with an object. Whenever XStream encounters an instance of this type, it will use the default implementation instead. For example, java.util.ArrayList is the default implementation of java.util.List. |
| `com.feilong.xml.xstream.XStreamConfig` | `void setImplicitCollectionMap(Map<String, Class<?>> implicitCollectionMap)` | 设置 隐式集合 隐藏,隐藏,比如下面有list,泛型中的第二个参数 Class 是 ownerType. |
| `com.feilong.xml.xstream.XStreamConfig` | `void setIsPrettyPrint(boolean isPrettyPrint)` | 是否格式化输出. 默认 是true,使用 PrettyPrintWriter,如果设置成false ,将使用 CompactWriter |
| `com.feilong.xml.xstream.XStreamConfig` | `void setProcessAnnotationsTypes(Class<?>[] processAnnotationsTypes)` | 哪个类的注解需要被激活. |
| `com.feilong.xml.xstream.XStreamConfigBuilder` | `XStreamConfig buildSimpleMapXStreamConfig(String rootElementName,boolean isPrettyPrint)` | 【原文待译】Builds the simple map X stream config. |
| `com.feilong.xml.xstream.XStreamConfigBuilder` | `XStreamConfig buildSimpleMapXStreamConfig(String rootName)` | 【原文待译】Builds the simple map X stream config. |
