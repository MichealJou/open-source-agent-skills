# cn.hutool.core.map

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.map.AbsEntry` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.AbsEntry` | `V setValue(V value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.AbsEntry` | `boolean equals(Object object)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.AbsEntry` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.BiMap` | `K getKey(V value)` | 根据值获得键 |
| `cn.hutool.core.map.BiMap` | `Map<V, K> getInverse()` | 获取反向Map |
| `cn.hutool.core.map.BiMap` | `V compute(K key,BiFunction<? super K, ? super V, ? extends V> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.BiMap` | `V computeIfAbsent(K key,Function<? super K, ? extends V> mappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.BiMap` | `V computeIfPresent(K key,BiFunction<? super K, ? super V, ? extends V> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.BiMap` | `V merge(K key,V value,BiFunction<? super V, ? super V, ? extends V> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.BiMap` | `V put(K key,V value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.BiMap` | `V putIfAbsent(K key,V value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.BiMap` | `V remove(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.BiMap` | `boolean remove(Object key,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.BiMap` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.BiMap` | `void putAll(Map<? extends K, ? extends V> m)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.FixedLinkedHashMap` | `int getCapacity()` | 获取容量 |
| `cn.hutool.core.map.FixedLinkedHashMap` | `void setCapacity(int capacity)` | 设置容量 |
| `cn.hutool.core.map.FixedLinkedHashMap` | `void setRemoveListener(final Consumer<Map.Entry<K, V>> removeListener)` | 设置自定义移除监听 |
| `cn.hutool.core.map.ForestMap` | `Collection<TreeEntry<K, V>> getChildNodes(K key)` | 获取指定父节点的全部子节点 比如：若存在 a -> b -> c 的关系，此时输入 b 将返回 c，输入 a 将返回 b，c |
| `cn.hutool.core.map.ForestMap` | `Collection<TreeEntry<K, V>> getDeclaredChildNodes(K key)` | 获取指定父节点直接关联的子节点 比如：若存在 a -> b -> c 的关系，此时输入 b 将返回 c，输入 a 将返回 b |
| `cn.hutool.core.map.ForestMap` | `Set<TreeEntry<K, V>> getTreeNodes(K key)` | 获取指定节点所在树结构的全部树节点 比如：存在 a -> b -> c 的关系，则输入 a/b/c 都将返回 a, b, c |
| `cn.hutool.core.map.ForestMap` | `TreeEntry<K, V> getDeclaredParentNode(K key)` | 获取指定节点的直接父节点 比如：若存在 a -> b -> c 的关系，此时输入 a 将返回 null，输入 b 将返回 a，输入 c 将返回 b |
| `cn.hutool.core.map.ForestMap` | `TreeEntry<K, V> getParentNode(K key,K parentKey)` | 获取以指定节点作为叶子节点的树结构，然后获取该树结构中指定节点的指定父节点 |
| `cn.hutool.core.map.ForestMap` | `TreeEntry<K, V> getRootNode(K key)` | 获取以指定节点作为叶子节点的树结构，然后获取该树结构的根节点 比如：存在 a -> b -> c 的关系，则输入 a/b/c 都将返回 a |
| `cn.hutool.core.map.ForestMap` | `TreeEntry<K, V> put(K key,TreeEntry<K, V> node)` | 添加一个节点，效果等同于 putNode(key, node.getValue()) 若key对应节点不存在，则以传入的键值创建一个新的节点； 若key对应节点存在，则将该节点的值替换为node指定的值； |
| `cn.hutool.core.map.ForestMap` | `TreeEntry<K, V> putNode(K key,V value)` | 添加一个节点 若key对应节点不存在，则以传入的键值创建一个新的节点； 若key对应节点存在，则将该节点的值替换为node指定的值； |
| `cn.hutool.core.map.ForestMap` | `TreeEntry<K, V> remove(Object key)` | 将指定节点从当前Map中删除 若存在父节点或子节点，则将其断开其与父节点或子节点的引用关系； 若同时存在父节点或子节点，则会在删除后将让子节点直接成为父节点的子节点，比如： 现有引用关系 a -> b -> c，删除 b 后，将有 a -> c |
| `cn.hutool.core.map.ForestMap` | `V getNodeValue(K key)` | 获取指定节点的值 |
| `cn.hutool.core.map.ForestMap` | `boolean containsChildNode(K parentKey,K childKey)` | 判断以该父节点作为根节点的树结构中是否具有指定子节点 |
| `cn.hutool.core.map.ForestMap` | `boolean containsParentNode(K key,K parentKey)` | 获取以指定节点作为叶子节点的树结构，然后确认该树结构中当前节点是否存在指定父节点 |
| `cn.hutool.core.map.ForestMap` | `void clear()` | 将当前集合清空，并清除全部节点间的引用关系 |
| `cn.hutool.core.map.ForestMap` | `void linkNodes(K parentKey,K childKey)` | 为集合中的指定的节点建立父子关系 |
| `cn.hutool.core.map.ForestMap` | `void linkNodes(K parentKey,K childKey,BiConsumer<TreeEntry<K, V>, TreeEntry<K, V>> consumer)` | 为集合中的指定的节点建立父子关系 |
| `cn.hutool.core.map.ForestMap` | `void putAll(Map<? extends K, ? extends TreeEntry<K, V>> treeEntryMap)` | 批量添加节点，若节点具有父节点或者子节点，则一并在当前实例中引入该关系 |
| `cn.hutool.core.map.ForestMap` | `void putAllNode(C values,Function<V, K> keyGenerator,Function<V, K> parentKeyGenerator,boolean ignoreNullNode)` | 批量添加节点 |
| `cn.hutool.core.map.ForestMap` | `void putLinkedNodes(K parentKey,K childKey,V childValue)` | 添加子节点，并为子节点指定父节点： 若parentKey或childKey对应的节点不存在，则会根据键值创建一个对应的节点； 若parentKey或childKey对应的节点存在，则会更新对应节点的值； |
| `cn.hutool.core.map.ForestMap` | `void putLinkedNodes(K parentKey,V parentValue,K childKey,V childValue)` | 同时添加父子节点： 若parentKey或childKey对应的节点不存在，则会根据键值创建一个对应的节点； 若parentKey或childKey对应的节点存在，则会更新对应节点的值； 该操作等同于： |
| `cn.hutool.core.map.ForestMap` | `void unlinkNode(K parentKey,K childKey)` | 若parentKey或childKey对应节点都存在，则移除指定该父节点与其直接关联的指定子节点间的引用关系 |
| `cn.hutool.core.map.LinkedForestMap` | `Collection<TreeEntry<K, V>> values()` | 返回当前实例中全部TreeEntry组成的Collection集合 |
| `cn.hutool.core.map.LinkedForestMap` | `Set<K> keySet()` | 返回当前实例中全部的key组成的Set集合 |
| `cn.hutool.core.map.LinkedForestMap` | `Set<Map.Entry<K, TreeEntry<K, V>>> entrySet()` | 由key与TreeEntry组成的键值对实体的Set集合。 注意，返回集合中Map.Entry#setValue(Object)不支持调用。 |
| `cn.hutool.core.map.LinkedForestMap` | `TreeEntry<K, V> get(Object key)` | 获取key对应的节点 |
| `cn.hutool.core.map.LinkedForestMap` | `TreeEntry<K, V> remove(Object key)` | 将指定节点从当前Map中删除 若存在父节点或子节点，则将其断开其与父节点或子节点的引用关系； 若同时存在父节点或子节点，则会在删除后将让子节点直接成为父节点的子节点，比如： 现有引用关系 a -> b -> c，删除 b 后，将有 a -> c |
| `cn.hutool.core.map.LinkedForestMap` | `TreeEntryNode<K, V> putNode(K key,V value)` | 添加一个节点 若key对应节点不存在，则以传入的键值创建一个新的节点； 若key对应节点存在，则将该节点的值替换为node指定的值； |
| `cn.hutool.core.map.LinkedForestMap` | `boolean containsKey(Object key)` | 当前实例中是否存在key对应的节点 |
| `cn.hutool.core.map.LinkedForestMap` | `boolean containsValue(Object value)` | 当前实例中是否存在对应的TreeEntry实例 |
| `cn.hutool.core.map.LinkedForestMap` | `boolean isEmpty()` | 当前实例是否为空 |
| `cn.hutool.core.map.LinkedForestMap` | `int size()` | 获取当前实例中的节点个数 |
| `cn.hutool.core.map.LinkedForestMap` | `void clear()` | 将当前集合清空，并清除全部节点间的引用关系 |
| `cn.hutool.core.map.LinkedForestMap` | `void linkNodes(K parentKey,K childKey,BiConsumer<TreeEntry<K, V>, TreeEntry<K, V>> consumer)` | 为指定的节点建立父子关系，若parentKey或childKey对应节点不存在，则会创建一个对应的值为null的空节点 |
| `cn.hutool.core.map.LinkedForestMap` | `void putLinkedNodes(K parentKey,K childKey,V childValue)` | 添加子节点，并为子节点指定父节点： 若parentKey或childKey对应的节点不存在，则会根据键值创建一个对应的节点； 若parentKey或childKey对应的节点存在，则会更新对应节点的值； |
| `cn.hutool.core.map.LinkedForestMap` | `void putLinkedNodes(K parentKey,V parentValue,K childKey,V childValue)` | 同时添加父子节点： 若parentKey或childKey对应的节点不存在，则会根据键值创建一个对应的节点； 若parentKey或childKey对应的节点存在，则会更新对应节点的值； 该操作等同于： |
| `cn.hutool.core.map.LinkedForestMap` | `void unlinkNode(K parentKey,K childKey)` | 移除指定父节点与其直接关联的子节点间的引用关系，但是不会将该节点从集合中删除 |
| `cn.hutool.core.map.LinkedForestMap$EntryNodeWrapper` | `K getKey()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.LinkedForestMap$EntryNodeWrapper` | `TreeEntry<K, V> getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.LinkedForestMap$EntryNodeWrapper` | `TreeEntry<K, V> setValue(TreeEntry<K, V> value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `K getKey()` | 获取当前节点的key |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `Map<K, TreeEntry<K, V>> getChildren()` | 获取以当前节点作为根节点的树结构，然后按广度优先获取该树结构中的当前节点的全部子节点 |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `Map<K, TreeEntry<K, V>> getDeclaredChildren()` | 获取当前节点直接关联的子节点 |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `TreeEntryNode<K, V> getChild(K key)` | 获取以当前节点作为根节点的树结构，然后获取该树结构中的当前节点的指定子节点 |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `TreeEntryNode<K, V> getDeclaredParent()` | 获取当前节点直接关联的父节点 |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `TreeEntryNode<K, V> getParent(K key)` | 获取以当前节点作为叶子节点的树结构，然后获取该树结构中当前节点的指定父节点 |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `TreeEntryNode<K, V> getRoot()` | 获取以当前节点作为叶子节点的树结构，然后获取该树结构的根节点 |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `V getValue()` | 获取节点的value |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `V setValue(V value)` | 设置节点的value |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `boolean equals(Object o)` | 比较目标对象与当前TreeEntry是否相等。 默认只要TreeEntry#getKey()的返回值相同，即认为两者相等 |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `boolean equalsKey(K key)` | 指定key与当前节点的key是否相等 |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `boolean isRoot()` | 当前节点是否为根节点 |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `int getWeight()` | 获取当前节点与根节点的距离 |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `int hashCode()` | 返回当前TreeEntry的哈希值。 默认总是返回TreeEntry#getKey()的哈希值 |
| `cn.hutool.core.map.LinkedForestMap$TreeEntryNode` | `void forEachChild(boolean includeSelf,Consumer<TreeEntry<K, V>> nodeConsumer)` | 获取以当前节点作为根节点的树结构，然后遍历所有节点 |
| `cn.hutool.core.map.MapBuilder` | `Map<K, V> build()` | 创建后的map |
| `cn.hutool.core.map.MapBuilder` | `Map<K, V> map()` | 创建后的map |
| `cn.hutool.core.map.MapBuilder` | `MapBuilder<K, V> clear()` | 清空Map |
| `cn.hutool.core.map.MapBuilder` | `MapBuilder<K, V> create()` | 创建Builder，默认HashMap实现 |
| `cn.hutool.core.map.MapBuilder` | `MapBuilder<K, V> create(Map<K, V> map)` | 创建Builder |
| `cn.hutool.core.map.MapBuilder` | `MapBuilder<K, V> create(boolean isLinked)` | 创建Builder |
| `cn.hutool.core.map.MapBuilder` | `MapBuilder<K, V> put(K k,V v)` | 链式Map创建 |
| `cn.hutool.core.map.MapBuilder` | `MapBuilder<K, V> put(boolean condition,K k,Supplier<V> supplier)` | 链式Map创建 |
| `cn.hutool.core.map.MapBuilder` | `MapBuilder<K, V> put(boolean condition,K k,V v)` | 链式Map创建 |
| `cn.hutool.core.map.MapBuilder` | `MapBuilder<K, V> putAll(Map<K, V> map)` | 链式Map创建 |
| `cn.hutool.core.map.MapBuilder` | `String join(String separator,final String keyValueSeparator)` | 将map转成字符串 |
| `cn.hutool.core.map.MapBuilder` | `String join(String separator,final String keyValueSeparator,boolean isIgnoreNull)` | 将map转成字符串 |
| `cn.hutool.core.map.MapBuilder` | `String joinIgnoreNull(String separator,final String keyValueSeparator)` | 将map转成字符串 |
| `cn.hutool.core.map.MapProxy` | `Collection<Object> values()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapProxy` | `MapProxy create(Map<?, ?> map)` | 创建代理Map 此类对Map做一次包装，提供各种getXXX方法 |
| `cn.hutool.core.map.MapProxy` | `Object get(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapProxy` | `Object getObj(Object key,Object defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapProxy` | `Object invoke(Object proxy,Method method,Object[] args)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapProxy` | `Object put(Object key,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapProxy` | `Object remove(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapProxy` | `Set<Entry<Object, Object>> entrySet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapProxy` | `Set<Object> keySet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapProxy` | `T toProxyBean(Class<T> interfaceClass)` | 将Map代理为指定接口的动态代理对象 |
| `cn.hutool.core.map.MapProxy` | `boolean containsKey(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapProxy` | `boolean containsValue(Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapProxy` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapProxy` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapProxy` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapProxy` | `void putAll(Map<?, ?> m)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapUtil` | `ArrayList<V> valuesOfKeys(Map<K, V> map,Iterator<K> keys)` | 从Map中获取指定键列表对应的值列表 如果key在map中不存在或key对应值为null，则返回值列表对应位置的值也为null |
| `cn.hutool.core.map.MapUtil` | `Boolean getBool(Map<?, ?> map,Object key)` | 获取Map指定key的值，并转换为Bool |
| `cn.hutool.core.map.MapUtil` | `Boolean getBool(Map<?, ?> map,Object key,Boolean defaultValue)` | 获取Map指定key的值，并转换为Bool |
| `cn.hutool.core.map.MapUtil` | `Character getChar(Map<?, ?> map,Object key)` | 获取Map指定key的值，并转换为Character |
| `cn.hutool.core.map.MapUtil` | `Character getChar(Map<?, ?> map,Object key,Character defaultValue)` | 获取Map指定key的值，并转换为Character |
| `cn.hutool.core.map.MapUtil` | `ConcurrentHashMap<K, V> newConcurrentHashMap()` | 新建一个初始容量为MapUtil#DEFAULT_INITIAL_CAPACITY 的ConcurrentHashMap |
| `cn.hutool.core.map.MapUtil` | `ConcurrentHashMap<K, V> newConcurrentHashMap(Map<K, V> map)` | 传入一个Map将其转化为ConcurrentHashMap类型 |
| `cn.hutool.core.map.MapUtil` | `ConcurrentHashMap<K, V> newConcurrentHashMap(int size)` | 新建一个ConcurrentHashMap |
| `cn.hutool.core.map.MapUtil` | `Date getDate(Map<?, ?> map,Object key)` | 获取Map指定key的值，并转换为Date |
| `cn.hutool.core.map.MapUtil` | `Date getDate(Map<?, ?> map,Object key,Date defaultValue)` | 获取Map指定key的值，并转换为Date |
| `cn.hutool.core.map.MapUtil` | `Double getDouble(Map<?, ?> map,Object key)` | 获取Map指定key的值，并转换为Double |
| `cn.hutool.core.map.MapUtil` | `Double getDouble(Map<?, ?> map,Object key,Double defaultValue)` | 获取Map指定key的值，并转换为Double |
| `cn.hutool.core.map.MapUtil` | `Float getFloat(Map<?, ?> map,Object key)` | 获取Map指定key的值，并转换为Float |
| `cn.hutool.core.map.MapUtil` | `Float getFloat(Map<?, ?> map,Object key,Float defaultValue)` | 获取Map指定key的值，并转换为Float |
| `cn.hutool.core.map.MapUtil` | `HashMap<K, V> newHashMap()` | 新建一个HashMap |
| `cn.hutool.core.map.MapUtil` | `HashMap<K, V> newHashMap(boolean isLinked)` | 新建一个HashMap |
| `cn.hutool.core.map.MapUtil` | `HashMap<K, V> newHashMap(int size)` | 新建一个HashMap |
| `cn.hutool.core.map.MapUtil` | `HashMap<K, V> newHashMap(int size,boolean isLinked)` | 新建一个HashMap |
| `cn.hutool.core.map.MapUtil` | `HashMap<K, V> of(K key,V value)` | 将单一键值对转换为Map |
| `cn.hutool.core.map.MapUtil` | `HashMap<K, V> of(K key,V value,boolean isOrder)` | 将单一键值对转换为Map |
| `cn.hutool.core.map.MapUtil` | `HashMap<Object, Object> of(Object[] array)` | 将数组转换为Map（HashMap），支持数组元素类型为： |
| `cn.hutool.core.map.MapUtil` | `Integer getInt(Map<?, ?> map,Object key)` | 获取Map指定key的值，并转换为Integer |
| `cn.hutool.core.map.MapUtil` | `Integer getInt(Map<?, ?> map,Object key,Integer defaultValue)` | 获取Map指定key的值，并转换为Integer |
| `cn.hutool.core.map.MapUtil` | `List<Map<K, V>> partition(Map<K, V> map,int size)` | 将一个Map按照固定大小拆分成多个子Map |
| `cn.hutool.core.map.MapUtil` | `List<Map<K, V>> toMapList(Map<K, ? extends Iterable<V>> listMap)` | 列转行。将Map中值列表分别按照其位置与key组成新的map。 是#toListMap(Iterable)的逆方法 比如传入数据： |
| `cn.hutool.core.map.MapUtil` | `Long getLong(Map<?, ?> map,Object key)` | 获取Map指定key的值，并转换为Long |
| `cn.hutool.core.map.MapUtil` | `Long getLong(Map<?, ?> map,Object key,Long defaultValue)` | 获取Map指定key的值，并转换为Long |
| `cn.hutool.core.map.MapUtil` | `Map.Entry<K, V> entry(K key,V value)` | 将键和值转换为AbstractMap.SimpleImmutableEntry 返回的Entry不可变 |
| `cn.hutool.core.map.MapUtil` | `Map.Entry<K, V> entry(K key,V value,boolean isImmutable)` | 将键和值转换为AbstractMap.SimpleEntry 或者 AbstractMap.SimpleImmutableEntry |
| `cn.hutool.core.map.MapUtil` | `Map<K, List<V>> grouping(Iterable<Map.Entry<K, V>> entries)` | 根据给定的entry列表，根据entry的key进行分组; |
| `cn.hutool.core.map.MapUtil` | `Map<K, List<V>> toListMap(Iterable<? extends Map<K, V>> mapList)` | 行转列，合并相同的键，值合并为列表 将Map列表中相同key的值组成列表做为Map的value 是#toMapList(Map)的逆方法 比如传入数据： |
| `cn.hutool.core.map.MapUtil` | `Map<K, R> map(Map<K, V> map,BiFunction<K, V, R> biFunction)` | 通过biFunction自定义一个规则，此规则将原Map中的元素转换成新的元素，生成新的Map返回 变更过程通过传入的 BiFunction 实现来返回一个值可以为不同类型的 Map |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> createMap(Class<?> mapType)` | 创建Map 传入抽象MapAbstractMap和Map类将默认创建HashMap |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> edit(Map<K, V> map,Editor<Entry<K, V>> editor)` | 编辑Map 编辑过程通过传入的Editor实现来返回需要的元素内容，这个Editor实现可以实现以下功能： |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> empty()` | 返回一个空Map |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> emptyIfNull(Map<K, V> set)` | 如果提供的集合为null，返回一个不可变的默认空集合，否则返回原集合 空集合使用Collections#emptyMap() |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> filter(Map<K, V> map,Filter<Entry<K, V>> filter)` | 过滤 过滤过程通过传入的Editor实现来返回需要的元素内容，这个Filter实现可以实现以下功能： |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> filter(Map<K, V> map,K... keys)` | 过滤Map保留指定键值对，如果键不存在跳过 |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> flatten(final Map<K, V> map)` | 将多层级Map处理为一个层级Map类型 |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> flatten(final Map<K, V> map,Map<K, V> flatMap)` | 递归调用将多层级Map处理为一个层级Map类型 |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> getAny(Map<K, V> map,final K... keys)` | 获取Map的部分key生成新的Map |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> newIdentityMap(int size)` | 创建键不重复Map |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> of(Pair<K, V>... pairs)` | 根据给定的Pair数组创建Map对象 |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> ofEntries(Map.Entry<K, V>... entries)` | 根据给定的Pair数组创建Map对象 |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> removeAny(Map<K, V> map,final K... keys)` | 去掉Map中指定key的键值对，修改原Map |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> removeByValue(final Map<K, V> map,final V value)` | 去除Map中值为指定值的键值对 注意：此方法在传入的Map上直接修改。 |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> removeIf(final Map<K, V> map,final Predicate<Entry<K, V>> predicate)` | 去除Map中值为null的键值对 注意：此方法在传入的Map上直接修改。 |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> removeNullValue(Map<K, V> map)` | 去除Map中值为null的键值对 注意：此方法在传入的Map上直接修改。 |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> renameKey(Map<K, V> map,K oldKey,K newKey)` | 重命名键 实现方式为移除然后重新put，当旧的key不存在直接返回 当新的key存在，抛出IllegalArgumentException 异常 |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> sortByValue(Map<K, V> map,boolean isDesc)` | 按照值排序，可选是否倒序 |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> toCamelCaseMap(Map<K, V> map)` | 将已知Map转换为key为驼峰风格的Map 如果KEY为非String类型，保留原值 |
| `cn.hutool.core.map.MapUtil` | `Map<K, V> unmodifiable(Map<K, V> map)` | 将对应Map转换为不可修改的Map |
| `cn.hutool.core.map.MapUtil` | `Map<T, T> reverse(Map<T, T> map)` | Map的键和值互换 互换键值对不检查值是否有重复，如果有则后加入的元素替换先加入的元素 值的顺序在HashMap中不确定，所以谁覆盖谁也不确定，在有序的Map中按照先后顺序覆盖，保留最后的值 |
| `cn.hutool.core.map.MapUtil` | `Map<V, K> inverse(Map<K, V> map)` | Map的键和值互换 互换键值对不检查值是否有重复，如果有则后加入的元素替换先加入的元素 值的顺序在HashMap中不确定，所以谁覆盖谁也不确定，在有序的Map中按照先后顺序覆盖，保留最后的值 |
| `cn.hutool.core.map.MapUtil` | `MapBuilder<K, V> builder()` | 创建链接调用map |
| `cn.hutool.core.map.MapUtil` | `MapBuilder<K, V> builder(K k,V v)` | 创建链接调用map |
| `cn.hutool.core.map.MapUtil` | `MapBuilder<K, V> builder(Map<K, V> map)` | 创建链接调用map |
| `cn.hutool.core.map.MapUtil` | `MapProxy createProxy(Map<?, ?> map)` | 创建代理Map MapProxy对Map做一次包装，提供各种getXXX方法 |
| `cn.hutool.core.map.MapUtil` | `MapWrapper<K, V> wrap(Map<K, V> map)` | 创建Map包装类MapWrapper MapWrapper对Map做一次包装 |
| `cn.hutool.core.map.MapUtil` | `Object[][] toObjectArray(Map<?, ?> map)` | 将键值对转换为二维数组，第一维是key，第二维是value |
| `cn.hutool.core.map.MapUtil` | `Short getShort(Map<?, ?> map,Object key)` | 获取Map指定key的值，并转换为Short |
| `cn.hutool.core.map.MapUtil` | `Short getShort(Map<?, ?> map,Object key,Short defaultValue)` | 获取Map指定key的值，并转换为Short |
| `cn.hutool.core.map.MapUtil` | `String getStr(Map<?, ?> map,Object key)` | 获取Map指定key的值，并转换为字符串 |
| `cn.hutool.core.map.MapUtil` | `String getStr(Map<?, ?> map,Object key,String defaultValue)` | 获取Map指定key的值，并转换为字符串 |
| `cn.hutool.core.map.MapUtil` | `String join(Map<K, V> map,String separator,String keyValueSeparator,String... otherParams)` | 将map转成字符串 |
| `cn.hutool.core.map.MapUtil` | `String join(Map<K, V> map,String separator,String keyValueSeparator,boolean isIgnoreNull,String... otherParams)` | 将map转成字符串 |
| `cn.hutool.core.map.MapUtil` | `String joinIgnoreNull(Map<K, V> map,String separator,String keyValueSeparator,String... otherParams)` | 将map转成字符串，忽略null的键和值 |
| `cn.hutool.core.map.MapUtil` | `String sortJoin(Map<?, ?> params,String separator,String keyValueSeparator,boolean isIgnoreNull,String... otherParams)` | 根据参数排序后拼接为字符串，常用于签名 |
| `cn.hutool.core.map.MapUtil` | `T defaultIfEmpty(T map,T defaultMap)` | 如果给定Map为空，返回默认Map |
| `cn.hutool.core.map.MapUtil` | `T empty(Class<?> mapClass)` | 根据传入的Map类型不同，返回对应类型的空Map，支持类型包括： |
| `cn.hutool.core.map.MapUtil` | `T get(Map<?, ?> map,Object key,Class<T> type)` | 获取Map指定key的值，并转换为指定类型 |
| `cn.hutool.core.map.MapUtil` | `T get(Map<?, ?> map,Object key,Class<T> type,T defaultValue)` | 获取Map指定key的值，并转换为指定类型 |
| `cn.hutool.core.map.MapUtil` | `T get(Map<?, ?> map,Object key,TypeReference<T> type)` | 获取Map指定key的值，并转换为指定类型 |
| `cn.hutool.core.map.MapUtil` | `T get(Map<?, ?> map,Object key,TypeReference<T> type,T defaultValue)` | 获取Map指定key的值，并转换为指定类型 |
| `cn.hutool.core.map.MapUtil` | `T getQuietly(Map<?, ?> map,Object key,Class<T> type,T defaultValue)` | 获取Map指定key的值，并转换为指定类型，此方法在转换失败后不抛异常，返回null。 |
| `cn.hutool.core.map.MapUtil` | `T getQuietly(Map<?, ?> map,Object key,TypeReference<T> type,T defaultValue)` | 获取Map指定key的值，并转换为指定类型，转换失败后返回null，不抛异常 |
| `cn.hutool.core.map.MapUtil` | `TreeMap<K, V> newTreeMap(Comparator<? super K> comparator)` | 新建TreeMap，Key有序的Map |
| `cn.hutool.core.map.MapUtil` | `TreeMap<K, V> newTreeMap(Map<K, V> map,Comparator<? super K> comparator)` | 新建TreeMap，Key有序的Map |
| `cn.hutool.core.map.MapUtil` | `TreeMap<K, V> sort(Map<K, V> map)` | 排序已有Map，Key有序的Map，使用默认Key排序方式（字母顺序） |
| `cn.hutool.core.map.MapUtil` | `TreeMap<K, V> sort(Map<K, V> map,Comparator<? super K> comparator)` | 排序已有Map，Key有序的Map |
| `cn.hutool.core.map.MapUtil` | `V computeIfAbsent(Map<K, V> map,K key,Function<? super K, ? extends V> mappingFunction)` | 如果 key 对应的 value 不存在，则使用获取 mappingFunction 重新计算后的值，并保存为该 key 的 value，否则返回 value。 方法来自Dubbo，解决使用ConcurrentHashMap.computeIfAbsent导致的死循环问题。（issues#2349） A temporary workaround for Java 8 specific performance issue JDK-8161372 . This class should be removed once we drop Java 8 support. 参考：https://githu… |
| `cn.hutool.core.map.MapUtil` | `V computeIfAbsentForJdk8(final Map<K, V> map,final K key,final Function<? super K, ? extends V> mappingFunction)` | 如果 key 对应的 value 不存在，则使用获取 mappingFunction 重新计算后的值，并保存为该 key 的 value，否则返回 value。 解决使用ConcurrentHashMap.computeIfAbsent导致的死循环问题。（issues#2349） A temporary workaround for Java 8 specific performance issue JDK-8161372 . This class should be removed once we drop Java 8 support. 注意此方法只能用于JDK8 |
| `cn.hutool.core.map.MapUtil` | `boolean isEmpty(Map<?, ?> map)` | Map是否为空 |
| `cn.hutool.core.map.MapUtil` | `boolean isNotEmpty(Map<?, ?> map)` | Map是否为非空 |
| `cn.hutool.core.map.MapUtil` | `void clear(Map<?, ?>... maps)` | 清除一个或多个Map集合内的元素，每个Map调用clear()方法 |
| `cn.hutool.core.map.MapWrapper` | `Collection<V> values()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `Iterator<Entry<K, V>> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `Map<K, V> getRaw()` | 获取原始的Map |
| `cn.hutool.core.map.MapWrapper` | `MapWrapper<K, V> clone()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `Set<Entry<K, V>> entrySet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `Set<K> keySet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `V compute(K key,BiFunction<? super K, ? super V, ? extends V> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `V computeIfAbsent(K key,Function<? super K, ? extends V> mappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `V computeIfPresent(K key,BiFunction<? super K, ? super V, ? extends V> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `V get(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `V getOrDefault(Object key,V defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `V merge(K key,V value,BiFunction<? super V, ? super V, ? extends V> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `V put(K key,V value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `V putIfAbsent(K key,V value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `V remove(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `V replace(K key,V value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `boolean containsKey(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `boolean containsValue(Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `boolean equals(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `boolean remove(Object key,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `boolean replace(K key,V oldValue,V newValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `void forEach(BiConsumer<? super K, ? super V> action)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `void putAll(Map<? extends K, ? extends V> m)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.MapWrapper` | `void replaceAll(BiFunction<? super K, ? super V, ? extends V> function)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `Collection<V> values()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `Iterator<Entry<K, V>> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `Set<Entry<K, V>> entrySet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `Set<K> keySet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `V compute(K key,BiFunction<? super K, ? super V, ? extends V> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `V computeIfAbsent(K key,Func0<? extends V> supplier)` | 从缓存中获得对象，当对象不在缓存中或已经过期返回Func0回调产生的对象 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `V computeIfAbsent(K key,Function<? super K, ? extends V> mappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `V computeIfPresent(K key,BiFunction<? super K, ? super V, ? extends V> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `V get(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `V merge(K key,V value,BiFunction<? super V, ? super V, ? extends V> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `V put(K key,V value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `V putIfAbsent(K key,V value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `V remove(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `V replace(K key,V value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `boolean containsKey(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `boolean containsValue(Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `boolean remove(Object key,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `boolean replace(K key,V oldValue,V newValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `void forEach(BiConsumer<? super K, ? super V> action)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `void putAll(Map<? extends K, ? extends V> m)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `void replaceAll(BiFunction<? super K, ? super V, ? extends V> function)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.ReferenceConcurrentMap` | `void setPurgeListener(BiConsumer<Reference<? extends K>, V> purgeListener)` | 设置对象回收清除监听 |
| `cn.hutool.core.map.SafeConcurrentHashMap` | `V computeIfAbsent(K key,Function<? super K, ? extends V> mappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `Collection<V> values()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `Iterator<Map.Entry<K, V>> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `K getKey(V value)` | 根据value获得对应的key，只返回找到的第一个value对应的key值 |
| `cn.hutool.core.map.TableMap` | `List<K> getKeys(V value)` | 获取指定value对应的所有key |
| `cn.hutool.core.map.TableMap` | `List<K> keys()` | 获取所有键，可重复，不可修改 |
| `cn.hutool.core.map.TableMap` | `List<V> getValues(K key)` | 获取指定key对应的所有值 |
| `cn.hutool.core.map.TableMap` | `Set<K> keySet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `Set<Map.Entry<K, V>> entrySet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `V computeIfPresent(final K key,final BiFunction<? super K, ? super V, ? extends V> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `V get(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `V put(K key,V value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `V remove(Object key)` | 移除指定的所有键和对应的所有值 |
| `cn.hutool.core.map.TableMap` | `V removeByIndex(final int index)` | 移除指定位置的键值对 |
| `cn.hutool.core.map.TableMap` | `V replace(final K key,final V value)` | 替换指定key的所有值为指定值 |
| `cn.hutool.core.map.TableMap` | `boolean containsKey(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `boolean containsValue(Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `boolean remove(final Object key,final Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `boolean replace(final K key,final V oldValue,final V newValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `void forEach(final BiConsumer<? super K, ? super V> action)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `void putAll(Map<? extends K, ? extends V> m)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TableMap` | `void replaceAll(final BiFunction<? super K, ? super V, ? extends V> function)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TolerantMap` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TolerantMap` | `TolerantMap<K, V> of(Map<K, V> map,V defaultValue)` | 构建TolerantMap |
| `cn.hutool.core.map.TolerantMap` | `V get(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TolerantMap` | `boolean equals(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TolerantMap` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TransMap` | `V compute(K key,BiFunction<? super K, ? super V, ? extends V> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TransMap` | `V computeIfAbsent(final K key,final Function<? super K, ? extends V> mappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TransMap` | `V computeIfPresent(K key,BiFunction<? super K, ? super V, ? extends V> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TransMap` | `V get(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TransMap` | `V getOrDefault(Object key,V defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TransMap` | `V merge(K key,V value,BiFunction<? super V, ? super V, ? extends V> remappingFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TransMap` | `V put(K key,V value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TransMap` | `V putIfAbsent(K key,V value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TransMap` | `V remove(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TransMap` | `V replace(K key,V value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TransMap` | `boolean containsKey(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TransMap` | `boolean remove(Object key,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TransMap` | `boolean replace(K key,V oldValue,V newValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TransMap` | `void putAll(Map<? extends K, ? extends V> m)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.TreeEntry` | `Map<K, TreeEntry<K, V>> getChildren()` | 获取以当前节点作为根节点的树结构，然后获取该树结构中的当前节点的全部子节点 |
| `cn.hutool.core.map.TreeEntry` | `Map<K, TreeEntry<K, V>> getDeclaredChildren()` | 获取当前节点直接关联的子节点 |
| `cn.hutool.core.map.TreeEntry` | `TreeEntry<K, V> getChild(K key)` | 获取以当前节点作为根节点的树结构，然后获取该树结构中的当前节点的指定子节点 |
| `cn.hutool.core.map.TreeEntry` | `TreeEntry<K, V> getDeclaredParent()` | 获取当前节点直接关联的父节点 |
| `cn.hutool.core.map.TreeEntry` | `TreeEntry<K, V> getParent(K key)` | 获取以当前节点作为叶子节点的树结构，然后获取该树结构中当前节点的指定父节点 |
| `cn.hutool.core.map.TreeEntry` | `TreeEntry<K, V> getRoot()` | 获取以当前节点作为叶子节点的树结构，然后获取该树结构的根节点 |
| `cn.hutool.core.map.TreeEntry` | `boolean containsChild(K key)` | 获取以当前节点作为根节点的树结构，然后确认该树结构中当前节点是否存在指定子节点 |
| `cn.hutool.core.map.TreeEntry` | `boolean containsParent(K key)` | 获取以当前节点作为叶子节点的树结构，然后确认该树结构中当前节点是否存在指定父节点 |
| `cn.hutool.core.map.TreeEntry` | `boolean equals(Object o)` | 比较目标对象与当前TreeEntry是否相等。 默认只要TreeEntry#getKey()的返回值相同，即认为两者相等 |
| `cn.hutool.core.map.TreeEntry` | `boolean hasChildren()` | 当前节点是否有子节点 |
| `cn.hutool.core.map.TreeEntry` | `boolean hasParent()` | 当前节点是否存在直接关联的父节点 |
| `cn.hutool.core.map.TreeEntry` | `int getWeight()` | 获取以当前节点作为叶子节点的树结构，然后获取当前节点与根节点的距离 |
| `cn.hutool.core.map.TreeEntry` | `int hashCode()` | 返回当前TreeEntry的哈希值。 默认总是返回TreeEntry#getKey()的哈希值 |
| `cn.hutool.core.map.TreeEntry` | `void forEachChild(boolean includeSelf,Consumer<TreeEntry<K, V>> nodeConsumer)` | 获取以当前节点作为根节点的树结构，然后遍历所有节点 |
