# com.feilong.core.util

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.core.util.AggregateUtil` | `BigDecimal avg(Iterable<O> beanIterable,String propertyName,int scale)` | 计算bean list,bean指定属性值的算术平均值. |
| `com.feilong.core.util.AggregateUtil` | `BigDecimal sum(Iterable<O> beanIterable,String propertyName)` | 总和,计算集合对象 beanIterable 内指定的属性名 propertyName 值的总和. |
| `com.feilong.core.util.AggregateUtil` | `BigDecimal sum(Iterable<O> beanIterable,String propertyName,Predicate<O> includePredicate)` | 迭代 beanIterable ,提取 符合 includePredicate 的元素的指定 propertyName 元素的值 ,累计总和. |
| `com.feilong.core.util.AggregateUtil` | `Map<String, BigDecimal> avg(Iterable<O> beanIterable,String[] propertyNames,int scale)` | 算术平均值. |
| `com.feilong.core.util.AggregateUtil` | `Map<String, BigDecimal> sum(Iterable<O> beanIterable,String... propertyNames)` | 求和,分别计算集合对象 beanIterable 内指定的不同属性名 propertyNames 值的总和. |
| `com.feilong.core.util.AggregateUtil` | `Map<String, BigDecimal> sum(Iterable<O> beanIterable,String[] propertyNames,Predicate<O> includePredicate)` | 迭代 beanIterable ,提取符合 includePredicate 的元素的指定 propertyNames 元素的值 ,累计总和. |
| `com.feilong.core.util.AggregateUtil` | `Map<String, Map<Object, Integer>> groupCount(Iterable<O> beanIterable,String... propertyNames)` | 循环 beanIterable ,统计不同 propertyNames 的不同值出现的次数. |
| `com.feilong.core.util.AggregateUtil` | `Map<String, Map<Object, Integer>> groupCount(Iterable<O> beanIterable,String[] propertyNames,Map<String, Transformer<Object, Object>> propertyValueAndTransformerMap)` | 循环 beanIterable ,分别统计 propertyNames 的值出现的次数,统计的时候支持使用 propertyValueAndTransformerMap 属性值的转换. |
| `com.feilong.core.util.AggregateUtil` | `Map<String, Map<Object, Integer>> groupCount(Iterable<O> beanIterable,String[] propertyNames,Map<String, Transformer<Object, Object>> propertyValueAndTransformerMap,Predicate<O> includePredicate)` | 循环 beanIterable ,只选择符合 includePredicate 的对象,分别统计 propertyNames 的值出现的次数,统计的时候支持使用 propertyValueAndTransformerMap 属性值的转换. |
| `com.feilong.core.util.AggregateUtil` | `Map<String, Map<Object, Integer>> groupCount(Iterable<O> beanIterable,String[] propertyNames,Predicate<O> includePredicate)` | 循环 beanIterable ,只选择符合 includePredicate 的对象,分别统计 propertyNames 的值出现的次数. |
| `com.feilong.core.util.AggregateUtil` | `Map<T, BigDecimal> groupSum(Iterable<O> beanIterable,String keyPropertyName,String sumPropertyName)` | 迭代 beanIterable ,取元素 keyPropertyName 的值为 key ,累计 sumPropertyName 属性值 为 value,返回 map. |
| `com.feilong.core.util.AggregateUtil` | `Map<T, BigDecimal> groupSum(Iterable<O> beanIterable,String keyPropertyName,String sumPropertyName,Predicate<O> includePredicate)` | 迭代 beanIterable ,提取符合 includePredicate 的元素,取元素 keyPropertyName 的值为 key ,累计 sumPropertyName 属性值 为 value,返回 map. 统计 user list 所有 age 小于等于30的, 按照姓名分组, 累加每个人的 age 总和 |
| `com.feilong.core.util.AggregateUtil` | `Map<T, Integer> groupCount(Iterable<O> beanIterable,String propertyName)` | 循环 beanIterable ,统计 propertyName 的值出现的次数. |
| `com.feilong.core.util.AggregateUtil` | `Map<T, Integer> groupCount(Iterable<O> beanIterable,String propertyName,Predicate<O> includePredicate)` | 循环 beanIterable ,只选择符合 includePredicate 的对象,统计 propertyName 的值出现的次数. |
| `com.feilong.core.util.CollectionsUtil` | `List<E> newArrayList()` | 创建 a mutable , empty ArrayList instance . |
| `com.feilong.core.util.CollectionsUtil` | `List<E> newArrayList(Collection<? extends E> collection)` | 【原文待译】Constructs a list containing the elements of the specified collection, in the order they are returned by the collection's iterator. |
| `com.feilong.core.util.CollectionsUtil` | `List<E> newCopyOnWriteArrayList()` | 创建 a mutable , empty CopyOnWriteArrayList instance . |
| `com.feilong.core.util.CollectionsUtil` | `List<E> newCopyOnWriteArrayList(Collection<? extends E> collection)` | 【原文待译】Creates a list containing the elements of the specified collection, in the order they are returned by the collection's iterator. |
| `com.feilong.core.util.CollectionsUtil` | `List<E> newLinkedList()` | 创建 a mutable , empty LinkedList instance . |
| `com.feilong.core.util.CollectionsUtil` | `List<E> newLinkedList(Collection<? extends E> collection)` | 【原文待译】Constructs a list containing the elements of the specified collection, in the order they are returned by the collection's iterator. |
| `com.feilong.core.util.CollectionsUtil` | `List<List<T>> partition(List<T> list,int size)` | 【原文待译】Returns consecutive List#subList(int, int) sublists of a list, each of the same size (the final list may be smaller). For example, partitioning a list containing [a, b, c, d, e] with a partition size of 3 yields [[a, b, c], [d, e]] -- an outer list containing two inner lists of three and two element… |
| `com.feilong.core.util.CollectionsUtil` | `List<O> collect(final Iterable<I> inputBeanIterable,final Class<O> outputListBeanType,final String... includePropertyNames)` | 循环 inputBeanIterable ,将每个元素使用转换程成新的 outputListBeanType 类型对象(如有需要只copy传入的 includePropertyNames 属性) 返回 新的list . |
| `com.feilong.core.util.CollectionsUtil` | `List<O> remove(Collection<O> objectCollection,O... removeElements)` | 从 objectCollection 中 删除 removeElements (原集合对象不变) . |
| `com.feilong.core.util.CollectionsUtil` | `List<O> removeAll(Collection<O> objectCollection,Collection<O> removeCollection)` | 从 objectCollection 中删除所有的 removeCollection (原集合对象不变) . |
| `com.feilong.core.util.CollectionsUtil` | `List<O> removeAllNull(Collection<O> objectCollection)` | 从 objectCollection 中删除所有的 null 元素 (原集合对象不变) . |
| `com.feilong.core.util.CollectionsUtil` | `List<O> removeDuplicate(Collection<O> objectCollection)` | 去重,返回没有重复元素的新list (原集合对象不变) . |
| `com.feilong.core.util.CollectionsUtil` | `List<O> removeDuplicate(Collection<O> objectCollection,String propertyName)` | 去重,返回 objectCollection 指定属性 propertyName 没有重复值的新list (原集合对象不变) . |
| `com.feilong.core.util.CollectionsUtil` | `List<O> removeDuplicate(Collection<O> objectCollection,String... propertyNames)` | 去重,返回指定属性 propertyNames 组合的值都不重复元素的新list (原集合对象不变) . |
| `com.feilong.core.util.CollectionsUtil` | `List<O> select(Iterable<O> beanIterable,Function<O, V> propertyExtractor,V... propertyValues)` | 循环 beanIterable ,获得元素 bean 的 propertyExtractor 的值,判断是否在 propertyValues 数组中;如果在,将该对象存入list中返回. 函数式版本 - 通过属性提取器选择元素 类型安全，无需反射 |
| `com.feilong.core.util.CollectionsUtil` | `List<O> select(Iterable<O> beanIterable,Map<String, ?> propertyNameAndPropertyValueMap)` | 找到 iterable 中,属性和属性值都是propertyNameAndPropertyValueMap的对应元素. |
| `com.feilong.core.util.CollectionsUtil` | `List<O> select(Iterable<O> beanIterable,Predicate<O> predicate)` | 按照指定的 Predicate,返回查询出来的集合. |
| `com.feilong.core.util.CollectionsUtil` | `List<O> select(Iterable<O> beanIterable,String propertyName,Collection<V> propertyValueList)` | 循环 beanIterable ,获得元素 bean 的 propertyName 的值,判断是否在 propertyValueList 集合中;如果在,将该对象存入list中返回. |
| `com.feilong.core.util.CollectionsUtil` | `List<O> select(Iterable<O> beanIterable,String propertyName,V... propertyValues)` | 循环 beanIterable ,获得元素 bean 的 propertyName 的值,判断是否在 propertyValues 数组中;如果在,将该对象存入list中返回. |
| `com.feilong.core.util.CollectionsUtil` | `List<O> selectRejected(Iterable<O> beanIterable,Map<String, ?> propertyNameAndPropertyValueMap)` | 找到 iterable 中,属性和属性值都 不是 propertyNameAndPropertyValueMap的对应元素. |
| `com.feilong.core.util.CollectionsUtil` | `List<O> selectRejected(Iterable<O> beanIterable,Predicate<O> predicate)` | 循环 beanIterable ,获得元素 bean ,判断是否不匹配 predicate , 如果不匹配 ,将该对象存入list中返回. |
| `com.feilong.core.util.CollectionsUtil` | `List<O> selectRejected(Iterable<O> beanIterable,String propertyName,Collection<V> propertyValueList)` | 循环 beanIterable ,获得元素 bean 的 propertyName 的值,判断是否不在 propertyValueList 集合中; 如果不在 ,将该对象存入list中返回. |
| `com.feilong.core.util.CollectionsUtil` | `List<O> selectRejected(Iterable<O> beanIterable,String propertyName,V... propertyValues)` | 循环 beanIterable ,获得元素 bean 的 propertyName 属性值 都不在 propertyValues 时候的list. |
| `com.feilong.core.util.CollectionsUtil` | `List<T> collect(final Iterable<O> inputIterable,final Transformer<? super O, ? extends T> transformer)` | 循环 inputIterable ,将每个元素使用 transformer 转换成新的对象,返回 新的list . |
| `com.feilong.core.util.CollectionsUtil` | `List<T> collect(final Iterator<O> inputIterator,final Transformer<? super O, ? extends T> transformer)` | 循环 inputIterator ,将每个元素使用 transformer 转换成新的对象 返回 新的list . |
| `com.feilong.core.util.CollectionsUtil` | `List<T> getPropertyValueList(Collection<O> beanIterable,Function<O, T> mapper)` | 循环集合 beanIterable ,用对象指定的 mapper 的值,拼成List(ArrayList). |
| `com.feilong.core.util.CollectionsUtil` | `List<T> getPropertyValueList(Iterable<O> beanIterable,String propertyName)` | 循环集合 beanIterable ,取到对象指定的属性 propertyName 的值,拼成List(ArrayList). |
| `com.feilong.core.util.CollectionsUtil` | `List<T> getPropertyValueList(Iterable<O> beanIterable,String propertyName,Class<T> returnElementClass)` | 循环集合 beanIterable ,取到对象指定的属性 propertyName 的值,将值转换成 returnElementClass 类型,拼成List(ArrayList). |
| `com.feilong.core.util.CollectionsUtil` | `Map<K, V> getPropertyValueMap(Iterable<O> beanIterable,Function<O, K> keyMapper,Function<O, V> valueMapper)` | 循环 beanIterable ,通过 keyMapper 函数提取key, 通过 valueMapper 函数提取value,组成map返回. |
| `com.feilong.core.util.CollectionsUtil` | `Map<K, V> getPropertyValueMap(Iterable<O> beanIterable,String keyPropertyName,String valuePropertyName)` | 循环 beanIterable ,以 keyPropertyName 属性值为key, valuePropertyName 属性值为value,组成map返回. |
| `com.feilong.core.util.CollectionsUtil` | `Map<T, List<O>> group(Iterable<O> beanIterable,Predicate<O> includePredicate,Transformer<O, T> keyTransformer)` | 循环 beanIterable ,找到符合条件的 includePredicate 的元素,将元素使用 keyTransformer 转成key ,相同值的元素组成list作为value,封装成map返回. |
| `com.feilong.core.util.CollectionsUtil` | `Map<T, List<O>> group(Iterable<O> beanIterable,String propertyName)` | 循环 beanIterable ,以 元素的 propertyName 属性值为key,相同值的元素组成list作为value,封装成map返回. |
| `com.feilong.core.util.CollectionsUtil` | `Map<T, List<O>> group(Iterable<O> beanIterable,Transformer<O, T> keyTransformer)` | 循环 beanIterable ,将元素使用 keyTransformer 转成key,相同值的元素组成list作为value,封装成map返回. |
| `com.feilong.core.util.CollectionsUtil` | `Map<T, List<O>> group(Iterable<O> beanIterable,final String propertyName,Predicate<O> includePredicate)` | 循环 beanIterable ,找到符合条件的 includePredicate 的元素,以元素的 propertyName 属性值为key,相同值的元素组成list作为value,封装成map返回. |
| `com.feilong.core.util.CollectionsUtil` | `Map<T, O> groupOne(Iterable<O> beanIterable,Function<O, T> keyExtractor)` | 使用 Lambda 和 Stream 实现分组,保留重复键的第一个元素,提高了类型安全性和性能,避免了反射开销. 接受一个Iterable, 使用一个函数来提取键分组时,如果键重复,只保留第一个对象 |
| `com.feilong.core.util.CollectionsUtil` | `Map<T, O> groupOne(Iterable<O> beanIterable,String propertyName)` | 循环 iterable ,以元素的 propertyName 属性值为key,元素为value,封装成map返回(map只put第一个匹配的元素, 后面出现相同的元素将会忽略 ). |
| `com.feilong.core.util.CollectionsUtil` | `O find(Iterable<O> beanIterable,Function<O, V> propertyValueExtractor,V propertyValue)` | 找到 iterable 中,第一个 propertyValueExtractor 属性值是 propertyValue 的对应元素. |
| `com.feilong.core.util.CollectionsUtil` | `O find(Iterable<O> beanIterable,Map<String, ?> propertyNameAndPropertyValueMap)` | 找到 iterable 中,第一个 propertyName 属性名称和值是 propertyValue 是 propertyNameAndPropertyValueMap 的对应元素. |
| `com.feilong.core.util.CollectionsUtil` | `O find(Iterable<O> beanIterable,String propertyName,V propertyValue)` | 找到 iterable 中,第一个 propertyName 属性名称值是 propertyValue 的对应元素. |
| `com.feilong.core.util.CollectionsUtil` | `O find(Iterable<O> iterable,Predicate<O> predicate)` | 迭代查找匹配 predicate 的第一个元素并返回. |
| `com.feilong.core.util.CollectionsUtil` | `Pair<List<O>, List<O>> splitDuplicate(Collection<O> objectCollection,String... propertyNames)` | 分隔集合,将新数据放left , 重复的数据放right. 请自行先进行排序处理 |
| `com.feilong.core.util.CollectionsUtil` | `Set<E> newHashSet()` | 创建 a mutable , empty newHashSet instance . |
| `com.feilong.core.util.CollectionsUtil` | `Set<E> newHashSet(Collection<? extends E> collection)` | 创建 a mutable , empty newHashSet instance . Constructs a new set containing the elements in the specified collection. The HashMap is created with default load factor (0.75) and an initial capacity sufficient to contain the elements in the specified collection. |
| `com.feilong.core.util.CollectionsUtil` | `Set<E> newLinkedHashSet()` | 创建 a mutable , empty LinkedHashSet instance . |
| `com.feilong.core.util.CollectionsUtil` | `Set<E> newLinkedHashSet(Collection<? extends E> collection)` | 【原文待译】Constructs a new linked hash set with the same elements as the specified collection. The linked hash set is created with an initial capacity sufficient to hold the elements in the specified collection and the default load factor (0.75). |
| `com.feilong.core.util.CollectionsUtil` | `Set<T> getPropertyValueSet(Collection<O> beanIterable,Function<O, T> mapper)` | 解析迭代集合 beanIterable ,取到对象指定的属性 mapper 的值,拼成(LinkedHashSet). |
| `com.feilong.core.util.CollectionsUtil` | `Set<T> getPropertyValueSet(Iterable<O> beanIterable,String propertyName)` | 解析迭代集合 beanIterable ,取到对象指定的属性 propertyName 的值,拼成Set(LinkedHashSet). |
| `com.feilong.core.util.CollectionsUtil` | `Set<T> getPropertyValueSet(Iterable<O> beanIterable,String propertyName,Class<T> returnElementClass)` | 解析迭代集合 beanIterable ,取到对象指定的属性 propertyName 的值,将值转换成 returnElementClass 类型,拼成Set(LinkedHashSet). |
| `com.feilong.core.util.CollectionsUtil` | `T first(final Iterable<T> iterable)` | Shortcut for get(iterator, 0). 返回 iterable Iterator 里面的第一个元素,如果没有,会抛出 IndexOutOfBoundsException . 如果 Iterable是个 List, 会使用 List#get(int). |
| `com.feilong.core.util.CollectionsUtil` | `T get(final Iterable<T> iterable,final int index)` | Returns the index -th value in the iterable 's Iterator, throwing IndexOutOfBoundsException if there is no such element. 如果 Iterable是个 List, 会使用 List#get(int). |
| `com.feilong.core.util.CollectionsUtil` | `T last(final Iterable<T> iterable)` | 返回 iterable Iterator 里面的最后元素,如果没有,会抛出 IndexOutOfBoundsException . 如果 Iterable是个 List, 会使用 List#get(int). |
| `com.feilong.core.util.CollectionsUtil` | `boolean addAllIgnoreNull(final Collection<O> objectCollection,final Iterable<? extends O> iterable)` | 添加所有的Iterable元素到指定的 objectCollection ,如果 iterable是null将忽略. |
| `com.feilong.core.util.CollectionsUtil` | `boolean addIfCondition(final Collection<T> objectCollection,final T element,boolean condition)` | 在condition 是true的情况下, 添加 element 元素到指定的 objectCollection . |
| `com.feilong.core.util.CollectionsUtil` | `boolean addIgnoreNullOrEmpty(final Collection<T> objectCollection,final Iterable<T> elementIterable)` | 添加 elementIterable 里面的元素到指定的 objectCollection ,如果其中 element null或者 empty元素将忽略. |
| `com.feilong.core.util.CollectionsUtil` | `boolean addIgnoreNullOrEmpty(final Collection<T> objectCollection,final T... elements)` | 添加一堆 elements 元素到指定的 objectCollection ,如果其中 element null或者 empty元素将忽略. |
| `com.feilong.core.util.CollectionsUtil` | `boolean contains(final Iterable<T> iterable,final T element)` | 循环 iterable , 判断元素和参数 element 是否equals, 如果有equals,那么返回true,否则返回false. 使用循环每个元素,然后equals判断 |
| `com.feilong.core.util.CollectionsUtil` | `boolean containsAny(final Iterable<T> iterable,final T... elements)` | 循环 iterable , 判断元素和参数 elements 是否有equals, 如果任何一个equals,那么返回true,否则返回false. 使用循环每个元素,然后equals判断 |
| `com.feilong.core.util.CollectionsUtil` | `boolean containsTrimAndIgnoreCase(final Iterable<String> iterable,final String element)` | 循环 iterable , 判断元素和参数 element 去空且忽视大小写后是否相等, 如果有相等的,那么返回true. |
| `com.feilong.core.util.CollectionsUtil` | `boolean exist(Iterable<O> beanIterable,Map<String, ?> propertyNameAndPropertyValueMap)` | 判断是否存在 iterable 中, propertyName 属性名称和值是 propertyValue 是 propertyNameAndPropertyValueMap 的对应元素. |
| `com.feilong.core.util.CollectionsUtil` | `boolean exist(Iterable<O> beanIterable,String propertyName,V propertyValue)` | 判断 iterable 中,是否存在 propertyName 属性名称值是 propertyValue 的元素. |
| `com.feilong.core.util.CollectionsUtil` | `boolean exist(Iterable<O> iterable,Predicate<O> predicate)` | 判断是否存在匹配 predicate 的元素. |
| `com.feilong.core.util.CollectionsUtil` | `int indexOf(List<O> list,String propertyName,V propertyValue)` | 在 list 中,查找第一个属性 propertyName 值是指定值 propertyValue 对象的索引位置. |
| `com.feilong.core.util.CollectionsUtil` | `int size(final Object object)` | 返回object 元素的大小. 支持object 如下类型: Collection - the collection size Map - the map size Array - the array size Iterator - the number of elements remaining in the iterator Iterable - the number of elements remaining in the iterator Enumeration - the number of elements remaining in the enumeration 如果 objec… |
| `com.feilong.core.util.CollectionsUtil` | `void forEach(final Iterable<O> beanIterable,String propertyName,Object propertyValue)` | 循环将 beanIterable 每个元素的每个指定属性 propertyName 的值改成 propertyValue . |
| `com.feilong.core.util.CollectionsUtil` | `void setIfCondition(final List<T> objectList,int index,final T element,boolean condition)` | 在condition 是true的情况下, 设置 objectList 指定index为 element 元素. |
| `com.feilong.core.util.EnumerationUtil` | `boolean contains(Enumeration<O> enumeration,O value)` | 判断 enumeration 枚举里面,是否有指定的元素 value . |
| `com.feilong.core.util.MapUtil` | `C getSubSumValue(Map<K, T> map,Iterable<K> keys,Class<C> klass)` | 提取map中指定的key 的value,累加起来,按照制定的 klass 类型返回. |
| `com.feilong.core.util.MapUtil` | `Map.Entry<K, V> get(Map<K, V> map,int index)` | 根据索引来获得map 的entry. |
| `com.feilong.core.util.MapUtil` | `Map<K, BigDecimal> putSumValue(Map<K, BigDecimal> map,K key,Number value)` | 将 key 和 value 累加的形式put到 map中,如果 map 中存在 key ,那么累加 value 值;如果不存在那么直接put. 常用于数据统计, 比如 com.feilong.core.util.AggregateUtil#groupSum(Iterable, String, String) |
| `com.feilong.core.util.MapUtil` | `Map<K, Integer> putSumValue(Map<K, Integer> map,K key,Integer value)` | 将 key 和 value 累加的形式put到 map中,如果 map 中存在 key ,那么累加 value 值;如果不存在那么直接put. |
| `com.feilong.core.util.MapUtil` | `Map<K, List<V>> putMultiValue(Map<K, List<V>> map,K key,V value)` | 往 map 中put 指定 key value(多值形式). |
| `com.feilong.core.util.MapUtil` | `Map<K, String[]> toArrayValueMap(Map<K, String> singleValueMap)` | 将单值的 singleValueMap 转成多值的map. |
| `com.feilong.core.util.MapUtil` | `Map<K, T> getSubMap(Map<K, T> map,Iterable<K> keys)` | 获得一个 map 中,按照指定的 keys 整理成新的map. |
| `com.feilong.core.util.MapUtil` | `Map<K, T> getSubMap(Map<K, T> map,K... keys)` | 获得一个 map 中,按照指定的 keys 整理成新的map. |
| `com.feilong.core.util.MapUtil` | `Map<K, T> getSubMapExcludeKeys(Map<K, T> map,Iterable<K> excludeKeys)` | 获得 sub map(排除指定的 excludeKeys). |
| `com.feilong.core.util.MapUtil` | `Map<K, T> getSubMapExcludeKeys(Map<K, T> map,K... excludeKeys)` | 获得 sub map(排除指定的 excludeKeys). |
| `com.feilong.core.util.MapUtil` | `Map<K, T> getSubMapExcludeValues(Map<K, T> map,T... excludeValues)` | 获得 sub map(排除指定的 value). |
| `com.feilong.core.util.MapUtil` | `Map<K, V> extractSubMap(Map<K, O> map,K[] includeKeys,String extractPropertyName)` | 以参数 map 的key为key,以参数 map value的指定 extractPropertyName 属性值为值,拼装成新的map返回. |
| `com.feilong.core.util.MapUtil` | `Map<K, V> extractSubMap(Map<K, O> map,String extractPropertyName)` | 以参数 map 的key为key,以参数 map value的指定 extractPropertyName 属性值为值,拼装成新的map返回. |
| `com.feilong.core.util.MapUtil` | `Map<K, V> newConcurrentHashMap()` | 【原文待译】New concurrent hash map. |
| `com.feilong.core.util.MapUtil` | `Map<K, V> newConcurrentHashMap(Map<K, V> map)` | 【原文待译】New concurrent hash map. |
| `com.feilong.core.util.MapUtil` | `Map<K, V> newConcurrentHashMap(int expectedSize)` | 创建 ConcurrentHashMap实例,拥有足够的 "initial capacity" 应该控制expectedSize elements without growth. This behavior cannot be broadly guaranteed, but it is observed to be true for OpenJDK 1.7. It also can't be guaranteed that the method isn't inadvertently oversizing the returned map. |
| `com.feilong.core.util.MapUtil` | `Map<K, V> newHashMap()` | 创建 HashMap实例. |
| `com.feilong.core.util.MapUtil` | `Map<K, V> newHashMap(Map<K, V> map)` | 【原文待译】New hash map. |
| `com.feilong.core.util.MapUtil` | `Map<K, V> newHashMap(int expectedSize)` | 创建 HashMap实例,拥有足够的 "initial capacity" 应该控制expectedSize elements without growth. This behavior cannot be broadly guaranteed, but it is observed to be true for OpenJDK 1.7. It also can't be guaranteed that the method isn't inadvertently oversizing the returned map. |
| `com.feilong.core.util.MapUtil` | `Map<K, V> newLinkedHashMap()` | 创建 LinkedHashMap实例. |
| `com.feilong.core.util.MapUtil` | `Map<K, V> newLinkedHashMap(Iterable<K> keys,V value)` | 基于keys 创建指定value的 LinkedHashMap实例. |
| `com.feilong.core.util.MapUtil` | `Map<K, V> newLinkedHashMap(Map<K, V> map)` | 【原文待译】New linked hash map. |
| `com.feilong.core.util.MapUtil` | `Map<K, V> newLinkedHashMap(int expectedSize)` | 创建 LinkedHashMap实例,拥有足够的 "initial capacity" 应该控制expectedSize elements without growth. This behavior cannot be broadly guaranteed, but it is observed to be true for OpenJDK 1.7. It also can't be guaranteed that the method isn't inadvertently oversizing the returned map. |
| `com.feilong.core.util.MapUtil` | `Map<K, V> newTreeMap()` | 【原文待译】New tree map. |
| `com.feilong.core.util.MapUtil` | `Map<K, V> newTreeMap(Map<K, V> map)` | 【原文待译】New tree map. |
| `com.feilong.core.util.MapUtil` | `Map<K, V> removeKeys(Map<K, V> map,Collection<K> keyList)` | 删除 map 的指定的 keyList . |
| `com.feilong.core.util.MapUtil` | `Map<K, V> removeKeys(Map<K, V> map,K... keys)` | 删除 map 的指定的 keys . |
| `com.feilong.core.util.MapUtil` | `Map<K, V> toSingleValueMap(Map<K, V[]> arrayValueMap)` | 将多值的 arrayValueMap 转成单值的map. |
| `com.feilong.core.util.MapUtil` | `Map<K, V[]> toArrayValueMap(Map<K, T> singleValueMap,Class<V> arrayComponentType)` | 将单值的 singleValueMap 转成多值的map. |
| `com.feilong.core.util.MapUtil` | `Map<T, V> extractIntersectionKeyDifferentValueMap(Map<T, V> targetMap,Map<T, I> toBeComparedMap)` | 提取 key 交集, 但是值不同的map 从targetMap 中, 提取key在toBeComparedMap,但是值即使转换成相同类型后还是不相等的数据 注意, 返回的是基于targetMap走的, 值的类型也是 targetMap value 类型 |
| `com.feilong.core.util.MapUtil` | `Map<V, K> invertMap(Map<K, V> map)` | 将 map 的key和value互转. |
| `com.feilong.core.util.MapUtil` | `String getDefaultEmptyStringIfNull(Map<K, V> map,K key)` | 获取value. |
| `com.feilong.core.util.MapUtil` | `V computeIfAbsent(Map<K, V> map,K key,Function<? super K, ? extends V> mappingFunction)` | 核心功能是"懒加载"——当Map中不存在某个key时，自动调用函数生成value并存入Map。这个设计模式在编程中很常见，但Java 8将其封装成了标准方法. 用于简化 ​键不存在时的值初始化与惰性计算，核心逻辑是“按需生成值并原子性插入” If the specified key is not already associated with a value (or is mapped to null), attempts to compute its value using the given mapping function and enters it into this map unle… |
| `com.feilong.core.util.MapUtil` | `V get(Map<K, V> map,K key)` | 获取value. 取值前,判断了map是否是null,如果是null直接返回null |
| `com.feilong.core.util.MapUtil` | `V getOrDefault(Map<K, V> map,K key,V defaultValue)` | 获取value. 取值前,判断了map是否是null,如果是null直接返回null |
| `com.feilong.core.util.MapUtil` | `void putAllIfNotNull(final Map<K, V> map,Map<? extends K, ? extends V> m)` | 仅当 null != map && null != m,才会进行 map.putAll(m) 操作 |
| `com.feilong.core.util.MapUtil` | `void putIfValueNotNull(final Map<K, V> map,final K key,final V value)` | 仅当 null != map 并且 null != value 才将key/value put到map中. |
| `com.feilong.core.util.MapUtil` | `void putIfValueNotNullOrEmpty(final Map<K, V> map,final K key,final V value)` | 仅当 null != map 并且 isNotNullOrEmpty(value) 才将key/value put到map中. |
| `com.feilong.core.util.RandomUtil` | `String createRandomFromString(String str,int length)` | 随机抽取字符串 char ,拼接成指定长度 length 的字符串. |
| `com.feilong.core.util.RandomUtil` | `String createRandomString(int length)` | 从com.feilong.core.Alphabet#DECIMAL_AND_LOWERCASE_LETTERS_DISTINGUISHABLE Alphabet.DECIMAL_AND_LOWERCASE_LETTERS_DISTINGUISHABLE 随机抽取字符串,拼接成指定长度 length 的字符串. |
| `com.feilong.core.util.RandomUtil` | `long createRandomWithLength(int length)` | 生成一个指定长度 length 的 随机正整数 . |
| `com.feilong.core.util.RegexUtil` | `Map<Integer, String> group(final String regexPattern,final CharSequence input)` | 返回在以前匹配操作期间由给定组捕获的输入子序列. 对于匹配器 m、输入序列 s 和组索引 g,表达式 m.group(g) 和 s.substring(m.start(g), m.end(g))是等效的. 捕获组是从 1开始从左到右的索引.组0表示整个模式,因此表达式 m.group(0)等效于 m.group(). |
| `com.feilong.core.util.RegexUtil` | `Pattern buildPattern(final String regexPattern,final int flags)` | 如果cache中有,那么直接返回, 如果没有构造一个并塞到cache中. |
| `com.feilong.core.util.RegexUtil` | `String group(final String regexPattern,final CharSequence input,final int groupNo)` | 返回在以前匹配操作期间由给定组捕获的输入子序列. 对于匹配器 m、输入序列 s 和组索引 g,表达式 m.group(g) 和 s.substring(m.start(g), m.end(g))是等效的. 捕获组是从 1开始从左到右的索引.组0表示整个模式,因此表达式 m.group(0)等效于 m.group(). |
| `com.feilong.core.util.RegexUtil` | `boolean matches(final String regexPattern,final CharSequence input)` | 编译给定正则表达式 regexPattern ,并尝试将给定输入 input 与其匹配. Pattern#matches(String, CharSequence) 等价于#getMatcher(String, CharSequence).matches(); |
| `com.feilong.core.util.ResourceBundleUtil` | `Map<String, String> toMap(ResourceBundle resourceBundle)` | 将 resourceBundle 转成map. |
| `com.feilong.core.util.ResourceBundleUtil` | `Map<String, String> toMap(String... baseNames)` | 解析 baseNamess 成map. |
| `com.feilong.core.util.ResourceBundleUtil` | `Properties toProperties(ResourceBundle resourceBundle)` | 将 resourceBundle 转成Properties. |
| `com.feilong.core.util.ResourceBundleUtil` | `ResourceBundle getResourceBundle(InputStream inputStream)` | 获得ResourceBundle(PropertyResourceBundle),新增这个方法的初衷是为了能读取任意的资源(包括本地file等). |
| `com.feilong.core.util.ResourceBundleUtil` | `ResourceBundle getResourceBundle(String baseName)` | 使用 Locale#getDefault() 获得ResourceBundle. |
| `com.feilong.core.util.ResourceBundleUtil` | `ResourceBundle getResourceBundle(String baseName,Locale locale)` | 使用 baseName 和 locale 获得ResourceBundle. |
| `com.feilong.core.util.ResourceBundleUtil` | `String getValue(ResourceBundle resourceBundle,String key,Object... arguments)` | 获取 resourceBundle 配置文件指定 key 键的值. |
| `com.feilong.core.util.ResourceBundleUtil` | `T toAliasBean(ResourceBundle resourceBundle,Class<T> aliasBeanClass)` | 将 resourceBundle 转换成 aliasBean . |
| `com.feilong.core.util.ResourceBundleUtil` | `T toBean(ResourceBundle resourceBundle,Class<T> beanClass)` | 读取 resourceBundle 转换成 bean . |
| `com.feilong.core.util.ResourceBundleUtil` | `T toBean(String baseName,Class<T> beanClass)` | 读取 baseName 转换成 bean . |
| `com.feilong.core.util.ServiceLoaderUtil` | `T loadFirst(Class<T> spiClass)` | 获取接口的首个 SPI 实现. |
| `com.feilong.core.util.SortUtil` | `List<O> sortList(List<O> list,Comparator<O>... comparators)` | 对集合 list ,使用指定的 comparators 进行排序. |
| `com.feilong.core.util.SortUtil` | `List<O> sortListByFixedOrderPropertyValueArray(List<O> list,String propertyName,V... propertyValues)` | 对 集合 list ,属性 propertyName 按照固定顺序值 propertyValues 进行排序. |
| `com.feilong.core.util.SortUtil` | `List<O> sortListByFixedOrderPropertyValueList(List<O> list,String propertyName,List<V> propertyValues)` | 对 集合 list ,属性 propertyName 按照固定顺序值 propertyValues 进行排序. |
| `com.feilong.core.util.SortUtil` | `List<O> sortListByPropertyNamesValue(List<O> list,String... propertyNameAndOrders)` | 对集合 list ,按照指定属性的值(组合)进行排序. |
| `com.feilong.core.util.SortUtil` | `List<T> sortList(List<T> list)` | 对 集合 list 进行排序. |
| `com.feilong.core.util.SortUtil` | `List<T> sortListByFixedOrderArray(List<T> list,T... fixedOrderItems)` | 对 集合 list 按照指定的固定顺序 fixedOrderItems 进行排序. |
| `com.feilong.core.util.SortUtil` | `List<T> sortListByFixedOrderList(List<T> list,List<T> fixedOrderItemList)` | 对 集合 list 按照指定的固定顺序 fixedOrderItemList 进行排序. |
| `com.feilong.core.util.SortUtil` | `Map<K, V> sortMap(Map<K, V> map,Comparator<Map.Entry<K, V>> mapEntryComparator)` | 使用 基于 java.util.Map.Entry Entry 的 mapEntryComparator 来对 map 进行排序. |
| `com.feilong.core.util.SortUtil` | `Map<K, V> sortMapByKeyAsc(Map<K, V> map)` | 按照key asc顺序排序. |
| `com.feilong.core.util.SortUtil` | `Map<K, V> sortMapByKeyDesc(Map<K, V> map)` | 按照key desc 倒序排序. |
| `com.feilong.core.util.SortUtil` | `Map<K, V> sortMapByKeyFixOrder(Map<K, V> map,K... keys)` | 按照key 指定名字顺序排序. |
| `com.feilong.core.util.SortUtil` | `Map<K, V> sortMapByValueAsc(Map<K, V> map)` | 根据value 来顺序排序(asc). |
| `com.feilong.core.util.SortUtil` | `Map<K, V> sortMapByValueDesc(Map<K, V> map)` | 根据value 来倒序排序(desc). |
| `com.feilong.core.util.SortUtil` | `T[] sortArray(T[] arrays)` | 对 数组 arrays 进行排序. |
| `com.feilong.core.util.SortUtil` | `T[] sortArray(T[] arrays,Comparator<T>... comparators)` | 对 数组 arrays 使用 comparator 进行排序. |
