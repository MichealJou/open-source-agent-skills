# cn.hutool.core.map

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.map.AbsEntry`

```java
public abstract class cn.hutool.core.map.AbsEntry<K, V> implements java.util.Map$Entry<K, V> {
  public cn.hutool.core.map.AbsEntry();
  public V setValue(V);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `cn.hutool.core.map.BiMap`

```java
public class cn.hutool.core.map.BiMap<K, V> extends cn.hutool.core.map.MapWrapper<K, V> {
  public cn.hutool.core.map.BiMap(java.util.Map<K, V>);
  public V put(K, V);
  public void putAll(java.util.Map<? extends K, ? extends V>);
  public V remove(java.lang.Object);
  public boolean remove(java.lang.Object, java.lang.Object);
  public void clear();
  public java.util.Map<V, K> getInverse();
  public K getKey(V);
  public V putIfAbsent(K, V);
  public V computeIfAbsent(K, java.util.function.Function<? super K, ? extends V>);
  public V computeIfPresent(K, java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public V compute(K, java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public V merge(K, V, java.util.function.BiFunction<? super V, ? super V, ? extends V>);
}
```

## `cn.hutool.core.map.CamelCaseLinkedMap`

```java
public class cn.hutool.core.map.CamelCaseLinkedMap<K, V> extends cn.hutool.core.map.CamelCaseMap<K, V> {
  public cn.hutool.core.map.CamelCaseLinkedMap();
  public cn.hutool.core.map.CamelCaseLinkedMap(int);
  public cn.hutool.core.map.CamelCaseLinkedMap(java.util.Map<? extends K, ? extends V>);
  public cn.hutool.core.map.CamelCaseLinkedMap(float, java.util.Map<? extends K, ? extends V>);
  public cn.hutool.core.map.CamelCaseLinkedMap(int, float);
}
```

## `cn.hutool.core.map.CamelCaseMap`

```java
public class cn.hutool.core.map.CamelCaseMap<K, V> extends cn.hutool.core.map.FuncKeyMap<K, V> {
  public cn.hutool.core.map.CamelCaseMap();
  public cn.hutool.core.map.CamelCaseMap(int);
  public cn.hutool.core.map.CamelCaseMap(java.util.Map<? extends K, ? extends V>);
  public cn.hutool.core.map.CamelCaseMap(float, java.util.Map<? extends K, ? extends V>);
  public cn.hutool.core.map.CamelCaseMap(int, float);
}
```

## `cn.hutool.core.map.CaseInsensitiveLinkedMap`

```java
public class cn.hutool.core.map.CaseInsensitiveLinkedMap<K, V> extends cn.hutool.core.map.CaseInsensitiveMap<K, V> {
  public cn.hutool.core.map.CaseInsensitiveLinkedMap();
  public cn.hutool.core.map.CaseInsensitiveLinkedMap(int);
  public cn.hutool.core.map.CaseInsensitiveLinkedMap(java.util.Map<? extends K, ? extends V>);
  public cn.hutool.core.map.CaseInsensitiveLinkedMap(float, java.util.Map<? extends K, ? extends V>);
  public cn.hutool.core.map.CaseInsensitiveLinkedMap(int, float);
}
```

## `cn.hutool.core.map.CaseInsensitiveMap`

```java
public class cn.hutool.core.map.CaseInsensitiveMap<K, V> extends cn.hutool.core.map.FuncKeyMap<K, V> {
  public cn.hutool.core.map.CaseInsensitiveMap();
  public cn.hutool.core.map.CaseInsensitiveMap(int);
  public cn.hutool.core.map.CaseInsensitiveMap(java.util.Map<? extends K, ? extends V>);
  public cn.hutool.core.map.CaseInsensitiveMap(float, java.util.Map<? extends K, ? extends V>);
  public cn.hutool.core.map.CaseInsensitiveMap(int, float);
}
```

## `cn.hutool.core.map.CaseInsensitiveTreeMap`

```java
public class cn.hutool.core.map.CaseInsensitiveTreeMap<K, V> extends cn.hutool.core.map.CaseInsensitiveMap<K, V> {
  public cn.hutool.core.map.CaseInsensitiveTreeMap();
  public cn.hutool.core.map.CaseInsensitiveTreeMap(java.util.Map<? extends K, ? extends V>);
  public cn.hutool.core.map.CaseInsensitiveTreeMap(java.util.SortedMap<? extends K, ? extends V>);
  public cn.hutool.core.map.CaseInsensitiveTreeMap(java.util.Comparator<? super K>);
}
```

## `cn.hutool.core.map.CustomKeyMap`

```java
public abstract class cn.hutool.core.map.CustomKeyMap<K, V> extends cn.hutool.core.map.TransMap<K, V> {
  public cn.hutool.core.map.CustomKeyMap(java.util.Map<K, V>);
}
```

## `cn.hutool.core.map.FixedLinkedHashMap`

```java
public class cn.hutool.core.map.FixedLinkedHashMap<K, V> extends java.util.LinkedHashMap<K, V> {
  public cn.hutool.core.map.FixedLinkedHashMap(int);
  public int getCapacity();
  public void setCapacity(int);
  public void setRemoveListener(java.util.function.Consumer<java.util.Map$Entry<K, V>>);
}
```

## `cn.hutool.core.map.ForestMap`

```java
public interface cn.hutool.core.map.ForestMap<K, V> extends java.util.Map<K, cn.hutool.core.map.TreeEntry<K, V>> {
  public default cn.hutool.core.map.TreeEntry<K, V> put(K, cn.hutool.core.map.TreeEntry<K, V>);
  public default void putAll(java.util.Map<? extends K, ? extends cn.hutool.core.map.TreeEntry<K, V>>);
  public abstract cn.hutool.core.map.TreeEntry<K, V> remove(java.lang.Object);
  public abstract void clear();
  public default <C extends java.util.Collection<V>> void putAllNode(C, java.util.function.Function<V, K>, java.util.function.Function<V, K>, boolean);
  public abstract cn.hutool.core.map.TreeEntry<K, V> putNode(K, V);
  public default void putLinkedNodes(K, V, K, V);
  public abstract void putLinkedNodes(K, K, V);
  public default void linkNodes(K, K);
  public abstract void linkNodes(K, K, java.util.function.BiConsumer<cn.hutool.core.map.TreeEntry<K, V>, cn.hutool.core.map.TreeEntry<K, V>>);
  public abstract void unlinkNode(K, K);
  public default java.util.Set<cn.hutool.core.map.TreeEntry<K, V>> getTreeNodes(K);
  public default cn.hutool.core.map.TreeEntry<K, V> getRootNode(K);
  public default cn.hutool.core.map.TreeEntry<K, V> getDeclaredParentNode(K);
  public default cn.hutool.core.map.TreeEntry<K, V> getParentNode(K, K);
  public default boolean containsParentNode(K, K);
  public default V getNodeValue(K);
  public default boolean containsChildNode(K, K);
  public default java.util.Collection<cn.hutool.core.map.TreeEntry<K, V>> getDeclaredChildNodes(K);
  public default java.util.Collection<cn.hutool.core.map.TreeEntry<K, V>> getChildNodes(K);
  public default java.lang.Object remove(java.lang.Object);
  public default java.lang.Object put(java.lang.Object, java.lang.Object);
}
```

## `cn.hutool.core.map.FuncKeyMap`

```java
public class cn.hutool.core.map.FuncKeyMap<K, V> extends cn.hutool.core.map.CustomKeyMap<K, V> {
  public cn.hutool.core.map.FuncKeyMap(java.util.Map<K, V>, java.util.function.Function<java.lang.Object, K>);
}
```

## `cn.hutool.core.map.FuncMap`

```java
public class cn.hutool.core.map.FuncMap<K, V> extends cn.hutool.core.map.TransMap<K, V> {
  public cn.hutool.core.map.FuncMap(java.util.function.Supplier<java.util.Map<K, V>>, java.util.function.Function<java.lang.Object, K>, java.util.function.Function<java.lang.Object, V>);
  public cn.hutool.core.map.FuncMap(java.util.Map<K, V>, java.util.function.Function<java.lang.Object, K>, java.util.function.Function<java.lang.Object, V>);
}
```

## `cn.hutool.core.map.LinkedForestMap`

```java
public class cn.hutool.core.map.LinkedForestMap<K, V> implements cn.hutool.core.map.ForestMap<K, V> {
  public cn.hutool.core.map.LinkedForestMap(boolean);
  public int size();
  public boolean isEmpty();
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public cn.hutool.core.map.TreeEntry<K, V> get(java.lang.Object);
  public cn.hutool.core.map.TreeEntry<K, V> remove(java.lang.Object);
  public void clear();
  public java.util.Set<K> keySet();
  public java.util.Collection<cn.hutool.core.map.TreeEntry<K, V>> values();
  public java.util.Set<java.util.Map$Entry<K, cn.hutool.core.map.TreeEntry<K, V>>> entrySet();
  public cn.hutool.core.map.LinkedForestMap$TreeEntryNode<K, V> putNode(K, V);
  public void putLinkedNodes(K, V, K, V);
  public void putLinkedNodes(K, K, V);
  public void linkNodes(K, K, java.util.function.BiConsumer<cn.hutool.core.map.TreeEntry<K, V>, cn.hutool.core.map.TreeEntry<K, V>>);
  public void unlinkNode(K, K);
  public cn.hutool.core.map.TreeEntry putNode(java.lang.Object, java.lang.Object);
  public java.lang.Object remove(java.lang.Object);
  public java.lang.Object get(java.lang.Object);
}
```

## `cn.hutool.core.map.LinkedForestMap$EntryNodeWrapper`

```java
public class cn.hutool.core.map.LinkedForestMap$EntryNodeWrapper<K, V, N extends cn.hutool.core.map.TreeEntry<K, V>> implements java.util.Map$Entry<K, cn.hutool.core.map.TreeEntry<K, V>> {
  public K getKey();
  public cn.hutool.core.map.TreeEntry<K, V> getValue();
  public cn.hutool.core.map.TreeEntry<K, V> setValue(cn.hutool.core.map.TreeEntry<K, V>);
  public java.lang.Object setValue(java.lang.Object);
  public java.lang.Object getValue();
}
```

## `cn.hutool.core.map.LinkedForestMap$TreeEntryNode`

```java
public class cn.hutool.core.map.LinkedForestMap$TreeEntryNode<K, V> implements cn.hutool.core.map.TreeEntry<K, V> {
  public cn.hutool.core.map.LinkedForestMap$TreeEntryNode(cn.hutool.core.map.LinkedForestMap$TreeEntryNode<K, V>, K);
  public cn.hutool.core.map.LinkedForestMap$TreeEntryNode(cn.hutool.core.map.LinkedForestMap$TreeEntryNode<K, V>, K, V);
  public K getKey();
  public int getWeight();
  public V getValue();
  public V setValue(V);
  public boolean isRoot();
  public cn.hutool.core.map.LinkedForestMap$TreeEntryNode<K, V> getRoot();
  public cn.hutool.core.map.LinkedForestMap$TreeEntryNode<K, V> getDeclaredParent();
  public cn.hutool.core.map.LinkedForestMap$TreeEntryNode<K, V> getParent(K);
  public void forEachChild(boolean, java.util.function.Consumer<cn.hutool.core.map.TreeEntry<K, V>>);
  public boolean equalsKey(K);
  public cn.hutool.core.map.LinkedForestMap$TreeEntryNode<K, V> getChild(K);
  public java.util.Map<K, cn.hutool.core.map.TreeEntry<K, V>> getDeclaredChildren();
  public java.util.Map<K, cn.hutool.core.map.TreeEntry<K, V>> getChildren();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public cn.hutool.core.map.TreeEntry getChild(java.lang.Object);
  public cn.hutool.core.map.TreeEntry getParent(java.lang.Object);
  public cn.hutool.core.map.TreeEntry getDeclaredParent();
  public cn.hutool.core.map.TreeEntry getRoot();
}
```

## `cn.hutool.core.map.MapBuilder`

```java
public class cn.hutool.core.map.MapBuilder<K, V> implements cn.hutool.core.builder.Builder<java.util.Map<K, V>> {
  public static <K, V> cn.hutool.core.map.MapBuilder<K, V> create();
  public static <K, V> cn.hutool.core.map.MapBuilder<K, V> create(boolean);
  public static <K, V> cn.hutool.core.map.MapBuilder<K, V> create(java.util.Map<K, V>);
  public cn.hutool.core.map.MapBuilder(java.util.Map<K, V>);
  public cn.hutool.core.map.MapBuilder<K, V> put(K, V);
  public cn.hutool.core.map.MapBuilder<K, V> put(boolean, K, V);
  public cn.hutool.core.map.MapBuilder<K, V> put(boolean, K, java.util.function.Supplier<V>);
  public cn.hutool.core.map.MapBuilder<K, V> putAll(java.util.Map<K, V>);
  public cn.hutool.core.map.MapBuilder<K, V> clear();
  public java.util.Map<K, V> map();
  public java.util.Map<K, V> build();
  public java.lang.String join(java.lang.String, java.lang.String);
  public java.lang.String joinIgnoreNull(java.lang.String, java.lang.String);
  public java.lang.String join(java.lang.String, java.lang.String, boolean);
  public java.lang.Object build();
}
```

## `cn.hutool.core.map.MapProxy`

```java
public class cn.hutool.core.map.MapProxy implements java.util.Map<java.lang.Object, java.lang.Object>, cn.hutool.core.getter.OptNullBasicTypeFromObjectGetter<java.lang.Object>, java.lang.reflect.InvocationHandler, java.io.Serializable {
  public static cn.hutool.core.map.MapProxy create(java.util.Map<?, ?>);
  public cn.hutool.core.map.MapProxy(java.util.Map<?, ?>);
  public java.lang.Object getObj(java.lang.Object, java.lang.Object);
  public int size();
  public boolean isEmpty();
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public java.lang.Object get(java.lang.Object);
  public java.lang.Object put(java.lang.Object, java.lang.Object);
  public java.lang.Object remove(java.lang.Object);
  public void putAll(java.util.Map<?, ?>);
  public void clear();
  public java.util.Set<java.lang.Object> keySet();
  public java.util.Collection<java.lang.Object> values();
  public java.util.Set<java.util.Map$Entry<java.lang.Object, java.lang.Object>> entrySet();
  public java.lang.Object invoke(java.lang.Object, java.lang.reflect.Method, java.lang.Object[]);
  public <T> T toProxyBean(java.lang.Class<T>);
}
```

## `cn.hutool.core.map.MapUtil`

```java
public class cn.hutool.core.map.MapUtil {
  public cn.hutool.core.map.MapUtil();
  public static boolean isEmpty(java.util.Map<?, ?>);
  public static boolean isNotEmpty(java.util.Map<?, ?>);
  public static <K, V> java.util.Map<K, V> emptyIfNull(java.util.Map<K, V>);
  public static <T extends java.util.Map<K, V>, K, V> T defaultIfEmpty(T, T);
  public static <K, V> java.util.HashMap<K, V> newHashMap();
  public static <K, V> java.util.HashMap<K, V> newHashMap(int, boolean);
  public static <K, V> java.util.HashMap<K, V> newHashMap(int);
  public static <K, V> java.util.HashMap<K, V> newHashMap(boolean);
  public static <K, V> java.util.TreeMap<K, V> newTreeMap(java.util.Comparator<? super K>);
  public static <K, V> java.util.TreeMap<K, V> newTreeMap(java.util.Map<K, V>, java.util.Comparator<? super K>);
  public static <K, V> java.util.Map<K, V> newIdentityMap(int);
  public static <K, V> java.util.concurrent.ConcurrentHashMap<K, V> newConcurrentHashMap();
  public static <K, V> java.util.concurrent.ConcurrentHashMap<K, V> newConcurrentHashMap(int);
  public static <K, V> java.util.concurrent.ConcurrentHashMap<K, V> newConcurrentHashMap(java.util.Map<K, V>);
  public static <K, V> java.util.Map<K, V> createMap(java.lang.Class<?>);
  public static <K, V> java.util.HashMap<K, V> of(K, V);
  public static <K, V> java.util.HashMap<K, V> of(K, V, boolean);
  public static <K, V> java.util.Map<K, V> of(cn.hutool.core.lang.Pair<K, V>...);
  public static <K, V> java.util.Map<K, V> ofEntries(java.util.Map$Entry<K, V>...);
  public static java.util.HashMap<java.lang.Object, java.lang.Object> of(java.lang.Object[]);
  public static <K, V> java.util.Map<K, java.util.List<V>> toListMap(java.lang.Iterable<? extends java.util.Map<K, V>>);
  public static <K, V> java.util.List<java.util.Map<K, V>> toMapList(java.util.Map<K, ? extends java.lang.Iterable<V>>);
  public static <K, V> java.util.Map<K, java.util.List<V>> grouping(java.lang.Iterable<java.util.Map$Entry<K, V>>);
  public static <K, V> java.util.Map<K, V> toCamelCaseMap(java.util.Map<K, V>);
  public static java.lang.Object[][] toObjectArray(java.util.Map<?, ?>);
  public static <K, V> java.lang.String join(java.util.Map<K, V>, java.lang.String, java.lang.String, java.lang.String...);
  public static java.lang.String sortJoin(java.util.Map<?, ?>, java.lang.String, java.lang.String, boolean, java.lang.String...);
  public static <K, V> java.lang.String joinIgnoreNull(java.util.Map<K, V>, java.lang.String, java.lang.String, java.lang.String...);
  public static <K, V> java.lang.String join(java.util.Map<K, V>, java.lang.String, java.lang.String, boolean, java.lang.String...);
  public static <K, V> java.util.Map<K, V> edit(java.util.Map<K, V>, cn.hutool.core.lang.Editor<java.util.Map$Entry<K, V>>);
  public static <K, V> java.util.Map<K, V> filter(java.util.Map<K, V>, cn.hutool.core.lang.Filter<java.util.Map$Entry<K, V>>);
  public static <K, V, R> java.util.Map<K, R> map(java.util.Map<K, V>, java.util.function.BiFunction<K, V, R>);
  public static <K, V> java.util.Map<K, V> filter(java.util.Map<K, V>, K...);
  public static <T> java.util.Map<T, T> reverse(java.util.Map<T, T>);
  public static <K, V> java.util.Map<V, K> inverse(java.util.Map<K, V>);
  public static <K, V> java.util.TreeMap<K, V> sort(java.util.Map<K, V>);
  public static <K, V> java.util.TreeMap<K, V> sort(java.util.Map<K, V>, java.util.Comparator<? super K>);
  public static <K, V extends java.lang.Comparable<? super V>> java.util.Map<K, V> sortByValue(java.util.Map<K, V>, boolean);
  public static cn.hutool.core.map.MapProxy createProxy(java.util.Map<?, ?>);
  public static <K, V> cn.hutool.core.map.MapWrapper<K, V> wrap(java.util.Map<K, V>);
  public static <K, V> java.util.Map<K, V> unmodifiable(java.util.Map<K, V>);
  public static <K, V> cn.hutool.core.map.MapBuilder<K, V> builder();
  public static <K, V> cn.hutool.core.map.MapBuilder<K, V> builder(java.util.Map<K, V>);
  public static <K, V> cn.hutool.core.map.MapBuilder<K, V> builder(K, V);
  public static <K, V> java.util.Map<K, V> getAny(java.util.Map<K, V>, K...);
  public static <K, V> java.util.Map<K, V> removeAny(java.util.Map<K, V>, K...);
  public static java.lang.String getStr(java.util.Map<?, ?>, java.lang.Object);
  public static java.lang.String getStr(java.util.Map<?, ?>, java.lang.Object, java.lang.String);
  public static java.lang.Integer getInt(java.util.Map<?, ?>, java.lang.Object);
  public static java.lang.Integer getInt(java.util.Map<?, ?>, java.lang.Object, java.lang.Integer);
  public static java.lang.Double getDouble(java.util.Map<?, ?>, java.lang.Object);
  public static java.lang.Double getDouble(java.util.Map<?, ?>, java.lang.Object, java.lang.Double);
  public static java.lang.Float getFloat(java.util.Map<?, ?>, java.lang.Object);
  public static java.lang.Float getFloat(java.util.Map<?, ?>, java.lang.Object, java.lang.Float);
  public static java.lang.Short getShort(java.util.Map<?, ?>, java.lang.Object);
  public static java.lang.Short getShort(java.util.Map<?, ?>, java.lang.Object, java.lang.Short);
  public static java.lang.Boolean getBool(java.util.Map<?, ?>, java.lang.Object);
  public static java.lang.Boolean getBool(java.util.Map<?, ?>, java.lang.Object, java.lang.Boolean);
  public static java.lang.Character getChar(java.util.Map<?, ?>, java.lang.Object);
  public static java.lang.Character getChar(java.util.Map<?, ?>, java.lang.Object, java.lang.Character);
  public static java.lang.Long getLong(java.util.Map<?, ?>, java.lang.Object);
  public static java.lang.Long getLong(java.util.Map<?, ?>, java.lang.Object, java.lang.Long);
  public static java.util.Date getDate(java.util.Map<?, ?>, java.lang.Object);
  public static java.util.Date getDate(java.util.Map<?, ?>, java.lang.Object, java.util.Date);
  public static <T> T get(java.util.Map<?, ?>, java.lang.Object, java.lang.Class<T>);
  public static <T> T get(java.util.Map<?, ?>, java.lang.Object, java.lang.Class<T>, T);
  public static <T> T getQuietly(java.util.Map<?, ?>, java.lang.Object, java.lang.Class<T>, T);
  public static <T> T get(java.util.Map<?, ?>, java.lang.Object, cn.hutool.core.lang.TypeReference<T>);
  public static <T> T get(java.util.Map<?, ?>, java.lang.Object, cn.hutool.core.lang.TypeReference<T>, T);
  public static <T> T getQuietly(java.util.Map<?, ?>, java.lang.Object, cn.hutool.core.lang.TypeReference<T>, T);
  public static <K, V> java.util.Map<K, V> renameKey(java.util.Map<K, V>, K, K);
  public static <K, V> java.util.Map<K, V> removeNullValue(java.util.Map<K, V>);
  public static <K, V> java.util.Map<K, V> removeByValue(java.util.Map<K, V>, V);
  public static <K, V> java.util.Map<K, V> removeIf(java.util.Map<K, V>, java.util.function.Predicate<java.util.Map$Entry<K, V>>);
  public static <K, V> java.util.Map<K, V> empty();
  public static <K, V, T extends java.util.Map<K, V>> T empty(java.lang.Class<?>);
  public static void clear(java.util.Map<?, ?>...);
  public static <K, V> java.util.ArrayList<V> valuesOfKeys(java.util.Map<K, V>, java.util.Iterator<K>);
  public static <K, V> java.util.Map$Entry<K, V> entry(K, V);
  public static <K, V> java.util.Map$Entry<K, V> entry(K, V, boolean);
  public static <K, V> V computeIfAbsent(java.util.Map<K, V>, K, java.util.function.Function<? super K, ? extends V>);
  public static <K, V> V computeIfAbsentForJdk8(java.util.Map<K, V>, K, java.util.function.Function<? super K, ? extends V>);
  public static <K, V> java.util.List<java.util.Map<K, V>> partition(java.util.Map<K, V>, int);
  public static <K, V> java.util.Map<K, V> flatten(java.util.Map<K, V>);
  public static <K, V> java.util.Map<K, V> flatten(java.util.Map<K, V>, java.util.Map<K, V>);
}
```

## `cn.hutool.core.map.MapWrapper`

```java
public class cn.hutool.core.map.MapWrapper<K, V> implements java.util.Map<K, V>, java.lang.Iterable<java.util.Map$Entry<K, V>>, java.io.Serializable, java.lang.Cloneable {
  public cn.hutool.core.map.MapWrapper(java.util.function.Supplier<java.util.Map<K, V>>);
  public cn.hutool.core.map.MapWrapper(java.util.Map<K, V>);
  public java.util.Map<K, V> getRaw();
  public int size();
  public boolean isEmpty();
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public V get(java.lang.Object);
  public V put(K, V);
  public V remove(java.lang.Object);
  public void putAll(java.util.Map<? extends K, ? extends V>);
  public void clear();
  public java.util.Collection<V> values();
  public java.util.Set<K> keySet();
  public java.util.Set<java.util.Map$Entry<K, V>> entrySet();
  public java.util.Iterator<java.util.Map$Entry<K, V>> iterator();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public void forEach(java.util.function.BiConsumer<? super K, ? super V>);
  public void replaceAll(java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public V putIfAbsent(K, V);
  public boolean remove(java.lang.Object, java.lang.Object);
  public boolean replace(K, V, V);
  public V replace(K, V);
  public V computeIfAbsent(K, java.util.function.Function<? super K, ? extends V>);
  public V getOrDefault(java.lang.Object, V);
  public V computeIfPresent(K, java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public V compute(K, java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public V merge(K, V, java.util.function.BiFunction<? super V, ? super V, ? extends V>);
  public cn.hutool.core.map.MapWrapper<K, V> clone() throws java.lang.CloneNotSupportedException;
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `cn.hutool.core.map.ReferenceConcurrentMap`

```java
public class cn.hutool.core.map.ReferenceConcurrentMap<K, V> implements java.util.concurrent.ConcurrentMap<K, V>, java.lang.Iterable<java.util.Map$Entry<K, V>>, java.io.Serializable {
  public cn.hutool.core.map.ReferenceConcurrentMap(java.util.concurrent.ConcurrentMap<java.lang.ref.Reference<K>, V>, cn.hutool.core.util.ReferenceUtil$ReferenceType);
  public void setPurgeListener(java.util.function.BiConsumer<java.lang.ref.Reference<? extends K>, V>);
  public int size();
  public boolean isEmpty();
  public V get(java.lang.Object);
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public V put(K, V);
  public V putIfAbsent(K, V);
  public void putAll(java.util.Map<? extends K, ? extends V>);
  public V replace(K, V);
  public boolean replace(K, V, V);
  public void replaceAll(java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public V computeIfAbsent(K, java.util.function.Function<? super K, ? extends V>);
  public V computeIfPresent(K, java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public V computeIfAbsent(K, cn.hutool.core.lang.func.Func0<? extends V>);
  public V remove(java.lang.Object);
  public boolean remove(java.lang.Object, java.lang.Object);
  public void clear();
  public java.util.Set<K> keySet();
  public java.util.Collection<V> values();
  public java.util.Set<java.util.Map$Entry<K, V>> entrySet();
  public void forEach(java.util.function.BiConsumer<? super K, ? super V>);
  public java.util.Iterator<java.util.Map$Entry<K, V>> iterator();
  public V compute(K, java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public V merge(K, V, java.util.function.BiFunction<? super V, ? super V, ? extends V>);
}
```

## `cn.hutool.core.map.SafeConcurrentHashMap`

```java
public class cn.hutool.core.map.SafeConcurrentHashMap<K, V> extends java.util.concurrent.ConcurrentHashMap<K, V> {
  public cn.hutool.core.map.SafeConcurrentHashMap();
  public cn.hutool.core.map.SafeConcurrentHashMap(int);
  public cn.hutool.core.map.SafeConcurrentHashMap(java.util.Map<? extends K, ? extends V>);
  public cn.hutool.core.map.SafeConcurrentHashMap(int, float);
  public cn.hutool.core.map.SafeConcurrentHashMap(int, float, int);
  public V computeIfAbsent(K, java.util.function.Function<? super K, ? extends V>);
}
```

## `cn.hutool.core.map.TableMap`

```java
public class cn.hutool.core.map.TableMap<K, V> implements java.util.Map<K, V>, java.lang.Iterable<java.util.Map$Entry<K, V>>, java.io.Serializable {
  public cn.hutool.core.map.TableMap();
  public cn.hutool.core.map.TableMap(int);
  public cn.hutool.core.map.TableMap(K[], V[]);
  public int size();
  public boolean isEmpty();
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public V get(java.lang.Object);
  public K getKey(V);
  public java.util.List<V> getValues(K);
  public java.util.List<K> getKeys(V);
  public V put(K, V);
  public V remove(java.lang.Object);
  public V removeByIndex(int);
  public void putAll(java.util.Map<? extends K, ? extends V>);
  public void clear();
  public java.util.Set<K> keySet();
  public java.util.List<K> keys();
  public java.util.Collection<V> values();
  public java.util.Set<java.util.Map$Entry<K, V>> entrySet();
  public java.util.Iterator<java.util.Map$Entry<K, V>> iterator();
  public java.lang.String toString();
  public void forEach(java.util.function.BiConsumer<? super K, ? super V>);
  public boolean remove(java.lang.Object, java.lang.Object);
  public void replaceAll(java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public boolean replace(K, V, V);
  public V replace(K, V);
  public V computeIfPresent(K, java.util.function.BiFunction<? super K, ? super V, ? extends V>);
}
```

## `cn.hutool.core.map.TolerantMap`

```java
public class cn.hutool.core.map.TolerantMap<K, V> extends cn.hutool.core.map.MapWrapper<K, V> {
  public cn.hutool.core.map.TolerantMap(V);
  public cn.hutool.core.map.TolerantMap(int, float, V);
  public cn.hutool.core.map.TolerantMap(int, V);
  public cn.hutool.core.map.TolerantMap(java.util.Map<K, V>, V);
  public static <K, V> cn.hutool.core.map.TolerantMap<K, V> of(java.util.Map<K, V>, V);
  public V get(java.lang.Object);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `cn.hutool.core.map.TransMap`

```java
public abstract class cn.hutool.core.map.TransMap<K, V> extends cn.hutool.core.map.MapWrapper<K, V> {
  public cn.hutool.core.map.TransMap(java.util.function.Supplier<java.util.Map<K, V>>);
  public cn.hutool.core.map.TransMap(java.util.Map<K, V>);
  public V get(java.lang.Object);
  public V put(K, V);
  public void putAll(java.util.Map<? extends K, ? extends V>);
  public boolean containsKey(java.lang.Object);
  public V remove(java.lang.Object);
  public boolean remove(java.lang.Object, java.lang.Object);
  public boolean replace(K, V, V);
  public V replace(K, V);
  public V getOrDefault(java.lang.Object, V);
  public V computeIfPresent(K, java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public V compute(K, java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public V merge(K, V, java.util.function.BiFunction<? super V, ? super V, ? extends V>);
  public V putIfAbsent(K, V);
  public V computeIfAbsent(K, java.util.function.Function<? super K, ? extends V>);
}
```

## `cn.hutool.core.map.TreeEntry`

```java
public interface cn.hutool.core.map.TreeEntry<K, V> extends java.util.Map$Entry<K, V> {
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
  public abstract int getWeight();
  public abstract cn.hutool.core.map.TreeEntry<K, V> getRoot();
  public default boolean hasParent();
  public abstract cn.hutool.core.map.TreeEntry<K, V> getDeclaredParent();
  public abstract cn.hutool.core.map.TreeEntry<K, V> getParent(K);
  public default boolean containsParent(K);
  public abstract void forEachChild(boolean, java.util.function.Consumer<cn.hutool.core.map.TreeEntry<K, V>>);
  public abstract java.util.Map<K, cn.hutool.core.map.TreeEntry<K, V>> getDeclaredChildren();
  public abstract java.util.Map<K, cn.hutool.core.map.TreeEntry<K, V>> getChildren();
  public default boolean hasChildren();
  public abstract cn.hutool.core.map.TreeEntry<K, V> getChild(K);
  public default boolean containsChild(K);
}
```

## `cn.hutool.core.map.WeakConcurrentMap`

```java
public class cn.hutool.core.map.WeakConcurrentMap<K, V> extends cn.hutool.core.map.ReferenceConcurrentMap<K, V> {
  public cn.hutool.core.map.WeakConcurrentMap();
  public cn.hutool.core.map.WeakConcurrentMap(java.util.concurrent.ConcurrentMap<java.lang.ref.Reference<K>, V>);
}
```
