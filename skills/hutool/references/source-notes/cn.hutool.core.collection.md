# cn.hutool.core.collection

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.collection.ArrayIter` | `E next()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.ArrayIter` | `Object getArray()` | 获得原始数组对象 |
| `cn.hutool.core.collection.ArrayIter` | `boolean hasNext()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.ArrayIter` | `void remove()` | 不允许操作数组元素 |
| `cn.hutool.core.collection.ArrayIter` | `void reset()` | 重置数组位置 |
| `cn.hutool.core.collection.AvgPartition` | `List<T> get(int index)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.AvgPartition` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.BoundedPriorityQueue` | `ArrayList<E> toList()` | @return 返回排序后的列表 |
| `cn.hutool.core.collection.BoundedPriorityQueue` | `Iterator<E> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.BoundedPriorityQueue` | `boolean addAll(E[] c)` | 添加多个元素 参数为集合的情况请使用PriorityQueue#addAll |
| `cn.hutool.core.collection.BoundedPriorityQueue` | `boolean offer(E e)` | 加入元素，当队列满时，淘汰末尾元素 |
| `cn.hutool.core.collection.CollStreamUtil` | `List<T> toList(Collection<E> collection,Function<E, T> function)` | 将collection转化为List集合，但是两者的泛型不同 Collection ------> List |
| `cn.hutool.core.collection.CollStreamUtil` | `List<T> toList(Collection<E> collection,Function<E, T> function,boolean isParallel)` | 将collection转化为List集合，但是两者的泛型不同 Collection ------> List |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<K, D> groupBy(Collection<E> collection,Function<E, K> key,Collector<E, ?, D> downstream)` | 作为所有groupingBy的公共方法，更接近于原生，灵活性更强 |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<K, D> groupBy(Collection<E> collection,Function<E, K> key,Collector<E, ?, D> downstream,boolean isParallel)` | 作为所有groupingBy的公共方法，更接近于原生，灵活性更强 |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<K, List<E>> groupByKey(Collection<E> collection,Function<E, K> key)` | 将collection按照规则(比如有相同的班级id)分组成map Collection -------> Map > |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<K, List<E>> groupByKey(Collection<E> collection,Function<E, K> key,boolean isParallel)` | 将collection按照规则(比如有相同的班级id)分组成map Collection -------> Map > |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<K, List<V>> groupKeyValue(Collection<E> collection,Function<E, K> key,Function<E, V> value)` | 将collection按照规则(比如有相同的班级id)分组成map，map中的key为班级id，value为班级名 Collection -------> Map > |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<K, List<V>> groupKeyValue(Collection<E> collection,Function<E, K> key,Function<E, V> value,boolean isParallel)` | 将collection按照规则(比如有相同的班级id)分组成map，map中的key为班级id，value为班级名 Collection -------> Map > |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<K, Map<U, List<E>>> groupBy2Key(Collection<E> collection,Function<E, K> key1,Function<E, U> key2)` | 将collection按照两个规则(比如有相同的年级id,班级id)分组成双层map Collection ---> Map >> |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<K, Map<U, List<E>>> groupBy2Key(Collection<E> collection,Function<E, K> key1,Function<E, U> key2,boolean isParallel)` | 将collection按照两个规则(比如有相同的年级id,班级id)分组成双层map Collection ---> Map >> |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<K, V> merge(Map<K, X> map1,Map<K, Y> map2,BiFunction<X, Y, V> merge)` | 合并两个相同key类型的map |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<K, V> toIdentityMap(Collection<V> collection,Function<V, K> key)` | 将collection转化为类型不变的map Collection ----> Map |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<K, V> toIdentityMap(Collection<V> collection,Function<V, K> key,boolean isParallel)` | 将collection转化为类型不变的map Collection ----> Map |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<K, V> toMap(Collection<E> collection,Function<E, K> key,Function<E, V> value)` | 将Collection转化为map(value类型与collection的泛型不同) Collection -----> Map |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<K, V> toMap(Collection<E> collection,Function<E, K> key,Function<E, V> value,boolean isParallel)` | @param collection 需要转化的集合 |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<T, Map<U, E>> group2Map(Collection<E> collection,Function<E, T> key1,Function<E, U> key2)` | 将collection按照两个规则(比如有相同的年级id,班级id)分组成双层map Collection ---> Map > |
| `cn.hutool.core.collection.CollStreamUtil` | `Map<T, Map<U, E>> group2Map(Collection<E> collection,Function<E, T> key1,Function<E, U> key2,boolean isParallel)` | 将collection按照两个规则(比如有相同的年级id,班级id)分组成双层map Collection ---> Map > |
| `cn.hutool.core.collection.CollStreamUtil` | `Set<T> toSet(Collection<E> collection,Function<E, T> function)` | 将collection转化为Set集合，但是两者的泛型不同 Collection ------> Set |
| `cn.hutool.core.collection.CollStreamUtil` | `Set<T> toSet(Collection<E> collection,Function<E, T> function,boolean isParallel)` | 将collection转化为Set集合，但是两者的泛型不同 Collection ------> Set |
| `cn.hutool.core.collection.CollUtil` | `ArrayList<T> distinct(Collection<T> collection)` | 去重集合 |
| `cn.hutool.core.collection.CollUtil` | `ArrayList<T> newArrayList(Collection<T> collection)` | 新建一个ArrayList |
| `cn.hutool.core.collection.CollUtil` | `ArrayList<T> newArrayList(Enumeration<T> enumeration)` | 新建一个ArrayList 提供的参数为null时返回空ArrayList |
| `cn.hutool.core.collection.CollUtil` | `ArrayList<T> newArrayList(Iterable<T> iterable)` | 新建一个ArrayList 提供的参数为null时返回空ArrayList |
| `cn.hutool.core.collection.CollUtil` | `ArrayList<T> newArrayList(Iterator<T> iterator)` | 新建一个ArrayList 提供的参数为null时返回空ArrayList |
| `cn.hutool.core.collection.CollUtil` | `ArrayList<T> newArrayList(T... values)` | 新建一个ArrayList |
| `cn.hutool.core.collection.CollUtil` | `ArrayList<T> toList(T... values)` | 数组转为ArrayList |
| `cn.hutool.core.collection.CollUtil` | `ArrayList<V> valuesOfKeys(Map<K, V> map,Iterable<K> keys)` | 从Map中获取指定键列表对应的值列表 如果key在map中不存在或key对应值为null，则返回值列表对应位置的值也为null |
| `cn.hutool.core.collection.CollUtil` | `ArrayList<V> valuesOfKeys(Map<K, V> map,Iterator<K> keys)` | 从Map中获取指定键列表对应的值列表 如果key在map中不存在或key对应值为null，则返回值列表对应位置的值也为null |
| `cn.hutool.core.collection.CollUtil` | `ArrayList<V> valuesOfKeys(Map<K, V> map,K... keys)` | 从Map中获取指定键列表对应的值列表 如果key在map中不存在或key对应值为null，则返回值列表对应位置的值也为null |
| `cn.hutool.core.collection.CollUtil` | `BlockingQueue<T> newBlockingQueue(int capacity,boolean isLinked)` | 新建BlockingQueue 在队列为空时，获取元素的线程会等待队列变为非空。当队列满时，存储元素的线程会等待队列可用。 |
| `cn.hutool.core.collection.CollUtil` | `Class<?> getElementType(Iterable<?> iterable)` | 获得Iterable对象的元素类型（通过第一个非空元素判断） |
| `cn.hutool.core.collection.CollUtil` | `Class<?> getElementType(Iterator<?> iterator)` | 获得Iterator对象的元素类型（通过第一个非空元素判断） |
| `cn.hutool.core.collection.CollUtil` | `Collection<E> toCollection(Iterable<E> iterable)` | Iterable转为Collection 首先尝试强转，强转失败则构建一个新的ArrayList |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> addAll(Collection<T> collection,Enumeration<T> enumeration)` | 加入全部 |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> addAll(Collection<T> collection,Iterable<T> iterable)` | 加入全部 |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> addAll(Collection<T> collection,Iterator<T> iterator)` | 加入全部 |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> addAll(Collection<T> collection,Object value)` | 将指定对象全部加入到集合中 提供的对象如果为集合类型，会自动转换为目标元素类型 |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> addAll(Collection<T> collection,Object value,Type elementType)` | 将指定对象全部加入到集合中 提供的对象如果为集合类型，会自动转换为目标元素类型 如果为String，支持类似于[1,2,3,4] 或者 1,2,3,4 这种格式 |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> addAll(Collection<T> collection,T[] values)` | 加入全部 |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> create(Class<?> collectionType)` | 创建新的集合对象 |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> create(Class<?> collectionType,Class<T> elementType)` | 创建新的集合对象，返回具体的泛型集合 |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> disjunction(Collection<T> coll1,Collection<T> coll2)` | 两个集合的对称差集 (A-B)∪(B-A) 针对一个集合中存在多个相同元素的情况，计算两个集合中此元素的个数，保留两个集合中此元素个数差的个数 例如： |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> edit(Collection<T> collection,Editor<T> editor)` | 编辑，此方法产生一个新集合 编辑过程通过传入的Editor实现来返回需要的元素内容，这个Editor实现可以实现以下功能： |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> filterNew(Collection<T> collection,Filter<T> filter)` | 过滤 过滤过程通过传入的Filter实现来过滤返回需要的元素内容，这个Filter实现可以实现以下功能： |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> intersection(Collection<T> coll1,Collection<T> coll2)` | 两个集合的交集 针对一个集合中存在多个相同元素的情况，计算两个集合中此元素的个数，保留最少的个数 例如：集合1：[a, b, c, c, c]，集合2：[a, b, c, c] 结果：[a, b, c, c]，此结果中只保留了两个c |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> intersection(Collection<T> coll1,Collection<T> coll2,Collection<T>... otherColls)` | 多个集合的交集 针对一个集合中存在多个相同元素的情况，计算两个集合中此元素的个数，保留最少的个数 例如：集合1：[a, b, c, c, c]，集合2：[a, b, c, c] 结果：[a, b, c, c]，此结果中只保留了两个c |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> subtract(Collection<T> coll1,Collection<T> coll2)` | 计算集合的单差集，即只返回【集合1】中有，但是【集合2】中没有的元素，例如： |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> trans(Collection<F> collection,Function<? super F, ? extends T> function)` | 使用给定的转换函数，转换源集合为新类型的集合 |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> union(Collection<T> coll1,Collection<T> coll2)` | 两个集合的并集 针对一个集合中存在多个相同元素的情况，计算两个集合中此元素的个数，保留最多的个数 例如：集合1：[a, b, c, c, c]，集合2：[a, b, c, c] 结果：[a, b, c, c, c]，此结果中只保留了三个c |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> union(Collection<T> coll1,Collection<T> coll2,Collection<T>... otherColls)` | 多个集合的并集 针对一个集合中存在多个相同元素的情况，计算两个集合中此元素的个数，保留最多的个数 例如：集合1：[a, b, c, c, c]，集合2：[a, b, c, c] 结果：[a, b, c, c, c]，此结果中只保留了三个c |
| `cn.hutool.core.collection.CollUtil` | `Collection<T> unmodifiable(Collection<? extends T> c)` | 转为只读集合 |
| `cn.hutool.core.collection.CollUtil` | `CopyOnWriteArrayList<T> newCopyOnWriteArrayList(Collection<T> collection)` | 新建一个CopyOnWriteArrayList |
| `cn.hutool.core.collection.CollUtil` | `Enumeration<E> asEnumeration(Iterator<E> iter)` | Iterator转换为Enumeration Adapt the specified Iterator to the Enumeration interface. |
| `cn.hutool.core.collection.CollUtil` | `HashMap<K, V> toMap(Iterable<Entry<K, V>> entryIter)` | 将Entry集合转换为HashMap |
| `cn.hutool.core.collection.CollUtil` | `HashMap<Object, Object> toMap(Object[] array)` | 将数组转换为Map（HashMap），支持数组元素类型为： |
| `cn.hutool.core.collection.CollUtil` | `HashSet<T> newHashSet(Collection<T> collection)` | 新建一个HashSet |
| `cn.hutool.core.collection.CollUtil` | `HashSet<T> newHashSet(T... ts)` | 新建一个HashSet |
| `cn.hutool.core.collection.CollUtil` | `HashSet<T> newHashSet(boolean isSorted,Collection<T> collection)` | 新建一个HashSet |
| `cn.hutool.core.collection.CollUtil` | `HashSet<T> newHashSet(boolean isSorted,Enumeration<T> enumeration)` | 新建一个HashSet |
| `cn.hutool.core.collection.CollUtil` | `HashSet<T> newHashSet(boolean isSorted,Iterator<T> iter)` | 新建一个HashSet |
| `cn.hutool.core.collection.CollUtil` | `HashSet<T> set(boolean isSorted,T... ts)` | 新建一个HashSet |
| `cn.hutool.core.collection.CollUtil` | `Iterable<E> asIterable(final Iterator<E> iter)` | Iterator 转为 Iterable |
| `cn.hutool.core.collection.CollUtil` | `Iterator<E> asIterator(Enumeration<E> e)` | Enumeration转换为Iterator Adapt the specified Enumeration to the Iterator interface |
| `cn.hutool.core.collection.CollUtil` | `LinkedHashMap<K, V> sortByEntry(Map<K, V> map,Comparator<Map.Entry<K, V>> comparator)` | 通过Entry排序，可以按照键排序，也可以按照值排序，亦或者两者综合排序 |
| `cn.hutool.core.collection.CollUtil` | `LinkedHashMap<K, V> sortToMap(Collection<Map.Entry<K, V>> entryCollection,Comparator<Map.Entry<K, V>> comparator)` | 通过Entry排序，可以按照键排序，也可以按照值排序，亦或者两者综合排序 |
| `cn.hutool.core.collection.CollUtil` | `LinkedHashSet<T> newLinkedHashSet(T... ts)` | 新建一个LinkedHashSet |
| `cn.hutool.core.collection.CollUtil` | `LinkedList<T> newLinkedList(T... values)` | 新建LinkedList |
| `cn.hutool.core.collection.CollUtil` | `List<E> removeWithAddIf(T targetCollection,Predicate<? super E> predicate)` | 移除集合中的多个元素，并将结果存放到生成的新集合中后返回 此方法直接修改原集合 |
| `cn.hutool.core.collection.CollUtil` | `List<Entry<K, V>> sortEntryToList(Collection<Entry<K, V>> collection)` | 将Set排序（根据Entry的值） |
| `cn.hutool.core.collection.CollUtil` | `List<List<T>> group(Collection<T> collection,Hash32<T> hash)` | 分组，按照Hash32接口定义的hash算法，集合中的元素放入hash值对应的子列表中 |
| `cn.hutool.core.collection.CollUtil` | `List<List<T>> groupByField(Collection<T> collection,final String fieldName)` | 根据元素的指定字段名分组，非Bean都放在第一个分组中 |
| `cn.hutool.core.collection.CollUtil` | `List<List<T>> split(Collection<T> collection,int size)` | 对集合按照指定长度分段，每一个段为单独的集合，返回这个集合的列表 |
| `cn.hutool.core.collection.CollUtil` | `List<List<T>> splitList(List<T> list,int size)` | 对集合按照指定长度分段，每一个段为单独的集合，返回这个集合的列表 需要特别注意的是，此方法调用List#subList(int, int)切分List， 此方法返回的是原List的视图，也就是说原List有变更，切分后的结果也会变更。 |
| `cn.hutool.core.collection.CollUtil` | `List<Map<K, V>> toMapList(Map<K, ? extends Iterable<V>> listMap)` | 列转行。将Map中值列表分别按照其位置与key组成新的map。 是#toListMap(Iterable)的逆方法 比如传入数据： |
| `cn.hutool.core.collection.CollUtil` | `List<Object> extract(Iterable<?> collection,Editor<Object> editor)` | 通过Editor抽取集合元素中的某些值返回为新列表 例如提供的是一个Bean列表，通过Editor接口实现获取某个字段值，返回这个字段值组成的新列表 |
| `cn.hutool.core.collection.CollUtil` | `List<Object> extract(Iterable<?> collection,Editor<Object> editor,boolean ignoreNull)` | 通过Editor抽取集合元素中的某些值返回为新列表 例如提供的是一个Bean列表，通过Editor接口实现获取某个字段值，返回这个字段值组成的新列表 |
| `cn.hutool.core.collection.CollUtil` | `List<Object> getFieldValues(Iterable<?> collection,final String fieldName)` | 获取给定Bean列表中指定字段名对应字段值的列表 列表元素支持Bean与Map |
| `cn.hutool.core.collection.CollUtil` | `List<Object> getFieldValues(Iterable<?> collection,final String fieldName,boolean ignoreNull)` | 获取给定Bean列表中指定字段名对应字段值的列表 列表元素支持Bean与Map |
| `cn.hutool.core.collection.CollUtil` | `List<R> map(Iterable<T> collection,Function<? super T, ? extends R> func,boolean ignoreNull)` | 通过func自定义一个规则，此规则将原集合中的元素转换成新的元素，生成新的列表返回 例如提供的是一个Bean列表，通过Function接口实现获取某个字段值，返回这个字段值组成的新列表 |
| `cn.hutool.core.collection.CollUtil` | `List<String> sortByPinyin(Collection<String> collection)` | 根据汉字的拼音顺序排序 |
| `cn.hutool.core.collection.CollUtil` | `List<String> sortByPinyin(List<String> list)` | 根据汉字的拼音顺序排序 |
| `cn.hutool.core.collection.CollUtil` | `List<T> addAllIfNotContains(List<T> list,List<T> otherList)` | 将另一个列表中的元素加入到列表中，如果列表中已经存在此元素则忽略之 |
| `cn.hutool.core.collection.CollUtil` | `List<T> distinct(Collection<T> collection,Function<T, K> uniqueGenerator,boolean override)` | 根据函数生成的KEY去重集合，如根据Bean的某个或者某些字段完成去重。 去重可选是保留最先加入的值还是后加入的值 |
| `cn.hutool.core.collection.CollUtil` | `List<T> emptyIfNull(List<T> list)` | 如果提供的集合为null，返回一个不可变的默认空集合，否则返回原集合 空集合使用Collections#emptyList() |
| `cn.hutool.core.collection.CollUtil` | `List<T> getAny(Collection<T> collection,int... indexes)` | 获取集合中指定多个下标的元素值，下标可以为负数，例如-1表示最后一个元素 |
| `cn.hutool.core.collection.CollUtil` | `List<T> getFieldValues(Iterable<?> collection,final String fieldName,final Class<T> elementType)` | 获取给定Bean列表中指定字段名对应字段值的列表 列表元素支持Bean与Map |
| `cn.hutool.core.collection.CollUtil` | `List<T> list(boolean isLinked)` | 新建一个空List |
| `cn.hutool.core.collection.CollUtil` | `List<T> list(boolean isLinked,Collection<T> collection)` | 新建一个List |
| `cn.hutool.core.collection.CollUtil` | `List<T> list(boolean isLinked,Enumeration<T> enumeration)` | 新建一个List 提供的参数为null时返回空ArrayList |
| `cn.hutool.core.collection.CollUtil` | `List<T> list(boolean isLinked,Iterable<T> iterable)` | 新建一个List 提供的参数为null时返回空ArrayList |
| `cn.hutool.core.collection.CollUtil` | `List<T> list(boolean isLinked,Iterator<T> iter)` | 新建一个ArrayList 提供的参数为null时返回空ArrayList |
| `cn.hutool.core.collection.CollUtil` | `List<T> list(boolean isLinked,T... values)` | 新建一个List |
| `cn.hutool.core.collection.CollUtil` | `List<T> page(int pageNo,int pageSize,List<T> list)` | 对指定List分页取值 |
| `cn.hutool.core.collection.CollUtil` | `List<T> popPart(Deque<T> surplusAlaDatas,int partSize)` | 切取部分数据 切取后的栈将减少这些元素 |
| `cn.hutool.core.collection.CollUtil` | `List<T> popPart(Stack<T> surplusAlaDatas,int partSize)` | 切取部分数据 切取后的栈将减少这些元素 |
| `cn.hutool.core.collection.CollUtil` | `List<T> reverse(List<T> list)` | 反序给定List，会在原List基础上直接修改 |
| `cn.hutool.core.collection.CollUtil` | `List<T> reverseNew(List<T> list)` | 反序给定List，会创建一个新的List，原List数据不变 |
| `cn.hutool.core.collection.CollUtil` | `List<T> setOrAppend(List<T> list,int index,T element)` | 设置或增加元素。当index小于List的长度时，替换指定位置的值，否则在尾部追加 |
| `cn.hutool.core.collection.CollUtil` | `List<T> sort(Collection<T> collection,Comparator<? super T> comparator)` | 排序集合，排序不会修改原集合 |
| `cn.hutool.core.collection.CollUtil` | `List<T> sort(List<T> list,Comparator<? super T> c)` | 针对List排序，排序会修改原List |
| `cn.hutool.core.collection.CollUtil` | `List<T> sortByProperty(Collection<T> collection,String property)` | 根据Bean的属性排序 |
| `cn.hutool.core.collection.CollUtil` | `List<T> sortByProperty(List<T> list,String property)` | 根据Bean的属性排序 |
| `cn.hutool.core.collection.CollUtil` | `List<T> sortPageAll(int pageNo,int pageSize,Comparator<T> comparator,Collection<T>... colls)` | 将多个集合排序并显示不同的段落（分页） 采用BoundedPriorityQueue实现分页取局部 |
| `cn.hutool.core.collection.CollUtil` | `List<T> sub(Collection<T> collection,int start,int end)` | 截取集合的部分 |
| `cn.hutool.core.collection.CollUtil` | `List<T> sub(Collection<T> collection,int start,int end,int step)` | 截取集合的部分 |
| `cn.hutool.core.collection.CollUtil` | `List<T> sub(List<T> list,int start,int end)` | 截取列表的部分 |
| `cn.hutool.core.collection.CollUtil` | `List<T> sub(List<T> list,int start,int end,int step)` | 截取列表的部分 |
| `cn.hutool.core.collection.CollUtil` | `List<T> subtractToList(Collection<T> coll1,Collection<T> coll2)` | 计算集合的单差集，即只返回【集合1】中有，但是【集合2】中没有的元素，例如： |
| `cn.hutool.core.collection.CollUtil` | `List<T> subtractToList(Collection<T> coll1,Collection<T> coll2,boolean isLinked)` | 计算集合的单差集，即只返回【集合1】中有，但是【集合2】中没有的元素 只要【集合1】中的某个元素在【集合2】中存在（equals和hashcode），就会被排除 |
| `cn.hutool.core.collection.CollUtil` | `List<T> unionAll(Collection<T> coll1,Collection<T> coll2,Collection<T>... otherColls)` | 多个集合的完全并集，类似于SQL中的“UNION ALL” 针对一个集合中存在多个相同元素的情况，保留全部元素 例如：集合1：[a, b, c, c, c]，集合2：[a, b, c, c] 结果：[a, b, c, c, c, a, b, c, c] |
| `cn.hutool.core.collection.CollUtil` | `List<V> values(Collection<Map<?, V>> mapCollection)` | 获取指定Map列表中所有的Value |
| `cn.hutool.core.collection.CollUtil` | `Map<K, List<V>> toListMap(Iterable<? extends Map<K, V>> mapList)` | 行转列，合并相同的键，值合并为列表 将Map列表中相同key的值组成列表做为Map的value 是#toMapList(Map)的逆方法 比如传入数据： |
| `cn.hutool.core.collection.CollUtil` | `Map<K, V> fieldValueAsMap(Iterable<?> iterable,String fieldNameForKey,String fieldNameForValue)` | 两个字段值组成新的Map |
| `cn.hutool.core.collection.CollUtil` | `Map<K, V> fieldValueMap(Iterable<V> iterable,String fieldName)` | 字段值与列表值对应的Map，常用于元素对象中有唯一ID时需要按照这个ID查找对象的情况 例如：车牌号 =》车 |
| `cn.hutool.core.collection.CollUtil` | `Map<K, V> toMap(Iterable<E> values,Map<K, V> map,Func1<E, K> keyFunc,Func1<E, V> valueFunc)` | 集合转换为Map，转换规则为： 按照keyFunc函数规则根据元素对象生成Key，按照valueFunc函数规则根据元素对象生成value组成新的Map |
| `cn.hutool.core.collection.CollUtil` | `Map<K, V> toMap(Iterable<V> values,Map<K, V> map,Func1<V, K> keyFunc)` | 集合转换为Map，转换规则为： 按照keyFunc函数规则根据元素对象生成Key，元素作为值 |
| `cn.hutool.core.collection.CollUtil` | `Map<K, V> zip(Collection<K> keys,Collection<V> values)` | 映射键值（参考Python的zip()函数） 例如： keys = [a,b,c,d] values = [1,2,3,4] 则得到的Map是 {a=1, b=2, c=3, d=4} 如果两个数组长度不同，则只对应最短部分 |
| `cn.hutool.core.collection.CollUtil` | `Map<String, String> zip(String keys,String values,String delimiter)` | 映射键值（参考Python的zip()函数），返回Map无序 例如： keys = a,b,c,d values = 1,2,3,4 delimiter = , 则得到的Map是 {a=1, b=2, c=3, d=4} 如果两个数组长度不同，则只对应最短部分 |
| `cn.hutool.core.collection.CollUtil` | `Map<String, String> zip(String keys,String values,String delimiter,boolean isOrder)` | 映射键值（参考Python的zip()函数） 例如： keys = a,b,c,d values = 1,2,3,4 delimiter = , 则得到的Map是 {a=1, b=2, c=3, d=4} 如果两个数组长度不同，则只对应最短部分 |
| `cn.hutool.core.collection.CollUtil` | `Map<T, Integer> countMap(Iterable<T> collection)` | 根据集合返回一个元素计数的 Map 所谓元素计数就是假如这个集合中某个元素出现了n次，那将这个元素做为key，n做为value 例如：[a,b,c,c,c] 得到： a: 1 b: 1 c: 3 |
| `cn.hutool.core.collection.CollUtil` | `Set<K> keySet(Collection<Map<K, ?>> mapCollection)` | 获取指定Map列表中所有的Key |
| `cn.hutool.core.collection.CollUtil` | `Set<T> emptyIfNull(Set<T> set)` | 如果提供的集合为null，返回一个不可变的默认空集合，否则返回原集合 空集合使用Collections#emptySet() |
| `cn.hutool.core.collection.CollUtil` | `Set<T> intersectionDistinct(Collection<T> coll1,Collection<T> coll2,Collection<T>... otherColls)` | 多个集合的交集 针对一个集合中存在多个相同元素的情况，只保留一个 例如：集合1：[a, b, c, c, c]，集合2：[a, b, c, c] 结果：[a, b, c]，此结果中只保留了一个c |
| `cn.hutool.core.collection.CollUtil` | `Set<T> unionDistinct(Collection<T> coll1,Collection<T> coll2,Collection<T>... otherColls)` | 多个集合的非重复并集，类似于SQL中的“UNION DISTINCT” 针对一个集合中存在多个相同元素的情况，只保留一个 例如：集合1：[a, b, c, c, c]，集合2：[a, b, c, c] 结果：[a, b, c]，此结果中只保留了一个c |
| `cn.hutool.core.collection.CollUtil` | `String join(Iterable<T> iterable,CharSequence conjunction)` | 以 conjunction 为分隔符将集合转换为字符串 如果集合元素为数组、Iterable或Iterator，则递归组合其为字符串 |
| `cn.hutool.core.collection.CollUtil` | `String join(Iterable<T> iterable,CharSequence conjunction,Function<T, ? extends CharSequence> func)` | 以 conjunction 为分隔符将集合转换为字符串 |
| `cn.hutool.core.collection.CollUtil` | `String join(Iterable<T> iterable,CharSequence conjunction,String prefix,String suffix)` | 以 conjunction 为分隔符将集合转换为字符串 |
| `cn.hutool.core.collection.CollUtil` | `String join(Iterator<T> iterator,CharSequence conjunction)` | 以 conjunction 为分隔符将集合转换为字符串 如果集合元素为数组、Iterable或Iterator，则递归组合其为字符串 |
| `cn.hutool.core.collection.CollUtil` | `T defaultIfEmpty(T collection,Supplier<? extends T> supplier)` | 如果给定集合为空，返回默认集合 |
| `cn.hutool.core.collection.CollUtil` | `T defaultIfEmpty(T collection,T defaultCollection)` | 如果给定集合为空，返回默认集合 |
| `cn.hutool.core.collection.CollUtil` | `T empty(Class<?> collectionClass)` | 根据给定的集合类型，返回对应的空集合，支持类型包括： * |
| `cn.hutool.core.collection.CollUtil` | `T filter(T collection,final Filter<E> filter)` | 去除指定元素，此方法直接修改原集合 |
| `cn.hutool.core.collection.CollUtil` | `T findOne(Iterable<T> collection,Filter<T> filter)` | 查找第一个匹配元素对象 |
| `cn.hutool.core.collection.CollUtil` | `T findOneByField(Iterable<T> collection,final String fieldName,final Object fieldValue)` | 查找第一个匹配元素对象 如果集合元素是Map，则比对键和值是否相同，相同则返回 如果为普通Bean，则通过反射比对元素字段名对应的字段值是否相同，相同则返回 如果给定字段值参数是null 且元素对象中的字段值也为null则认为相同 |
| `cn.hutool.core.collection.CollUtil` | `T get(Collection<T> collection,int index)` | 获取集合中指定下标的元素值，下标可以为负数，例如-1表示最后一个元素 如果元素越界，返回null |
| `cn.hutool.core.collection.CollUtil` | `T getFirst(Iterable<T> iterable)` | 获取集合的第一个元素 |
| `cn.hutool.core.collection.CollUtil` | `T getFirst(Iterator<T> iterator)` | 获取集合的第一个元素 |
| `cn.hutool.core.collection.CollUtil` | `T getLast(Collection<T> collection)` | 获取集合的最后一个元素 |
| `cn.hutool.core.collection.CollUtil` | `T max(Collection<T> coll)` | 取最大值 |
| `cn.hutool.core.collection.CollUtil` | `T min(Collection<T> coll)` | 取最小值 |
| `cn.hutool.core.collection.CollUtil` | `T removeAny(T collection,E... elesRemoved)` | 去掉集合中的多个元素，此方法直接修改原集合 |
| `cn.hutool.core.collection.CollUtil` | `T removeBlank(T collection)` | 去除null或者""或者空白字符串 元素，此方法直接修改原集合 |
| `cn.hutool.core.collection.CollUtil` | `T removeEmpty(T collection)` | 去除null或者"" 元素，此方法直接修改原集合 |
| `cn.hutool.core.collection.CollUtil` | `T removeNull(T collection)` | 去除null 元素，此方法直接修改原集合 |
| `cn.hutool.core.collection.CollUtil` | `T removeWithAddIf(T targetCollection,T resultCollection,Predicate<? super E> predicate)` | 移除集合中的多个元素，并将结果存放到指定的集合 此方法直接修改原集合 |
| `cn.hutool.core.collection.CollUtil` | `TreeMap<K, V> sort(Map<K, V> map,Comparator<? super K> comparator)` | 排序Map |
| `cn.hutool.core.collection.CollUtil` | `TreeSet<T> toTreeSet(Collection<T> collection,Comparator<T> comparator)` | 将集合转换为排序后的TreeSet |
| `cn.hutool.core.collection.CollUtil` | `boolean addIfAbsent(Collection<T> collection,S object)` | 一个对象不为空且不存在于该集合中时，加入到该集合中 |
| `cn.hutool.core.collection.CollUtil` | `boolean allMatch(Collection<T> collection,Predicate<T> predicate)` | 是否全部匹配判断条件 |
| `cn.hutool.core.collection.CollUtil` | `boolean anyMatch(Collection<T> collection,Predicate<T> predicate)` | 是否至少有一个符合判断条件 |
| `cn.hutool.core.collection.CollUtil` | `boolean contains(Collection<?> collection,Object value)` | 判断指定集合是否包含指定值，如果集合为空（null或者空），返回false，否则找到元素返回true |
| `cn.hutool.core.collection.CollUtil` | `boolean contains(Collection<T> collection,Predicate<? super T> containFunc)` | 自定义函数判断集合是否包含某类值 |
| `cn.hutool.core.collection.CollUtil` | `boolean containsAll(Collection<?> coll1,Collection<?> coll2)` | 集合1中是否包含集合2中所有的元素。 当集合1和集合2都为空时，返回true 当集合2为空时，返回true |
| `cn.hutool.core.collection.CollUtil` | `boolean containsAny(Collection<?> coll1,Collection<?> coll2)` | 其中一个集合在另一个集合中是否至少包含一个元素，即是两个集合是否至少有一个共同的元素 |
| `cn.hutool.core.collection.CollUtil` | `boolean hasNull(Iterable<?> iterable)` | 是否包含null元素 |
| `cn.hutool.core.collection.CollUtil` | `boolean isEmpty(Collection<?> collection)` | 集合是否为空 |
| `cn.hutool.core.collection.CollUtil` | `boolean isEmpty(Enumeration<?> enumeration)` | Enumeration是否为空 |
| `cn.hutool.core.collection.CollUtil` | `boolean isEmpty(Iterable<?> iterable)` | Iterable是否为空 |
| `cn.hutool.core.collection.CollUtil` | `boolean isEmpty(Iterator<?> Iterator)` | Iterator是否为空 |
| `cn.hutool.core.collection.CollUtil` | `boolean isEmpty(Map<?, ?> map)` | Map是否为空 |
| `cn.hutool.core.collection.CollUtil` | `boolean isEqualList(final Collection<?> list1,final Collection<?> list2)` | 判断两个Collection 是否元素和顺序相同，返回true的条件是： 两个Collection必须长度相同 两个Collection元素相同index的对象必须equals，满足Objects#equals(Object, Object) 此方法来自Apache-Commons-Collections4。 |
| `cn.hutool.core.collection.CollUtil` | `boolean isNotEmpty(Collection<?> collection)` | 集合是否为非空 |
| `cn.hutool.core.collection.CollUtil` | `boolean isNotEmpty(Enumeration<?> enumeration)` | Enumeration是否为空 |
| `cn.hutool.core.collection.CollUtil` | `boolean isNotEmpty(Iterable<?> iterable)` | Iterable是否为空 |
| `cn.hutool.core.collection.CollUtil` | `boolean isNotEmpty(Iterator<?> Iterator)` | Iterator是否为空 |
| `cn.hutool.core.collection.CollUtil` | `boolean isNotEmpty(Map<?, ?> map)` | Map是否为非空 |
| `cn.hutool.core.collection.CollUtil` | `boolean safeContains(Collection<?> collection,Object value)` | 判断指定集合是否包含指定值，如果集合为空（null或者空），返回false，否则找到元素返回true |
| `cn.hutool.core.collection.CollUtil` | `int count(Iterable<T> iterable,Matcher<T> matcher)` | 集合中匹配规则的数量 |
| `cn.hutool.core.collection.CollUtil` | `int indexOf(Collection<T> collection,Matcher<T> matcher)` | 获取匹配规则定义中匹配到元素的第一个位置 此方法对于某些无序集合的位置信息，以转换为数组后的位置为准。 |
| `cn.hutool.core.collection.CollUtil` | `int lastIndexOf(Collection<T> collection,Matcher<T> matcher)` | 获取匹配规则定义中匹配到元素的最后位置 此方法对于某些无序集合的位置信息，以转换为数组后的位置为准。 |
| `cn.hutool.core.collection.CollUtil` | `int size(final Object object)` | 获取Collection或者iterator的大小，此方法可以处理的对象类型如下： Collection - the collection size Map - the map size Array - the array size Iterator - the number of elements remaining in the iterator Enumeration - the number of elements remaining in the enumeration |
| `cn.hutool.core.collection.CollUtil` | `int[] indexOfAll(Collection<T> collection,Matcher<T> matcher)` | 获取匹配规则定义中匹配到元素的所有位置 此方法对于某些无序集合的位置信息，以转换为数组后的位置为准。 |
| `cn.hutool.core.collection.CollUtil` | `void clear(Collection<?>... collections)` | 清除一个或多个集合内的元素，每个集合调用clear()方法 |
| `cn.hutool.core.collection.CollUtil` | `void forEach(Enumeration<T> enumeration,Consumer<T> consumer)` | 循环遍历 Enumeration，使用Consumer 接受遍历的每条数据，并针对每条数据做处理 |
| `cn.hutool.core.collection.CollUtil` | `void forEach(Iterable<T> iterable,Consumer<T> consumer)` | 循环遍历 Iterable，使用Consumer 接受遍历的每条数据，并针对每条数据做处理 |
| `cn.hutool.core.collection.CollUtil` | `void forEach(Iterator<T> iterator,Consumer<T> consumer)` | 循环遍历 Iterator，使用Consumer 接受遍历的每条数据，并针对每条数据做处理 |
| `cn.hutool.core.collection.CollUtil` | `void forEach(Map<K, V> map,KVConsumer<K, V> kvConsumer)` | 循环遍历Map，使用KVConsumer 接受遍历的每条数据，并针对每条数据做处理 和JDK8中的map.forEach不同的是，此方法支持index |
| `cn.hutool.core.collection.CollUtil` | `void padLeft(List<T> list,int minLen,T padObj)` | 填充List，以达到最小长度 |
| `cn.hutool.core.collection.CollUtil` | `void padRight(Collection<T> list,int minLen,T padObj)` | 填充List，以达到最小长度 |
| `cn.hutool.core.collection.CollUtil` | `void setValueByMap(Iterable<E> iterable,Map<K, V> map,Function<E, K> keyGenerate,BiConsumer<E, V> biConsumer)` | 使用给定的map将集合中的原素进行属性或者值的重新设定 |
| `cn.hutool.core.collection.CollUtil$Consumer` | `void accept(T value,int index)` | 接受并处理一个参数 |
| `cn.hutool.core.collection.CollUtil$KVConsumer` | `void accept(K key,V value,int index)` | 接受并处理一对参数 |
| `cn.hutool.core.collection.ComputeIter` | `T next()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.ComputeIter` | `boolean hasNext()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.ComputeIter` | `void finish()` | 手动结束遍历器，用于关闭操作等 |
| `cn.hutool.core.collection.ComputeIter` | `void resetState()` | 重置状态，用于再次遍历 |
| `cn.hutool.core.collection.ConcurrentHashSet` | `Iterator<E> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.ConcurrentHashSet` | `boolean add(E e)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.ConcurrentHashSet` | `boolean contains(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.ConcurrentHashSet` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.ConcurrentHashSet` | `boolean remove(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.ConcurrentHashSet` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.ConcurrentHashSet` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.CopiedIter` | `CopiedIter<E> copyOf(Iterator<E> iterator)` | 根据已有Iterator，返回新的CopiedIter |
| `cn.hutool.core.collection.CopiedIter` | `E next()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.CopiedIter` | `boolean hasNext()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.CopiedIter` | `void remove()` | 此对象不支持移除元素 |
| `cn.hutool.core.collection.EnumerationIter` | `E next()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.EnumerationIter` | `boolean hasNext()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.EnumerationIter` | `void remove()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.FilterIter` | `E next()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.FilterIter` | `Filter<? super E> getFilter()` | 获取过滤函数 |
| `cn.hutool.core.collection.FilterIter` | `Iterator<? extends E> getIterator()` | 获取被包装的Iterator |
| `cn.hutool.core.collection.FilterIter` | `boolean hasNext()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.FilterIter` | `void remove()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.IterChain` | `IterChain<T> addChain(Iterator<T> iterator)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.IterChain` | `Iterator<Iterator<T>> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.IterChain` | `T next()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.IterChain` | `boolean hasNext()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.IterChain` | `void remove()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.IterUtil` | `Class<?> getElementType(Iterable<?> iterable)` | 获得Iterable对象的元素类型（通过第一个非空元素判断） 注意，此方法至少会调用多次next方法 |
| `cn.hutool.core.collection.IterUtil` | `Class<?> getElementType(Iterator<?> iterator)` | 获得Iterator对象的元素类型（通过第一个非空元素判断） 注意，此方法至少会调用多次next方法 |
| `cn.hutool.core.collection.IterUtil` | `E get(final Iterator<E> iterator,int index)` | 遍历Iterator，获取指定index位置的元素 |
| `cn.hutool.core.collection.IterUtil` | `FilterIter<E> filtered(final Iterator<? extends E> iterator,final Filter<? super E> filter)` | 获取一个新的 FilterIter，用于过滤指定元素 |
| `cn.hutool.core.collection.IterUtil` | `HashMap<K, V> toMap(Iterable<Entry<K, V>> entryIter)` | 将Entry集合转换为HashMap |
| `cn.hutool.core.collection.IterUtil` | `Iterable<E> asIterable(final Iterator<E> iter)` | Iterator 转为 Iterable |
| `cn.hutool.core.collection.IterUtil` | `Iterator<?> getIter(final Object obj)` | 从给定的对象中获取可能存在的Iterator，规则如下： null - null Iterator - 直接返回 Enumeration - EnumerationIter Collection - 调用Collection#iterator() Map - Entry的Iterator Dictionary - values (elements) enumeration returned as iterator array - ArrayIter NodeList - NodeListIter Node - 子节点 object with iterator() public method，通… |
| `cn.hutool.core.collection.IterUtil` | `Iterator<E> asIterator(Enumeration<E> e)` | Enumeration转换为Iterator Adapt the specified Enumeration to the Iterator interface |
| `cn.hutool.core.collection.IterUtil` | `Iterator<E> filter(Iterator<E> iter,Filter<E> filter)` | 过滤集合，此方法在原集合上直接修改 通过实现Filter接口，完成元素的过滤，这个Filter实现可以实现以下功能： |
| `cn.hutool.core.collection.IterUtil` | `Iterator<T> empty()` | 返回一个空Iterator |
| `cn.hutool.core.collection.IterUtil` | `Iterator<T> getIter(Iterable<T> iterable)` | 获取Iterator |
| `cn.hutool.core.collection.IterUtil` | `Iterator<T> trans(Iterator<F> iterator,Function<? super F, ? extends T> function)` | 按照给定函数，转换Iterator为另一种类型的Iterator |
| `cn.hutool.core.collection.IterUtil` | `List<E> filterToList(Iterator<E> iter,Filter<E> filter)` | 过滤Iterator并将过滤后满足条件的元素添加到List中 |
| `cn.hutool.core.collection.IterUtil` | `List<E> toList(Iterable<E> iter)` | Iterator转List 不判断，直接生成新的List |
| `cn.hutool.core.collection.IterUtil` | `List<E> toList(Iterator<E> iter)` | Iterator转List 不判断，直接生成新的List |
| `cn.hutool.core.collection.IterUtil` | `List<Object> fieldValueList(Iterable<V> iterable,String fieldName)` | 获取指定Bean列表中某个字段，生成新的列表 |
| `cn.hutool.core.collection.IterUtil` | `List<Object> fieldValueList(Iterator<V> iter,String fieldName)` | 获取指定Bean列表中某个字段，生成新的列表 |
| `cn.hutool.core.collection.IterUtil` | `List<T> edit(Iterable<T> iter,Editor<T> editor)` | 编辑，此方法产生一个新ArrayList 编辑过程通过传入的Editor实现来返回需要的元素内容，这个Editor实现可以实现以下功能： |
| `cn.hutool.core.collection.IterUtil` | `Map<K, List<V>> toListMap(Iterable<T> iterable,Function<T, K> keyMapper,Function<T, V> valueMapper)` | 将列表转成值为List的HashMap |
| `cn.hutool.core.collection.IterUtil` | `Map<K, List<V>> toListMap(Iterable<V> iterable,Function<V, K> keyMapper)` | 将列表转成值为List的HashMap |
| `cn.hutool.core.collection.IterUtil` | `Map<K, List<V>> toListMap(Map<K, List<V>> resultMap,Iterable<T> iterable,Function<T, K> keyMapper,Function<T, V> valueMapper)` | 将列表转成值为List的HashMap |
| `cn.hutool.core.collection.IterUtil` | `Map<K, V> fieldValueAsMap(Iterator<?> iter,String fieldNameForKey,String fieldNameForValue)` | 两个字段值组成新的Map |
| `cn.hutool.core.collection.IterUtil` | `Map<K, V> fieldValueMap(Iterator<V> iter,String fieldName)` | 字段值与列表值对应的Map，常用于元素对象中有唯一ID时需要按照这个ID查找对象的情况 例如：车牌号 =》车 |
| `cn.hutool.core.collection.IterUtil` | `Map<K, V> toMap(Iterable<K> keys,Iterable<V> values)` | 将键列表和值列表转换为Map 以键为准，值与键位置需对应。如果键元素数多于值元素，多余部分值用null代替。 如果值多于键，忽略多余的值。 |
| `cn.hutool.core.collection.IterUtil` | `Map<K, V> toMap(Iterable<K> keys,Iterable<V> values,boolean isOrder)` | 将键列表和值列表转换为Map 以键为准，值与键位置需对应。如果键元素数多于值元素，多余部分值用null代替。 如果值多于键，忽略多余的值。 |
| `cn.hutool.core.collection.IterUtil` | `Map<K, V> toMap(Iterable<T> iterable,Function<T, K> keyMapper,Function<T, V> valueMapper)` | 将列表转成HashMap |
| `cn.hutool.core.collection.IterUtil` | `Map<K, V> toMap(Iterable<V> iterable,Function<V, K> keyMapper)` | 将列表转成HashMap |
| `cn.hutool.core.collection.IterUtil` | `Map<K, V> toMap(Iterator<E> iterator,Map<K, V> map,Func1<E, K> keyFunc,Func1<E, V> valueFunc)` | 集合转换为Map，转换规则为： 按照keyFunc函数规则根据元素对象生成Key，按照valueFunc函数规则根据元素对象生成value组成新的Map |
| `cn.hutool.core.collection.IterUtil` | `Map<K, V> toMap(Iterator<K> keys,Iterator<V> values)` | 将键列表和值列表转换为Map 以键为准，值与键位置需对应。如果键元素数多于值元素，多余部分值用null代替。 如果值多于键，忽略多余的值。 |
| `cn.hutool.core.collection.IterUtil` | `Map<K, V> toMap(Iterator<K> keys,Iterator<V> values,boolean isOrder)` | 将键列表和值列表转换为Map 以键为准，值与键位置需对应。如果键元素数多于值元素，多余部分值用null代替。 如果值多于键，忽略多余的值。 |
| `cn.hutool.core.collection.IterUtil` | `Map<K, V> toMap(Iterator<V> iterator,Map<K, V> map,Func1<V, K> keyFunc)` | Iterator转换为Map，转换规则为： 按照keyFunc函数规则根据元素对象生成Key，元素作为值 |
| `cn.hutool.core.collection.IterUtil` | `Map<K, V> toMap(Map<K, V> resultMap,Iterable<T> iterable,Function<T, K> keyMapper,Function<T, V> valueMapper)` | 将列表转成Map |
| `cn.hutool.core.collection.IterUtil` | `Map<T, Integer> countMap(Iterator<T> iter)` | 根据集合返回一个元素计数的 Map 所谓元素计数就是假如这个集合中某个元素出现了n次，那将这个元素做为key，n做为value 例如：[a,b,c,c,c] 得到： a: 1 b: 1 c: 3 |
| `cn.hutool.core.collection.IterUtil` | `String join(Iterator<T> iterator,CharSequence conjunction)` | 以 conjunction 为分隔符将集合转换为字符串 如果集合元素为数组、Iterable或Iterator，则递归组合其为字符串 |
| `cn.hutool.core.collection.IterUtil` | `String join(Iterator<T> iterator,CharSequence conjunction,Function<T, ? extends CharSequence> func)` | 以 conjunction 为分隔符将集合转换为字符串 如果集合元素为数组、Iterable或Iterator，则递归组合其为字符串 |
| `cn.hutool.core.collection.IterUtil` | `String join(Iterator<T> iterator,CharSequence conjunction,String prefix,String suffix)` | 以 conjunction 为分隔符将集合转换为字符串 如果集合元素为数组、Iterable或Iterator，则递归组合其为字符串 |
| `cn.hutool.core.collection.IterUtil` | `String toStr(final Iterator<E> iterator)` | 拼接 Iterator为字符串 |
| `cn.hutool.core.collection.IterUtil` | `String toStr(final Iterator<E> iterator,final Function<? super E, String> transFunc)` | 拼接 Iterator为字符串 |
| `cn.hutool.core.collection.IterUtil` | `String toStr(final Iterator<E> iterator,final Function<? super E, String> transFunc,final String delimiter,final String prefix,final String suffix)` | 拼接 Iterator为字符串 |
| `cn.hutool.core.collection.IterUtil` | `T filter(T iter,Filter<E> filter)` | 过滤集合，此方法在原集合上直接修改 通过实现Filter接口，完成元素的过滤，这个Filter实现可以实现以下功能： |
| `cn.hutool.core.collection.IterUtil` | `T firstMatch(Iterator<T> iterator,Matcher<T> matcher)` | 返回Iterator中第一个匹配规则的值 |
| `cn.hutool.core.collection.IterUtil` | `T getFirst(Iterable<T> iterable)` | 获取集合的第一个元素，如果集合为空（null或者空集合），返回null |
| `cn.hutool.core.collection.IterUtil` | `T getFirst(Iterator<T> iterator)` | 获取集合的第一个元素 |
| `cn.hutool.core.collection.IterUtil` | `T getFirstNoneNull(Iterable<T> iterable)` | 获取集合的第一个非空元素 |
| `cn.hutool.core.collection.IterUtil` | `T getFirstNoneNull(Iterator<T> iterator)` | 获取集合的第一个非空元素 |
| `cn.hutool.core.collection.IterUtil` | `boolean hasNull(Iterable<?> iter)` | 是否包含null元素 |
| `cn.hutool.core.collection.IterUtil` | `boolean hasNull(Iterator<?> iter)` | 是否包含null元素 |
| `cn.hutool.core.collection.IterUtil` | `boolean isAllNull(Iterable<?> iter)` | 是否全部元素为null |
| `cn.hutool.core.collection.IterUtil` | `boolean isAllNull(Iterator<?> iter)` | 是否全部元素为null |
| `cn.hutool.core.collection.IterUtil` | `boolean isEmpty(Iterable<?> iterable)` | Iterable是否为空 |
| `cn.hutool.core.collection.IterUtil` | `boolean isEmpty(Iterator<?> Iterator)` | Iterator是否为空 |
| `cn.hutool.core.collection.IterUtil` | `boolean isEqualList(Iterable<?> list1,Iterable<?> list2)` | 判断两个Iterable 是否元素和顺序相同，返回true的条件是： 两个Iterable必须长度相同 两个Iterable元素相同index的对象必须equals，满足Objects#equals(Object, Object) 此方法来自Apache-Commons-Collections4。 |
| `cn.hutool.core.collection.IterUtil` | `boolean isNotEmpty(Iterable<?> iterable)` | Iterable是否为空 |
| `cn.hutool.core.collection.IterUtil` | `boolean isNotEmpty(Iterator<?> Iterator)` | Iterator是否为空 |
| `cn.hutool.core.collection.IterUtil` | `int size(Iterable<?> iterable)` | 返回 Iterable 对象的元素数量 |
| `cn.hutool.core.collection.IterUtil` | `int size(Iterator<?> iterator)` | 返回 Iterator 对象的元素数量 |
| `cn.hutool.core.collection.IterUtil` | `void clear(Iterator<?> iterator)` | 清空指定Iterator，此方法遍历后调用Iterator#remove()移除每个元素 |
| `cn.hutool.core.collection.IterUtil` | `void forEach(final Iterator<E> iterator,final Consumer<? super E> consumer)` | 遍历Iterator 当consumer为null表示不处理，但是依旧遍历Iterator |
| `cn.hutool.core.collection.IterableIter` | `Iterator<T> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.IteratorEnumeration` | `E nextElement()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.IteratorEnumeration` | `boolean hasMoreElements()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.LineIter` | `void close()` | 关闭Reader |
| `cn.hutool.core.collection.ListUtil` | `ArrayList<T> toList(Collection<T> collection)` | 新建一个ArrayList |
| `cn.hutool.core.collection.ListUtil` | `ArrayList<T> toList(Enumeration<T> enumeration)` | 新建一个ArrayList 提供的参数为null时返回空ArrayList |
| `cn.hutool.core.collection.ListUtil` | `ArrayList<T> toList(Iterable<T> iterable)` | 新建一个ArrayList 提供的参数为null时返回空ArrayList |
| `cn.hutool.core.collection.ListUtil` | `ArrayList<T> toList(Iterator<T> iterator)` | 新建一个ArrayList 提供的参数为null时返回空ArrayList |
| `cn.hutool.core.collection.ListUtil` | `ArrayList<T> toList(T... values)` | 新建一个ArrayList |
| `cn.hutool.core.collection.ListUtil` | `CopyOnWriteArrayList<T> toCopyOnWriteArrayList(Collection<T> collection)` | 新建一个CopyOnWriteArrayList |
| `cn.hutool.core.collection.ListUtil` | `LinkedList<T> toLinkedList(T... values)` | 新建LinkedList |
| `cn.hutool.core.collection.ListUtil` | `List<List<T>> partition(List<T> list,int size)` | 通过传入分区长度，将指定列表分区为不同的块，每块区域的长度相同（最后一块可能小于长度） 分区是在原List的基础上进行的，返回的分区是不可变的抽象列表，原列表元素变更，分区中元素也会变更。 需要特别注意的是，此方法调用List#subList(int, int)切分List， 此方法返回的是原List的视图，也就是说原List有变更，切分后的结果也会变更。 |
| `cn.hutool.core.collection.ListUtil` | `List<List<T>> split(List<T> list,int size)` | 对集合按照指定长度分段，每一个段为单独的集合，返回这个集合的列表 需要特别注意的是，此方法调用List#subList(int, int)切分List， 此方法返回的是原List的视图，也就是说原List有变更，切分后的结果也会变更。 |
| `cn.hutool.core.collection.ListUtil` | `List<List<T>> splitAvg(List<T> list,int limit)` | 将集合平均分成多个list，返回这个集合的列表 例： |
| `cn.hutool.core.collection.ListUtil` | `List<R> zip(List<A> listA,List<B> listB,BiFunction<A, B, R> zipper)` | 将两个列表的元素按照索引一一配对，通过指定的函数进行合并，返回一个新的结果列表。 新列表的长度将以两个输入列表中较短的那个为准。 |
| `cn.hutool.core.collection.ListUtil` | `List<String> sortByPinyin(List<String> list)` | 根据汉字的拼音顺序排序 |
| `cn.hutool.core.collection.ListUtil` | `List<T> empty()` | 获取一个空List，这个空List不可变 |
| `cn.hutool.core.collection.ListUtil` | `List<T> list(boolean isLinked)` | 新建一个空List |
| `cn.hutool.core.collection.ListUtil` | `List<T> list(boolean isLinked,Collection<T> collection)` | 新建一个List |
| `cn.hutool.core.collection.ListUtil` | `List<T> list(boolean isLinked,Enumeration<T> enumration)` | 新建一个List 提供的参数为null时返回空ArrayList |
| `cn.hutool.core.collection.ListUtil` | `List<T> list(boolean isLinked,Iterable<T> iterable)` | 新建一个List 提供的参数为null时返回空ArrayList |
| `cn.hutool.core.collection.ListUtil` | `List<T> list(boolean isLinked,Iterator<T> iter)` | 新建一个List 提供的参数为null时返回空ArrayList |
| `cn.hutool.core.collection.ListUtil` | `List<T> list(boolean isLinked,T... values)` | 新建一个List |
| `cn.hutool.core.collection.ListUtil` | `List<T> move(List<T> list,T element,int newPosition)` | 将元素移动到指定列表的新位置。 如果元素不在列表中，则将其添加到新位置。 如果元素已在列表中，则先移除它，然后再将其添加到新位置。 |
| `cn.hutool.core.collection.ListUtil` | `List<T> of(T... ts)` | 数组转为一个不可变List 类似于Java9中的List.of |
| `cn.hutool.core.collection.ListUtil` | `List<T> page(int pageNo,int pageSize,List<T> list)` | 对指定List分页取值 |
| `cn.hutool.core.collection.ListUtil` | `List<T> reverse(List<T> list)` | 反序给定List，会在原List基础上直接修改 |
| `cn.hutool.core.collection.ListUtil` | `List<T> reverseNew(List<T> list)` | 反序给定List，会创建一个新的List，原List数据不变 |
| `cn.hutool.core.collection.ListUtil` | `List<T> setOrAppend(List<T> list,int index,T element)` | 设置或增加元素。当index小于List的长度时，替换指定位置的值，否则在尾部追加 |
| `cn.hutool.core.collection.ListUtil` | `List<T> setOrPadding(List<T> list,int index,T element)` | 在指定位置设置元素。当index小于List的长度时，替换指定位置的值，否则追加null直到到达index后，设置值 |
| `cn.hutool.core.collection.ListUtil` | `List<T> setOrPadding(List<T> list,int index,T element,T paddingElement)` | 在指定位置设置元素。当index小于List的长度时，替换指定位置的值，否则追加paddingElement直到到达index后，设置值 注意：为避免OOM问题，此方法限制index的最大值为(list.size() + 1) * 10 |
| `cn.hutool.core.collection.ListUtil` | `List<T> setOrPadding(List<T> list,int index,T element,T paddingElement,int indexLimit)` | 在指定位置设置元素。当index小于List的长度时，替换指定位置的值，否则追加paddingElement直到到达index后，设置值 |
| `cn.hutool.core.collection.ListUtil` | `List<T> sort(List<T> list,Comparator<? super T> c)` | 针对List排序，排序会修改原List |
| `cn.hutool.core.collection.ListUtil` | `List<T> sortByProperty(List<T> list,String property)` | 根据Bean的属性排序 |
| `cn.hutool.core.collection.ListUtil` | `List<T> sub(List<T> list,int start,int end)` | 截取集合的部分 |
| `cn.hutool.core.collection.ListUtil` | `List<T> sub(List<T> list,int start,int end,int step)` | 截取集合的部分 此方法与List#subList(int, int) 不同在于子列表是新的副本，操作子列表不会影响原列表。 |
| `cn.hutool.core.collection.ListUtil` | `List<T> unmodifiable(List<T> list)` | 将对应List转换为不可修改的List |
| `cn.hutool.core.collection.ListUtil` | `int lastIndexOf(List<T> list,Matcher<T> matcher)` | 获取匹配规则定义中匹配到元素的最后位置 此方法对于某些无序集合的位置信息，以转换为数组后的位置为准。 |
| `cn.hutool.core.collection.ListUtil` | `int[] indexOfAll(List<T> list,Matcher<T> matcher)` | 获取匹配规则定义中匹配到元素的所有位置 |
| `cn.hutool.core.collection.ListUtil` | `void page(List<T> list,int pageSize,Consumer<List<T>> pageListConsumer)` | 对指定List进行分页，逐页返回数据 |
| `cn.hutool.core.collection.ListUtil` | `void swapElement(List<T> list,T element,T targetElement)` | 将指定元素交换到指定元素位置,其他元素的索引值不变 交换会修改原List 如果集合中有多个相同元素，只交换第一个找到的元素 |
| `cn.hutool.core.collection.ListUtil` | `void swapTo(List<T> list,T element,Integer targetIndex)` | 将指定元素交换到指定索引位置,其他元素的索引值不变 交换会修改原List 如果集合中有多个相同元素，只交换第一个找到的元素 |
| `cn.hutool.core.collection.NodeListIter` | `Node next()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.NodeListIter` | `boolean hasNext()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.NodeListIter` | `void remove()` | 【原文待译】Throws UnsupportedOperationException. |
| `cn.hutool.core.collection.NodeListIter` | `void reset()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.Partition` | `List<T> get(int index)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.Partition` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.Partition` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.PartitionIter` | `List<T> next()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.PartitionIter` | `boolean hasNext()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.ResettableIter` | `void reset()` | 重置，重置后可重新遍历 |
| `cn.hutool.core.collection.RingIndexUtil` | `int ringNextInt(int modulo,AtomicInteger atomicInteger)` | 通过cas操作 实现对指定值内的回环累加 |
| `cn.hutool.core.collection.RingIndexUtil` | `int ringNextIntByObj(Object object,AtomicInteger atomicInteger)` | 通过cas操作 实现对指定值内的回环累加 |
| `cn.hutool.core.collection.RingIndexUtil` | `long ringNextLong(long modulo,AtomicLong atomicLong)` | 通过cas操作 实现对指定值内的回环累加 此方法一般用于大量数据完成回环累加（如数据库中的值大于int最大值） |
| `cn.hutool.core.collection.SpliteratorUtil` | `Spliterator<T> trans(Spliterator<F> fromSpliterator,Function<? super F, ? extends T> function)` | 使用给定的转换函数，转换源Spliterator为新类型的Spliterator |
| `cn.hutool.core.collection.TransCollection` | `Iterator<T> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.TransCollection` | `Spliterator<T> spliterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.TransCollection` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.TransCollection` | `boolean removeIf(Predicate<? super T> filter)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.TransCollection` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.TransCollection` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.TransCollection` | `void forEach(Consumer<? super T> action)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.TransIter` | `T next()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.TransIter` | `boolean hasNext()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.TransIter` | `void remove()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.TransSpliterator` | `Spliterator<T> trySplit()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.TransSpliterator` | `boolean tryAdvance(Consumer<? super T> action)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.TransSpliterator` | `int characteristics()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.TransSpliterator` | `long estimateSize()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.TransSpliterator` | `void forEachRemaining(Consumer<? super T> action)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.UniqueKeySet` | `Iterator<V> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.UniqueKeySet` | `UniqueKeySet<K, V> clone()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.UniqueKeySet` | `boolean add(V v)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.UniqueKeySet` | `boolean addAllIfAbsent(Collection<? extends V> c)` | 加入集合中所有的值，如果值已经存在，则忽略之 |
| `cn.hutool.core.collection.UniqueKeySet` | `boolean addIfAbsent(V v)` | 加入值，如果值已经存在，则忽略之 |
| `cn.hutool.core.collection.UniqueKeySet` | `boolean contains(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.UniqueKeySet` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.UniqueKeySet` | `boolean remove(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.UniqueKeySet` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.collection.UniqueKeySet` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
