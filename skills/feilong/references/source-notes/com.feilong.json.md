# com.feilong.json

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.json.JavaToJsonConfig` | `Map<Class<?>, PropertyNameProcessor> getJsonTargetClassAndPropertyNameProcessorMap()` | 转成json的时候,对属性名字做特殊处理的控制器对映关系. |
| `com.feilong.json.JavaToJsonConfig` | `Map<String, JsonValueProcessor> getPropertyNameAndJsonValueProcessorMap()` | 指定属性名称使用的值修改处理器. |
| `com.feilong.json.JavaToJsonConfig` | `PropertyFilter getPropertyFilter()` | 过滤器, 对应com.feilong.lib.json.JsonConfig#getJsonPropertyFilter() , 如果返回true,该属性将会被过滤 |
| `com.feilong.json.JavaToJsonConfig` | `String toString()` | 【原文待译】To string. |
| `com.feilong.json.JavaToJsonConfig` | `String[] getIfIgnoreNullValueElementIncludes()` | 如果忽略null value元素,白名单. 仅当isIgnoreNullValueElement=true才生效 |
| `com.feilong.json.JavaToJsonConfig` | `String[] getIncludes()` | 获得 包含属性名称的数组. |
| `com.feilong.json.JavaToJsonConfig` | `boolean getIsIgnoreNullValueElement()` | 是否忽略 null value 元素,默认 false,表示不忽略. |
| `com.feilong.json.JavaToJsonConfig` | `boolean getIsMaskDefaultSensitiveWords()` | 是否 mask 默认的敏感字符. 默认是 true, 表示会将默认的敏感字符(JsonConfigBuilder#SENSITIVE_WORDS_PROPERTY_NAMES),格式化的时候,输出成 *******代替 |
| `com.feilong.json.JavaToJsonConfig` | `void setIfIgnoreNullValueElementIncludes(String[] ifIgnoreNullValueElementIncludes)` | 如果忽略null value元素,白名单. 仅当isIgnoreNullValueElement=true才生效 |
| `com.feilong.json.JavaToJsonConfig` | `void setIncludes(String... includes)` | 设置 包含属性名称的数组. |
| `com.feilong.json.JavaToJsonConfig` | `void setIsIgnoreNullValueElement(boolean isIgnoreNullValueElement)` | 是否忽略 null value 元素,默认 false,表示不忽略. |
| `com.feilong.json.JavaToJsonConfig` | `void setIsMaskDefaultSensitiveWords(boolean isMaskDefaultSensitiveWords)` | 是否 mask 默认的敏感字符. 默认是 true, 表示会将默认的敏感字符(JsonConfigBuilder#SENSITIVE_WORDS_PROPERTY_NAMES),格式化的时候,输出成 *******代替 |
| `com.feilong.json.JavaToJsonConfig` | `void setJsonTargetClassAndPropertyNameProcessorMap(Map<Class<?>, PropertyNameProcessor> jsonTargetClassAndPropertyNameProcessorMap)` | 转成json的时候,对属性名字做特殊处理的控制器对映关系. |
| `com.feilong.json.JavaToJsonConfig` | `void setPropertyFilter(PropertyFilter propertyFilter)` | 过滤器, 对应com.feilong.lib.json.JsonConfig#getJsonPropertyFilter() , 如果返回true,该属性将会被过滤 |
| `com.feilong.json.JavaToJsonConfig` | `void setPropertyNameAndJsonValueProcessorMap(Map<String, JsonValueProcessor> propertyNameAndJsonValueProcessorMap)` | 指定属性名称使用的值修改处理器. |
| `com.feilong.json.JsonHelper` | `JSON toJSON(Object obj,JsonConfig jsonConfig)` | 把实体Bean、Map对象、数组、列表集合转换成JSON. |
| `com.feilong.json.JsonHelper` | `boolean isCommonString(Object obj)` | 是否是普通的字符串. |
| `com.feilong.json.JsonHelper` | `boolean isNeedConvertToJSONArray(Object obj)` | 是否需要转成 JSONArray类型. |
| `com.feilong.json.JsonToJavaConfig` | `Class<?> getRootClass()` | 【原文待译】Gets the root class. |
| `com.feilong.json.JsonToJavaConfig` | `JavaIdentifierTransformer getJavaIdentifierTransformer()` | java标识符号转换器. JSON 规范 指出一个对象的key是个字符串,并且该字符串是零个或多个Unicode字符的集合，用双引号括起来，使用反斜杠转义。 字符表示为单个字符串。 这就意味着,当你从json格式转成java的时候,你可能有一个有效的 JSON key ,但是他是个无效的java 标识符.此时你可以设置 JavaIdentifierTransformer |
| `com.feilong.json.JsonToJavaConfig` | `Map<String, Class<?>> getClassMap()` | 用来设置复杂自定义对象转换. |
| `com.feilong.json.JsonToJavaConfig` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.json.JsonToJavaConfig` | `void setClassMap(Map<String, Class<?>> classMap)` | 用来设置复杂自定义对象转换. |
| `com.feilong.json.JsonToJavaConfig` | `void setJavaIdentifierTransformer(JavaIdentifierTransformer javaIdentifierTransformer)` | java标识符号转换器. JSON 规范 指出一个对象的key是个字符串,并且该字符串是零个或多个Unicode字符的集合，用双引号括起来，使用反斜杠转义。 字符表示为单个字符串。 这就意味着,当你从json格式转成java的时候,你可能有一个有效的 JSON key ,但是他是个无效的java 标识符.此时你可以设置 JavaIdentifierTransformer |
| `com.feilong.json.JsonToJavaConfig` | `void setRootClass(Class<?> rootClass)` | 【原文待译】Sets the root class. |
| `com.feilong.json.JsonUtil` | `List<T> toList(String json,Class<T> rootClass)` | 把一个json数组串转换成集合,集合里存放的为实例Bean. |
| `com.feilong.json.JsonUtil` | `List<T> toList(String json,JsonToJavaConfig jsonToJavaConfig)` | 把一个json数组串转换成集合,且集合里的对象的属性含有另外实例Bean. |
| `com.feilong.json.JsonUtil` | `Map<String, T> toMap(String json)` | 将简单的json字符串转成 map . |
| `com.feilong.json.JsonUtil` | `Map<String, T> toMap(String json,JsonToJavaConfig jsonToJavaConfig)` | 把json对象串转换成map对象,map对象里可以存放的其他实体Bean还含有另外实体Bean. |
| `com.feilong.json.JsonUtil` | `String format(Object obj)` | 将对象 obj 格式化成json字符串. 该方法还可以格式化json字符串成缩进形式的格式 |
| `com.feilong.json.JsonUtil` | `String format(Object obj,JavaToJsonConfig javaToJsonConfig)` | 使用配置 JavaToJsonConfig 来格式化成json字符串. |
| `com.feilong.json.JsonUtil` | `String format(Object obj,JavaToJsonConfig javaToJsonConfig,int indentFactor,int indent)` | 【原文待译】Format. |
| `com.feilong.json.JsonUtil` | `String format(Object obj,String... excludes)` | 将对象格式化 成json字符串( 排除 指定名称的属性 excludes ),并且 toString(4, 4) 输出. 和该方法对应的有,仅仅 包含 某些属性,see #formatWithIncludes(Object, String...) |
| `com.feilong.json.JsonUtil` | `String format(Object obj,String[] excludes,int indentFactor,int indent)` | 将对象格式化 成json字符串( 排除 指定名称的属性 excludes ),并且按照指定的缩进( indentFactor 和 indent ) 输出. 和该方法对应的有,仅仅 包含 某些属性,see #formatWithIncludes(Object, String...) |
| `com.feilong.json.JsonUtil` | `String format(Object obj,boolean isIgnoreNullValueElement)` | 将对象 obj 格式化成json字符串,支持 isIgnoreNullValueElement 参数控制是否输出 null 值元素. |
| `com.feilong.json.JsonUtil` | `String format(Object obj,boolean isIgnoreNullValueElement,String... ifIgnoreNullValueElementIncludes)` | 将对象 obj 格式化成json字符串,支持 isIgnoreNullValueElement 参数控制是否输出 null 值元素,如果isIgnoreNullValueElement设置为true,还可以使用 ifIgnoreNullValueElementIncludes来控制需要强行输出的白名单. |
| `com.feilong.json.JsonUtil` | `String format(Object obj,int indentFactor,int indent)` | 将 obj 格式化成json字符串,并且按照指定的缩进( indentFactor 和 indent ) 输出. |
| `com.feilong.json.JsonUtil` | `String formatObjectFieldsNameAndValueMap(Object obj)` | 格式化一个对象 obj 里面所有的field 的名字和值. |
| `com.feilong.json.JsonUtil` | `String formatSimpleMap(Map<K, V> inputMap)` | 有些map 值很复杂,比如带有request信息, 这样的map转成json很可能由于一些级联关系而抛异常. |
| `com.feilong.json.JsonUtil` | `String formatSimpleMap(Map<K, V> inputMap,Class<?>... allowFormatClassTypes)` | 有些map 值很复杂,比如带有request信息, 这样的map转成json很可能由于一些级联关系而抛异常. |
| `com.feilong.json.JsonUtil` | `String formatWithIncludes(Object obj,final String... includes)` | 将对象格式化成json字符串( 仅仅包含 指定名称的属性 includes ). 和该方法对应的有,仅仅 排除 某些属性,see #format(Object, String[])以及 #format(Object, String[], int, int) |
| `com.feilong.json.JsonUtil` | `String toString(Object obj)` | 将对象格式化成json字符串,并且 toString(0, 0) 输出. =com.feilong.json.JsonUtil.format(Object, 0, 0) |
| `com.feilong.json.JsonUtil` | `String toString(Object obj,JavaToJsonConfig javaToJsonConfig)` | 使用配置 JavaToJsonConfig 来转成json字符串. |
| `com.feilong.json.JsonUtil` | `String toString(Object obj,String... excludes)` | 将对象 obj 格式化成json字符串( 排除 指定名称的属性 excludes ),并且 toString(0, 0) 输出. 和该方法对应的有,仅仅 包含 某些属性,see #formatWithIncludes(Object, String...) |
| `com.feilong.json.JsonUtil` | `String toString(Object obj,boolean isIgnoreNullValueElement)` | 将对象 obj 格式化成json字符串,支持 isIgnoreNullValueElement 参数控制是否输出 null 值元素. |
| `com.feilong.json.JsonUtil` | `String toString(Object obj,boolean isIgnoreNullValueElement,String... ifIgnoreNullValueElementIncludes)` | 将对象 obj 格式化成json字符串,支持 isIgnoreNullValueElement 参数控制是否输出 null 值元素,如果isIgnoreNullValueElement设置为true,还可以使用 ifIgnoreNullValueElementIncludes来控制需要强行输出的白名单. |
| `com.feilong.json.JsonUtil` | `T toBean(String json,Class<T> rootClass)` | json串,转换成实体对象. |
| `com.feilong.json.JsonUtil` | `T toBean(String json,JsonToJavaConfig jsonToJavaConfig)` | 从json串转换成 javabean 实体对象,支持实体集合属性可能存有另外实体Bean. |
| `com.feilong.json.JsonUtil` | `T[] toArray(String json,JsonToJavaConfig jsonToJavaConfig)` | 把一个json数组串转换成实体数组,数组元素的属性可以含有另外实例Bean. |
