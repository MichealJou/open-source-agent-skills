# cn.hutool.core.collection

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.collection.ArrayIter`

```java
public class cn.hutool.core.collection.ArrayIter<E> implements cn.hutool.core.collection.IterableIter<E>, cn.hutool.core.collection.ResettableIter<E>, java.io.Serializable {
  public cn.hutool.core.collection.ArrayIter(E[]);
  public cn.hutool.core.collection.ArrayIter(java.lang.Object);
  public cn.hutool.core.collection.ArrayIter(java.lang.Object, int);
  public cn.hutool.core.collection.ArrayIter(java.lang.Object, int, int);
  public boolean hasNext();
  public E next();
  public void remove();
  public java.lang.Object getArray();
  public void reset();
}
```

## `cn.hutool.core.collection.AvgPartition`

```java
public class cn.hutool.core.collection.AvgPartition<T> extends cn.hutool.core.collection.Partition<T> {
  public cn.hutool.core.collection.AvgPartition(java.util.List<T>, int);
  public java.util.List<T> get(int);
  public int size();
  public java.lang.Object get(int);
}
```

## `cn.hutool.core.collection.BoundedPriorityQueue`

```java
public class cn.hutool.core.collection.BoundedPriorityQueue<E> extends java.util.PriorityQueue<E> {
  public cn.hutool.core.collection.BoundedPriorityQueue(int);
  public cn.hutool.core.collection.BoundedPriorityQueue(int, java.util.Comparator<? super E>);
  public boolean offer(E);
  public boolean addAll(E[]);
  public java.util.ArrayList<E> toList();
  public java.util.Iterator<E> iterator();
}
```

## `cn.hutool.core.collection.CollStreamUtil`

```java
public class cn.hutool.core.collection.CollStreamUtil {
  public cn.hutool.core.collection.CollStreamUtil();
  public static <V, K> java.util.Map<K, V> toIdentityMap(java.util.Collection<V>, java.util.function.Function<V, K>);
  public static <V, K> java.util.Map<K, V> toIdentityMap(java.util.Collection<V>, java.util.function.Function<V, K>, boolean);
  public static <E, K, V> java.util.Map<K, V> toMap(java.util.Collection<E>, java.util.function.Function<E, K>, java.util.function.Function<E, V>);
  public static <E, K, V> java.util.Map<K, V> toMap(java.util.Collection<E>, java.util.function.Function<E, K>, java.util.function.Function<E, V>, boolean);
  public static <E, K> java.util.Map<K, java.util.List<E>> groupByKey(java.util.Collection<E>, java.util.function.Function<E, K>);
  public static <E, K> java.util.Map<K, java.util.List<E>> groupByKey(java.util.Collection<E>, java.util.function.Function<E, K>, boolean);
  public static <E, K, U> java.util.Map<K, java.util.Map<U, java.util.List<E>>> groupBy2Key(java.util.Collection<E>, java.util.function.Function<E, K>, java.util.function.Function<E, U>);
  public static <E, K, U> java.util.Map<K, java.util.Map<U, java.util.List<E>>> groupBy2Key(java.util.Collection<E>, java.util.function.Function<E, K>, java.util.function.Function<E, U>, boolean);
  public static <E, T, U> java.util.Map<T, java.util.Map<U, E>> group2Map(java.util.Collection<E>, java.util.function.Function<E, T>, java.util.function.Function<E, U>);
  public static <E, T, U> java.util.Map<T, java.util.Map<U, E>> group2Map(java.util.Collection<E>, java.util.function.Function<E, T>, java.util.function.Function<E, U>, boolean);
  public static <E, K, V> java.util.Map<K, java.util.List<V>> groupKeyValue(java.util.Collection<E>, java.util.function.Function<E, K>, java.util.function.Function<E, V>);
  public static <E, K, V> java.util.Map<K, java.util.List<V>> groupKeyValue(java.util.Collection<E>, java.util.function.Function<E, K>, java.util.function.Function<E, V>, boolean);
  public static <E, K, D> java.util.Map<K, D> groupBy(java.util.Collection<E>, java.util.function.Function<E, K>, java.util.stream.Collector<E, ?, D>);
  public static <E, K, D> java.util.Map<K, D> groupBy(java.util.Collection<E>, java.util.function.Function<E, K>, java.util.stream.Collector<E, ?, D>, boolean);
  public static <E, T> java.util.List<T> toList(java.util.Collection<E>, java.util.function.Function<E, T>);
  public static <E, T> java.util.List<T> toList(java.util.Collection<E>, java.util.function.Function<E, T>, boolean);
  public static <E, T> java.util.Set<T> toSet(java.util.Collection<E>, java.util.function.Function<E, T>);
  public static <E, T> java.util.Set<T> toSet(java.util.Collection<E>, java.util.function.Function<E, T>, boolean);
  public static <K, X, Y, V> java.util.Map<K, V> merge(java.util.Map<K, X>, java.util.Map<K, Y>, java.util.function.BiFunction<X, Y, V>);
}
```

## `cn.hutool.core.collection.CollUtil`

```java
public class cn.hutool.core.collection.CollUtil {
  public cn.hutool.core.collection.CollUtil();
  public static <T> java.util.Set<T> emptyIfNull(java.util.Set<T>);
  public static <T> java.util.List<T> emptyIfNull(java.util.List<T>);
  public static <T> java.util.Collection<T> union(java.util.Collection<T>, java.util.Collection<T>);
  public static <T> java.util.Collection<T> union(java.util.Collection<T>, java.util.Collection<T>, java.util.Collection<T>...);
  public static <T> java.util.Set<T> unionDistinct(java.util.Collection<T>, java.util.Collection<T>, java.util.Collection<T>...);
  public static <T> java.util.List<T> unionAll(java.util.Collection<T>, java.util.Collection<T>, java.util.Collection<T>...);
  public static <T> java.util.Collection<T> intersection(java.util.Collection<T>, java.util.Collection<T>);
  public static <T> java.util.Collection<T> intersection(java.util.Collection<T>, java.util.Collection<T>, java.util.Collection<T>...);
  public static <T> java.util.Set<T> intersectionDistinct(java.util.Collection<T>, java.util.Collection<T>, java.util.Collection<T>...);
  public static <T> java.util.Collection<T> disjunction(java.util.Collection<T>, java.util.Collection<T>);
  public static <T> java.util.Collection<T> subtract(java.util.Collection<T>, java.util.Collection<T>);
  public static <T> java.util.List<T> subtractToList(java.util.Collection<T>, java.util.Collection<T>);
  public static <T> java.util.List<T> subtractToList(java.util.Collection<T>, java.util.Collection<T>, boolean);
  public static boolean contains(java.util.Collection<?>, java.lang.Object);
  public static boolean safeContains(java.util.Collection<?>, java.lang.Object);
  public static <T> boolean contains(java.util.Collection<T>, java.util.function.Predicate<? super T>);
  public static boolean containsAny(java.util.Collection<?>, java.util.Collection<?>);
  public static boolean containsAll(java.util.Collection<?>, java.util.Collection<?>);
  public static <T> java.util.Map<T, java.lang.Integer> countMap(java.lang.Iterable<T>);
  public static <T> java.lang.String join(java.lang.Iterable<T>, java.lang.CharSequence, java.util.function.Function<T, ? extends java.lang.CharSequence>);
  public static <T> java.lang.String join(java.lang.Iterable<T>, java.lang.CharSequence);
  public static <T> java.lang.String join(java.lang.Iterable<T>, java.lang.CharSequence, java.lang.String, java.lang.String);
  public static <T> java.lang.String join(java.util.Iterator<T>, java.lang.CharSequence);
  public static <T> java.util.List<T> popPart(java.util.Stack<T>, int);
  public static <T> java.util.List<T> popPart(java.util.Deque<T>, int);
  public static <T> boolean anyMatch(java.util.Collection<T>, java.util.function.Predicate<T>);
  public static <T> boolean allMatch(java.util.Collection<T>, java.util.function.Predicate<T>);
  public static <T> java.util.HashSet<T> newHashSet(T...);
  public static <T> java.util.LinkedHashSet<T> newLinkedHashSet(T...);
  public static <T> java.util.HashSet<T> set(boolean, T...);
  public static <T> java.util.HashSet<T> newHashSet(java.util.Collection<T>);
  public static <T> java.util.HashSet<T> newHashSet(boolean, java.util.Collection<T>);
  public static <T> java.util.HashSet<T> newHashSet(boolean, java.util.Iterator<T>);
  public static <T> java.util.HashSet<T> newHashSet(boolean, java.util.Enumeration<T>);
  public static <T> java.util.List<T> list(boolean);
  public static <T> java.util.List<T> list(boolean, T...);
  public static <T> java.util.List<T> list(boolean, java.util.Collection<T>);
  public static <T> java.util.List<T> list(boolean, java.lang.Iterable<T>);
  public static <T> java.util.List<T> list(boolean, java.util.Iterator<T>);
  public static <T> java.util.List<T> list(boolean, java.util.Enumeration<T>);
  public static <T> java.util.ArrayList<T> newArrayList(T...);
  public static <T> java.util.ArrayList<T> toList(T...);
  public static <T> java.util.ArrayList<T> newArrayList(java.util.Collection<T>);
  public static <T> java.util.ArrayList<T> newArrayList(java.lang.Iterable<T>);
  public static <T> java.util.ArrayList<T> newArrayList(java.util.Iterator<T>);
  public static <T> java.util.ArrayList<T> newArrayList(java.util.Enumeration<T>);
  public static <T> java.util.LinkedList<T> newLinkedList(T...);
  public static <T> java.util.concurrent.CopyOnWriteArrayList<T> newCopyOnWriteArrayList(java.util.Collection<T>);
  public static <T> java.util.concurrent.BlockingQueue<T> newBlockingQueue(int, boolean);
  public static <T> java.util.Collection<T> create(java.lang.Class<?>);
  public static <T> java.util.Collection<T> create(java.lang.Class<?>, java.lang.Class<T>);
  public static <T> java.util.ArrayList<T> distinct(java.util.Collection<T>);
  public static <T, K> java.util.List<T> distinct(java.util.Collection<T>, java.util.function.Function<T, K>, boolean);
  public static <T> java.util.List<T> sub(java.util.List<T>, int, int);
  public static <T> java.util.List<T> sub(java.util.List<T>, int, int, int);
  public static <T> java.util.List<T> sub(java.util.Collection<T>, int, int);
  public static <T> java.util.List<T> sub(java.util.Collection<T>, int, int, int);
  public static <T> java.util.List<java.util.List<T>> splitList(java.util.List<T>, int);
  public static <T> java.util.List<java.util.List<T>> split(java.util.Collection<T>, int);
  public static <T> java.util.Collection<T> edit(java.util.Collection<T>, cn.hutool.core.lang.Editor<T>);
  public static <T> java.util.Collection<T> filterNew(java.util.Collection<T>, cn.hutool.core.lang.Filter<T>);
  public static <T extends java.util.Collection<E>, E> T removeAny(T, E...);
  public static <T extends java.util.Collection<E>, E> T filter(T, cn.hutool.core.lang.Filter<E>);
  public static <T extends java.util.Collection<E>, E> T removeNull(T);
  public static <T extends java.util.Collection<E>, E extends java.lang.CharSequence> T removeEmpty(T);
  public static <T extends java.util.Collection<E>, E extends java.lang.CharSequence> T removeBlank(T);
  public static <T extends java.util.Collection<E>, E> T removeWithAddIf(T, T, java.util.function.Predicate<? super E>);
  public static <T extends java.util.Collection<E>, E> java.util.List<E> removeWithAddIf(T, java.util.function.Predicate<? super E>);
  public static java.util.List<java.lang.Object> extract(java.lang.Iterable<?>, cn.hutool.core.lang.Editor<java.lang.Object>);
  public static java.util.List<java.lang.Object> extract(java.lang.Iterable<?>, cn.hutool.core.lang.Editor<java.lang.Object>, boolean);
  public static <T, R> java.util.List<R> map(java.lang.Iterable<T>, java.util.function.Function<? super T, ? extends R>, boolean);
  public static java.util.List<java.lang.Object> getFieldValues(java.lang.Iterable<?>, java.lang.String);
  public static java.util.List<java.lang.Object> getFieldValues(java.lang.Iterable<?>, java.lang.String, boolean);
  public static <T> java.util.List<T> getFieldValues(java.lang.Iterable<?>, java.lang.String, java.lang.Class<T>);
  public static <K, V> java.util.Map<K, V> fieldValueMap(java.lang.Iterable<V>, java.lang.String);
  public static <K, V> java.util.Map<K, V> fieldValueAsMap(java.lang.Iterable<?>, java.lang.String, java.lang.String);
  public static <T> T findOne(java.lang.Iterable<T>, cn.hutool.core.lang.Filter<T>);
  public static <T> T findOneByField(java.lang.Iterable<T>, java.lang.String, java.lang.Object);
  public static <T> int count(java.lang.Iterable<T>, cn.hutool.core.lang.Matcher<T>);
  public static <T> int indexOf(java.util.Collection<T>, cn.hutool.core.lang.Matcher<T>);
  public static <T> int lastIndexOf(java.util.Collection<T>, cn.hutool.core.lang.Matcher<T>);
  public static <T> int[] indexOfAll(java.util.Collection<T>, cn.hutool.core.lang.Matcher<T>);
  public static boolean isEmpty(java.util.Collection<?>);
  public static <T extends java.util.Collection<E>, E> T defaultIfEmpty(T, T);
  public static <T extends java.util.Collection<E>, E> T defaultIfEmpty(T, java.util.function.Supplier<? extends T>);
  public static boolean isEmpty(java.lang.Iterable<?>);
  public static boolean isEmpty(java.util.Iterator<?>);
  public static boolean isEmpty(java.util.Enumeration<?>);
  public static boolean isEmpty(java.util.Map<?, ?>);
  public static boolean isNotEmpty(java.util.Collection<?>);
  public static boolean isNotEmpty(java.lang.Iterable<?>);
  public static boolean isNotEmpty(java.util.Iterator<?>);
  public static boolean isNotEmpty(java.util.Enumeration<?>);
  public static boolean hasNull(java.lang.Iterable<?>);
  public static boolean isNotEmpty(java.util.Map<?, ?>);
  public static java.util.Map<java.lang.String, java.lang.String> zip(java.lang.String, java.lang.String, java.lang.String, boolean);
  public static java.util.Map<java.lang.String, java.lang.String> zip(java.lang.String, java.lang.String, java.lang.String);
  public static <K, V> java.util.Map<K, V> zip(java.util.Collection<K>, java.util.Collection<V>);
  public static <K, V> java.util.HashMap<K, V> toMap(java.lang.Iterable<java.util.Map$Entry<K, V>>);
  public static java.util.HashMap<java.lang.Object, java.lang.Object> toMap(java.lang.Object[]);
  public static <T> java.util.TreeSet<T> toTreeSet(java.util.Collection<T>, java.util.Comparator<T>);
  public static <E> java.util.Enumeration<E> asEnumeration(java.util.Iterator<E>);
  public static <E> java.util.Iterator<E> asIterator(java.util.Enumeration<E>);
  public static <E> java.lang.Iterable<E> asIterable(java.util.Iterator<E>);
  public static <E> java.util.Collection<E> toCollection(java.lang.Iterable<E>);
  public static <K, V> java.util.Map<K, java.util.List<V>> toListMap(java.lang.Iterable<? extends java.util.Map<K, V>>);
  public static <K, V> java.util.List<java.util.Map<K, V>> toMapList(java.util.Map<K, ? extends java.lang.Iterable<V>>);
  public static <K, V> java.util.Map<K, V> toMap(java.lang.Iterable<V>, java.util.Map<K, V>, cn.hutool.core.lang.func.Func1<V, K>);
  public static <K, V, E> java.util.Map<K, V> toMap(java.lang.Iterable<E>, java.util.Map<K, V>, cn.hutool.core.lang.func.Func1<E, K>, cn.hutool.core.lang.func.Func1<E, V>);
  public static <T, S extends T> boolean addIfAbsent(java.util.Collection<T>, S);
  public static <T> java.util.Collection<T> addAll(java.util.Collection<T>, java.lang.Object);
  public static <T> java.util.Collection<T> addAll(java.util.Collection<T>, java.lang.Object, java.lang.reflect.Type);
  public static <T> java.util.Collection<T> addAll(java.util.Collection<T>, java.util.Iterator<T>);
  public static <T> java.util.Collection<T> addAll(java.util.Collection<T>, java.lang.Iterable<T>);
  public static <T> java.util.Collection<T> addAll(java.util.Collection<T>, java.util.Enumeration<T>);
  public static <T> java.util.Collection<T> addAll(java.util.Collection<T>, T[]);
  public static <T> java.util.List<T> addAllIfNotContains(java.util.List<T>, java.util.List<T>);
  public static <T> T get(java.util.Collection<T>, int);
  public static <T> java.util.List<T> getAny(java.util.Collection<T>, int...);
  public static <T> T getFirst(java.lang.Iterable<T>);
  public static <T> T getFirst(java.util.Iterator<T>);
  public static <T> T getLast(java.util.Collection<T>);
  public static java.lang.Class<?> getElementType(java.lang.Iterable<?>);
  public static java.lang.Class<?> getElementType(java.util.Iterator<?>);
  public static <K, V> java.util.ArrayList<V> valuesOfKeys(java.util.Map<K, V>, K...);
  public static <K, V> java.util.ArrayList<V> valuesOfKeys(java.util.Map<K, V>, java.lang.Iterable<K>);
  public static <K, V> java.util.ArrayList<V> valuesOfKeys(java.util.Map<K, V>, java.util.Iterator<K>);
  public static <T> java.util.List<T> sortPageAll(int, int, java.util.Comparator<T>, java.util.Collection<T>...);
  public static <T> java.util.List<T> page(int, int, java.util.List<T>);
  public static <T> java.util.List<T> sort(java.util.Collection<T>, java.util.Comparator<? super T>);
  public static <T> java.util.List<T> sort(java.util.List<T>, java.util.Comparator<? super T>);
  public static <T> java.util.List<T> sortByProperty(java.util.Collection<T>, java.lang.String);
  public static <T> java.util.List<T> sortByProperty(java.util.List<T>, java.lang.String);
  public static java.util.List<java.lang.String> sortByPinyin(java.util.Collection<java.lang.String>);
  public static java.util.List<java.lang.String> sortByPinyin(java.util.List<java.lang.String>);
  public static <K, V> java.util.TreeMap<K, V> sort(java.util.Map<K, V>, java.util.Comparator<? super K>);
  public static <K, V> java.util.LinkedHashMap<K, V> sortToMap(java.util.Collection<java.util.Map$Entry<K, V>>, java.util.Comparator<java.util.Map$Entry<K, V>>);
  public static <K, V> java.util.LinkedHashMap<K, V> sortByEntry(java.util.Map<K, V>, java.util.Comparator<java.util.Map$Entry<K, V>>);
  public static <K, V> java.util.List<java.util.Map$Entry<K, V>> sortEntryToList(java.util.Collection<java.util.Map$Entry<K, V>>);
  public static <T> void forEach(java.lang.Iterable<T>, cn.hutool.core.collection.CollUtil$Consumer<T>);
  public static <T> void forEach(java.util.Iterator<T>, cn.hutool.core.collection.CollUtil$Consumer<T>);
  public static <T> void forEach(java.util.Enumeration<T>, cn.hutool.core.collection.CollUtil$Consumer<T>);
  public static <K, V> void forEach(java.util.Map<K, V>, cn.hutool.core.collection.CollUtil$KVConsumer<K, V>);
  public static <T> java.util.List<java.util.List<T>> group(java.util.Collection<T>, cn.hutool.core.lang.hash.Hash32<T>);
  public static <T> java.util.List<java.util.List<T>> groupByField(java.util.Collection<T>, java.lang.String);
  public static <T> java.util.List<T> reverse(java.util.List<T>);
  public static <T> java.util.List<T> reverseNew(java.util.List<T>);
  public static <T> java.util.List<T> setOrAppend(java.util.List<T>, int, T);
  public static <K> java.util.Set<K> keySet(java.util.Collection<java.util.Map<K, ?>>);
  public static <V> java.util.List<V> values(java.util.Collection<java.util.Map<?, V>>);
  public static <T extends java.lang.Comparable<? super T>> T max(java.util.Collection<T>);
  public static <T extends java.lang.Comparable<? super T>> T min(java.util.Collection<T>);
  public static <T> java.util.Collection<T> unmodifiable(java.util.Collection<? extends T>);
  public static <E, T extends java.util.Collection<E>> T empty(java.lang.Class<?>);
  public static void clear(java.util.Collection<?>...);
  public static <T> void padLeft(java.util.List<T>, int, T);
  public static <T> void padRight(java.util.Collection<T>, int, T);
  public static <F, T> java.util.Collection<T> trans(java.util.Collection<F>, java.util.function.Function<? super F, ? extends T>);
  public static <E, K, V> void setValueByMap(java.lang.Iterable<E>, java.util.Map<K, V>, java.util.function.Function<E, K>, java.util.function.BiConsumer<E, V>);
  public static int size(java.lang.Object);
  public static boolean isEqualList(java.util.Collection<?>, java.util.Collection<?>);
}
```

## `cn.hutool.core.collection.CollUtil$Consumer`

```java
public interface cn.hutool.core.collection.CollUtil$Consumer<T> extends java.io.Serializable {
  public abstract void accept(T, int);
}
```

## `cn.hutool.core.collection.CollUtil$KVConsumer`

```java
public interface cn.hutool.core.collection.CollUtil$KVConsumer<K, V> extends java.io.Serializable {
  public abstract void accept(K, V, int);
}
```

## `cn.hutool.core.collection.CollectionUtil`

```java
public class cn.hutool.core.collection.CollectionUtil extends cn.hutool.core.collection.CollUtil {
  public cn.hutool.core.collection.CollectionUtil();
}
```

## `cn.hutool.core.collection.ComputeIter`

```java
public abstract class cn.hutool.core.collection.ComputeIter<T> implements java.util.Iterator<T> {
  public cn.hutool.core.collection.ComputeIter();
  public boolean hasNext();
  public T next();
  public void finish();
  public void resetState();
}
```

## `cn.hutool.core.collection.ConcurrentHashSet`

```java
public class cn.hutool.core.collection.ConcurrentHashSet<E> extends java.util.AbstractSet<E> implements java.io.Serializable {
  public cn.hutool.core.collection.ConcurrentHashSet();
  public cn.hutool.core.collection.ConcurrentHashSet(int);
  public cn.hutool.core.collection.ConcurrentHashSet(int, float);
  public cn.hutool.core.collection.ConcurrentHashSet(int, float, int);
  public cn.hutool.core.collection.ConcurrentHashSet(java.lang.Iterable<E>);
  public java.util.Iterator<E> iterator();
  public int size();
  public boolean isEmpty();
  public boolean contains(java.lang.Object);
  public boolean add(E);
  public boolean remove(java.lang.Object);
  public void clear();
}
```

## `cn.hutool.core.collection.CopiedIter`

```java
public class cn.hutool.core.collection.CopiedIter<E> implements cn.hutool.core.collection.IterableIter<E>, java.io.Serializable {
  public static <E> cn.hutool.core.collection.CopiedIter<E> copyOf(java.util.Iterator<E>);
  public cn.hutool.core.collection.CopiedIter(java.util.Iterator<E>);
  public boolean hasNext();
  public E next();
  public void remove() throws java.lang.UnsupportedOperationException;
}
```

## `cn.hutool.core.collection.EnumerationIter`

```java
public class cn.hutool.core.collection.EnumerationIter<E> implements cn.hutool.core.collection.IterableIter<E>, java.io.Serializable {
  public cn.hutool.core.collection.EnumerationIter(java.util.Enumeration<E>);
  public boolean hasNext();
  public E next();
  public void remove();
}
```

## `cn.hutool.core.collection.FilterIter`

```java
public class cn.hutool.core.collection.FilterIter<E> implements java.util.Iterator<E> {
  public cn.hutool.core.collection.FilterIter(java.util.Iterator<? extends E>, cn.hutool.core.lang.Filter<? super E>);
  public boolean hasNext();
  public E next();
  public void remove();
  public java.util.Iterator<? extends E> getIterator();
  public cn.hutool.core.lang.Filter<? super E> getFilter();
}
```

## `cn.hutool.core.collection.IterChain`

```java
public class cn.hutool.core.collection.IterChain<T> implements java.util.Iterator<T>, cn.hutool.core.lang.Chain<java.util.Iterator<T>, cn.hutool.core.collection.IterChain<T>> {
  public cn.hutool.core.collection.IterChain();
  public cn.hutool.core.collection.IterChain(java.util.Iterator<T>...);
  public cn.hutool.core.collection.IterChain<T> addChain(java.util.Iterator<T>);
  public boolean hasNext();
  public T next();
  public void remove();
  public java.util.Iterator<java.util.Iterator<T>> iterator();
  public java.lang.Object addChain(java.lang.Object);
}
```

## `cn.hutool.core.collection.IterUtil`

```java
public class cn.hutool.core.collection.IterUtil {
  public cn.hutool.core.collection.IterUtil();
  public static <T> java.util.Iterator<T> getIter(java.lang.Iterable<T>);
  public static boolean isEmpty(java.lang.Iterable<?>);
  public static boolean isEmpty(java.util.Iterator<?>);
  public static boolean isNotEmpty(java.lang.Iterable<?>);
  public static boolean isNotEmpty(java.util.Iterator<?>);
  public static boolean hasNull(java.lang.Iterable<?>);
  public static boolean hasNull(java.util.Iterator<?>);
  public static boolean isAllNull(java.lang.Iterable<?>);
  public static boolean isAllNull(java.util.Iterator<?>);
  public static <T> java.util.Map<T, java.lang.Integer> countMap(java.util.Iterator<T>);
  public static <K, V> java.util.Map<K, V> fieldValueMap(java.util.Iterator<V>, java.lang.String);
  public static <K, V> java.util.Map<K, V> fieldValueAsMap(java.util.Iterator<?>, java.lang.String, java.lang.String);
  public static <V> java.util.List<java.lang.Object> fieldValueList(java.lang.Iterable<V>, java.lang.String);
  public static <V> java.util.List<java.lang.Object> fieldValueList(java.util.Iterator<V>, java.lang.String);
  public static <T> java.lang.String join(java.util.Iterator<T>, java.lang.CharSequence);
  public static <T> java.lang.String join(java.util.Iterator<T>, java.lang.CharSequence, java.lang.String, java.lang.String);
  public static <T> java.lang.String join(java.util.Iterator<T>, java.lang.CharSequence, java.util.function.Function<T, ? extends java.lang.CharSequence>);
  public static <K, V> java.util.HashMap<K, V> toMap(java.lang.Iterable<java.util.Map$Entry<K, V>>);
  public static <K, V> java.util.Map<K, V> toMap(java.lang.Iterable<K>, java.lang.Iterable<V>);
  public static <K, V> java.util.Map<K, V> toMap(java.lang.Iterable<K>, java.lang.Iterable<V>, boolean);
  public static <K, V> java.util.Map<K, V> toMap(java.util.Iterator<K>, java.util.Iterator<V>);
  public static <K, V> java.util.Map<K, V> toMap(java.util.Iterator<K>, java.util.Iterator<V>, boolean);
  public static <K, V> java.util.Map<K, java.util.List<V>> toListMap(java.lang.Iterable<V>, java.util.function.Function<V, K>);
  public static <T, K, V> java.util.Map<K, java.util.List<V>> toListMap(java.lang.Iterable<T>, java.util.function.Function<T, K>, java.util.function.Function<T, V>);
  public static <T, K, V> java.util.Map<K, java.util.List<V>> toListMap(java.util.Map<K, java.util.List<V>>, java.lang.Iterable<T>, java.util.function.Function<T, K>, java.util.function.Function<T, V>);
  public static <K, V> java.util.Map<K, V> toMap(java.lang.Iterable<V>, java.util.function.Function<V, K>);
  public static <T, K, V> java.util.Map<K, V> toMap(java.lang.Iterable<T>, java.util.function.Function<T, K>, java.util.function.Function<T, V>);
  public static <T, K, V> java.util.Map<K, V> toMap(java.util.Map<K, V>, java.lang.Iterable<T>, java.util.function.Function<T, K>, java.util.function.Function<T, V>);
  public static <E> java.util.List<E> toList(java.lang.Iterable<E>);
  public static <E> java.util.List<E> toList(java.util.Iterator<E>);
  public static <E> java.util.Iterator<E> asIterator(java.util.Enumeration<E>);
  public static <E> java.lang.Iterable<E> asIterable(java.util.Iterator<E>);
  public static <E> E get(java.util.Iterator<E>, int) throws java.lang.IndexOutOfBoundsException;
  public static <T> T getFirst(java.lang.Iterable<T>);
  public static <T> T getFirstNoneNull(java.lang.Iterable<T>);
  public static <T> T getFirst(java.util.Iterator<T>);
  public static <T> T getFirstNoneNull(java.util.Iterator<T>);
  public static <T> T firstMatch(java.util.Iterator<T>, cn.hutool.core.lang.Matcher<T>);
  public static java.lang.Class<?> getElementType(java.lang.Iterable<?>);
  public static java.lang.Class<?> getElementType(java.util.Iterator<?>);
  public static <T> java.util.List<T> edit(java.lang.Iterable<T>, cn.hutool.core.lang.Editor<T>);
  public static <T extends java.lang.Iterable<E>, E> T filter(T, cn.hutool.core.lang.Filter<E>);
  public static <E> java.util.Iterator<E> filter(java.util.Iterator<E>, cn.hutool.core.lang.Filter<E>);
  public static <E> java.util.List<E> filterToList(java.util.Iterator<E>, cn.hutool.core.lang.Filter<E>);
  public static <E> cn.hutool.core.collection.FilterIter<E> filtered(java.util.Iterator<? extends E>, cn.hutool.core.lang.Filter<? super E>);
  public static <K, V> java.util.Map<K, V> toMap(java.util.Iterator<V>, java.util.Map<K, V>, cn.hutool.core.lang.func.Func1<V, K>);
  public static <K, V, E> java.util.Map<K, V> toMap(java.util.Iterator<E>, java.util.Map<K, V>, cn.hutool.core.lang.func.Func1<E, K>, cn.hutool.core.lang.func.Func1<E, V>);
  public static <T> java.util.Iterator<T> empty();
  public static <F, T> java.util.Iterator<T> trans(java.util.Iterator<F>, java.util.function.Function<? super F, ? extends T>);
  public static int size(java.lang.Iterable<?>);
  public static int size(java.util.Iterator<?>);
  public static boolean isEqualList(java.lang.Iterable<?>, java.lang.Iterable<?>);
  public static void clear(java.util.Iterator<?>);
  public static <E> void forEach(java.util.Iterator<E>, java.util.function.Consumer<? super E>);
  public static <E> java.lang.String toStr(java.util.Iterator<E>);
  public static <E> java.lang.String toStr(java.util.Iterator<E>, java.util.function.Function<? super E, java.lang.String>);
  public static <E> java.lang.String toStr(java.util.Iterator<E>, java.util.function.Function<? super E, java.lang.String>, java.lang.String, java.lang.String, java.lang.String);
  public static java.util.Iterator<?> getIter(java.lang.Object);
}
```

## `cn.hutool.core.collection.IterableIter`

```java
public interface cn.hutool.core.collection.IterableIter<T> extends java.lang.Iterable<T>, java.util.Iterator<T> {
  public default java.util.Iterator<T> iterator();
}
```

## `cn.hutool.core.collection.IteratorEnumeration`

```java
public class cn.hutool.core.collection.IteratorEnumeration<E> implements java.util.Enumeration<E>, java.io.Serializable {
  public cn.hutool.core.collection.IteratorEnumeration(java.util.Iterator<E>);
  public boolean hasMoreElements();
  public E nextElement();
}
```

## `cn.hutool.core.collection.LineIter`

```java
public class cn.hutool.core.collection.LineIter extends cn.hutool.core.collection.ComputeIter<java.lang.String> implements cn.hutool.core.collection.IterableIter<java.lang.String>, java.io.Closeable, java.io.Serializable {
  public cn.hutool.core.collection.LineIter(java.io.InputStream, java.nio.charset.Charset) throws java.lang.IllegalArgumentException;
  public cn.hutool.core.collection.LineIter(java.io.Reader) throws java.lang.IllegalArgumentException;
  public void close();
}
```

## `cn.hutool.core.collection.ListUtil`

```java
public class cn.hutool.core.collection.ListUtil {
  public cn.hutool.core.collection.ListUtil();
  public static <T> java.util.List<T> list(boolean);
  public static <T> java.util.List<T> list(boolean, T...);
  public static <T> java.util.List<T> list(boolean, java.util.Collection<T>);
  public static <T> java.util.List<T> list(boolean, java.lang.Iterable<T>);
  public static <T> java.util.List<T> list(boolean, java.util.Iterator<T>);
  public static <T> java.util.List<T> list(boolean, java.util.Enumeration<T>);
  public static <T> java.util.ArrayList<T> toList(T...);
  public static <T> java.util.LinkedList<T> toLinkedList(T...);
  public static <T> java.util.List<T> of(T...);
  public static <T> java.util.concurrent.CopyOnWriteArrayList<T> toCopyOnWriteArrayList(java.util.Collection<T>);
  public static <T> java.util.ArrayList<T> toList(java.util.Collection<T>);
  public static <T> java.util.ArrayList<T> toList(java.lang.Iterable<T>);
  public static <T> java.util.ArrayList<T> toList(java.util.Iterator<T>);
  public static <T> java.util.ArrayList<T> toList(java.util.Enumeration<T>);
  public static <T> java.util.List<T> page(int, int, java.util.List<T>);
  public static <T> void page(java.util.List<T>, int, java.util.function.Consumer<java.util.List<T>>);
  public static <T> java.util.List<T> sort(java.util.List<T>, java.util.Comparator<? super T>);
  public static <T> java.util.List<T> sortByProperty(java.util.List<T>, java.lang.String);
  public static java.util.List<java.lang.String> sortByPinyin(java.util.List<java.lang.String>);
  public static <T> java.util.List<T> reverse(java.util.List<T>);
  public static <T> java.util.List<T> reverseNew(java.util.List<T>);
  public static <T> java.util.List<T> setOrAppend(java.util.List<T>, int, T);
  public static <T> java.util.List<T> setOrPadding(java.util.List<T>, int, T);
  public static <T> java.util.List<T> setOrPadding(java.util.List<T>, int, T, T);
  public static <T> java.util.List<T> setOrPadding(java.util.List<T>, int, T, T, int);
  public static <T> java.util.List<T> sub(java.util.List<T>, int, int);
  public static <T> java.util.List<T> sub(java.util.List<T>, int, int, int);
  public static <T> int lastIndexOf(java.util.List<T>, cn.hutool.core.lang.Matcher<T>);
  public static <T> int[] indexOfAll(java.util.List<T>, cn.hutool.core.lang.Matcher<T>);
  public static <T> java.util.List<T> unmodifiable(java.util.List<T>);
  public static <T> java.util.List<T> empty();
  public static <T> java.util.List<java.util.List<T>> partition(java.util.List<T>, int);
  public static <T> java.util.List<java.util.List<T>> split(java.util.List<T>, int);
  public static <T> java.util.List<java.util.List<T>> splitAvg(java.util.List<T>, int);
  public static <T> void swapTo(java.util.List<T>, T, java.lang.Integer);
  public static <T> void swapElement(java.util.List<T>, T, T);
  public static <T> java.util.List<T> move(java.util.List<T>, T, int);
  public static <A, B, R> java.util.List<R> zip(java.util.List<A>, java.util.List<B>, java.util.function.BiFunction<A, B, R>);
}
```

## `cn.hutool.core.collection.NodeListIter`

```java
public class cn.hutool.core.collection.NodeListIter implements cn.hutool.core.collection.ResettableIter<org.w3c.dom.Node> {
  public cn.hutool.core.collection.NodeListIter(org.w3c.dom.NodeList);
  public boolean hasNext();
  public org.w3c.dom.Node next();
  public void remove();
  public void reset();
  public java.lang.Object next();
}
```

## `cn.hutool.core.collection.Partition`

```java
public class cn.hutool.core.collection.Partition<T> extends java.util.AbstractList<java.util.List<T>> {
  public cn.hutool.core.collection.Partition(java.util.List<T>, int);
  public java.util.List<T> get(int);
  public int size();
  public boolean isEmpty();
  public java.lang.Object get(int);
}
```

## `cn.hutool.core.collection.PartitionIter`

```java
public class cn.hutool.core.collection.PartitionIter<T> implements cn.hutool.core.collection.IterableIter<java.util.List<T>>, java.io.Serializable {
  public cn.hutool.core.collection.PartitionIter(java.util.Iterator<T>, int);
  public boolean hasNext();
  public java.util.List<T> next();
  public java.lang.Object next();
}
```

## `cn.hutool.core.collection.RandomAccessAvgPartition`

```java
public class cn.hutool.core.collection.RandomAccessAvgPartition<T> extends cn.hutool.core.collection.AvgPartition<T> implements java.util.RandomAccess {
  public cn.hutool.core.collection.RandomAccessAvgPartition(java.util.List<T>, int);
}
```

## `cn.hutool.core.collection.RandomAccessPartition`

```java
public class cn.hutool.core.collection.RandomAccessPartition<T> extends cn.hutool.core.collection.Partition<T> implements java.util.RandomAccess {
  public cn.hutool.core.collection.RandomAccessPartition(java.util.List<T>, int);
}
```

## `cn.hutool.core.collection.ResettableIter`

```java
public interface cn.hutool.core.collection.ResettableIter<E> extends java.util.Iterator<E> {
  public abstract void reset();
}
```

## `cn.hutool.core.collection.RingIndexUtil`

```java
public class cn.hutool.core.collection.RingIndexUtil {
  public cn.hutool.core.collection.RingIndexUtil();
  public static int ringNextIntByObj(java.lang.Object, java.util.concurrent.atomic.AtomicInteger);
  public static int ringNextInt(int, java.util.concurrent.atomic.AtomicInteger);
  public static long ringNextLong(long, java.util.concurrent.atomic.AtomicLong);
}
```

## `cn.hutool.core.collection.SpliteratorUtil`

```java
public class cn.hutool.core.collection.SpliteratorUtil {
  public cn.hutool.core.collection.SpliteratorUtil();
  public static <F, T> java.util.Spliterator<T> trans(java.util.Spliterator<F>, java.util.function.Function<? super F, ? extends T>);
}
```

## `cn.hutool.core.collection.TransCollection`

```java
public class cn.hutool.core.collection.TransCollection<F, T> extends java.util.AbstractCollection<T> {
  public cn.hutool.core.collection.TransCollection(java.util.Collection<F>, java.util.function.Function<? super F, ? extends T>);
  public java.util.Iterator<T> iterator();
  public void clear();
  public boolean isEmpty();
  public void forEach(java.util.function.Consumer<? super T>);
  public boolean removeIf(java.util.function.Predicate<? super T>);
  public java.util.Spliterator<T> spliterator();
  public int size();
}
```

## `cn.hutool.core.collection.TransIter`

```java
public class cn.hutool.core.collection.TransIter<F, T> implements java.util.Iterator<T> {
  public cn.hutool.core.collection.TransIter(java.util.Iterator<? extends F>, java.util.function.Function<? super F, ? extends T>);
  public final boolean hasNext();
  public final T next();
  public final void remove();
}
```

## `cn.hutool.core.collection.TransSpliterator`

```java
public class cn.hutool.core.collection.TransSpliterator<F, T> implements java.util.Spliterator<T> {
  public cn.hutool.core.collection.TransSpliterator(java.util.Spliterator<F>, java.util.function.Function<? super F, ? extends T>);
  public boolean tryAdvance(java.util.function.Consumer<? super T>);
  public void forEachRemaining(java.util.function.Consumer<? super T>);
  public java.util.Spliterator<T> trySplit();
  public long estimateSize();
  public int characteristics();
}
```

## `cn.hutool.core.collection.UniqueKeySet`

```java
public class cn.hutool.core.collection.UniqueKeySet<K, V> extends java.util.AbstractSet<V> implements java.io.Serializable {
  public cn.hutool.core.collection.UniqueKeySet(java.util.function.Function<V, K>);
  public cn.hutool.core.collection.UniqueKeySet(java.util.function.Function<V, K>, java.util.Collection<? extends V>);
  public cn.hutool.core.collection.UniqueKeySet(boolean, java.util.function.Function<V, K>);
  public cn.hutool.core.collection.UniqueKeySet(boolean, java.util.function.Function<V, K>, java.util.Collection<? extends V>);
  public cn.hutool.core.collection.UniqueKeySet(int, float, java.util.function.Function<V, K>);
  public cn.hutool.core.collection.UniqueKeySet(cn.hutool.core.map.MapBuilder<K, V>, java.util.function.Function<V, K>);
  public java.util.Iterator<V> iterator();
  public int size();
  public boolean isEmpty();
  public boolean contains(java.lang.Object);
  public boolean add(V);
  public boolean addIfAbsent(V);
  public boolean addAllIfAbsent(java.util.Collection<? extends V>);
  public boolean remove(java.lang.Object);
  public void clear();
  public cn.hutool.core.collection.UniqueKeySet<K, V> clone();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```
