# com.feilong.core.bean

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.core.bean.Alias` | `String name()` | 对应map里面的key(即别名). |
| `com.feilong.core.bean.Alias` | `String sampleValue()` | 示例结果(仅供查看的时候,知道这个字段的结果值格式和大致的值,没有其他作用). |
| `com.feilong.core.bean.BeanUtil` | `DynaBean newDynaBean(Map<?, ?> valueMap)` | 使用 valueMap 来构造一个 DynaBean. |
| `com.feilong.core.bean.BeanUtil` | `T cloneBean(T bean)` | 调用BeanUtils#cloneBean(Object). |
| `com.feilong.core.bean.BeanUtil` | `T populate(T bean,Map<String, ?> properties)` | 把properties/map里面的值 populate (填充) 到 bean 中. |
| `com.feilong.core.bean.BeanUtil` | `T populateAliasBean(T aliasBean,Map<String, ?> aliasAndValueMap)` | 将 alias 和value 的map populate (填充) 到 aliasBean . |
| `com.feilong.core.bean.BeanUtil` | `void copyProperties(Object toObj,Object fromObj,String... includePropertyNames)` | 将 fromObj 中的全部或者一组属性 includePropertyNames 的值,复制到 toObj 对象中. 如果需要copy的两个对象属性的 类型一样 ,那么调用此方法会有 性能消耗 , 强烈建议使用 PropertyUtil#copyProperties(Object, Object, String...) |
| `com.feilong.core.bean.ConvertUtil` | `BigDecimal toBigDecimal(Object toBeConvertedValue)` | 将 toBeConvertedValue 转换成 java.math.BigDecimal. |
| `com.feilong.core.bean.ConvertUtil` | `BigDecimal toBigDecimal(Object toBeConvertedValue,BigDecimal defaultValue)` | 将 toBeConvertedValue 转换成 java.math.BigDecimal,如果有异常或者是null 使用默认值 defaultValue . |
| `com.feilong.core.bean.ConvertUtil` | `Boolean toBoolean(Object toBeConvertedValue)` | 将 toBeConvertedValue 转换成 Boolean类型. |
| `com.feilong.core.bean.ConvertUtil` | `Boolean toBoolean(Object toBeConvertedValue,Boolean defaultValue)` | 将 toBeConvertedValue 转换成 Boolean类型,如果结果是null或者转换异常 使用默认值. |
| `com.feilong.core.bean.ConvertUtil` | `Enumeration<T> toEnumeration(final Collection<T> collection)` | 将集合 collection 转成 Enumeration . |
| `com.feilong.core.bean.ConvertUtil` | `Integer toInteger(Object toBeConvertedValue)` | 将 toBeConvertedValue 转换成 Integer类型. |
| `com.feilong.core.bean.ConvertUtil` | `Integer toInteger(Object toBeConvertedValue,Integer defaultValue)` | 将 toBeConvertedValue 转换成 Integer类型,如果转换不了返回默认值 defaultValue . |
| `com.feilong.core.bean.ConvertUtil` | `Integer[] toIntegers(Object toBeConvertedValue)` | 将 toBeConvertedValue 转成Integer 数组. |
| `com.feilong.core.bean.ConvertUtil` | `Iterator<T> toIterator(Object toBeConvertedValue)` | 将 toBeConvertedValue 转成Iterator类型. |
| `com.feilong.core.bean.ConvertUtil` | `List<Integer> toIntegerList(Object toBeConvertedValue)` | 将 toBeConvertedValue 转成 Integer list. toBeConvertedValue 支持字符串,数组,集合 |
| `com.feilong.core.bean.ConvertUtil` | `List<Long> toLongList(Object toBeConvertedValue)` | 将 toBeConvertedValue 转成 long list. toBeConvertedValue 支持字符串,数组,集合 |
| `com.feilong.core.bean.ConvertUtil` | `List<String> toStringList(Object toBeConvertedValue)` | 将 toBeConvertedValue 转成 string list. toBeConvertedValue 支持字符串,数组,集合 |
| `com.feilong.core.bean.ConvertUtil` | `List<T> toList(T... arrays)` | 数组转成 (java.util.ArrayList ArrayList). |
| `com.feilong.core.bean.ConvertUtil` | `List<T> toList(final Collection<T> collection)` | 将 集合 collection 转成 list. |
| `com.feilong.core.bean.ConvertUtil` | `List<T> toList(final Enumeration<T> enumeration)` | 将枚举 enumeration 转成 List. |
| `com.feilong.core.bean.ConvertUtil` | `Locale toLocale(Object locale)` | 将对象转成 Locale. |
| `com.feilong.core.bean.ConvertUtil` | `Long toLong(Object toBeConvertedValue)` | 将 toBeConvertedValue 转换成 Long类型. |
| `com.feilong.core.bean.ConvertUtil` | `Long toLong(Object toBeConvertedValue,Long defaultValue)` | 将 toBeConvertedValue 转换成 Long类型,如果转换不了返回默认值 defaultValue . |
| `com.feilong.core.bean.ConvertUtil` | `Long[] toLongs(Object toBeConvertedValue)` | 将 toBeConvertedValue 转成Long 数组. |
| `com.feilong.core.bean.ConvertUtil` | `Map<I, J> toMap(Map<K, V> inputMap,final Class<I> keyTargetType,final Class<J> valueTargetType)` | 将诸如 Map 类型转成 Map 类型. |
| `com.feilong.core.bean.ConvertUtil` | `Map<I, J> toMap(Map<K, V> inputMap,final Transformer<K, I> keyTransformer,final Transformer<V, J> valueTransformer)` | 将诸如 Map 类型转成 Map 类型. |
| `com.feilong.core.bean.ConvertUtil` | `Map<K, J> toMap(Map<K, V> inputMap,final Class<J> valueTargetType)` | 将诸如 Map 类型转成 Map 类型. |
| `com.feilong.core.bean.ConvertUtil` | `Map<K, V> toMap(Collection<E> mapEntryCollection)` | 将 mapEntryCollection 转成map (LinkedHashMap). |
| `com.feilong.core.bean.ConvertUtil` | `Map<K, V> toMap(K key,V value)` | 将 key 和 value 直接转成map. |
| `com.feilong.core.bean.ConvertUtil` | `Map<K, V> toMap(K key1,V value1,K key2,V value2)` | 将 key1 和 value1 / key2 和 value2 直接转成map. |
| `com.feilong.core.bean.ConvertUtil` | `Map<K, V> toMapUseEntrys(Map.Entry<K, V>... mapEntrys)` | 将 java.util.Map.Entry数组转成map (LinkedHashMap). |
| `com.feilong.core.bean.ConvertUtil` | `Map<String, String> toMap(Properties properties)` | 将 properties 转换成map. |
| `com.feilong.core.bean.ConvertUtil` | `Properties toProperties(final Map<String, String> map)` | 将map转成 Properties. |
| `com.feilong.core.bean.ConvertUtil` | `Set<T> toSet(T... arrays)` | 数组转成 Set (java.util.LinkedHashSet LinkedHashSet). |
| `com.feilong.core.bean.ConvertUtil` | `String toString(Object toBeConvertedValue)` | 把对象 toBeConvertedValue 转换成字符串. |
| `com.feilong.core.bean.ConvertUtil` | `String toString(Object[] arrays,String connector)` | 将数组 arrays 通过 connector 拼接成字符串. |
| `com.feilong.core.bean.ConvertUtil` | `String toString(Object[] arrays,ToStringConfig toStringConfig)` | 将数组 arrays 通过ToStringConfig 拼接成字符串. |
| `com.feilong.core.bean.ConvertUtil` | `String toString(final Collection<?> collection,String connector)` | 将集合 collection 使用拼接 connector 拼接成字符串. |
| `com.feilong.core.bean.ConvertUtil` | `String toString(final Collection<?> collection,ToStringConfig toStringConfig)` | 将集合 collection 使用拼接配置 toStringConfig 拼接成字符串. |
| `com.feilong.core.bean.ConvertUtil` | `String[] toStrings(Object toBeConvertedValue)` | 将 toBeConvertedValue 转成String数组. |
| `com.feilong.core.bean.ConvertUtil` | `T convert(Object toBeConvertedValue,Class<T> targetType)` | 将 toBeConvertedValue 转成指定 targetType 类型的对象. |
| `com.feilong.core.bean.ConvertUtil` | `T[] toArray(Collection<T> collection,Class<T> arrayComponentType)` | 将集合 collection 转成数组. |
| `com.feilong.core.bean.ConvertUtil` | `T[] toArray(String[] toBeConvertedValue,Class<T> targetType)` | 将字符串数组 toBeConvertedValue 转成指定类型 targetType 的数组. |
| `com.feilong.core.bean.ConvertUtil` | `T[] toArray(T... arrays)` | 将动态数组转成数组. |
| `com.feilong.core.bean.ConvertUtil` | `void registerSimpleDateLocaleConverter(String pattern)` | 【原文待译】Register simple date locale converter. |
| `com.feilong.core.bean.ConvertUtil` | `void registerStandardDefaultNull()` | 【原文待译】Register standard default null. |
| `com.feilong.core.bean.PropertyUtil` | `Map<String, Object> describe(Object bean,String... propertyNames)` | 返回一个 bean 中指定属性 propertyNames 可读属性 ,并将属性名/属性值放入一个 java.util.LinkedHashMap LinkedHashMap 中. |
| `com.feilong.core.bean.PropertyUtil` | `PropertyDescriptor[] getPropertyDescriptors(Class<?> klass)` | 【原文待译】Retrieve the property descriptors for the specified class, introspecting and caching them the first time a particular bean class is encountered. |
| `com.feilong.core.bean.PropertyUtil` | `T findValueOfType(Object obj,Class<T> toBeFindedClassType)` | 从指定的 obj 中,查找指定类型 toBeFindedClassType 的值. |
| `com.feilong.core.bean.PropertyUtil` | `T getProperty(Object bean,String propertyName)` | 使用 PropertyUtils#getProperty(Object, String) 从指定bean对象中取得指定属性名称的值. |
| `com.feilong.core.bean.PropertyUtil` | `void copyProperties(Object toObj,Object fromObj,String... includePropertyNames)` | 将 fromObj 中的全部或者一组属性的值,复制到 toObj 对象中. |
| `com.feilong.core.bean.PropertyUtil` | `void setProperty(Object bean,String propertyName,Object value)` | 使用 PropertyUtils#setProperty(Object, String, Object) 来设置指定bean对象中的指定属性的值. |
| `com.feilong.core.bean.PropertyUtil` | `void setPropertyIfValueNotNull(Object bean,String propertyName,Object value)` | 如果 null != value ,那么才调用 #setProperty(Object, String, Object). |
| `com.feilong.core.bean.PropertyUtil` | `void setPropertyIfValueNotNullOrEmpty(Object bean,String propertyName,Object value)` | 如果 value isNotNullOrEmpty,那么才调用 #setProperty(Object, String, Object). |
| `com.feilong.core.bean.PropertyValueObtainer` | `K getPropertyValueCollection(Iterable<O> beanIterable,String propertyName,K returnCollection)` | 循环 beanIterable ,调用 PropertyUtil#getProperty(Object, String) 获得 propertyName的值,塞到 returnCollection 中返回. |
| `com.feilong.core.bean.PropertyValueObtainer` | `K getPropertyValueCollection(Iterable<O> beanIterable,String propertyName,K returnCollection,Class<T> returnElementClass)` | 循环 beanIterable ,调用 PropertyUtil#getProperty(Object, String) 获得 propertyName的值,将值进行类型转换成 returnElementClass ,塞到 returnCollection 中返回. |
| `com.feilong.core.bean.PropertyValueObtainer` | `T getValue(O obj,PropertyDescriptor propertyDescriptor)` | 【原文待译】Gets the value. |
| `com.feilong.core.bean.ToStringConfig` | `String getConnector()` | 获得 连接符,默认=#DEFAULT_CONNECTOR. |
| `com.feilong.core.bean.ToStringConfig` | `String getPrefix()` | 获得 循环拼接元素的时候,支持给每个元素拼接一个前缀. |
| `com.feilong.core.bean.ToStringConfig` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.core.bean.ToStringConfig` | `boolean getIsJoinNullOrEmpty()` | 是否拼接null或者empty的元素,如果是true ,表示拼接,如果是false,那么拼接的时候跳过这个元素. |
| `com.feilong.core.bean.ToStringConfig` | `void setConnector(String connector)` | 设置 连接符,默认=#DEFAULT_CONNECTOR. |
| `com.feilong.core.bean.ToStringConfig` | `void setIsJoinNullOrEmpty(boolean isJoinNullOrEmpty)` | 是否拼接null或者empty的元素,如果是true ,表示拼接,如果是false,那么拼接的时候跳过这个元素. |
| `com.feilong.core.bean.ToStringConfig` | `void setPrefix(String prefix)` | 设置 循环拼接元素的时候,支持给每个元素拼接一个前缀. |
