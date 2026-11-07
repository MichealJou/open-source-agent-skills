# com.feilong.core.util

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.core.util.AggregateUtil`

```java
public final class com.feilong.core.util.AggregateUtil {
  public static <O> java.math.BigDecimal avg(java.lang.Iterable<O>, java.lang.String, int);
  public static <O> java.util.Map<java.lang.String, java.math.BigDecimal> avg(java.lang.Iterable<O>, java.lang.String[], int);
  public static <O> java.math.BigDecimal sum(java.lang.Iterable<O>, java.lang.String);
  public static <O> java.math.BigDecimal sum(java.lang.Iterable<O>, java.lang.String, org.apache.commons.collections4.Predicate<O>);
  public static <O> java.util.Map<java.lang.String, java.math.BigDecimal> sum(java.lang.Iterable<O>, java.lang.String...);
  public static <O> java.util.Map<java.lang.String, java.math.BigDecimal> sum(java.lang.Iterable<O>, java.lang.String[], org.apache.commons.collections4.Predicate<O>);
  public static <O, T> java.util.Map<T, java.math.BigDecimal> groupSum(java.lang.Iterable<O>, java.lang.String, java.lang.String);
  public static <O, T> java.util.Map<T, java.math.BigDecimal> groupSum(java.lang.Iterable<O>, java.lang.String, java.lang.String, org.apache.commons.collections4.Predicate<O>);
  public static <O, T> java.util.Map<T, java.lang.Integer> groupCount(java.lang.Iterable<O>, java.lang.String);
  public static <O, T> java.util.Map<T, java.lang.Integer> groupCount(java.lang.Iterable<O>, java.lang.String, org.apache.commons.collections4.Predicate<O>);
  public static <O> java.util.Map<java.lang.String, java.util.Map<java.lang.Object, java.lang.Integer>> groupCount(java.lang.Iterable<O>, java.lang.String...);
  public static <O> java.util.Map<java.lang.String, java.util.Map<java.lang.Object, java.lang.Integer>> groupCount(java.lang.Iterable<O>, java.lang.String[], org.apache.commons.collections4.Predicate<O>);
  public static <O> java.util.Map<java.lang.String, java.util.Map<java.lang.Object, java.lang.Integer>> groupCount(java.lang.Iterable<O>, java.lang.String[], java.util.Map<java.lang.String, org.apache.commons.collections4.Transformer<java.lang.Object, java.lang.Object>>);
  public static <O> java.util.Map<java.lang.String, java.util.Map<java.lang.Object, java.lang.Integer>> groupCount(java.lang.Iterable<O>, java.lang.String[], java.util.Map<java.lang.String, org.apache.commons.collections4.Transformer<java.lang.Object, java.lang.Object>>, org.apache.commons.collections4.Predicate<O>);
}
```

## `com.feilong.core.util.CollectionsUtil`

```java
public final class com.feilong.core.util.CollectionsUtil {
  public static <T> java.util.List<java.util.List<T>> partition(java.util.List<T>, int);
  public static int size(java.lang.Object);
  public static <T> T first(java.lang.Iterable<T>);
  public static <T> T last(java.lang.Iterable<T>);
  public static <T> T get(java.lang.Iterable<T>, int);
  public static <T> boolean contains(java.lang.Iterable<T>, T);
  public static <T> boolean containsAny(java.lang.Iterable<T>, T...);
  public static boolean containsTrimAndIgnoreCase(java.lang.Iterable<java.lang.String>, java.lang.String);
  public static <O> void forEach(java.lang.Iterable<O>, java.lang.String, java.lang.Object);
  public static <O> boolean addAllIgnoreNull(java.util.Collection<O>, java.lang.Iterable<? extends O>);
  public static <T> boolean addIgnoreNullOrEmpty(java.util.Collection<T>, T...);
  public static <T> boolean addIgnoreNullOrEmpty(java.util.Collection<T>, java.lang.Iterable<T>);
  public static <T> boolean addIfCondition(java.util.Collection<T>, T, boolean);
  public static <T> void setIfCondition(java.util.List<T>, int, T, boolean);
  public static <O, V> int indexOf(java.util.List<O>, java.lang.String, V);
  public static <O> java.util.List<O> removeAll(java.util.Collection<O>, java.util.Collection<O>);
  public static <O> java.util.List<O> removeAllNull(java.util.Collection<O>);
  public static <O> java.util.List<O> remove(java.util.Collection<O>, O...);
  public static <O> java.util.List<O> removeDuplicate(java.util.Collection<O>);
  public static <O> java.util.List<O> removeDuplicate(java.util.Collection<O>, java.lang.String);
  public static <O> java.util.List<O> removeDuplicate(java.util.Collection<O>, java.lang.String...);
  public static <O> com.feilong.lib.lang3.tuple.Pair<java.util.List<O>, java.util.List<O>> splitDuplicate(java.util.Collection<O>, java.lang.String...);
  public static <T, O> java.util.List<T> getPropertyValueList(java.lang.Iterable<O>, java.lang.String);
  public static <T, O> java.util.List<T> getPropertyValueList(java.util.Collection<O>, java.util.function.Function<O, T>);
  public static <T, O> java.util.List<T> getPropertyValueList(java.lang.Iterable<O>, java.lang.String, java.lang.Class<T>);
  public static <T, O> java.util.Set<T> getPropertyValueSet(java.lang.Iterable<O>, java.lang.String);
  public static <T, O> java.util.Set<T> getPropertyValueSet(java.util.Collection<O>, java.util.function.Function<O, T>);
  public static <T, O> java.util.Set<T> getPropertyValueSet(java.lang.Iterable<O>, java.lang.String, java.lang.Class<T>);
  public static <K, V, O> java.util.Map<K, V> getPropertyValueMap(java.lang.Iterable<O>, java.lang.String, java.lang.String);
  public static <K, V, O> java.util.Map<K, V> getPropertyValueMap(java.lang.Iterable<O>, java.util.function.Function<O, K>, java.util.function.Function<O, V>);
  public static <O, V> boolean exist(java.lang.Iterable<O>, java.lang.String, V);
  public static <O> boolean exist(java.lang.Iterable<O>, java.util.Map<java.lang.String, ?>);
  public static <O> boolean exist(java.lang.Iterable<O>, org.apache.commons.collections4.Predicate<O>);
  public static <O, V> O find(java.lang.Iterable<O>, java.lang.String, V);
  public static <O, V> O find(java.lang.Iterable<O>, java.util.function.Function<O, V>, V);
  public static <O> O find(java.lang.Iterable<O>, java.util.Map<java.lang.String, ?>);
  public static <O> O find(java.lang.Iterable<O>, org.apache.commons.collections4.Predicate<O>);
  public static <O, V> java.util.List<O> select(java.lang.Iterable<O>, java.lang.String, V...);
  public static <O, V> java.util.List<O> select(java.lang.Iterable<O>, java.util.function.Function<O, V>, V...);
  public static <O, V> java.util.List<O> select(java.lang.Iterable<O>, java.lang.String, java.util.Collection<V>);
  public static <O> java.util.List<O> select(java.lang.Iterable<O>, java.util.Map<java.lang.String, ?>);
  public static <O> java.util.List<O> select(java.lang.Iterable<O>, org.apache.commons.collections4.Predicate<O>);
  public static <O, V> java.util.List<O> selectRejected(java.lang.Iterable<O>, java.lang.String, V...);
  public static <O, V> java.util.List<O> selectRejected(java.lang.Iterable<O>, java.lang.String, java.util.Collection<V>);
  public static <O> java.util.List<O> selectRejected(java.lang.Iterable<O>, java.util.Map<java.lang.String, ?>);
  public static <O> java.util.List<O> selectRejected(java.lang.Iterable<O>, org.apache.commons.collections4.Predicate<O>);
  public static <O, T> java.util.List<T> collect(java.lang.Iterable<O>, org.apache.commons.collections4.Transformer<? super O, ? extends T>);
  public static <O, I> java.util.List<O> collect(java.lang.Iterable<I>, java.lang.Class<O>, java.lang.String...);
  public static <O, T> java.util.List<T> collect(java.util.Iterator<O>, org.apache.commons.collections4.Transformer<? super O, ? extends T>);
  public static <T, O> java.util.Map<T, java.util.List<O>> group(java.lang.Iterable<O>, java.lang.String);
  public static <T, O> java.util.Map<T, java.util.List<O>> group(java.lang.Iterable<O>, java.lang.String, org.apache.commons.collections4.Predicate<O>);
  public static <T, O> java.util.Map<T, java.util.List<O>> group(java.lang.Iterable<O>, org.apache.commons.collections4.Transformer<O, T>);
  public static <T, O> java.util.Map<T, java.util.List<O>> group(java.lang.Iterable<O>, org.apache.commons.collections4.Predicate<O>, org.apache.commons.collections4.Transformer<O, T>);
  public static <T, O> java.util.Map<T, O> groupOne(java.lang.Iterable<O>, java.util.function.Function<O, T>);
  public static <T, O> java.util.Map<T, O> groupOne(java.lang.Iterable<O>, java.lang.String);
  public static <E> java.util.List<E> newArrayList();
  public static <E> java.util.List<E> newArrayList(java.util.Collection<? extends E>);
  public static <E> java.util.List<E> newLinkedList();
  public static <E> java.util.List<E> newLinkedList(java.util.Collection<? extends E>);
  public static <E> java.util.List<E> newCopyOnWriteArrayList();
  public static <E> java.util.List<E> newCopyOnWriteArrayList(java.util.Collection<? extends E>);
  public static <E> java.util.Set<E> newHashSet();
  public static <E> java.util.Set<E> newHashSet(java.util.Collection<? extends E>);
  public static <E> java.util.Set<E> newLinkedHashSet();
  public static <E> java.util.Set<E> newLinkedHashSet(java.util.Collection<? extends E>);
}
```

## `com.feilong.core.util.EnumerationUtil`

```java
public final class com.feilong.core.util.EnumerationUtil {
  public static <O> boolean contains(java.util.Enumeration<O>, O);
}
```

## `com.feilong.core.util.MapUtil`

```java
public final class com.feilong.core.util.MapUtil {
  public static <K, V> V computeIfAbsent(java.util.Map<K, V>, K, java.util.function.Function<? super K, ? extends V>);
  public static <K, V> java.util.Map$Entry<K, V> get(java.util.Map<K, V>, int);
  public static <K, V> V get(java.util.Map<K, V>, K);
  public static <K, V> java.lang.String getDefaultEmptyStringIfNull(java.util.Map<K, V>, K);
  public static <K, V> V getOrDefault(java.util.Map<K, V>, K, V);
  public static <K, V> java.util.Map<K, V> toSingleValueMap(java.util.Map<K, V[]>);
  public static <K> java.util.Map<K, java.lang.String[]> toArrayValueMap(java.util.Map<K, java.lang.String>);
  public static <K, V, T> java.util.Map<K, V[]> toArrayValueMap(java.util.Map<K, T>, java.lang.Class<V>);
  public static <K, V> void putIfValueNotNull(java.util.Map<K, V>, K, V);
  public static <K, V> void putAllIfNotNull(java.util.Map<K, V>, java.util.Map<? extends K, ? extends V>);
  public static <K, V> void putIfValueNotNullOrEmpty(java.util.Map<K, V>, K, V);
  public static <K> java.util.Map<K, java.lang.Integer> putSumValue(java.util.Map<K, java.lang.Integer>, K, java.lang.Integer);
  public static <K> java.util.Map<K, java.math.BigDecimal> putSumValue(java.util.Map<K, java.math.BigDecimal>, K, java.lang.Number);
  public static <K, T extends java.lang.Number, C extends java.lang.Number> C getSubSumValue(java.util.Map<K, T>, java.lang.Iterable<K>, java.lang.Class<C>);
  public static <K, V> java.util.Map<K, java.util.List<V>> putMultiValue(java.util.Map<K, java.util.List<V>>, K, V);
  public static <K, T> java.util.Map<K, T> getSubMap(java.util.Map<K, T>, K...);
  public static <K, T> java.util.Map<K, T> getSubMap(java.util.Map<K, T>, java.lang.Iterable<K>);
  public static <K, T> java.util.Map<K, T> getSubMapExcludeValues(java.util.Map<K, T>, T...);
  public static <K, T> java.util.Map<K, T> getSubMapExcludeKeys(java.util.Map<K, T>, K...);
  public static <K, T> java.util.Map<K, T> getSubMapExcludeKeys(java.util.Map<K, T>, java.lang.Iterable<K>);
  public static <K, V> java.util.Map<K, V> removeKeys(java.util.Map<K, V>, K...);
  public static <K, V> java.util.Map<K, V> removeKeys(java.util.Map<K, V>, java.util.Collection<K>);
  public static <K, V> java.util.Map<V, K> invertMap(java.util.Map<K, V>);
  public static <T, V, I> java.util.Map<T, V> extractIntersectionKeyDifferentValueMap(java.util.Map<T, V>, java.util.Map<T, I>);
  public static <K, O, V> java.util.Map<K, V> extractSubMap(java.util.Map<K, O>, java.lang.String);
  public static <K, O, V> java.util.Map<K, V> extractSubMap(java.util.Map<K, O>, K[], java.lang.String);
  public static <K, V> java.util.Map<K, V> newConcurrentHashMap();
  public static <K, V> java.util.Map<K, V> newConcurrentHashMap(java.util.Map<K, V>);
  public static <K, V> java.util.Map<K, V> newConcurrentHashMap(int);
  public static <K extends java.lang.Comparable, V> java.util.Map<K, V> newTreeMap();
  public static <K extends java.lang.Comparable, V> java.util.Map<K, V> newTreeMap(java.util.Map<K, V>);
  public static <K, V> java.util.Map<K, V> newHashMap();
  public static <K, V> java.util.Map<K, V> newHashMap(java.util.Map<K, V>);
  public static <K, V> java.util.Map<K, V> newHashMap(int);
  public static <K, V> java.util.Map<K, V> newLinkedHashMap();
  public static <K, V> java.util.Map<K, V> newLinkedHashMap(java.lang.Iterable<K>, V);
  public static <K, V> java.util.Map<K, V> newLinkedHashMap(java.util.Map<K, V>);
  public static <K, V> java.util.Map<K, V> newLinkedHashMap(int);
}
```

## `com.feilong.core.util.RandomUtil`

```java
public final class com.feilong.core.util.RandomUtil {
  public static long createRandomWithLength(int);
  public static java.lang.String createRandomFromString(java.lang.String, int);
  public static java.lang.String createRandomString(int);
}
```

## `com.feilong.core.util.RegexUtil`

```java
public final class com.feilong.core.util.RegexUtil {
  public static boolean matches(java.lang.String, java.lang.CharSequence);
  public static java.util.Map<java.lang.Integer, java.lang.String> group(java.lang.String, java.lang.CharSequence);
  public static java.lang.String group(java.lang.String, java.lang.CharSequence, int);
  public static java.util.regex.Pattern buildPattern(java.lang.String, int);
}
```

## `com.feilong.core.util.ResourceBundleUtil`

```java
public final class com.feilong.core.util.ResourceBundleUtil {
  public static java.lang.String getValue(java.util.ResourceBundle, java.lang.String, java.lang.Object...);
  public static java.util.Map<java.lang.String, java.lang.String> toMap(java.lang.String...);
  public static java.util.Map<java.lang.String, java.lang.String> toMap(java.util.ResourceBundle);
  public static java.util.Properties toProperties(java.util.ResourceBundle);
  public static <T> T toAliasBean(java.util.ResourceBundle, java.lang.Class<T>);
  public static <T> T toBean(java.lang.String, java.lang.Class<T>);
  public static <T> T toBean(java.util.ResourceBundle, java.lang.Class<T>);
  public static java.util.ResourceBundle getResourceBundle(java.lang.String);
  public static java.util.ResourceBundle getResourceBundle(java.lang.String, java.util.Locale);
  public static java.util.ResourceBundle getResourceBundle(java.io.InputStream);
}
```

## `com.feilong.core.util.ServiceLoaderUtil`

```java
public class com.feilong.core.util.ServiceLoaderUtil {
  public com.feilong.core.util.ServiceLoaderUtil();
  public static <T> T loadFirst(java.lang.Class<T>);
}
```

## `com.feilong.core.util.SortUtil`

```java
public final class com.feilong.core.util.SortUtil {
  public static <T> T[] sortArray(T[]);
  public static <T> T[] sortArray(T[], java.util.Comparator<T>...);
  public static <T extends java.lang.Comparable<? super T>> java.util.List<T> sortList(java.util.List<T>);
  public static <T extends java.lang.Comparable<? super T>> java.util.List<T> sortListByFixedOrderArray(java.util.List<T>, T...);
  public static <T extends java.lang.Comparable<? super T>> java.util.List<T> sortListByFixedOrderList(java.util.List<T>, java.util.List<T>);
  public static <O> java.util.List<O> sortList(java.util.List<O>, java.util.Comparator<O>...);
  public static <O> java.util.List<O> sortListByPropertyNamesValue(java.util.List<O>, java.lang.String...);
  public static <O, V> java.util.List<O> sortListByFixedOrderPropertyValueArray(java.util.List<O>, java.lang.String, V...);
  public static <O, V> java.util.List<O> sortListByFixedOrderPropertyValueList(java.util.List<O>, java.lang.String, java.util.List<V>);
  public static <K, V> java.util.Map<K, V> sortMapByKeyAsc(java.util.Map<K, V>);
  public static <K, V> java.util.Map<K, V> sortMapByKeyDesc(java.util.Map<K, V>);
  public static <K, V> java.util.Map<K, V> sortMapByKeyFixOrder(java.util.Map<K, V>, K...);
  public static <K, V extends java.lang.Comparable<V>> java.util.Map<K, V> sortMapByValueAsc(java.util.Map<K, V>);
  public static <K, V extends java.lang.Comparable<V>> java.util.Map<K, V> sortMapByValueDesc(java.util.Map<K, V>);
  public static <K, V> java.util.Map<K, V> sortMap(java.util.Map<K, V>, java.util.Comparator<java.util.Map$Entry<K, V>>);
}
```
