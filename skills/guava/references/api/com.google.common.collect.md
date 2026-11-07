# com.google.common.collect

版本：33.4.8-jre。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.google.common.collect.AbstractIterator`

```java
public abstract class com.google.common.collect.AbstractIterator<T> extends com.google.common.collect.UnmodifiableIterator<T> {
  public final boolean hasNext();
  public final T next();
  public final T peek();
}
```

## `com.google.common.collect.AbstractSequentialIterator`

```java
public abstract class com.google.common.collect.AbstractSequentialIterator<T> extends com.google.common.collect.UnmodifiableIterator<T> {
  public final boolean hasNext();
  public final T next();
}
```

## `com.google.common.collect.ArrayListMultimap`

```java
public final class com.google.common.collect.ArrayListMultimap<K, V> extends com.google.common.collect.ArrayListMultimapGwtSerializationDependencies<K, V> {
  public static <K, V> com.google.common.collect.ArrayListMultimap<K, V> create();
  public static <K, V> com.google.common.collect.ArrayListMultimap<K, V> create(int, int);
  public static <K, V> com.google.common.collect.ArrayListMultimap<K, V> create(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public void trimToSize();
  public boolean equals(java.lang.Object);
  public java.util.Map asMap();
  public boolean put(java.lang.Object, java.lang.Object);
  public java.util.List replaceValues(java.lang.Object, java.lang.Iterable);
  public java.util.List removeAll(java.lang.Object);
  public java.util.List get(java.lang.Object);
  public void forEach(java.util.function.BiConsumer);
  public java.util.Collection entries();
  public java.util.Collection values();
  public void clear();
  public boolean containsKey(java.lang.Object);
  public int size();
  public java.lang.String toString();
  public int hashCode();
  public com.google.common.collect.Multiset keys();
  public java.util.Set keySet();
  public boolean putAll(com.google.common.collect.Multimap);
  public boolean putAll(java.lang.Object, java.lang.Iterable);
  public boolean remove(java.lang.Object, java.lang.Object);
  public boolean containsEntry(java.lang.Object, java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public boolean isEmpty();
}
```

## `com.google.common.collect.ArrayTable`

```java
public final class com.google.common.collect.ArrayTable<R, C, V> extends com.google.common.collect.AbstractTable<R, C, V> implements java.io.Serializable {
  public static <R, C, V> com.google.common.collect.ArrayTable<R, C, V> create(java.lang.Iterable<? extends R>, java.lang.Iterable<? extends C>);
  public static <R, C, V> com.google.common.collect.ArrayTable<R, C, V> create(com.google.common.collect.Table<R, C, ? extends V>);
  public com.google.common.collect.ImmutableList<R> rowKeyList();
  public com.google.common.collect.ImmutableList<C> columnKeyList();
  public V at(int, int);
  public V set(int, int, V);
  public V[][] toArray(java.lang.Class<V>);
  public void clear();
  public void eraseAll();
  public boolean contains(java.lang.Object, java.lang.Object);
  public boolean containsColumn(java.lang.Object);
  public boolean containsRow(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public V get(java.lang.Object, java.lang.Object);
  public boolean isEmpty();
  public V put(R, C, V);
  public void putAll(com.google.common.collect.Table<? extends R, ? extends C, ? extends V>);
  public V remove(java.lang.Object, java.lang.Object);
  public V erase(java.lang.Object, java.lang.Object);
  public int size();
  public java.util.Set<com.google.common.collect.Table$Cell<R, C, V>> cellSet();
  public java.util.Map<R, V> column(C);
  public com.google.common.collect.ImmutableSet<C> columnKeySet();
  public java.util.Map<C, java.util.Map<R, V>> columnMap();
  public java.util.Map<C, V> row(R);
  public com.google.common.collect.ImmutableSet<R> rowKeySet();
  public java.util.Map<R, java.util.Map<C, V>> rowMap();
  public java.util.Collection<V> values();
  public java.lang.String toString();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.util.Set columnKeySet();
  public java.util.Set rowKeySet();
}
```

## `com.google.common.collect.BiMap`

```java
public interface com.google.common.collect.BiMap<K, V> extends java.util.Map<K, V> {
  public abstract V put(K, V);
  public abstract V forcePut(K, V);
  public abstract void putAll(java.util.Map<? extends K, ? extends V>);
  public abstract java.util.Set<V> values();
  public abstract com.google.common.collect.BiMap<V, K> inverse();
  public default java.util.Collection values();
}
```

## `com.google.common.collect.BoundType`

```java
public final class com.google.common.collect.BoundType extends java.lang.Enum<com.google.common.collect.BoundType> {
  public static com.google.common.collect.BoundType[] values();
  public static com.google.common.collect.BoundType valueOf(java.lang.String);
}
```

## `com.google.common.collect.ClassToInstanceMap`

```java
public interface com.google.common.collect.ClassToInstanceMap<B> extends java.util.Map<java.lang.Class<? extends B>, B> {
  public abstract <T extends B> T getInstance(java.lang.Class<T>);
  public abstract <T extends B> T putInstance(java.lang.Class<T>, T);
}
```

## `com.google.common.collect.Collections2`

```java
public final class com.google.common.collect.Collections2 {
  public static <E> java.util.Collection<E> filter(java.util.Collection<E>, com.google.common.base.Predicate<? super E>);
  public static <F, T> java.util.Collection<T> transform(java.util.Collection<F>, com.google.common.base.Function<? super F, T>);
  public static <E extends java.lang.Comparable<? super E>> java.util.Collection<java.util.List<E>> orderedPermutations(java.lang.Iterable<E>);
  public static <E> java.util.Collection<java.util.List<E>> orderedPermutations(java.lang.Iterable<E>, java.util.Comparator<? super E>);
  public static <E> java.util.Collection<java.util.List<E>> permutations(java.util.Collection<E>);
}
```

## `com.google.common.collect.Comparators`

```java
public final class com.google.common.collect.Comparators {
  public static <T, S extends T> java.util.Comparator<java.lang.Iterable<S>> lexicographical(java.util.Comparator<T>);
  public static <T> boolean isInOrder(java.lang.Iterable<? extends T>, java.util.Comparator<T>);
  public static <T> boolean isInStrictOrder(java.lang.Iterable<? extends T>, java.util.Comparator<T>);
  public static <T> java.util.stream.Collector<T, ?, java.util.List<T>> least(int, java.util.Comparator<? super T>);
  public static <T> java.util.stream.Collector<T, ?, java.util.List<T>> greatest(int, java.util.Comparator<? super T>);
  public static <T> java.util.Comparator<java.util.Optional<T>> emptiesFirst(java.util.Comparator<? super T>);
  public static <T> java.util.Comparator<java.util.Optional<T>> emptiesLast(java.util.Comparator<? super T>);
  public static <T extends java.lang.Comparable<? super T>> T min(T, T);
  public static <T> T min(T, T, java.util.Comparator<? super T>);
  public static <T extends java.lang.Comparable<? super T>> T max(T, T);
  public static <T> T max(T, T, java.util.Comparator<? super T>);
}
```

## `com.google.common.collect.ComparisonChain`

```java
public abstract class com.google.common.collect.ComparisonChain {
  public static com.google.common.collect.ComparisonChain start();
  public abstract com.google.common.collect.ComparisonChain compare(java.lang.Comparable<?>, java.lang.Comparable<?>);
  public abstract <T> com.google.common.collect.ComparisonChain compare(T, T, java.util.Comparator<T>);
  public abstract com.google.common.collect.ComparisonChain compare(int, int);
  public abstract com.google.common.collect.ComparisonChain compare(long, long);
  public abstract com.google.common.collect.ComparisonChain compare(float, float);
  public abstract com.google.common.collect.ComparisonChain compare(double, double);
  public final com.google.common.collect.ComparisonChain compare(java.lang.Boolean, java.lang.Boolean);
  public abstract com.google.common.collect.ComparisonChain compareTrueFirst(boolean, boolean);
  public abstract com.google.common.collect.ComparisonChain compareFalseFirst(boolean, boolean);
  public abstract int result();
}
```

## `com.google.common.collect.ComputationException`

```java
public class com.google.common.collect.ComputationException extends java.lang.RuntimeException {
  public com.google.common.collect.ComputationException(java.lang.Throwable);
}
```

## `com.google.common.collect.ConcurrentHashMultiset`

```java
public final class com.google.common.collect.ConcurrentHashMultiset<E> extends com.google.common.collect.AbstractMultiset<E> implements java.io.Serializable {
  public static <E> com.google.common.collect.ConcurrentHashMultiset<E> create();
  public static <E> com.google.common.collect.ConcurrentHashMultiset<E> create(java.lang.Iterable<? extends E>);
  public static <E> com.google.common.collect.ConcurrentHashMultiset<E> create(java.util.concurrent.ConcurrentMap<E, java.util.concurrent.atomic.AtomicInteger>);
  public int count(java.lang.Object);
  public int size();
  public java.lang.Object[] toArray();
  public <T> T[] toArray(T[]);
  public int add(E, int);
  public int remove(java.lang.Object, int);
  public boolean removeExactly(java.lang.Object, int);
  public int setCount(E, int);
  public boolean setCount(E, int, int);
  public java.util.Set<com.google.common.collect.Multiset$Entry<E>> createEntrySet();
  public boolean isEmpty();
  public java.util.Iterator<E> iterator();
  public void clear();
  public java.util.Set entrySet();
  public java.util.Set elementSet();
  public boolean contains(java.lang.Object);
}
```

## `com.google.common.collect.ContiguousSet`

```java
public abstract class com.google.common.collect.ContiguousSet<C extends java.lang.Comparable> extends com.google.common.collect.ImmutableSortedSet<C> {
  public static <C extends java.lang.Comparable> com.google.common.collect.ContiguousSet<C> create(com.google.common.collect.Range<C>, com.google.common.collect.DiscreteDomain<C>);
  public static com.google.common.collect.ContiguousSet<java.lang.Integer> closed(int, int);
  public static com.google.common.collect.ContiguousSet<java.lang.Long> closed(long, long);
  public static com.google.common.collect.ContiguousSet<java.lang.Integer> closedOpen(int, int);
  public static com.google.common.collect.ContiguousSet<java.lang.Long> closedOpen(long, long);
  public com.google.common.collect.ContiguousSet<C> headSet(C);
  public com.google.common.collect.ContiguousSet<C> headSet(C, boolean);
  public com.google.common.collect.ContiguousSet<C> subSet(C, C);
  public com.google.common.collect.ContiguousSet<C> subSet(C, boolean, C, boolean);
  public com.google.common.collect.ContiguousSet<C> tailSet(C);
  public com.google.common.collect.ContiguousSet<C> tailSet(C, boolean);
  public abstract com.google.common.collect.ContiguousSet<C> intersection(com.google.common.collect.ContiguousSet<C>);
  public abstract com.google.common.collect.Range<C> range();
  public abstract com.google.common.collect.Range<C> range(com.google.common.collect.BoundType, com.google.common.collect.BoundType);
  public java.lang.String toString();
  public static <E> com.google.common.collect.ImmutableSortedSet$Builder<E> builder();
  public com.google.common.collect.ImmutableSortedSet tailSet(java.lang.Object, boolean);
  public com.google.common.collect.ImmutableSortedSet tailSet(java.lang.Object);
  public com.google.common.collect.ImmutableSortedSet subSet(java.lang.Object, boolean, java.lang.Object, boolean);
  public com.google.common.collect.ImmutableSortedSet subSet(java.lang.Object, java.lang.Object);
  public com.google.common.collect.ImmutableSortedSet headSet(java.lang.Object, boolean);
  public com.google.common.collect.ImmutableSortedSet headSet(java.lang.Object);
  public java.util.SortedSet tailSet(java.lang.Object);
  public java.util.SortedSet headSet(java.lang.Object);
  public java.util.SortedSet subSet(java.lang.Object, java.lang.Object);
  public java.util.NavigableSet tailSet(java.lang.Object, boolean);
  public java.util.NavigableSet headSet(java.lang.Object, boolean);
  public java.util.NavigableSet subSet(java.lang.Object, boolean, java.lang.Object, boolean);
}
```

## `com.google.common.collect.DiscreteDomain`

```java
public abstract class com.google.common.collect.DiscreteDomain<C extends java.lang.Comparable> {
  public static com.google.common.collect.DiscreteDomain<java.lang.Integer> integers();
  public static com.google.common.collect.DiscreteDomain<java.lang.Long> longs();
  public static com.google.common.collect.DiscreteDomain<java.math.BigInteger> bigIntegers();
  public abstract C next(C);
  public abstract C previous(C);
  public abstract long distance(C, C);
  public C minValue();
  public C maxValue();
}
```

## `com.google.common.collect.EnumBiMap`

```java
public final class com.google.common.collect.EnumBiMap<K extends java.lang.Enum<K>, V extends java.lang.Enum<V>> extends com.google.common.collect.AbstractBiMap<K, V> {
  public static <K extends java.lang.Enum<K>, V extends java.lang.Enum<V>> com.google.common.collect.EnumBiMap<K, V> create(java.lang.Class<K>, java.lang.Class<V>);
  public static <K extends java.lang.Enum<K>, V extends java.lang.Enum<V>> com.google.common.collect.EnumBiMap<K, V> create(java.util.Map<K, V>);
  public java.lang.Class<K> keyType();
  public java.lang.Class<V> valueType();
  public java.util.Set entrySet();
  public java.util.Set values();
  public java.util.Set keySet();
  public com.google.common.collect.BiMap inverse();
  public void clear();
  public void replaceAll(java.util.function.BiFunction);
  public void putAll(java.util.Map);
  public java.lang.Object remove(java.lang.Object);
  public java.lang.Object forcePut(java.lang.Object, java.lang.Object);
  public java.lang.Object put(java.lang.Object, java.lang.Object);
  public boolean containsValue(java.lang.Object);
}
```

## `com.google.common.collect.EnumHashBiMap`

```java
public final class com.google.common.collect.EnumHashBiMap<K extends java.lang.Enum<K>, V> extends com.google.common.collect.AbstractBiMap<K, V> {
  public static <K extends java.lang.Enum<K>, V> com.google.common.collect.EnumHashBiMap<K, V> create(java.lang.Class<K>);
  public static <K extends java.lang.Enum<K>, V> com.google.common.collect.EnumHashBiMap<K, V> create(java.util.Map<K, ? extends V>);
  public V put(K, V);
  public V forcePut(K, V);
  public java.lang.Class<K> keyType();
  public java.util.Set entrySet();
  public java.util.Set values();
  public java.util.Set keySet();
  public com.google.common.collect.BiMap inverse();
  public void clear();
  public void replaceAll(java.util.function.BiFunction);
  public void putAll(java.util.Map);
  public java.lang.Object remove(java.lang.Object);
  public java.lang.Object forcePut(java.lang.Object, java.lang.Object);
  public java.lang.Object put(java.lang.Object, java.lang.Object);
  public boolean containsValue(java.lang.Object);
}
```

## `com.google.common.collect.EnumMultiset`

```java
public final class com.google.common.collect.EnumMultiset<E extends java.lang.Enum<E>> extends com.google.common.collect.AbstractMultiset<E> implements java.io.Serializable {
  public static <E extends java.lang.Enum<E>> com.google.common.collect.EnumMultiset<E> create(java.lang.Class<E>);
  public static <E extends java.lang.Enum<E>> com.google.common.collect.EnumMultiset<E> create(java.lang.Iterable<E>);
  public static <E extends java.lang.Enum<E>> com.google.common.collect.EnumMultiset<E> create(java.lang.Iterable<E>, java.lang.Class<E>);
  public int size();
  public int count(java.lang.Object);
  public int add(E, int);
  public int remove(java.lang.Object, int);
  public int setCount(E, int);
  public void clear();
  public void forEachEntry(java.util.function.ObjIntConsumer<? super E>);
  public java.util.Iterator<E> iterator();
  public java.util.Set entrySet();
  public java.util.Set elementSet();
  public boolean setCount(java.lang.Object, int, int);
  public int setCount(java.lang.Object, int);
  public int add(java.lang.Object, int);
  public boolean contains(java.lang.Object);
  public boolean isEmpty();
}
```

## `com.google.common.collect.EvictingQueue`

```java
public final class com.google.common.collect.EvictingQueue<E> extends com.google.common.collect.ForwardingQueue<E> implements java.io.Serializable {
  public static <E> com.google.common.collect.EvictingQueue<E> create(int);
  public int remainingCapacity();
  public boolean offer(E);
  public boolean add(E);
  public boolean addAll(java.util.Collection<? extends E>);
  public java.lang.Object[] toArray();
}
```

## `com.google.common.collect.FluentIterable`

```java
public abstract class com.google.common.collect.FluentIterable<E> implements java.lang.Iterable<E> {
  public static <E> com.google.common.collect.FluentIterable<E> from(java.lang.Iterable<E>);
  public static <E> com.google.common.collect.FluentIterable<E> from(E[]);
  public static <E> com.google.common.collect.FluentIterable<E> from(com.google.common.collect.FluentIterable<E>);
  public static <T> com.google.common.collect.FluentIterable<T> concat(java.lang.Iterable<? extends T>, java.lang.Iterable<? extends T>);
  public static <T> com.google.common.collect.FluentIterable<T> concat(java.lang.Iterable<? extends T>, java.lang.Iterable<? extends T>, java.lang.Iterable<? extends T>);
  public static <T> com.google.common.collect.FluentIterable<T> concat(java.lang.Iterable<? extends T>, java.lang.Iterable<? extends T>, java.lang.Iterable<? extends T>, java.lang.Iterable<? extends T>);
  public static <T> com.google.common.collect.FluentIterable<T> concat(java.lang.Iterable<? extends T>...);
  public static <T> com.google.common.collect.FluentIterable<T> concat(java.lang.Iterable<? extends java.lang.Iterable<? extends T>>);
  public static <E> com.google.common.collect.FluentIterable<E> of();
  public static <E> com.google.common.collect.FluentIterable<E> of(E, E...);
  public java.lang.String toString();
  public final int size();
  public final boolean contains(java.lang.Object);
  public final com.google.common.collect.FluentIterable<E> cycle();
  public final com.google.common.collect.FluentIterable<E> append(java.lang.Iterable<? extends E>);
  public final com.google.common.collect.FluentIterable<E> append(E...);
  public final com.google.common.collect.FluentIterable<E> filter(com.google.common.base.Predicate<? super E>);
  public final <T> com.google.common.collect.FluentIterable<T> filter(java.lang.Class<T>);
  public final boolean anyMatch(com.google.common.base.Predicate<? super E>);
  public final boolean allMatch(com.google.common.base.Predicate<? super E>);
  public final com.google.common.base.Optional<E> firstMatch(com.google.common.base.Predicate<? super E>);
  public final <T> com.google.common.collect.FluentIterable<T> transform(com.google.common.base.Function<? super E, T>);
  public <T> com.google.common.collect.FluentIterable<T> transformAndConcat(com.google.common.base.Function<? super E, ? extends java.lang.Iterable<? extends T>>);
  public final com.google.common.base.Optional<E> first();
  public final com.google.common.base.Optional<E> last();
  public final com.google.common.collect.FluentIterable<E> skip(int);
  public final com.google.common.collect.FluentIterable<E> limit(int);
  public final boolean isEmpty();
  public final com.google.common.collect.ImmutableList<E> toList();
  public final com.google.common.collect.ImmutableList<E> toSortedList(java.util.Comparator<? super E>);
  public final com.google.common.collect.ImmutableSet<E> toSet();
  public final com.google.common.collect.ImmutableSortedSet<E> toSortedSet(java.util.Comparator<? super E>);
  public final com.google.common.collect.ImmutableMultiset<E> toMultiset();
  public final <V> com.google.common.collect.ImmutableMap<E, V> toMap(com.google.common.base.Function<? super E, V>);
  public final <K> com.google.common.collect.ImmutableListMultimap<K, E> index(com.google.common.base.Function<? super E, K>);
  public final <K> com.google.common.collect.ImmutableMap<K, E> uniqueIndex(com.google.common.base.Function<? super E, K>);
  public final E[] toArray(java.lang.Class<E>);
  public final <C extends java.util.Collection<? super E>> C copyInto(C);
  public final java.lang.String join(com.google.common.base.Joiner);
  public final E get(int);
  public final java.util.stream.Stream<E> stream();
}
```

## `com.google.common.collect.ForwardingBlockingDeque`

```java
public abstract class com.google.common.collect.ForwardingBlockingDeque<E> extends com.google.common.collect.ForwardingDeque<E> implements java.util.concurrent.BlockingDeque<E> {
  public int remainingCapacity();
  public void putFirst(E) throws java.lang.InterruptedException;
  public void putLast(E) throws java.lang.InterruptedException;
  public boolean offerFirst(E, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public boolean offerLast(E, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public E takeFirst() throws java.lang.InterruptedException;
  public E takeLast() throws java.lang.InterruptedException;
  public E pollFirst(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public E pollLast(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public void put(E) throws java.lang.InterruptedException;
  public boolean offer(E, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public E take() throws java.lang.InterruptedException;
  public E poll(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public int drainTo(java.util.Collection<? super E>);
  public int drainTo(java.util.Collection<? super E>, int);
}
```

## `com.google.common.collect.ForwardingCollection`

```java
public abstract class com.google.common.collect.ForwardingCollection<E> extends com.google.common.collect.ForwardingObject implements java.util.Collection<E> {
  public java.util.Iterator<E> iterator();
  public int size();
  public boolean removeAll(java.util.Collection<?>);
  public boolean isEmpty();
  public boolean contains(java.lang.Object);
  public boolean add(E);
  public boolean remove(java.lang.Object);
  public boolean containsAll(java.util.Collection<?>);
  public boolean addAll(java.util.Collection<? extends E>);
  public boolean retainAll(java.util.Collection<?>);
  public void clear();
  public java.lang.Object[] toArray();
  public <T> T[] toArray(T[]);
}
```

## `com.google.common.collect.ForwardingConcurrentMap`

```java
public abstract class com.google.common.collect.ForwardingConcurrentMap<K, V> extends com.google.common.collect.ForwardingMap<K, V> implements java.util.concurrent.ConcurrentMap<K, V> {
  public V putIfAbsent(K, V);
  public boolean remove(java.lang.Object, java.lang.Object);
  public V replace(K, V);
  public boolean replace(K, V, V);
}
```

## `com.google.common.collect.ForwardingDeque`

```java
public abstract class com.google.common.collect.ForwardingDeque<E> extends com.google.common.collect.ForwardingQueue<E> implements java.util.Deque<E> {
  public void addFirst(E);
  public void addLast(E);
  public java.util.Iterator<E> descendingIterator();
  public E getFirst();
  public E getLast();
  public boolean offerFirst(E);
  public boolean offerLast(E);
  public E peekFirst();
  public E peekLast();
  public E pollFirst();
  public E pollLast();
  public E pop();
  public void push(E);
  public E removeFirst();
  public E removeLast();
  public boolean removeFirstOccurrence(java.lang.Object);
  public boolean removeLastOccurrence(java.lang.Object);
}
```

## `com.google.common.collect.ForwardingIterator`

```java
public abstract class com.google.common.collect.ForwardingIterator<T> extends com.google.common.collect.ForwardingObject implements java.util.Iterator<T> {
  public boolean hasNext();
  public T next();
  public void remove();
}
```

## `com.google.common.collect.ForwardingList`

```java
public abstract class com.google.common.collect.ForwardingList<E> extends com.google.common.collect.ForwardingCollection<E> implements java.util.List<E> {
  public void add(int, E);
  public boolean addAll(int, java.util.Collection<? extends E>);
  public E get(int);
  public int indexOf(java.lang.Object);
  public int lastIndexOf(java.lang.Object);
  public java.util.ListIterator<E> listIterator();
  public java.util.ListIterator<E> listIterator(int);
  public E remove(int);
  public E set(int, E);
  public java.util.List<E> subList(int, int);
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.google.common.collect.ForwardingListIterator`

```java
public abstract class com.google.common.collect.ForwardingListIterator<E> extends com.google.common.collect.ForwardingIterator<E> implements java.util.ListIterator<E> {
  public void add(E);
  public boolean hasPrevious();
  public int nextIndex();
  public E previous();
  public int previousIndex();
  public void set(E);
}
```

## `com.google.common.collect.ForwardingListMultimap`

```java
public abstract class com.google.common.collect.ForwardingListMultimap<K, V> extends com.google.common.collect.ForwardingMultimap<K, V> implements com.google.common.collect.ListMultimap<K, V> {
  public java.util.List<V> get(K);
  public java.util.List<V> removeAll(java.lang.Object);
  public java.util.List<V> replaceValues(K, java.lang.Iterable<? extends V>);
  public java.util.Collection replaceValues(java.lang.Object, java.lang.Iterable);
  public java.util.Collection removeAll(java.lang.Object);
  public java.util.Collection get(java.lang.Object);
}
```

## `com.google.common.collect.ForwardingMap`

```java
public abstract class com.google.common.collect.ForwardingMap<K, V> extends com.google.common.collect.ForwardingObject implements java.util.Map<K, V> {
  public int size();
  public boolean isEmpty();
  public V remove(java.lang.Object);
  public void clear();
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public V get(java.lang.Object);
  public V put(K, V);
  public void putAll(java.util.Map<? extends K, ? extends V>);
  public java.util.Set<K> keySet();
  public java.util.Collection<V> values();
  public java.util.Set<java.util.Map$Entry<K, V>> entrySet();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.google.common.collect.ForwardingMap$StandardKeySet`

```java
public class com.google.common.collect.ForwardingMap$StandardKeySet extends com.google.common.collect.Maps$KeySet<K, V> {
  public com.google.common.collect.ForwardingMap$StandardKeySet(com.google.common.collect.ForwardingMap);
}
```

## `com.google.common.collect.ForwardingMap$StandardValues`

```java
public class com.google.common.collect.ForwardingMap$StandardValues extends com.google.common.collect.Maps$Values<K, V> {
  public com.google.common.collect.ForwardingMap$StandardValues(com.google.common.collect.ForwardingMap);
}
```

## `com.google.common.collect.ForwardingMapEntry`

```java
public abstract class com.google.common.collect.ForwardingMapEntry<K, V> extends com.google.common.collect.ForwardingObject implements java.util.Map$Entry<K, V> {
  public K getKey();
  public V getValue();
  public V setValue(V);
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.google.common.collect.ForwardingMultimap`

```java
public abstract class com.google.common.collect.ForwardingMultimap<K, V> extends com.google.common.collect.ForwardingObject implements com.google.common.collect.Multimap<K, V> {
  public java.util.Map<K, java.util.Collection<V>> asMap();
  public void clear();
  public boolean containsEntry(java.lang.Object, java.lang.Object);
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public java.util.Collection<java.util.Map$Entry<K, V>> entries();
  public java.util.Collection<V> get(K);
  public boolean isEmpty();
  public com.google.common.collect.Multiset<K> keys();
  public java.util.Set<K> keySet();
  public boolean put(K, V);
  public boolean putAll(K, java.lang.Iterable<? extends V>);
  public boolean putAll(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public boolean remove(java.lang.Object, java.lang.Object);
  public java.util.Collection<V> removeAll(java.lang.Object);
  public java.util.Collection<V> replaceValues(K, java.lang.Iterable<? extends V>);
  public int size();
  public java.util.Collection<V> values();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.google.common.collect.ForwardingMultiset`

```java
public abstract class com.google.common.collect.ForwardingMultiset<E> extends com.google.common.collect.ForwardingCollection<E> implements com.google.common.collect.Multiset<E> {
  public int count(java.lang.Object);
  public int add(E, int);
  public int remove(java.lang.Object, int);
  public java.util.Set<E> elementSet();
  public java.util.Set<com.google.common.collect.Multiset$Entry<E>> entrySet();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public int setCount(E, int);
  public boolean setCount(E, int, int);
}
```

## `com.google.common.collect.ForwardingMultiset$StandardElementSet`

```java
public class com.google.common.collect.ForwardingMultiset$StandardElementSet extends com.google.common.collect.Multisets$ElementSet<E> {
  public com.google.common.collect.ForwardingMultiset$StandardElementSet(com.google.common.collect.ForwardingMultiset);
  public java.util.Iterator<E> iterator();
}
```

## `com.google.common.collect.ForwardingNavigableMap`

```java
public abstract class com.google.common.collect.ForwardingNavigableMap<K, V> extends com.google.common.collect.ForwardingSortedMap<K, V> implements java.util.NavigableMap<K, V> {
  public java.util.Map$Entry<K, V> lowerEntry(K);
  public K lowerKey(K);
  public java.util.Map$Entry<K, V> floorEntry(K);
  public K floorKey(K);
  public java.util.Map$Entry<K, V> ceilingEntry(K);
  public K ceilingKey(K);
  public java.util.Map$Entry<K, V> higherEntry(K);
  public K higherKey(K);
  public java.util.Map$Entry<K, V> firstEntry();
  public java.util.Map$Entry<K, V> lastEntry();
  public java.util.Map$Entry<K, V> pollFirstEntry();
  public java.util.Map$Entry<K, V> pollLastEntry();
  public java.util.NavigableMap<K, V> descendingMap();
  public java.util.NavigableSet<K> navigableKeySet();
  public java.util.NavigableSet<K> descendingKeySet();
  public java.util.NavigableMap<K, V> subMap(K, boolean, K, boolean);
  public java.util.NavigableMap<K, V> headMap(K, boolean);
  public java.util.NavigableMap<K, V> tailMap(K, boolean);
}
```

## `com.google.common.collect.ForwardingNavigableMap$StandardDescendingMap`

```java
public class com.google.common.collect.ForwardingNavigableMap$StandardDescendingMap extends com.google.common.collect.Maps$DescendingMap<K, V> {
  public com.google.common.collect.ForwardingNavigableMap$StandardDescendingMap(com.google.common.collect.ForwardingNavigableMap);
  public void replaceAll(java.util.function.BiFunction<? super K, ? super V, ? extends V>);
}
```

## `com.google.common.collect.ForwardingNavigableMap$StandardNavigableKeySet`

```java
public class com.google.common.collect.ForwardingNavigableMap$StandardNavigableKeySet extends com.google.common.collect.Maps$NavigableKeySet<K, V> {
  public com.google.common.collect.ForwardingNavigableMap$StandardNavigableKeySet(com.google.common.collect.ForwardingNavigableMap);
}
```

## `com.google.common.collect.ForwardingNavigableSet`

```java
public abstract class com.google.common.collect.ForwardingNavigableSet<E> extends com.google.common.collect.ForwardingSortedSet<E> implements java.util.NavigableSet<E> {
  public E lower(E);
  public E floor(E);
  public E ceiling(E);
  public E higher(E);
  public E pollFirst();
  public E pollLast();
  public java.util.NavigableSet<E> descendingSet();
  public java.util.Iterator<E> descendingIterator();
  public java.util.NavigableSet<E> subSet(E, boolean, E, boolean);
  public java.util.NavigableSet<E> headSet(E, boolean);
  public java.util.NavigableSet<E> tailSet(E, boolean);
}
```

## `com.google.common.collect.ForwardingNavigableSet$StandardDescendingSet`

```java
public class com.google.common.collect.ForwardingNavigableSet$StandardDescendingSet extends com.google.common.collect.Sets$DescendingSet<E> {
  public com.google.common.collect.ForwardingNavigableSet$StandardDescendingSet(com.google.common.collect.ForwardingNavigableSet);
}
```

## `com.google.common.collect.ForwardingObject`

```java
public abstract class com.google.common.collect.ForwardingObject {
  public java.lang.String toString();
}
```

## `com.google.common.collect.ForwardingQueue`

```java
public abstract class com.google.common.collect.ForwardingQueue<E> extends com.google.common.collect.ForwardingCollection<E> implements java.util.Queue<E> {
  public boolean offer(E);
  public E poll();
  public E remove();
  public E peek();
  public E element();
}
```

## `com.google.common.collect.ForwardingSet`

```java
public abstract class com.google.common.collect.ForwardingSet<E> extends com.google.common.collect.ForwardingCollection<E> implements java.util.Set<E> {
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.google.common.collect.ForwardingSetMultimap`

```java
public abstract class com.google.common.collect.ForwardingSetMultimap<K, V> extends com.google.common.collect.ForwardingMultimap<K, V> implements com.google.common.collect.SetMultimap<K, V> {
  public com.google.common.collect.ForwardingSetMultimap();
  public java.util.Set<java.util.Map$Entry<K, V>> entries();
  public java.util.Set<V> get(K);
  public java.util.Set<V> removeAll(java.lang.Object);
  public java.util.Set<V> replaceValues(K, java.lang.Iterable<? extends V>);
  public java.util.Collection replaceValues(java.lang.Object, java.lang.Iterable);
  public java.util.Collection removeAll(java.lang.Object);
  public java.util.Collection get(java.lang.Object);
  public java.util.Collection entries();
}
```

## `com.google.common.collect.ForwardingSortedMap`

```java
public abstract class com.google.common.collect.ForwardingSortedMap<K, V> extends com.google.common.collect.ForwardingMap<K, V> implements java.util.SortedMap<K, V> {
  public java.util.Comparator<? super K> comparator();
  public K firstKey();
  public java.util.SortedMap<K, V> headMap(K);
  public K lastKey();
  public java.util.SortedMap<K, V> subMap(K, K);
  public java.util.SortedMap<K, V> tailMap(K);
}
```

## `com.google.common.collect.ForwardingSortedMap$StandardKeySet`

```java
public class com.google.common.collect.ForwardingSortedMap$StandardKeySet extends com.google.common.collect.Maps$SortedKeySet<K, V> {
  public com.google.common.collect.ForwardingSortedMap$StandardKeySet(com.google.common.collect.ForwardingSortedMap);
}
```

## `com.google.common.collect.ForwardingSortedMultiset`

```java
public abstract class com.google.common.collect.ForwardingSortedMultiset<E> extends com.google.common.collect.ForwardingMultiset<E> implements com.google.common.collect.SortedMultiset<E> {
  public java.util.NavigableSet<E> elementSet();
  public java.util.Comparator<? super E> comparator();
  public com.google.common.collect.SortedMultiset<E> descendingMultiset();
  public com.google.common.collect.Multiset$Entry<E> firstEntry();
  public com.google.common.collect.Multiset$Entry<E> lastEntry();
  public com.google.common.collect.Multiset$Entry<E> pollFirstEntry();
  public com.google.common.collect.Multiset$Entry<E> pollLastEntry();
  public com.google.common.collect.SortedMultiset<E> headMultiset(E, com.google.common.collect.BoundType);
  public com.google.common.collect.SortedMultiset<E> subMultiset(E, com.google.common.collect.BoundType, E, com.google.common.collect.BoundType);
  public com.google.common.collect.SortedMultiset<E> tailMultiset(E, com.google.common.collect.BoundType);
  public java.util.Set elementSet();
  public java.util.SortedSet elementSet();
}
```

## `com.google.common.collect.ForwardingSortedMultiset$StandardDescendingMultiset`

```java
public abstract class com.google.common.collect.ForwardingSortedMultiset$StandardDescendingMultiset extends com.google.common.collect.DescendingMultiset<E> {
  public com.google.common.collect.ForwardingSortedMultiset$StandardDescendingMultiset(com.google.common.collect.ForwardingSortedMultiset);
}
```

## `com.google.common.collect.ForwardingSortedMultiset$StandardElementSet`

```java
public class com.google.common.collect.ForwardingSortedMultiset$StandardElementSet extends com.google.common.collect.SortedMultisets$NavigableElementSet<E> {
  public com.google.common.collect.ForwardingSortedMultiset$StandardElementSet(com.google.common.collect.ForwardingSortedMultiset);
}
```

## `com.google.common.collect.ForwardingSortedSet`

```java
public abstract class com.google.common.collect.ForwardingSortedSet<E> extends com.google.common.collect.ForwardingSet<E> implements java.util.SortedSet<E> {
  public java.util.Comparator<? super E> comparator();
  public E first();
  public java.util.SortedSet<E> headSet(E);
  public E last();
  public java.util.SortedSet<E> subSet(E, E);
  public java.util.SortedSet<E> tailSet(E);
}
```

## `com.google.common.collect.ForwardingSortedSetMultimap`

```java
public abstract class com.google.common.collect.ForwardingSortedSetMultimap<K, V> extends com.google.common.collect.ForwardingSetMultimap<K, V> implements com.google.common.collect.SortedSetMultimap<K, V> {
  public java.util.SortedSet<V> get(K);
  public java.util.SortedSet<V> removeAll(java.lang.Object);
  public java.util.SortedSet<V> replaceValues(K, java.lang.Iterable<? extends V>);
  public java.util.Comparator<? super V> valueComparator();
  public java.util.Set replaceValues(java.lang.Object, java.lang.Iterable);
  public java.util.Set removeAll(java.lang.Object);
  public java.util.Set get(java.lang.Object);
  public java.util.Collection get(java.lang.Object);
  public java.util.Collection removeAll(java.lang.Object);
  public java.util.Collection replaceValues(java.lang.Object, java.lang.Iterable);
}
```

## `com.google.common.collect.ForwardingTable`

```java
public abstract class com.google.common.collect.ForwardingTable<R, C, V> extends com.google.common.collect.ForwardingObject implements com.google.common.collect.Table<R, C, V> {
  public java.util.Set<com.google.common.collect.Table$Cell<R, C, V>> cellSet();
  public void clear();
  public java.util.Map<R, V> column(C);
  public java.util.Set<C> columnKeySet();
  public java.util.Map<C, java.util.Map<R, V>> columnMap();
  public boolean contains(java.lang.Object, java.lang.Object);
  public boolean containsColumn(java.lang.Object);
  public boolean containsRow(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public V get(java.lang.Object, java.lang.Object);
  public boolean isEmpty();
  public V put(R, C, V);
  public void putAll(com.google.common.collect.Table<? extends R, ? extends C, ? extends V>);
  public V remove(java.lang.Object, java.lang.Object);
  public java.util.Map<C, V> row(R);
  public java.util.Set<R> rowKeySet();
  public java.util.Map<R, java.util.Map<C, V>> rowMap();
  public int size();
  public java.util.Collection<V> values();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.google.common.collect.HashBasedTable`

```java
public class com.google.common.collect.HashBasedTable<R, C, V> extends com.google.common.collect.StandardTable<R, C, V> {
  public static <R, C, V> com.google.common.collect.HashBasedTable<R, C, V> create();
  public static <R, C, V> com.google.common.collect.HashBasedTable<R, C, V> create(int, int);
  public static <R, C, V> com.google.common.collect.HashBasedTable<R, C, V> create(com.google.common.collect.Table<? extends R, ? extends C, ? extends V>);
  public java.util.Map columnMap();
  public java.util.Map rowMap();
  public java.util.Collection values();
  public java.util.Set columnKeySet();
  public java.util.Set rowKeySet();
  public java.util.Map column(java.lang.Object);
  public java.util.Map row(java.lang.Object);
  public java.util.Set cellSet();
  public java.lang.Object remove(java.lang.Object, java.lang.Object);
  public java.lang.Object put(java.lang.Object, java.lang.Object, java.lang.Object);
  public void clear();
  public int size();
  public boolean isEmpty();
  public java.lang.Object get(java.lang.Object, java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public boolean containsRow(java.lang.Object);
  public boolean containsColumn(java.lang.Object);
  public boolean contains(java.lang.Object, java.lang.Object);
  public java.lang.String toString();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public void putAll(com.google.common.collect.Table);
}
```

## `com.google.common.collect.HashBiMap`

```java
public final class com.google.common.collect.HashBiMap<K, V> extends com.google.common.collect.Maps$IteratorBasedAbstractMap<K, V> implements com.google.common.collect.BiMap<K, V>, java.io.Serializable {
  public static <K, V> com.google.common.collect.HashBiMap<K, V> create();
  public static <K, V> com.google.common.collect.HashBiMap<K, V> create(int);
  public static <K, V> com.google.common.collect.HashBiMap<K, V> create(java.util.Map<? extends K, ? extends V>);
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public V get(java.lang.Object);
  public V put(K, V);
  public V forcePut(K, V);
  public V remove(java.lang.Object);
  public void clear();
  public int size();
  public java.util.Set<K> keySet();
  public java.util.Set<V> values();
  public void forEach(java.util.function.BiConsumer<? super K, ? super V>);
  public void replaceAll(java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public com.google.common.collect.BiMap<V, K> inverse();
  public java.util.Set entrySet();
  public java.util.Collection values();
}
```

## `com.google.common.collect.HashMultimap`

```java
public final class com.google.common.collect.HashMultimap<K, V> extends com.google.common.collect.HashMultimapGwtSerializationDependencies<K, V> {
  public static <K, V> com.google.common.collect.HashMultimap<K, V> create();
  public static <K, V> com.google.common.collect.HashMultimap<K, V> create(int, int);
  public static <K, V> com.google.common.collect.HashMultimap<K, V> create(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public boolean equals(java.lang.Object);
  public boolean put(java.lang.Object, java.lang.Object);
  public java.util.Map asMap();
  public java.util.Set replaceValues(java.lang.Object, java.lang.Iterable);
  public java.util.Set removeAll(java.lang.Object);
  public java.util.Set entries();
  public java.util.Set get(java.lang.Object);
  public void forEach(java.util.function.BiConsumer);
  public java.util.Collection values();
  public void clear();
  public boolean containsKey(java.lang.Object);
  public int size();
  public java.lang.String toString();
  public int hashCode();
  public com.google.common.collect.Multiset keys();
  public java.util.Set keySet();
  public boolean putAll(com.google.common.collect.Multimap);
  public boolean putAll(java.lang.Object, java.lang.Iterable);
  public boolean remove(java.lang.Object, java.lang.Object);
  public boolean containsEntry(java.lang.Object, java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public boolean isEmpty();
}
```

## `com.google.common.collect.HashMultiset`

```java
public final class com.google.common.collect.HashMultiset<E> extends com.google.common.collect.AbstractMapBasedMultiset<E> {
  public static <E> com.google.common.collect.HashMultiset<E> create();
  public static <E> com.google.common.collect.HashMultiset<E> create(int);
  public static <E> com.google.common.collect.HashMultiset<E> create(java.lang.Iterable<? extends E>);
  public int setCount(java.lang.Object, int);
  public int remove(java.lang.Object, int);
  public int add(java.lang.Object, int);
  public int count(java.lang.Object);
  public java.util.Iterator iterator();
  public int size();
  public void clear();
  public void forEachEntry(java.util.function.ObjIntConsumer);
  public java.util.Set entrySet();
  public java.util.Set elementSet();
  public boolean setCount(java.lang.Object, int, int);
  public boolean contains(java.lang.Object);
  public boolean isEmpty();
}
```

## `com.google.common.collect.ImmutableBiMap`

```java
public abstract class com.google.common.collect.ImmutableBiMap<K, V> extends com.google.common.collect.ImmutableMap<K, V> implements com.google.common.collect.BiMap<K, V> {
  public static <T, K, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableBiMap<K, V>> toImmutableBiMap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends V>);
  public static <K, V> com.google.common.collect.ImmutableBiMap<K, V> of();
  public static <K, V> com.google.common.collect.ImmutableBiMap<K, V> of(K, V);
  public static <K, V> com.google.common.collect.ImmutableBiMap<K, V> of(K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableBiMap<K, V> of(K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableBiMap<K, V> of(K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableBiMap<K, V> of(K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableBiMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableBiMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableBiMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableBiMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableBiMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableBiMap<K, V> ofEntries(java.util.Map$Entry<? extends K, ? extends V>...);
  public static <K, V> com.google.common.collect.ImmutableBiMap$Builder<K, V> builder();
  public static <K, V> com.google.common.collect.ImmutableBiMap$Builder<K, V> builderWithExpectedSize(int);
  public static <K, V> com.google.common.collect.ImmutableBiMap<K, V> copyOf(java.util.Map<? extends K, ? extends V>);
  public static <K, V> com.google.common.collect.ImmutableBiMap<K, V> copyOf(java.lang.Iterable<? extends java.util.Map$Entry<? extends K, ? extends V>>);
  public abstract com.google.common.collect.ImmutableBiMap<V, K> inverse();
  public com.google.common.collect.ImmutableSet<V> values();
  public final V forcePut(K, V);
  public static <T, K, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableMap<K, V>> toImmutableMap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends V>);
  public static <T, K, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableMap<K, V>> toImmutableMap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends V>, java.util.function.BinaryOperator<V>);
  public com.google.common.collect.ImmutableCollection values();
  public java.util.Collection values();
  public com.google.common.collect.BiMap inverse();
  public java.util.Set values();
}
```

## `com.google.common.collect.ImmutableBiMap$Builder`

```java
public final class com.google.common.collect.ImmutableBiMap$Builder<K, V> extends com.google.common.collect.ImmutableMap$Builder<K, V> {
  public com.google.common.collect.ImmutableBiMap$Builder();
  public com.google.common.collect.ImmutableBiMap$Builder<K, V> put(K, V);
  public com.google.common.collect.ImmutableBiMap$Builder<K, V> put(java.util.Map$Entry<? extends K, ? extends V>);
  public com.google.common.collect.ImmutableBiMap$Builder<K, V> putAll(java.util.Map<? extends K, ? extends V>);
  public com.google.common.collect.ImmutableBiMap$Builder<K, V> putAll(java.lang.Iterable<? extends java.util.Map$Entry<? extends K, ? extends V>>);
  public com.google.common.collect.ImmutableBiMap$Builder<K, V> orderEntriesByValue(java.util.Comparator<? super V>);
  public com.google.common.collect.ImmutableBiMap<K, V> build();
  public com.google.common.collect.ImmutableBiMap<K, V> buildOrThrow();
  public com.google.common.collect.ImmutableBiMap<K, V> buildKeepingLast();
  public com.google.common.collect.ImmutableMap buildKeepingLast();
  public com.google.common.collect.ImmutableMap buildOrThrow();
  public com.google.common.collect.ImmutableMap build();
  public com.google.common.collect.ImmutableMap$Builder orderEntriesByValue(java.util.Comparator);
  public com.google.common.collect.ImmutableMap$Builder putAll(java.lang.Iterable);
  public com.google.common.collect.ImmutableMap$Builder putAll(java.util.Map);
  public com.google.common.collect.ImmutableMap$Builder put(java.util.Map$Entry);
  public com.google.common.collect.ImmutableMap$Builder put(java.lang.Object, java.lang.Object);
}
```

## `com.google.common.collect.ImmutableClassToInstanceMap`

```java
public final class com.google.common.collect.ImmutableClassToInstanceMap<B> extends com.google.common.collect.ForwardingMap<java.lang.Class<? extends B>, B> implements com.google.common.collect.ClassToInstanceMap<B>, java.io.Serializable {
  public static <B> com.google.common.collect.ImmutableClassToInstanceMap<B> of();
  public static <B, T extends B> com.google.common.collect.ImmutableClassToInstanceMap<B> of(java.lang.Class<T>, T);
  public static <B> com.google.common.collect.ImmutableClassToInstanceMap$Builder<B> builder();
  public static <B, S extends B> com.google.common.collect.ImmutableClassToInstanceMap<B> copyOf(java.util.Map<? extends java.lang.Class<? extends S>, ? extends S>);
  public <T extends B> T getInstance(java.lang.Class<T>);
  public <T extends B> T putInstance(java.lang.Class<T>, T);
}
```

## `com.google.common.collect.ImmutableClassToInstanceMap$Builder`

```java
public final class com.google.common.collect.ImmutableClassToInstanceMap$Builder<B> {
  public com.google.common.collect.ImmutableClassToInstanceMap$Builder();
  public <T extends B> com.google.common.collect.ImmutableClassToInstanceMap$Builder<B> put(java.lang.Class<T>, T);
  public <T extends B> com.google.common.collect.ImmutableClassToInstanceMap$Builder<B> putAll(java.util.Map<? extends java.lang.Class<? extends T>, ? extends T>);
  public com.google.common.collect.ImmutableClassToInstanceMap<B> build();
}
```

## `com.google.common.collect.ImmutableCollection`

```java
public abstract class com.google.common.collect.ImmutableCollection<E> extends java.util.AbstractCollection<E> implements java.io.Serializable {
  public abstract com.google.common.collect.UnmodifiableIterator<E> iterator();
  public java.util.Spliterator<E> spliterator();
  public final java.lang.Object[] toArray();
  public final <T> T[] toArray(T[]);
  public abstract boolean contains(java.lang.Object);
  public final boolean add(E);
  public final boolean remove(java.lang.Object);
  public final boolean addAll(java.util.Collection<? extends E>);
  public final boolean removeAll(java.util.Collection<?>);
  public final boolean removeIf(java.util.function.Predicate<? super E>);
  public final boolean retainAll(java.util.Collection<?>);
  public final void clear();
  public com.google.common.collect.ImmutableList<E> asList();
  public java.util.Iterator iterator();
}
```

## `com.google.common.collect.ImmutableCollection$Builder`

```java
public abstract class com.google.common.collect.ImmutableCollection$Builder<E> {
  public abstract com.google.common.collect.ImmutableCollection$Builder<E> add(E);
  public com.google.common.collect.ImmutableCollection$Builder<E> add(E...);
  public com.google.common.collect.ImmutableCollection$Builder<E> addAll(java.lang.Iterable<? extends E>);
  public com.google.common.collect.ImmutableCollection$Builder<E> addAll(java.util.Iterator<? extends E>);
  public abstract com.google.common.collect.ImmutableCollection<E> build();
}
```

## `com.google.common.collect.ImmutableList`

```java
public abstract class com.google.common.collect.ImmutableList<E> extends com.google.common.collect.ImmutableCollection<E> implements java.util.List<E>, java.util.RandomAccess {
  public static <E> java.util.stream.Collector<E, ?, com.google.common.collect.ImmutableList<E>> toImmutableList();
  public static <E> com.google.common.collect.ImmutableList<E> of();
  public static <E> com.google.common.collect.ImmutableList<E> of(E);
  public static <E> com.google.common.collect.ImmutableList<E> of(E, E);
  public static <E> com.google.common.collect.ImmutableList<E> of(E, E, E);
  public static <E> com.google.common.collect.ImmutableList<E> of(E, E, E, E);
  public static <E> com.google.common.collect.ImmutableList<E> of(E, E, E, E, E);
  public static <E> com.google.common.collect.ImmutableList<E> of(E, E, E, E, E, E);
  public static <E> com.google.common.collect.ImmutableList<E> of(E, E, E, E, E, E, E);
  public static <E> com.google.common.collect.ImmutableList<E> of(E, E, E, E, E, E, E, E);
  public static <E> com.google.common.collect.ImmutableList<E> of(E, E, E, E, E, E, E, E, E);
  public static <E> com.google.common.collect.ImmutableList<E> of(E, E, E, E, E, E, E, E, E, E);
  public static <E> com.google.common.collect.ImmutableList<E> of(E, E, E, E, E, E, E, E, E, E, E);
  public static <E> com.google.common.collect.ImmutableList<E> of(E, E, E, E, E, E, E, E, E, E, E, E, E...);
  public static <E> com.google.common.collect.ImmutableList<E> copyOf(java.lang.Iterable<? extends E>);
  public static <E> com.google.common.collect.ImmutableList<E> copyOf(java.util.Collection<? extends E>);
  public static <E> com.google.common.collect.ImmutableList<E> copyOf(java.util.Iterator<? extends E>);
  public static <E> com.google.common.collect.ImmutableList<E> copyOf(E[]);
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableList<E> sortedCopyOf(java.lang.Iterable<? extends E>);
  public static <E> com.google.common.collect.ImmutableList<E> sortedCopyOf(java.util.Comparator<? super E>, java.lang.Iterable<? extends E>);
  public com.google.common.collect.UnmodifiableIterator<E> iterator();
  public com.google.common.collect.UnmodifiableListIterator<E> listIterator();
  public com.google.common.collect.UnmodifiableListIterator<E> listIterator(int);
  public void forEach(java.util.function.Consumer<? super E>);
  public int indexOf(java.lang.Object);
  public int lastIndexOf(java.lang.Object);
  public boolean contains(java.lang.Object);
  public com.google.common.collect.ImmutableList<E> subList(int, int);
  public final boolean addAll(int, java.util.Collection<? extends E>);
  public final E set(int, E);
  public final void add(int, E);
  public final E remove(int);
  public final void replaceAll(java.util.function.UnaryOperator<E>);
  public final void sort(java.util.Comparator<? super E>);
  public final com.google.common.collect.ImmutableList<E> asList();
  public java.util.Spliterator<E> spliterator();
  public com.google.common.collect.ImmutableList<E> reverse();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public static <E> com.google.common.collect.ImmutableList$Builder<E> builder();
  public static <E> com.google.common.collect.ImmutableList$Builder<E> builderWithExpectedSize(int);
  public java.util.Iterator iterator();
  public java.util.List subList(int, int);
  public java.util.ListIterator listIterator(int);
  public java.util.ListIterator listIterator();
}
```

## `com.google.common.collect.ImmutableList$Builder`

```java
public final class com.google.common.collect.ImmutableList$Builder<E> extends com.google.common.collect.ImmutableCollection$Builder<E> {
  public com.google.common.collect.ImmutableList$Builder();
  public com.google.common.collect.ImmutableList$Builder<E> add(E);
  public com.google.common.collect.ImmutableList$Builder<E> add(E...);
  public com.google.common.collect.ImmutableList$Builder<E> addAll(java.lang.Iterable<? extends E>);
  public com.google.common.collect.ImmutableList$Builder<E> addAll(java.util.Iterator<? extends E>);
  public com.google.common.collect.ImmutableList<E> build();
  public com.google.common.collect.ImmutableCollection build();
  public com.google.common.collect.ImmutableCollection$Builder addAll(java.util.Iterator);
  public com.google.common.collect.ImmutableCollection$Builder addAll(java.lang.Iterable);
  public com.google.common.collect.ImmutableCollection$Builder add(java.lang.Object[]);
  public com.google.common.collect.ImmutableCollection$Builder add(java.lang.Object);
}
```

## `com.google.common.collect.ImmutableListMultimap`

```java
public class com.google.common.collect.ImmutableListMultimap<K, V> extends com.google.common.collect.ImmutableMultimap<K, V> implements com.google.common.collect.ListMultimap<K, V> {
  public static <T, K, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableListMultimap<K, V>> toImmutableListMultimap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends V>);
  public static <T, K, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableListMultimap<K, V>> flatteningToImmutableListMultimap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends java.util.stream.Stream<? extends V>>);
  public static <K, V> com.google.common.collect.ImmutableListMultimap<K, V> of();
  public static <K, V> com.google.common.collect.ImmutableListMultimap<K, V> of(K, V);
  public static <K, V> com.google.common.collect.ImmutableListMultimap<K, V> of(K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableListMultimap<K, V> of(K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableListMultimap<K, V> of(K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableListMultimap<K, V> of(K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableListMultimap$Builder<K, V> builder();
  public static <K, V> com.google.common.collect.ImmutableListMultimap$Builder<K, V> builderWithExpectedKeys(int);
  public static <K, V> com.google.common.collect.ImmutableListMultimap<K, V> copyOf(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public static <K, V> com.google.common.collect.ImmutableListMultimap<K, V> copyOf(java.lang.Iterable<? extends java.util.Map$Entry<? extends K, ? extends V>>);
  public com.google.common.collect.ImmutableList<V> get(K);
  public com.google.common.collect.ImmutableListMultimap<V, K> inverse();
  public final com.google.common.collect.ImmutableList<V> removeAll(java.lang.Object);
  public final com.google.common.collect.ImmutableList<V> replaceValues(K, java.lang.Iterable<? extends V>);
  public com.google.common.collect.ImmutableMultimap inverse();
  public com.google.common.collect.ImmutableCollection get(java.lang.Object);
  public com.google.common.collect.ImmutableCollection replaceValues(java.lang.Object, java.lang.Iterable);
  public com.google.common.collect.ImmutableCollection removeAll(java.lang.Object);
  public java.util.Collection replaceValues(java.lang.Object, java.lang.Iterable);
  public java.util.Collection get(java.lang.Object);
  public java.util.Collection removeAll(java.lang.Object);
  public java.util.List replaceValues(java.lang.Object, java.lang.Iterable);
  public java.util.List removeAll(java.lang.Object);
  public java.util.List get(java.lang.Object);
}
```

## `com.google.common.collect.ImmutableListMultimap$Builder`

```java
public final class com.google.common.collect.ImmutableListMultimap$Builder<K, V> extends com.google.common.collect.ImmutableMultimap$Builder<K, V> {
  public com.google.common.collect.ImmutableListMultimap$Builder();
  public com.google.common.collect.ImmutableListMultimap$Builder<K, V> expectedValuesPerKey(int);
  public com.google.common.collect.ImmutableListMultimap$Builder<K, V> put(K, V);
  public com.google.common.collect.ImmutableListMultimap$Builder<K, V> put(java.util.Map$Entry<? extends K, ? extends V>);
  public com.google.common.collect.ImmutableListMultimap$Builder<K, V> putAll(java.lang.Iterable<? extends java.util.Map$Entry<? extends K, ? extends V>>);
  public com.google.common.collect.ImmutableListMultimap$Builder<K, V> putAll(K, java.lang.Iterable<? extends V>);
  public com.google.common.collect.ImmutableListMultimap$Builder<K, V> putAll(K, V...);
  public com.google.common.collect.ImmutableListMultimap$Builder<K, V> putAll(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public com.google.common.collect.ImmutableListMultimap$Builder<K, V> orderKeysBy(java.util.Comparator<? super K>);
  public com.google.common.collect.ImmutableListMultimap$Builder<K, V> orderValuesBy(java.util.Comparator<? super V>);
  public com.google.common.collect.ImmutableListMultimap<K, V> build();
  public com.google.common.collect.ImmutableMultimap build();
  public com.google.common.collect.ImmutableMultimap$Builder orderValuesBy(java.util.Comparator);
  public com.google.common.collect.ImmutableMultimap$Builder orderKeysBy(java.util.Comparator);
  public com.google.common.collect.ImmutableMultimap$Builder putAll(com.google.common.collect.Multimap);
  public com.google.common.collect.ImmutableMultimap$Builder putAll(java.lang.Object, java.lang.Object[]);
  public com.google.common.collect.ImmutableMultimap$Builder putAll(java.lang.Object, java.lang.Iterable);
  public com.google.common.collect.ImmutableMultimap$Builder putAll(java.lang.Iterable);
  public com.google.common.collect.ImmutableMultimap$Builder put(java.util.Map$Entry);
  public com.google.common.collect.ImmutableMultimap$Builder put(java.lang.Object, java.lang.Object);
  public com.google.common.collect.ImmutableMultimap$Builder expectedValuesPerKey(int);
}
```

## `com.google.common.collect.ImmutableMap`

```java
public abstract class com.google.common.collect.ImmutableMap<K, V> implements java.util.Map<K, V>, java.io.Serializable {
  public static <T, K, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableMap<K, V>> toImmutableMap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends V>);
  public static <T, K, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableMap<K, V>> toImmutableMap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends V>, java.util.function.BinaryOperator<V>);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> of();
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> of(K, V);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> of(K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> of(K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> of(K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> of(K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> ofEntries(java.util.Map$Entry<? extends K, ? extends V>...);
  public static <K, V> com.google.common.collect.ImmutableMap$Builder<K, V> builder();
  public static <K, V> com.google.common.collect.ImmutableMap$Builder<K, V> builderWithExpectedSize(int);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> copyOf(java.util.Map<? extends K, ? extends V>);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> copyOf(java.lang.Iterable<? extends java.util.Map$Entry<? extends K, ? extends V>>);
  public final V put(K, V);
  public final V putIfAbsent(K, V);
  public final boolean replace(K, V, V);
  public final V replace(K, V);
  public final V computeIfAbsent(K, java.util.function.Function<? super K, ? extends V>);
  public final V computeIfPresent(K, java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public final V compute(K, java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public final V merge(K, V, java.util.function.BiFunction<? super V, ? super V, ? extends V>);
  public final void putAll(java.util.Map<? extends K, ? extends V>);
  public final void replaceAll(java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public final V remove(java.lang.Object);
  public final boolean remove(java.lang.Object, java.lang.Object);
  public final void clear();
  public boolean isEmpty();
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public abstract V get(java.lang.Object);
  public final V getOrDefault(java.lang.Object, V);
  public com.google.common.collect.ImmutableSet<java.util.Map$Entry<K, V>> entrySet();
  public com.google.common.collect.ImmutableSet<K> keySet();
  public com.google.common.collect.ImmutableCollection<V> values();
  public com.google.common.collect.ImmutableSetMultimap<K, V> asMultimap();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public java.util.Set entrySet();
  public java.util.Collection values();
  public java.util.Set keySet();
}
```

## `com.google.common.collect.ImmutableMap$Builder`

```java
public class com.google.common.collect.ImmutableMap$Builder<K, V> {
  public com.google.common.collect.ImmutableMap$Builder();
  public com.google.common.collect.ImmutableMap$Builder<K, V> put(K, V);
  public com.google.common.collect.ImmutableMap$Builder<K, V> put(java.util.Map$Entry<? extends K, ? extends V>);
  public com.google.common.collect.ImmutableMap$Builder<K, V> putAll(java.util.Map<? extends K, ? extends V>);
  public com.google.common.collect.ImmutableMap$Builder<K, V> putAll(java.lang.Iterable<? extends java.util.Map$Entry<? extends K, ? extends V>>);
  public com.google.common.collect.ImmutableMap$Builder<K, V> orderEntriesByValue(java.util.Comparator<? super V>);
  public com.google.common.collect.ImmutableMap<K, V> build();
  public com.google.common.collect.ImmutableMap<K, V> buildOrThrow();
  public com.google.common.collect.ImmutableMap<K, V> buildKeepingLast();
}
```

## `com.google.common.collect.ImmutableMultimap`

```java
public abstract class com.google.common.collect.ImmutableMultimap<K, V> extends com.google.common.collect.BaseImmutableMultimap<K, V> implements java.io.Serializable {
  public static <K, V> com.google.common.collect.ImmutableMultimap<K, V> of();
  public static <K, V> com.google.common.collect.ImmutableMultimap<K, V> of(K, V);
  public static <K, V> com.google.common.collect.ImmutableMultimap<K, V> of(K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableMultimap<K, V> of(K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableMultimap<K, V> of(K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableMultimap<K, V> of(K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableMultimap$Builder<K, V> builder();
  public static <K, V> com.google.common.collect.ImmutableMultimap$Builder<K, V> builderWithExpectedKeys(int);
  public static <K, V> com.google.common.collect.ImmutableMultimap<K, V> copyOf(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public static <K, V> com.google.common.collect.ImmutableMultimap<K, V> copyOf(java.lang.Iterable<? extends java.util.Map$Entry<? extends K, ? extends V>>);
  public com.google.common.collect.ImmutableCollection<V> removeAll(java.lang.Object);
  public com.google.common.collect.ImmutableCollection<V> replaceValues(K, java.lang.Iterable<? extends V>);
  public final void clear();
  public abstract com.google.common.collect.ImmutableCollection<V> get(K);
  public abstract com.google.common.collect.ImmutableMultimap<V, K> inverse();
  public final boolean put(K, V);
  public final boolean putAll(K, java.lang.Iterable<? extends V>);
  public final boolean putAll(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public final boolean remove(java.lang.Object, java.lang.Object);
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public int size();
  public com.google.common.collect.ImmutableSet<K> keySet();
  public com.google.common.collect.ImmutableMap<K, java.util.Collection<V>> asMap();
  public com.google.common.collect.ImmutableCollection<java.util.Map$Entry<K, V>> entries();
  public void forEach(java.util.function.BiConsumer<? super K, ? super V>);
  public com.google.common.collect.ImmutableMultiset<K> keys();
  public com.google.common.collect.ImmutableCollection<V> values();
  public java.lang.String toString();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.util.Map asMap();
  public java.util.Collection values();
  public com.google.common.collect.Multiset keys();
  public java.util.Set keySet();
  public java.util.Collection entries();
  public java.util.Collection replaceValues(java.lang.Object, java.lang.Iterable);
  public boolean containsEntry(java.lang.Object, java.lang.Object);
  public boolean isEmpty();
  public java.util.Collection get(java.lang.Object);
  public java.util.Collection removeAll(java.lang.Object);
}
```

## `com.google.common.collect.ImmutableMultimap$Builder`

```java
public class com.google.common.collect.ImmutableMultimap$Builder<K, V> {
  public com.google.common.collect.ImmutableMultimap$Builder();
  public com.google.common.collect.ImmutableMultimap$Builder<K, V> expectedValuesPerKey(int);
  public com.google.common.collect.ImmutableMultimap$Builder<K, V> put(K, V);
  public com.google.common.collect.ImmutableMultimap$Builder<K, V> put(java.util.Map$Entry<? extends K, ? extends V>);
  public com.google.common.collect.ImmutableMultimap$Builder<K, V> putAll(java.lang.Iterable<? extends java.util.Map$Entry<? extends K, ? extends V>>);
  public com.google.common.collect.ImmutableMultimap$Builder<K, V> putAll(K, java.lang.Iterable<? extends V>);
  public com.google.common.collect.ImmutableMultimap$Builder<K, V> putAll(K, V...);
  public com.google.common.collect.ImmutableMultimap$Builder<K, V> putAll(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public com.google.common.collect.ImmutableMultimap$Builder<K, V> orderKeysBy(java.util.Comparator<? super K>);
  public com.google.common.collect.ImmutableMultimap$Builder<K, V> orderValuesBy(java.util.Comparator<? super V>);
  public com.google.common.collect.ImmutableMultimap<K, V> build();
}
```

## `com.google.common.collect.ImmutableMultiset`

```java
public abstract class com.google.common.collect.ImmutableMultiset<E> extends com.google.common.collect.ImmutableMultisetGwtSerializationDependencies<E> implements com.google.common.collect.Multiset<E> {
  public static <E> java.util.stream.Collector<E, ?, com.google.common.collect.ImmutableMultiset<E>> toImmutableMultiset();
  public static <T, E> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableMultiset<E>> toImmutableMultiset(java.util.function.Function<? super T, ? extends E>, java.util.function.ToIntFunction<? super T>);
  public static <E> com.google.common.collect.ImmutableMultiset<E> of();
  public static <E> com.google.common.collect.ImmutableMultiset<E> of(E);
  public static <E> com.google.common.collect.ImmutableMultiset<E> of(E, E);
  public static <E> com.google.common.collect.ImmutableMultiset<E> of(E, E, E);
  public static <E> com.google.common.collect.ImmutableMultiset<E> of(E, E, E, E);
  public static <E> com.google.common.collect.ImmutableMultiset<E> of(E, E, E, E, E);
  public static <E> com.google.common.collect.ImmutableMultiset<E> of(E, E, E, E, E, E, E...);
  public static <E> com.google.common.collect.ImmutableMultiset<E> copyOf(E[]);
  public static <E> com.google.common.collect.ImmutableMultiset<E> copyOf(java.lang.Iterable<? extends E>);
  public static <E> com.google.common.collect.ImmutableMultiset<E> copyOf(java.util.Iterator<? extends E>);
  public com.google.common.collect.UnmodifiableIterator<E> iterator();
  public com.google.common.collect.ImmutableList<E> asList();
  public boolean contains(java.lang.Object);
  public final int add(E, int);
  public final int remove(java.lang.Object, int);
  public final int setCount(E, int);
  public final boolean setCount(E, int, int);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public abstract com.google.common.collect.ImmutableSet<E> elementSet();
  public com.google.common.collect.ImmutableSet<com.google.common.collect.Multiset$Entry<E>> entrySet();
  public static <E> com.google.common.collect.ImmutableMultiset$Builder<E> builder();
  public java.util.Iterator iterator();
  public java.util.Set entrySet();
  public java.util.Set elementSet();
}
```

## `com.google.common.collect.ImmutableMultiset$Builder`

```java
public class com.google.common.collect.ImmutableMultiset$Builder<E> extends com.google.common.collect.ImmutableCollection$Builder<E> {
  public com.google.common.collect.ImmutableMultiset$Builder();
  public com.google.common.collect.ImmutableMultiset$Builder<E> add(E);
  public com.google.common.collect.ImmutableMultiset$Builder<E> add(E...);
  public com.google.common.collect.ImmutableMultiset$Builder<E> addCopies(E, int);
  public com.google.common.collect.ImmutableMultiset$Builder<E> setCount(E, int);
  public com.google.common.collect.ImmutableMultiset$Builder<E> addAll(java.lang.Iterable<? extends E>);
  public com.google.common.collect.ImmutableMultiset$Builder<E> addAll(java.util.Iterator<? extends E>);
  public com.google.common.collect.ImmutableMultiset<E> build();
  public com.google.common.collect.ImmutableCollection build();
  public com.google.common.collect.ImmutableCollection$Builder addAll(java.util.Iterator);
  public com.google.common.collect.ImmutableCollection$Builder addAll(java.lang.Iterable);
  public com.google.common.collect.ImmutableCollection$Builder add(java.lang.Object[]);
  public com.google.common.collect.ImmutableCollection$Builder add(java.lang.Object);
}
```

## `com.google.common.collect.ImmutableRangeMap`

```java
public class com.google.common.collect.ImmutableRangeMap<K extends java.lang.Comparable<?>, V> implements com.google.common.collect.RangeMap<K, V>, java.io.Serializable {
  public static <T, K extends java.lang.Comparable<? super K>, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableRangeMap<K, V>> toImmutableRangeMap(java.util.function.Function<? super T, com.google.common.collect.Range<K>>, java.util.function.Function<? super T, ? extends V>);
  public static <K extends java.lang.Comparable<?>, V> com.google.common.collect.ImmutableRangeMap<K, V> of();
  public static <K extends java.lang.Comparable<?>, V> com.google.common.collect.ImmutableRangeMap<K, V> of(com.google.common.collect.Range<K>, V);
  public static <K extends java.lang.Comparable<?>, V> com.google.common.collect.ImmutableRangeMap<K, V> copyOf(com.google.common.collect.RangeMap<K, ? extends V>);
  public static <K extends java.lang.Comparable<?>, V> com.google.common.collect.ImmutableRangeMap$Builder<K, V> builder();
  public V get(K);
  public java.util.Map$Entry<com.google.common.collect.Range<K>, V> getEntry(K);
  public com.google.common.collect.Range<K> span();
  public final void put(com.google.common.collect.Range<K>, V);
  public final void putCoalescing(com.google.common.collect.Range<K>, V);
  public final void putAll(com.google.common.collect.RangeMap<K, ? extends V>);
  public final void clear();
  public final void remove(com.google.common.collect.Range<K>);
  public final void merge(com.google.common.collect.Range<K>, V, java.util.function.BiFunction<? super V, ? super V, ? extends V>);
  public com.google.common.collect.ImmutableMap<com.google.common.collect.Range<K>, V> asMapOfRanges();
  public com.google.common.collect.ImmutableMap<com.google.common.collect.Range<K>, V> asDescendingMapOfRanges();
  public com.google.common.collect.ImmutableRangeMap<K, V> subRangeMap(com.google.common.collect.Range<K>);
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
  public com.google.common.collect.RangeMap subRangeMap(com.google.common.collect.Range);
  public java.util.Map asDescendingMapOfRanges();
  public java.util.Map asMapOfRanges();
}
```

## `com.google.common.collect.ImmutableRangeMap$Builder`

```java
public final class com.google.common.collect.ImmutableRangeMap$Builder<K extends java.lang.Comparable<?>, V> {
  public com.google.common.collect.ImmutableRangeMap$Builder();
  public com.google.common.collect.ImmutableRangeMap$Builder<K, V> put(com.google.common.collect.Range<K>, V);
  public com.google.common.collect.ImmutableRangeMap$Builder<K, V> putAll(com.google.common.collect.RangeMap<K, ? extends V>);
  public com.google.common.collect.ImmutableRangeMap<K, V> build();
}
```

## `com.google.common.collect.ImmutableRangeSet`

```java
public final class com.google.common.collect.ImmutableRangeSet<C extends java.lang.Comparable> extends com.google.common.collect.AbstractRangeSet<C> implements java.io.Serializable {
  public static <E extends java.lang.Comparable<? super E>> java.util.stream.Collector<com.google.common.collect.Range<E>, ?, com.google.common.collect.ImmutableRangeSet<E>> toImmutableRangeSet();
  public static <C extends java.lang.Comparable> com.google.common.collect.ImmutableRangeSet<C> of();
  public static <C extends java.lang.Comparable> com.google.common.collect.ImmutableRangeSet<C> of(com.google.common.collect.Range<C>);
  public static <C extends java.lang.Comparable> com.google.common.collect.ImmutableRangeSet<C> copyOf(com.google.common.collect.RangeSet<C>);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.ImmutableRangeSet<C> copyOf(java.lang.Iterable<com.google.common.collect.Range<C>>);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.ImmutableRangeSet<C> unionOf(java.lang.Iterable<com.google.common.collect.Range<C>>);
  public boolean intersects(com.google.common.collect.Range<C>);
  public boolean encloses(com.google.common.collect.Range<C>);
  public com.google.common.collect.Range<C> rangeContaining(C);
  public com.google.common.collect.Range<C> span();
  public boolean isEmpty();
  public void add(com.google.common.collect.Range<C>);
  public void addAll(com.google.common.collect.RangeSet<C>);
  public void addAll(java.lang.Iterable<com.google.common.collect.Range<C>>);
  public void remove(com.google.common.collect.Range<C>);
  public void removeAll(com.google.common.collect.RangeSet<C>);
  public void removeAll(java.lang.Iterable<com.google.common.collect.Range<C>>);
  public com.google.common.collect.ImmutableSet<com.google.common.collect.Range<C>> asRanges();
  public com.google.common.collect.ImmutableSet<com.google.common.collect.Range<C>> asDescendingSetOfRanges();
  public com.google.common.collect.ImmutableRangeSet<C> complement();
  public com.google.common.collect.ImmutableRangeSet<C> union(com.google.common.collect.RangeSet<C>);
  public com.google.common.collect.ImmutableRangeSet<C> intersection(com.google.common.collect.RangeSet<C>);
  public com.google.common.collect.ImmutableRangeSet<C> difference(com.google.common.collect.RangeSet<C>);
  public com.google.common.collect.ImmutableRangeSet<C> subRangeSet(com.google.common.collect.Range<C>);
  public com.google.common.collect.ImmutableSortedSet<C> asSet(com.google.common.collect.DiscreteDomain<C>);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.ImmutableRangeSet$Builder<C> builder();
  public boolean equals(java.lang.Object);
  public boolean enclosesAll(com.google.common.collect.RangeSet);
  public void clear();
  public boolean contains(java.lang.Comparable);
  public com.google.common.collect.RangeSet subRangeSet(com.google.common.collect.Range);
  public com.google.common.collect.RangeSet complement();
  public java.util.Set asDescendingSetOfRanges();
  public java.util.Set asRanges();
}
```

## `com.google.common.collect.ImmutableRangeSet$Builder`

```java
public class com.google.common.collect.ImmutableRangeSet$Builder<C extends java.lang.Comparable<?>> {
  public com.google.common.collect.ImmutableRangeSet$Builder();
  public com.google.common.collect.ImmutableRangeSet$Builder<C> add(com.google.common.collect.Range<C>);
  public com.google.common.collect.ImmutableRangeSet$Builder<C> addAll(com.google.common.collect.RangeSet<C>);
  public com.google.common.collect.ImmutableRangeSet$Builder<C> addAll(java.lang.Iterable<com.google.common.collect.Range<C>>);
  public com.google.common.collect.ImmutableRangeSet<C> build();
}
```

## `com.google.common.collect.ImmutableSet`

```java
public abstract class com.google.common.collect.ImmutableSet<E> extends com.google.common.collect.ImmutableCollection<E> implements java.util.Set<E> {
  public static <E> java.util.stream.Collector<E, ?, com.google.common.collect.ImmutableSet<E>> toImmutableSet();
  public static <E> com.google.common.collect.ImmutableSet<E> of();
  public static <E> com.google.common.collect.ImmutableSet<E> of(E);
  public static <E> com.google.common.collect.ImmutableSet<E> of(E, E);
  public static <E> com.google.common.collect.ImmutableSet<E> of(E, E, E);
  public static <E> com.google.common.collect.ImmutableSet<E> of(E, E, E, E);
  public static <E> com.google.common.collect.ImmutableSet<E> of(E, E, E, E, E);
  public static <E> com.google.common.collect.ImmutableSet<E> of(E, E, E, E, E, E, E...);
  public static <E> com.google.common.collect.ImmutableSet<E> copyOf(java.util.Collection<? extends E>);
  public static <E> com.google.common.collect.ImmutableSet<E> copyOf(java.lang.Iterable<? extends E>);
  public static <E> com.google.common.collect.ImmutableSet<E> copyOf(java.util.Iterator<? extends E>);
  public static <E> com.google.common.collect.ImmutableSet<E> copyOf(E[]);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public abstract com.google.common.collect.UnmodifiableIterator<E> iterator();
  public static <E> com.google.common.collect.ImmutableSet$Builder<E> builder();
  public static <E> com.google.common.collect.ImmutableSet$Builder<E> builderWithExpectedSize(int);
  public java.util.Iterator iterator();
}
```

## `com.google.common.collect.ImmutableSet$Builder`

```java
public class com.google.common.collect.ImmutableSet$Builder<E> extends com.google.common.collect.ImmutableCollection$Builder<E> {
  public com.google.common.collect.ImmutableSet$Builder();
  public com.google.common.collect.ImmutableSet$Builder<E> add(E);
  public com.google.common.collect.ImmutableSet$Builder<E> add(E...);
  public com.google.common.collect.ImmutableSet$Builder<E> addAll(java.lang.Iterable<? extends E>);
  public com.google.common.collect.ImmutableSet$Builder<E> addAll(java.util.Iterator<? extends E>);
  public com.google.common.collect.ImmutableSet<E> build();
  public com.google.common.collect.ImmutableCollection build();
  public com.google.common.collect.ImmutableCollection$Builder addAll(java.util.Iterator);
  public com.google.common.collect.ImmutableCollection$Builder addAll(java.lang.Iterable);
  public com.google.common.collect.ImmutableCollection$Builder add(java.lang.Object[]);
  public com.google.common.collect.ImmutableCollection$Builder add(java.lang.Object);
}
```

## `com.google.common.collect.ImmutableSetMultimap`

```java
public class com.google.common.collect.ImmutableSetMultimap<K, V> extends com.google.common.collect.ImmutableMultimap<K, V> implements com.google.common.collect.SetMultimap<K, V> {
  public static <T, K, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableSetMultimap<K, V>> toImmutableSetMultimap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends V>);
  public static <T, K, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableSetMultimap<K, V>> flatteningToImmutableSetMultimap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends java.util.stream.Stream<? extends V>>);
  public static <K, V> com.google.common.collect.ImmutableSetMultimap<K, V> of();
  public static <K, V> com.google.common.collect.ImmutableSetMultimap<K, V> of(K, V);
  public static <K, V> com.google.common.collect.ImmutableSetMultimap<K, V> of(K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableSetMultimap<K, V> of(K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableSetMultimap<K, V> of(K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableSetMultimap<K, V> of(K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableSetMultimap$Builder<K, V> builder();
  public static <K, V> com.google.common.collect.ImmutableSetMultimap$Builder<K, V> builderWithExpectedKeys(int);
  public static <K, V> com.google.common.collect.ImmutableSetMultimap<K, V> copyOf(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public static <K, V> com.google.common.collect.ImmutableSetMultimap<K, V> copyOf(java.lang.Iterable<? extends java.util.Map$Entry<? extends K, ? extends V>>);
  public com.google.common.collect.ImmutableSet<V> get(K);
  public com.google.common.collect.ImmutableSetMultimap<V, K> inverse();
  public final com.google.common.collect.ImmutableSet<V> removeAll(java.lang.Object);
  public final com.google.common.collect.ImmutableSet<V> replaceValues(K, java.lang.Iterable<? extends V>);
  public com.google.common.collect.ImmutableSet<java.util.Map$Entry<K, V>> entries();
  public com.google.common.collect.ImmutableCollection entries();
  public com.google.common.collect.ImmutableMultimap inverse();
  public com.google.common.collect.ImmutableCollection get(java.lang.Object);
  public com.google.common.collect.ImmutableCollection replaceValues(java.lang.Object, java.lang.Iterable);
  public com.google.common.collect.ImmutableCollection removeAll(java.lang.Object);
  public java.util.Collection entries();
  public java.util.Collection replaceValues(java.lang.Object, java.lang.Iterable);
  public java.util.Collection get(java.lang.Object);
  public java.util.Collection removeAll(java.lang.Object);
  public java.util.Set entries();
  public java.util.Set replaceValues(java.lang.Object, java.lang.Iterable);
  public java.util.Set removeAll(java.lang.Object);
  public java.util.Set get(java.lang.Object);
}
```

## `com.google.common.collect.ImmutableSetMultimap$Builder`

```java
public final class com.google.common.collect.ImmutableSetMultimap$Builder<K, V> extends com.google.common.collect.ImmutableMultimap$Builder<K, V> {
  public com.google.common.collect.ImmutableSetMultimap$Builder();
  public com.google.common.collect.ImmutableSetMultimap$Builder<K, V> expectedValuesPerKey(int);
  public com.google.common.collect.ImmutableSetMultimap$Builder<K, V> put(K, V);
  public com.google.common.collect.ImmutableSetMultimap$Builder<K, V> put(java.util.Map$Entry<? extends K, ? extends V>);
  public com.google.common.collect.ImmutableSetMultimap$Builder<K, V> putAll(java.lang.Iterable<? extends java.util.Map$Entry<? extends K, ? extends V>>);
  public com.google.common.collect.ImmutableSetMultimap$Builder<K, V> putAll(K, java.lang.Iterable<? extends V>);
  public com.google.common.collect.ImmutableSetMultimap$Builder<K, V> putAll(K, V...);
  public com.google.common.collect.ImmutableSetMultimap$Builder<K, V> putAll(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public com.google.common.collect.ImmutableSetMultimap$Builder<K, V> orderKeysBy(java.util.Comparator<? super K>);
  public com.google.common.collect.ImmutableSetMultimap$Builder<K, V> orderValuesBy(java.util.Comparator<? super V>);
  public com.google.common.collect.ImmutableSetMultimap<K, V> build();
  public com.google.common.collect.ImmutableMultimap build();
  public com.google.common.collect.ImmutableMultimap$Builder orderValuesBy(java.util.Comparator);
  public com.google.common.collect.ImmutableMultimap$Builder orderKeysBy(java.util.Comparator);
  public com.google.common.collect.ImmutableMultimap$Builder putAll(com.google.common.collect.Multimap);
  public com.google.common.collect.ImmutableMultimap$Builder putAll(java.lang.Object, java.lang.Object[]);
  public com.google.common.collect.ImmutableMultimap$Builder putAll(java.lang.Object, java.lang.Iterable);
  public com.google.common.collect.ImmutableMultimap$Builder putAll(java.lang.Iterable);
  public com.google.common.collect.ImmutableMultimap$Builder put(java.util.Map$Entry);
  public com.google.common.collect.ImmutableMultimap$Builder put(java.lang.Object, java.lang.Object);
  public com.google.common.collect.ImmutableMultimap$Builder expectedValuesPerKey(int);
}
```

## `com.google.common.collect.ImmutableSortedMap`

```java
public final class com.google.common.collect.ImmutableSortedMap<K, V> extends com.google.common.collect.ImmutableMap<K, V> implements java.util.NavigableMap<K, V> {
  public static <T, K, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableSortedMap<K, V>> toImmutableSortedMap(java.util.Comparator<? super K>, java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends V>);
  public static <T, K, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableSortedMap<K, V>> toImmutableSortedMap(java.util.Comparator<? super K>, java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends V>, java.util.function.BinaryOperator<V>);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> of();
  public static <K extends java.lang.Comparable<? super K>, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V);
  public static <K extends java.lang.Comparable<? super K>, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V);
  public static <K extends java.lang.Comparable<? super K>, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V);
  public static <K extends java.lang.Comparable<? super K>, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V, K, V);
  public static <K extends java.lang.Comparable<? super K>, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V, K, V, K, V);
  public static <K extends java.lang.Comparable<? super K>, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K extends java.lang.Comparable<? super K>, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K extends java.lang.Comparable<? super K>, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K extends java.lang.Comparable<? super K>, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K extends java.lang.Comparable<? super K>, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> copyOf(java.util.Map<? extends K, ? extends V>);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> copyOf(java.util.Map<? extends K, ? extends V>, java.util.Comparator<? super K>);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> copyOf(java.lang.Iterable<? extends java.util.Map$Entry<? extends K, ? extends V>>);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> copyOf(java.lang.Iterable<? extends java.util.Map$Entry<? extends K, ? extends V>>, java.util.Comparator<? super K>);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> copyOfSorted(java.util.SortedMap<K, ? extends V>);
  public static <K extends java.lang.Comparable<?>, V> com.google.common.collect.ImmutableSortedMap$Builder<K, V> naturalOrder();
  public static <K, V> com.google.common.collect.ImmutableSortedMap$Builder<K, V> orderedBy(java.util.Comparator<K>);
  public static <K extends java.lang.Comparable<?>, V> com.google.common.collect.ImmutableSortedMap$Builder<K, V> reverseOrder();
  public int size();
  public void forEach(java.util.function.BiConsumer<? super K, ? super V>);
  public V get(java.lang.Object);
  public com.google.common.collect.ImmutableSet<java.util.Map$Entry<K, V>> entrySet();
  public com.google.common.collect.ImmutableSortedSet<K> keySet();
  public com.google.common.collect.ImmutableCollection<V> values();
  public java.util.Comparator<? super K> comparator();
  public K firstKey();
  public K lastKey();
  public com.google.common.collect.ImmutableSortedMap<K, V> headMap(K);
  public com.google.common.collect.ImmutableSortedMap<K, V> headMap(K, boolean);
  public com.google.common.collect.ImmutableSortedMap<K, V> subMap(K, K);
  public com.google.common.collect.ImmutableSortedMap<K, V> subMap(K, boolean, K, boolean);
  public com.google.common.collect.ImmutableSortedMap<K, V> tailMap(K);
  public com.google.common.collect.ImmutableSortedMap<K, V> tailMap(K, boolean);
  public java.util.Map$Entry<K, V> lowerEntry(K);
  public K lowerKey(K);
  public java.util.Map$Entry<K, V> floorEntry(K);
  public K floorKey(K);
  public java.util.Map$Entry<K, V> ceilingEntry(K);
  public K ceilingKey(K);
  public java.util.Map$Entry<K, V> higherEntry(K);
  public K higherKey(K);
  public java.util.Map$Entry<K, V> firstEntry();
  public java.util.Map$Entry<K, V> lastEntry();
  public final java.util.Map$Entry<K, V> pollFirstEntry();
  public final java.util.Map$Entry<K, V> pollLastEntry();
  public com.google.common.collect.ImmutableSortedMap<K, V> descendingMap();
  public com.google.common.collect.ImmutableSortedSet<K> navigableKeySet();
  public com.google.common.collect.ImmutableSortedSet<K> descendingKeySet();
  public static <T, K, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableMap<K, V>> toImmutableMap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends V>);
  public static <T, K, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableMap<K, V>> toImmutableMap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends V>, java.util.function.BinaryOperator<V>);
  public static <K, V> com.google.common.collect.ImmutableSortedMap$Builder<K, V> builder();
  public static <K, V> com.google.common.collect.ImmutableSortedMap$Builder<K, V> builderWithExpectedSize(int);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> of(K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V, K, V);
  public static <K, V> com.google.common.collect.ImmutableSortedMap<K, V> ofEntries(java.util.Map$Entry<? extends K, ? extends V>...);
  public com.google.common.collect.ImmutableSet keySet();
  public java.util.Set entrySet();
  public java.util.Collection values();
  public java.util.Set keySet();
  public java.util.SortedMap tailMap(java.lang.Object);
  public java.util.SortedMap headMap(java.lang.Object);
  public java.util.SortedMap subMap(java.lang.Object, java.lang.Object);
  public java.util.NavigableMap tailMap(java.lang.Object, boolean);
  public java.util.NavigableMap headMap(java.lang.Object, boolean);
  public java.util.NavigableMap subMap(java.lang.Object, boolean, java.lang.Object, boolean);
  public java.util.NavigableSet descendingKeySet();
  public java.util.NavigableSet navigableKeySet();
  public java.util.NavigableMap descendingMap();
}
```

## `com.google.common.collect.ImmutableSortedMap$Builder`

```java
public class com.google.common.collect.ImmutableSortedMap$Builder<K, V> extends com.google.common.collect.ImmutableMap$Builder<K, V> {
  public com.google.common.collect.ImmutableSortedMap$Builder(java.util.Comparator<? super K>);
  public com.google.common.collect.ImmutableSortedMap$Builder<K, V> put(K, V);
  public com.google.common.collect.ImmutableSortedMap$Builder<K, V> put(java.util.Map$Entry<? extends K, ? extends V>);
  public com.google.common.collect.ImmutableSortedMap$Builder<K, V> putAll(java.util.Map<? extends K, ? extends V>);
  public com.google.common.collect.ImmutableSortedMap$Builder<K, V> putAll(java.lang.Iterable<? extends java.util.Map$Entry<? extends K, ? extends V>>);
  public final com.google.common.collect.ImmutableSortedMap$Builder<K, V> orderEntriesByValue(java.util.Comparator<? super V>);
  public com.google.common.collect.ImmutableSortedMap<K, V> build();
  public com.google.common.collect.ImmutableSortedMap<K, V> buildOrThrow();
  public final com.google.common.collect.ImmutableSortedMap<K, V> buildKeepingLast();
  public com.google.common.collect.ImmutableMap buildKeepingLast();
  public com.google.common.collect.ImmutableMap buildOrThrow();
  public com.google.common.collect.ImmutableMap build();
  public com.google.common.collect.ImmutableMap$Builder orderEntriesByValue(java.util.Comparator);
  public com.google.common.collect.ImmutableMap$Builder putAll(java.lang.Iterable);
  public com.google.common.collect.ImmutableMap$Builder putAll(java.util.Map);
  public com.google.common.collect.ImmutableMap$Builder put(java.util.Map$Entry);
  public com.google.common.collect.ImmutableMap$Builder put(java.lang.Object, java.lang.Object);
}
```

## `com.google.common.collect.ImmutableSortedMultiset`

```java
public abstract class com.google.common.collect.ImmutableSortedMultiset<E> extends com.google.common.collect.ImmutableMultiset<E> implements com.google.common.collect.SortedMultiset<E> {
  public static <E> java.util.stream.Collector<E, ?, com.google.common.collect.ImmutableSortedMultiset<E>> toImmutableSortedMultiset(java.util.Comparator<? super E>);
  public static <T, E> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableSortedMultiset<E>> toImmutableSortedMultiset(java.util.Comparator<? super E>, java.util.function.Function<? super T, ? extends E>, java.util.function.ToIntFunction<? super T>);
  public static <E> com.google.common.collect.ImmutableSortedMultiset<E> of();
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableSortedMultiset<E> of(E);
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableSortedMultiset<E> of(E, E);
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableSortedMultiset<E> of(E, E, E);
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableSortedMultiset<E> of(E, E, E, E);
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableSortedMultiset<E> of(E, E, E, E, E);
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableSortedMultiset<E> of(E, E, E, E, E, E, E...);
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableSortedMultiset<E> copyOf(E[]);
  public static <E> com.google.common.collect.ImmutableSortedMultiset<E> copyOf(java.lang.Iterable<? extends E>);
  public static <E> com.google.common.collect.ImmutableSortedMultiset<E> copyOf(java.util.Iterator<? extends E>);
  public static <E> com.google.common.collect.ImmutableSortedMultiset<E> copyOf(java.util.Comparator<? super E>, java.util.Iterator<? extends E>);
  public static <E> com.google.common.collect.ImmutableSortedMultiset<E> copyOf(java.util.Comparator<? super E>, java.lang.Iterable<? extends E>);
  public static <E> com.google.common.collect.ImmutableSortedMultiset<E> copyOfSorted(com.google.common.collect.SortedMultiset<E>);
  public final java.util.Comparator<? super E> comparator();
  public abstract com.google.common.collect.ImmutableSortedSet<E> elementSet();
  public com.google.common.collect.ImmutableSortedMultiset<E> descendingMultiset();
  public final com.google.common.collect.Multiset$Entry<E> pollFirstEntry();
  public final com.google.common.collect.Multiset$Entry<E> pollLastEntry();
  public abstract com.google.common.collect.ImmutableSortedMultiset<E> headMultiset(E, com.google.common.collect.BoundType);
  public com.google.common.collect.ImmutableSortedMultiset<E> subMultiset(E, com.google.common.collect.BoundType, E, com.google.common.collect.BoundType);
  public abstract com.google.common.collect.ImmutableSortedMultiset<E> tailMultiset(E, com.google.common.collect.BoundType);
  public static <E> com.google.common.collect.ImmutableSortedMultiset$Builder<E> orderedBy(java.util.Comparator<E>);
  public static <E extends java.lang.Comparable<?>> com.google.common.collect.ImmutableSortedMultiset$Builder<E> reverseOrder();
  public static <E extends java.lang.Comparable<?>> com.google.common.collect.ImmutableSortedMultiset$Builder<E> naturalOrder();
  public static <E> java.util.stream.Collector<E, ?, com.google.common.collect.ImmutableMultiset<E>> toImmutableMultiset();
  public static <T, E> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableMultiset<E>> toImmutableMultiset(java.util.function.Function<? super T, ? extends E>, java.util.function.ToIntFunction<? super T>);
  public static <E> com.google.common.collect.ImmutableSortedMultiset$Builder<E> builder();
  public static <E> com.google.common.collect.ImmutableSortedMultiset<E> of(E);
  public static <E> com.google.common.collect.ImmutableSortedMultiset<E> of(E, E);
  public static <E> com.google.common.collect.ImmutableSortedMultiset<E> of(E, E, E);
  public static <E> com.google.common.collect.ImmutableSortedMultiset<E> of(E, E, E, E);
  public static <E> com.google.common.collect.ImmutableSortedMultiset<E> of(E, E, E, E, E);
  public static <E> com.google.common.collect.ImmutableSortedMultiset<E> of(E, E, E, E, E, E, E...);
  public static <Z> com.google.common.collect.ImmutableSortedMultiset<Z> copyOf(Z[]);
  public com.google.common.collect.ImmutableSet elementSet();
  public java.util.Set elementSet();
  public com.google.common.collect.SortedMultiset tailMultiset(java.lang.Object, com.google.common.collect.BoundType);
  public com.google.common.collect.SortedMultiset subMultiset(java.lang.Object, com.google.common.collect.BoundType, java.lang.Object, com.google.common.collect.BoundType);
  public com.google.common.collect.SortedMultiset headMultiset(java.lang.Object, com.google.common.collect.BoundType);
  public com.google.common.collect.SortedMultiset descendingMultiset();
  public java.util.NavigableSet elementSet();
  public java.util.SortedSet elementSet();
}
```

## `com.google.common.collect.ImmutableSortedMultiset$Builder`

```java
public class com.google.common.collect.ImmutableSortedMultiset$Builder<E> extends com.google.common.collect.ImmutableMultiset$Builder<E> {
  public com.google.common.collect.ImmutableSortedMultiset$Builder(java.util.Comparator<? super E>);
  public com.google.common.collect.ImmutableSortedMultiset$Builder<E> add(E);
  public com.google.common.collect.ImmutableSortedMultiset$Builder<E> add(E...);
  public com.google.common.collect.ImmutableSortedMultiset$Builder<E> addCopies(E, int);
  public com.google.common.collect.ImmutableSortedMultiset$Builder<E> setCount(E, int);
  public com.google.common.collect.ImmutableSortedMultiset$Builder<E> addAll(java.lang.Iterable<? extends E>);
  public com.google.common.collect.ImmutableSortedMultiset$Builder<E> addAll(java.util.Iterator<? extends E>);
  public com.google.common.collect.ImmutableSortedMultiset<E> build();
  public com.google.common.collect.ImmutableMultiset build();
  public com.google.common.collect.ImmutableMultiset$Builder addAll(java.util.Iterator);
  public com.google.common.collect.ImmutableMultiset$Builder addAll(java.lang.Iterable);
  public com.google.common.collect.ImmutableMultiset$Builder setCount(java.lang.Object, int);
  public com.google.common.collect.ImmutableMultiset$Builder addCopies(java.lang.Object, int);
  public com.google.common.collect.ImmutableMultiset$Builder add(java.lang.Object[]);
  public com.google.common.collect.ImmutableMultiset$Builder add(java.lang.Object);
  public com.google.common.collect.ImmutableCollection build();
  public com.google.common.collect.ImmutableCollection$Builder addAll(java.util.Iterator);
  public com.google.common.collect.ImmutableCollection$Builder addAll(java.lang.Iterable);
  public com.google.common.collect.ImmutableCollection$Builder add(java.lang.Object[]);
  public com.google.common.collect.ImmutableCollection$Builder add(java.lang.Object);
}
```

## `com.google.common.collect.ImmutableSortedSet`

```java
public abstract class com.google.common.collect.ImmutableSortedSet<E> extends com.google.common.collect.ImmutableSet$CachingAsList<E> implements java.util.NavigableSet<E>, com.google.common.collect.SortedIterable<E> {
  public static <E> java.util.stream.Collector<E, ?, com.google.common.collect.ImmutableSortedSet<E>> toImmutableSortedSet(java.util.Comparator<? super E>);
  public static <E> com.google.common.collect.ImmutableSortedSet<E> of();
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableSortedSet<E> of(E);
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableSortedSet<E> of(E, E);
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableSortedSet<E> of(E, E, E);
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableSortedSet<E> of(E, E, E, E);
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableSortedSet<E> of(E, E, E, E, E);
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableSortedSet<E> of(E, E, E, E, E, E, E...);
  public static <E extends java.lang.Comparable<? super E>> com.google.common.collect.ImmutableSortedSet<E> copyOf(E[]);
  public static <E> com.google.common.collect.ImmutableSortedSet<E> copyOf(java.lang.Iterable<? extends E>);
  public static <E> com.google.common.collect.ImmutableSortedSet<E> copyOf(java.util.Collection<? extends E>);
  public static <E> com.google.common.collect.ImmutableSortedSet<E> copyOf(java.util.Iterator<? extends E>);
  public static <E> com.google.common.collect.ImmutableSortedSet<E> copyOf(java.util.Comparator<? super E>, java.util.Iterator<? extends E>);
  public static <E> com.google.common.collect.ImmutableSortedSet<E> copyOf(java.util.Comparator<? super E>, java.lang.Iterable<? extends E>);
  public static <E> com.google.common.collect.ImmutableSortedSet<E> copyOf(java.util.Comparator<? super E>, java.util.Collection<? extends E>);
  public static <E> com.google.common.collect.ImmutableSortedSet<E> copyOfSorted(java.util.SortedSet<E>);
  public static <E> com.google.common.collect.ImmutableSortedSet$Builder<E> orderedBy(java.util.Comparator<E>);
  public static <E extends java.lang.Comparable<?>> com.google.common.collect.ImmutableSortedSet$Builder<E> reverseOrder();
  public static <E extends java.lang.Comparable<?>> com.google.common.collect.ImmutableSortedSet$Builder<E> naturalOrder();
  public java.util.Comparator<? super E> comparator();
  public abstract com.google.common.collect.UnmodifiableIterator<E> iterator();
  public com.google.common.collect.ImmutableSortedSet<E> headSet(E);
  public com.google.common.collect.ImmutableSortedSet<E> headSet(E, boolean);
  public com.google.common.collect.ImmutableSortedSet<E> subSet(E, E);
  public com.google.common.collect.ImmutableSortedSet<E> subSet(E, boolean, E, boolean);
  public com.google.common.collect.ImmutableSortedSet<E> tailSet(E);
  public com.google.common.collect.ImmutableSortedSet<E> tailSet(E, boolean);
  public E lower(E);
  public E floor(E);
  public E ceiling(E);
  public E higher(E);
  public E first();
  public E last();
  public final E pollFirst();
  public final E pollLast();
  public com.google.common.collect.ImmutableSortedSet<E> descendingSet();
  public java.util.Spliterator<E> spliterator();
  public abstract com.google.common.collect.UnmodifiableIterator<E> descendingIterator();
  public static <E> java.util.stream.Collector<E, ?, com.google.common.collect.ImmutableSet<E>> toImmutableSet();
  public static <E> com.google.common.collect.ImmutableSortedSet$Builder<E> builder();
  public static <E> com.google.common.collect.ImmutableSortedSet$Builder<E> builderWithExpectedSize(int);
  public static <E> com.google.common.collect.ImmutableSortedSet<E> of(E);
  public static <E> com.google.common.collect.ImmutableSortedSet<E> of(E, E);
  public static <E> com.google.common.collect.ImmutableSortedSet<E> of(E, E, E);
  public static <E> com.google.common.collect.ImmutableSortedSet<E> of(E, E, E, E);
  public static <E> com.google.common.collect.ImmutableSortedSet<E> of(E, E, E, E, E);
  public static <E> com.google.common.collect.ImmutableSortedSet<E> of(E, E, E, E, E, E, E...);
  public static <Z> com.google.common.collect.ImmutableSortedSet<Z> copyOf(Z[]);
  public com.google.common.collect.ImmutableList asList();
  public java.util.Iterator iterator();
  public java.util.SortedSet tailSet(java.lang.Object);
  public java.util.SortedSet headSet(java.lang.Object);
  public java.util.SortedSet subSet(java.lang.Object, java.lang.Object);
  public java.util.NavigableSet tailSet(java.lang.Object, boolean);
  public java.util.NavigableSet headSet(java.lang.Object, boolean);
  public java.util.NavigableSet subSet(java.lang.Object, boolean, java.lang.Object, boolean);
  public java.util.Iterator descendingIterator();
  public java.util.NavigableSet descendingSet();
}
```

## `com.google.common.collect.ImmutableSortedSet$Builder`

```java
public final class com.google.common.collect.ImmutableSortedSet$Builder<E> extends com.google.common.collect.ImmutableSet$Builder<E> {
  public com.google.common.collect.ImmutableSortedSet$Builder(java.util.Comparator<? super E>);
  public com.google.common.collect.ImmutableSortedSet$Builder<E> add(E);
  public com.google.common.collect.ImmutableSortedSet$Builder<E> add(E...);
  public com.google.common.collect.ImmutableSortedSet$Builder<E> addAll(java.lang.Iterable<? extends E>);
  public com.google.common.collect.ImmutableSortedSet$Builder<E> addAll(java.util.Iterator<? extends E>);
  public com.google.common.collect.ImmutableSortedSet<E> build();
  public com.google.common.collect.ImmutableSet build();
  public com.google.common.collect.ImmutableSet$Builder addAll(java.util.Iterator);
  public com.google.common.collect.ImmutableSet$Builder addAll(java.lang.Iterable);
  public com.google.common.collect.ImmutableSet$Builder add(java.lang.Object[]);
  public com.google.common.collect.ImmutableSet$Builder add(java.lang.Object);
  public com.google.common.collect.ImmutableCollection build();
  public com.google.common.collect.ImmutableCollection$Builder addAll(java.util.Iterator);
  public com.google.common.collect.ImmutableCollection$Builder addAll(java.lang.Iterable);
  public com.google.common.collect.ImmutableCollection$Builder add(java.lang.Object[]);
  public com.google.common.collect.ImmutableCollection$Builder add(java.lang.Object);
}
```

## `com.google.common.collect.ImmutableTable`

```java
public abstract class com.google.common.collect.ImmutableTable<R, C, V> extends com.google.common.collect.AbstractTable<R, C, V> implements java.io.Serializable {
  public static <T, R, C, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableTable<R, C, V>> toImmutableTable(java.util.function.Function<? super T, ? extends R>, java.util.function.Function<? super T, ? extends C>, java.util.function.Function<? super T, ? extends V>);
  public static <T, R, C, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableTable<R, C, V>> toImmutableTable(java.util.function.Function<? super T, ? extends R>, java.util.function.Function<? super T, ? extends C>, java.util.function.Function<? super T, ? extends V>, java.util.function.BinaryOperator<V>);
  public static <R, C, V> com.google.common.collect.ImmutableTable<R, C, V> of();
  public static <R, C, V> com.google.common.collect.ImmutableTable<R, C, V> of(R, C, V);
  public static <R, C, V> com.google.common.collect.ImmutableTable<R, C, V> copyOf(com.google.common.collect.Table<? extends R, ? extends C, ? extends V>);
  public static <R, C, V> com.google.common.collect.ImmutableTable$Builder<R, C, V> builder();
  public com.google.common.collect.ImmutableSet<com.google.common.collect.Table$Cell<R, C, V>> cellSet();
  public com.google.common.collect.ImmutableCollection<V> values();
  public com.google.common.collect.ImmutableMap<R, V> column(C);
  public com.google.common.collect.ImmutableSet<C> columnKeySet();
  public abstract com.google.common.collect.ImmutableMap<C, java.util.Map<R, V>> columnMap();
  public com.google.common.collect.ImmutableMap<C, V> row(R);
  public com.google.common.collect.ImmutableSet<R> rowKeySet();
  public abstract com.google.common.collect.ImmutableMap<R, java.util.Map<C, V>> rowMap();
  public boolean contains(java.lang.Object, java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public final void clear();
  public final V put(R, C, V);
  public final void putAll(com.google.common.collect.Table<? extends R, ? extends C, ? extends V>);
  public final V remove(java.lang.Object, java.lang.Object);
  public java.lang.String toString();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.util.Collection values();
  public java.util.Set cellSet();
  public boolean isEmpty();
  public java.lang.Object get(java.lang.Object, java.lang.Object);
  public java.util.Set columnKeySet();
  public java.util.Set rowKeySet();
  public boolean containsColumn(java.lang.Object);
  public boolean containsRow(java.lang.Object);
  public java.util.Map columnMap();
  public java.util.Map rowMap();
  public java.util.Map column(java.lang.Object);
  public java.util.Map row(java.lang.Object);
}
```

## `com.google.common.collect.ImmutableTable$Builder`

```java
public final class com.google.common.collect.ImmutableTable$Builder<R, C, V> {
  public com.google.common.collect.ImmutableTable$Builder();
  public com.google.common.collect.ImmutableTable$Builder<R, C, V> orderRowsBy(java.util.Comparator<? super R>);
  public com.google.common.collect.ImmutableTable$Builder<R, C, V> orderColumnsBy(java.util.Comparator<? super C>);
  public com.google.common.collect.ImmutableTable$Builder<R, C, V> put(R, C, V);
  public com.google.common.collect.ImmutableTable$Builder<R, C, V> put(com.google.common.collect.Table$Cell<? extends R, ? extends C, ? extends V>);
  public com.google.common.collect.ImmutableTable$Builder<R, C, V> putAll(com.google.common.collect.Table<? extends R, ? extends C, ? extends V>);
  public com.google.common.collect.ImmutableTable<R, C, V> build();
  public com.google.common.collect.ImmutableTable<R, C, V> buildOrThrow();
}
```

## `com.google.common.collect.Interner`

```java
public interface com.google.common.collect.Interner<E> {
  public abstract E intern(E);
}
```

## `com.google.common.collect.Interners`

```java
public final class com.google.common.collect.Interners {
  public static com.google.common.collect.Interners$InternerBuilder newBuilder();
  public static <E> com.google.common.collect.Interner<E> newStrongInterner();
  public static <E> com.google.common.collect.Interner<E> newWeakInterner();
  public static <E> com.google.common.base.Function<E, E> asFunction(com.google.common.collect.Interner<E>);
}
```

## `com.google.common.collect.Interners$InternerBuilder`

```java
public class com.google.common.collect.Interners$InternerBuilder {
  public com.google.common.collect.Interners$InternerBuilder strong();
  public com.google.common.collect.Interners$InternerBuilder weak();
  public com.google.common.collect.Interners$InternerBuilder concurrencyLevel(int);
  public <E> com.google.common.collect.Interner<E> build();
}
```

## `com.google.common.collect.Iterables`

```java
public final class com.google.common.collect.Iterables {
  public static <T> java.lang.Iterable<T> unmodifiableIterable(java.lang.Iterable<? extends T>);
  public static <E> java.lang.Iterable<E> unmodifiableIterable(com.google.common.collect.ImmutableCollection<E>);
  public static int size(java.lang.Iterable<?>);
  public static boolean contains(java.lang.Iterable<?>, java.lang.Object);
  public static boolean removeAll(java.lang.Iterable<?>, java.util.Collection<?>);
  public static boolean retainAll(java.lang.Iterable<?>, java.util.Collection<?>);
  public static <T> boolean removeIf(java.lang.Iterable<T>, com.google.common.base.Predicate<? super T>);
  public static boolean elementsEqual(java.lang.Iterable<?>, java.lang.Iterable<?>);
  public static java.lang.String toString(java.lang.Iterable<?>);
  public static <T> T getOnlyElement(java.lang.Iterable<T>);
  public static <T> T getOnlyElement(java.lang.Iterable<? extends T>, T);
  public static <T> T[] toArray(java.lang.Iterable<? extends T>, java.lang.Class<T>);
  public static <T> boolean addAll(java.util.Collection<T>, java.lang.Iterable<? extends T>);
  public static int frequency(java.lang.Iterable<?>, java.lang.Object);
  public static <T> java.lang.Iterable<T> cycle(java.lang.Iterable<T>);
  public static <T> java.lang.Iterable<T> cycle(T...);
  public static <T> java.lang.Iterable<T> concat(java.lang.Iterable<? extends T>, java.lang.Iterable<? extends T>);
  public static <T> java.lang.Iterable<T> concat(java.lang.Iterable<? extends T>, java.lang.Iterable<? extends T>, java.lang.Iterable<? extends T>);
  public static <T> java.lang.Iterable<T> concat(java.lang.Iterable<? extends T>, java.lang.Iterable<? extends T>, java.lang.Iterable<? extends T>, java.lang.Iterable<? extends T>);
  public static <T> java.lang.Iterable<T> concat(java.lang.Iterable<? extends T>...);
  public static <T> java.lang.Iterable<T> concat(java.lang.Iterable<? extends java.lang.Iterable<? extends T>>);
  public static <T> java.lang.Iterable<java.util.List<T>> partition(java.lang.Iterable<T>, int);
  public static <T> java.lang.Iterable<java.util.List<T>> paddedPartition(java.lang.Iterable<T>, int);
  public static <T> java.lang.Iterable<T> filter(java.lang.Iterable<T>, com.google.common.base.Predicate<? super T>);
  public static <T> java.lang.Iterable<T> filter(java.lang.Iterable<?>, java.lang.Class<T>);
  public static <T> boolean any(java.lang.Iterable<T>, com.google.common.base.Predicate<? super T>);
  public static <T> boolean all(java.lang.Iterable<T>, com.google.common.base.Predicate<? super T>);
  public static <T> T find(java.lang.Iterable<T>, com.google.common.base.Predicate<? super T>);
  public static <T> T find(java.lang.Iterable<? extends T>, com.google.common.base.Predicate<? super T>, T);
  public static <T> com.google.common.base.Optional<T> tryFind(java.lang.Iterable<T>, com.google.common.base.Predicate<? super T>);
  public static <T> int indexOf(java.lang.Iterable<T>, com.google.common.base.Predicate<? super T>);
  public static <F, T> java.lang.Iterable<T> transform(java.lang.Iterable<F>, com.google.common.base.Function<? super F, ? extends T>);
  public static <T> T get(java.lang.Iterable<T>, int);
  public static <T> T get(java.lang.Iterable<? extends T>, int, T);
  public static <T> T getFirst(java.lang.Iterable<? extends T>, T);
  public static <T> T getLast(java.lang.Iterable<T>);
  public static <T> T getLast(java.lang.Iterable<? extends T>, T);
  public static <T> java.lang.Iterable<T> skip(java.lang.Iterable<T>, int);
  public static <T> java.lang.Iterable<T> limit(java.lang.Iterable<T>, int);
  public static <T> java.lang.Iterable<T> consumingIterable(java.lang.Iterable<T>);
  public static boolean isEmpty(java.lang.Iterable<?>);
  public static <T> java.lang.Iterable<T> mergeSorted(java.lang.Iterable<? extends java.lang.Iterable<? extends T>>, java.util.Comparator<? super T>);
}
```

## `com.google.common.collect.Iterators`

```java
public final class com.google.common.collect.Iterators {
  public static <T> com.google.common.collect.UnmodifiableIterator<T> unmodifiableIterator(java.util.Iterator<? extends T>);
  public static <T> com.google.common.collect.UnmodifiableIterator<T> unmodifiableIterator(com.google.common.collect.UnmodifiableIterator<T>);
  public static int size(java.util.Iterator<?>);
  public static boolean contains(java.util.Iterator<?>, java.lang.Object);
  public static boolean removeAll(java.util.Iterator<?>, java.util.Collection<?>);
  public static <T> boolean removeIf(java.util.Iterator<T>, com.google.common.base.Predicate<? super T>);
  public static boolean retainAll(java.util.Iterator<?>, java.util.Collection<?>);
  public static boolean elementsEqual(java.util.Iterator<?>, java.util.Iterator<?>);
  public static java.lang.String toString(java.util.Iterator<?>);
  public static <T> T getOnlyElement(java.util.Iterator<T>);
  public static <T> T getOnlyElement(java.util.Iterator<? extends T>, T);
  public static <T> T[] toArray(java.util.Iterator<? extends T>, java.lang.Class<T>);
  public static <T> boolean addAll(java.util.Collection<T>, java.util.Iterator<? extends T>);
  public static int frequency(java.util.Iterator<?>, java.lang.Object);
  public static <T> java.util.Iterator<T> cycle(java.lang.Iterable<T>);
  public static <T> java.util.Iterator<T> cycle(T...);
  public static <T> java.util.Iterator<T> concat(java.util.Iterator<? extends T>, java.util.Iterator<? extends T>);
  public static <T> java.util.Iterator<T> concat(java.util.Iterator<? extends T>, java.util.Iterator<? extends T>, java.util.Iterator<? extends T>);
  public static <T> java.util.Iterator<T> concat(java.util.Iterator<? extends T>, java.util.Iterator<? extends T>, java.util.Iterator<? extends T>, java.util.Iterator<? extends T>);
  public static <T> java.util.Iterator<T> concat(java.util.Iterator<? extends T>...);
  public static <T> java.util.Iterator<T> concat(java.util.Iterator<? extends java.util.Iterator<? extends T>>);
  public static <T> com.google.common.collect.UnmodifiableIterator<java.util.List<T>> partition(java.util.Iterator<T>, int);
  public static <T> com.google.common.collect.UnmodifiableIterator<java.util.List<T>> paddedPartition(java.util.Iterator<T>, int);
  public static <T> com.google.common.collect.UnmodifiableIterator<T> filter(java.util.Iterator<T>, com.google.common.base.Predicate<? super T>);
  public static <T> com.google.common.collect.UnmodifiableIterator<T> filter(java.util.Iterator<?>, java.lang.Class<T>);
  public static <T> boolean any(java.util.Iterator<T>, com.google.common.base.Predicate<? super T>);
  public static <T> boolean all(java.util.Iterator<T>, com.google.common.base.Predicate<? super T>);
  public static <T> T find(java.util.Iterator<T>, com.google.common.base.Predicate<? super T>);
  public static <T> T find(java.util.Iterator<? extends T>, com.google.common.base.Predicate<? super T>, T);
  public static <T> com.google.common.base.Optional<T> tryFind(java.util.Iterator<T>, com.google.common.base.Predicate<? super T>);
  public static <T> int indexOf(java.util.Iterator<T>, com.google.common.base.Predicate<? super T>);
  public static <F, T> java.util.Iterator<T> transform(java.util.Iterator<F>, com.google.common.base.Function<? super F, ? extends T>);
  public static <T> T get(java.util.Iterator<T>, int);
  public static <T> T get(java.util.Iterator<? extends T>, int, T);
  public static <T> T getNext(java.util.Iterator<? extends T>, T);
  public static <T> T getLast(java.util.Iterator<T>);
  public static <T> T getLast(java.util.Iterator<? extends T>, T);
  public static int advance(java.util.Iterator<?>, int);
  public static <T> java.util.Iterator<T> limit(java.util.Iterator<T>, int);
  public static <T> java.util.Iterator<T> consumingIterator(java.util.Iterator<T>);
  public static <T> com.google.common.collect.UnmodifiableIterator<T> forArray(T...);
  public static <T> com.google.common.collect.UnmodifiableIterator<T> singletonIterator(T);
  public static <T> com.google.common.collect.UnmodifiableIterator<T> forEnumeration(java.util.Enumeration<T>);
  public static <T> java.util.Enumeration<T> asEnumeration(java.util.Iterator<T>);
  public static <T> com.google.common.collect.PeekingIterator<T> peekingIterator(java.util.Iterator<? extends T>);
  public static <T> com.google.common.collect.PeekingIterator<T> peekingIterator(com.google.common.collect.PeekingIterator<T>);
  public static <T> com.google.common.collect.UnmodifiableIterator<T> mergeSorted(java.lang.Iterable<? extends java.util.Iterator<? extends T>>, java.util.Comparator<? super T>);
}
```

## `com.google.common.collect.LinkedHashMultimap`

```java
public final class com.google.common.collect.LinkedHashMultimap<K, V> extends com.google.common.collect.LinkedHashMultimapGwtSerializationDependencies<K, V> {
  public static <K, V> com.google.common.collect.LinkedHashMultimap<K, V> create();
  public static <K, V> com.google.common.collect.LinkedHashMultimap<K, V> create(int, int);
  public static <K, V> com.google.common.collect.LinkedHashMultimap<K, V> create(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public java.util.Set<V> replaceValues(K, java.lang.Iterable<? extends V>);
  public java.util.Set<java.util.Map$Entry<K, V>> entries();
  public java.util.Set<K> keySet();
  public java.util.Collection<V> values();
  public void clear();
  public boolean equals(java.lang.Object);
  public boolean put(java.lang.Object, java.lang.Object);
  public java.util.Map asMap();
  public java.util.Set removeAll(java.lang.Object);
  public java.util.Set get(java.lang.Object);
  public java.util.Collection entries();
  public java.util.Collection replaceValues(java.lang.Object, java.lang.Iterable);
  public void forEach(java.util.function.BiConsumer);
  public boolean containsKey(java.lang.Object);
  public int size();
  public java.lang.String toString();
  public int hashCode();
  public com.google.common.collect.Multiset keys();
  public boolean putAll(com.google.common.collect.Multimap);
  public boolean putAll(java.lang.Object, java.lang.Iterable);
  public boolean remove(java.lang.Object, java.lang.Object);
  public boolean containsEntry(java.lang.Object, java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public boolean isEmpty();
}
```

## `com.google.common.collect.LinkedHashMultiset`

```java
public final class com.google.common.collect.LinkedHashMultiset<E> extends com.google.common.collect.AbstractMapBasedMultiset<E> {
  public static <E> com.google.common.collect.LinkedHashMultiset<E> create();
  public static <E> com.google.common.collect.LinkedHashMultiset<E> create(int);
  public static <E> com.google.common.collect.LinkedHashMultiset<E> create(java.lang.Iterable<? extends E>);
  public int setCount(java.lang.Object, int);
  public int remove(java.lang.Object, int);
  public int add(java.lang.Object, int);
  public int count(java.lang.Object);
  public java.util.Iterator iterator();
  public int size();
  public void clear();
  public void forEachEntry(java.util.function.ObjIntConsumer);
  public java.util.Set entrySet();
  public java.util.Set elementSet();
  public boolean setCount(java.lang.Object, int, int);
  public boolean contains(java.lang.Object);
  public boolean isEmpty();
}
```

## `com.google.common.collect.LinkedListMultimap`

```java
public class com.google.common.collect.LinkedListMultimap<K, V> extends com.google.common.collect.AbstractMultimap<K, V> implements com.google.common.collect.ListMultimap<K, V>, java.io.Serializable {
  public static <K, V> com.google.common.collect.LinkedListMultimap<K, V> create();
  public static <K, V> com.google.common.collect.LinkedListMultimap<K, V> create(int);
  public static <K, V> com.google.common.collect.LinkedListMultimap<K, V> create(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public int size();
  public boolean isEmpty();
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public boolean put(K, V);
  public java.util.List<V> replaceValues(K, java.lang.Iterable<? extends V>);
  public java.util.List<V> removeAll(java.lang.Object);
  public void clear();
  public java.util.List<V> get(K);
  public java.util.List<V> values();
  public java.util.List<java.util.Map$Entry<K, V>> entries();
  public java.lang.String toString();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.util.Map asMap();
  public java.util.Collection values();
  public com.google.common.collect.Multiset keys();
  public java.util.Set keySet();
  public java.util.Collection entries();
  public java.util.Collection replaceValues(java.lang.Object, java.lang.Iterable);
  public boolean putAll(com.google.common.collect.Multimap);
  public boolean putAll(java.lang.Object, java.lang.Iterable);
  public boolean remove(java.lang.Object, java.lang.Object);
  public boolean containsEntry(java.lang.Object, java.lang.Object);
  public java.util.Collection get(java.lang.Object);
  public java.util.Collection removeAll(java.lang.Object);
}
```

## `com.google.common.collect.ListMultimap`

```java
public interface com.google.common.collect.ListMultimap<K, V> extends com.google.common.collect.Multimap<K, V> {
  public abstract java.util.List<V> get(K);
  public abstract java.util.List<V> removeAll(java.lang.Object);
  public abstract java.util.List<V> replaceValues(K, java.lang.Iterable<? extends V>);
  public abstract java.util.Map<K, java.util.Collection<V>> asMap();
  public abstract boolean equals(java.lang.Object);
  public default java.util.Collection get(java.lang.Object);
  public default java.util.Collection removeAll(java.lang.Object);
  public default java.util.Collection replaceValues(java.lang.Object, java.lang.Iterable);
}
```

## `com.google.common.collect.Lists`

```java
public final class com.google.common.collect.Lists {
  public static <E> java.util.ArrayList<E> newArrayList();
  public static <E> java.util.ArrayList<E> newArrayList(E...);
  public static <E> java.util.ArrayList<E> newArrayList(java.lang.Iterable<? extends E>);
  public static <E> java.util.ArrayList<E> newArrayList(java.util.Iterator<? extends E>);
  public static <E> java.util.ArrayList<E> newArrayListWithCapacity(int);
  public static <E> java.util.ArrayList<E> newArrayListWithExpectedSize(int);
  public static <E> java.util.LinkedList<E> newLinkedList();
  public static <E> java.util.LinkedList<E> newLinkedList(java.lang.Iterable<? extends E>);
  public static <E> java.util.concurrent.CopyOnWriteArrayList<E> newCopyOnWriteArrayList();
  public static <E> java.util.concurrent.CopyOnWriteArrayList<E> newCopyOnWriteArrayList(java.lang.Iterable<? extends E>);
  public static <E> java.util.List<E> asList(E, E[]);
  public static <E> java.util.List<E> asList(E, E, E[]);
  public static <B> java.util.List<java.util.List<B>> cartesianProduct(java.util.List<? extends java.util.List<? extends B>>);
  public static <B> java.util.List<java.util.List<B>> cartesianProduct(java.util.List<? extends B>...);
  public static <F, T> java.util.List<T> transform(java.util.List<F>, com.google.common.base.Function<? super F, ? extends T>);
  public static <T> java.util.List<java.util.List<T>> partition(java.util.List<T>, int);
  public static com.google.common.collect.ImmutableList<java.lang.Character> charactersOf(java.lang.String);
  public static java.util.List<java.lang.Character> charactersOf(java.lang.CharSequence);
  public static <T> java.util.List<T> reverse(java.util.List<T>);
}
```

## `com.google.common.collect.MapDifference`

```java
public interface com.google.common.collect.MapDifference<K, V> {
  public abstract boolean areEqual();
  public abstract java.util.Map<K, V> entriesOnlyOnLeft();
  public abstract java.util.Map<K, V> entriesOnlyOnRight();
  public abstract java.util.Map<K, V> entriesInCommon();
  public abstract java.util.Map<K, com.google.common.collect.MapDifference$ValueDifference<V>> entriesDiffering();
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
}
```

## `com.google.common.collect.MapDifference$ValueDifference`

```java
public interface com.google.common.collect.MapDifference$ValueDifference<V> {
  public abstract V leftValue();
  public abstract V rightValue();
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
}
```

## `com.google.common.collect.MapMaker`

```java
public final class com.google.common.collect.MapMaker {
  public com.google.common.collect.MapMaker();
  public com.google.common.collect.MapMaker initialCapacity(int);
  public com.google.common.collect.MapMaker concurrencyLevel(int);
  public com.google.common.collect.MapMaker weakKeys();
  public com.google.common.collect.MapMaker weakValues();
  public <K, V> java.util.concurrent.ConcurrentMap<K, V> makeMap();
  public java.lang.String toString();
}
```

## `com.google.common.collect.Maps`

```java
public final class com.google.common.collect.Maps {
  public static <K extends java.lang.Enum<K>, V> com.google.common.collect.ImmutableMap<K, V> immutableEnumMap(java.util.Map<K, ? extends V>);
  public static <T, K extends java.lang.Enum<K>, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableMap<K, V>> toImmutableEnumMap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends V>);
  public static <T, K extends java.lang.Enum<K>, V> java.util.stream.Collector<T, ?, com.google.common.collect.ImmutableMap<K, V>> toImmutableEnumMap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends V>, java.util.function.BinaryOperator<V>);
  public static <K, V> java.util.HashMap<K, V> newHashMap();
  public static <K, V> java.util.HashMap<K, V> newHashMap(java.util.Map<? extends K, ? extends V>);
  public static <K, V> java.util.HashMap<K, V> newHashMapWithExpectedSize(int);
  public static <K, V> java.util.LinkedHashMap<K, V> newLinkedHashMap();
  public static <K, V> java.util.LinkedHashMap<K, V> newLinkedHashMap(java.util.Map<? extends K, ? extends V>);
  public static <K, V> java.util.LinkedHashMap<K, V> newLinkedHashMapWithExpectedSize(int);
  public static <K, V> java.util.concurrent.ConcurrentMap<K, V> newConcurrentMap();
  public static <K extends java.lang.Comparable, V> java.util.TreeMap<K, V> newTreeMap();
  public static <K, V> java.util.TreeMap<K, V> newTreeMap(java.util.SortedMap<K, ? extends V>);
  public static <C, K extends C, V> java.util.TreeMap<K, V> newTreeMap(java.util.Comparator<C>);
  public static <K extends java.lang.Enum<K>, V> java.util.EnumMap<K, V> newEnumMap(java.lang.Class<K>);
  public static <K extends java.lang.Enum<K>, V> java.util.EnumMap<K, V> newEnumMap(java.util.Map<K, ? extends V>);
  public static <K, V> java.util.IdentityHashMap<K, V> newIdentityHashMap();
  public static <K, V> com.google.common.collect.MapDifference<K, V> difference(java.util.Map<? extends K, ? extends V>, java.util.Map<? extends K, ? extends V>);
  public static <K, V> com.google.common.collect.MapDifference<K, V> difference(java.util.Map<? extends K, ? extends V>, java.util.Map<? extends K, ? extends V>, com.google.common.base.Equivalence<? super V>);
  public static <K, V> com.google.common.collect.SortedMapDifference<K, V> difference(java.util.SortedMap<K, ? extends V>, java.util.Map<? extends K, ? extends V>);
  public static <K, V> java.util.Map<K, V> asMap(java.util.Set<K>, com.google.common.base.Function<? super K, V>);
  public static <K, V> java.util.SortedMap<K, V> asMap(java.util.SortedSet<K>, com.google.common.base.Function<? super K, V>);
  public static <K, V> java.util.NavigableMap<K, V> asMap(java.util.NavigableSet<K>, com.google.common.base.Function<? super K, V>);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> toMap(java.lang.Iterable<K>, com.google.common.base.Function<? super K, V>);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> toMap(java.util.Iterator<K>, com.google.common.base.Function<? super K, V>);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> uniqueIndex(java.lang.Iterable<V>, com.google.common.base.Function<? super V, K>);
  public static <K, V> com.google.common.collect.ImmutableMap<K, V> uniqueIndex(java.util.Iterator<V>, com.google.common.base.Function<? super V, K>);
  public static com.google.common.collect.ImmutableMap<java.lang.String, java.lang.String> fromProperties(java.util.Properties);
  public static <K, V> java.util.Map$Entry<K, V> immutableEntry(K, V);
  public static <A, B> com.google.common.base.Converter<A, B> asConverter(com.google.common.collect.BiMap<A, B>);
  public static <K, V> com.google.common.collect.BiMap<K, V> synchronizedBiMap(com.google.common.collect.BiMap<K, V>);
  public static <K, V> com.google.common.collect.BiMap<K, V> unmodifiableBiMap(com.google.common.collect.BiMap<? extends K, ? extends V>);
  public static <K, V1, V2> java.util.Map<K, V2> transformValues(java.util.Map<K, V1>, com.google.common.base.Function<? super V1, V2>);
  public static <K, V1, V2> java.util.SortedMap<K, V2> transformValues(java.util.SortedMap<K, V1>, com.google.common.base.Function<? super V1, V2>);
  public static <K, V1, V2> java.util.NavigableMap<K, V2> transformValues(java.util.NavigableMap<K, V1>, com.google.common.base.Function<? super V1, V2>);
  public static <K, V1, V2> java.util.Map<K, V2> transformEntries(java.util.Map<K, V1>, com.google.common.collect.Maps$EntryTransformer<? super K, ? super V1, V2>);
  public static <K, V1, V2> java.util.SortedMap<K, V2> transformEntries(java.util.SortedMap<K, V1>, com.google.common.collect.Maps$EntryTransformer<? super K, ? super V1, V2>);
  public static <K, V1, V2> java.util.NavigableMap<K, V2> transformEntries(java.util.NavigableMap<K, V1>, com.google.common.collect.Maps$EntryTransformer<? super K, ? super V1, V2>);
  public static <K, V> java.util.Map<K, V> filterKeys(java.util.Map<K, V>, com.google.common.base.Predicate<? super K>);
  public static <K, V> java.util.SortedMap<K, V> filterKeys(java.util.SortedMap<K, V>, com.google.common.base.Predicate<? super K>);
  public static <K, V> java.util.NavigableMap<K, V> filterKeys(java.util.NavigableMap<K, V>, com.google.common.base.Predicate<? super K>);
  public static <K, V> com.google.common.collect.BiMap<K, V> filterKeys(com.google.common.collect.BiMap<K, V>, com.google.common.base.Predicate<? super K>);
  public static <K, V> java.util.Map<K, V> filterValues(java.util.Map<K, V>, com.google.common.base.Predicate<? super V>);
  public static <K, V> java.util.SortedMap<K, V> filterValues(java.util.SortedMap<K, V>, com.google.common.base.Predicate<? super V>);
  public static <K, V> java.util.NavigableMap<K, V> filterValues(java.util.NavigableMap<K, V>, com.google.common.base.Predicate<? super V>);
  public static <K, V> com.google.common.collect.BiMap<K, V> filterValues(com.google.common.collect.BiMap<K, V>, com.google.common.base.Predicate<? super V>);
  public static <K, V> java.util.Map<K, V> filterEntries(java.util.Map<K, V>, com.google.common.base.Predicate<? super java.util.Map$Entry<K, V>>);
  public static <K, V> java.util.SortedMap<K, V> filterEntries(java.util.SortedMap<K, V>, com.google.common.base.Predicate<? super java.util.Map$Entry<K, V>>);
  public static <K, V> java.util.NavigableMap<K, V> filterEntries(java.util.NavigableMap<K, V>, com.google.common.base.Predicate<? super java.util.Map$Entry<K, V>>);
  public static <K, V> com.google.common.collect.BiMap<K, V> filterEntries(com.google.common.collect.BiMap<K, V>, com.google.common.base.Predicate<? super java.util.Map$Entry<K, V>>);
  public static <K, V> java.util.NavigableMap<K, V> unmodifiableNavigableMap(java.util.NavigableMap<K, ? extends V>);
  public static <K, V> java.util.NavigableMap<K, V> synchronizedNavigableMap(java.util.NavigableMap<K, V>);
  public static <K extends java.lang.Comparable<? super K>, V> java.util.NavigableMap<K, V> subMap(java.util.NavigableMap<K, V>, com.google.common.collect.Range<K>);
}
```

## `com.google.common.collect.Maps$EntryTransformer`

```java
public interface com.google.common.collect.Maps$EntryTransformer<K, V1, V2> {
  public abstract V2 transformEntry(K, V1);
}
```

## `com.google.common.collect.MinMaxPriorityQueue`

```java
public final class com.google.common.collect.MinMaxPriorityQueue<E> extends java.util.AbstractQueue<E> {
  public static <E extends java.lang.Comparable<E>> com.google.common.collect.MinMaxPriorityQueue<E> create();
  public static <E extends java.lang.Comparable<E>> com.google.common.collect.MinMaxPriorityQueue<E> create(java.lang.Iterable<? extends E>);
  public static <B> com.google.common.collect.MinMaxPriorityQueue$Builder<B> orderedBy(java.util.Comparator<B>);
  public static com.google.common.collect.MinMaxPriorityQueue$Builder<java.lang.Comparable> expectedSize(int);
  public static com.google.common.collect.MinMaxPriorityQueue$Builder<java.lang.Comparable> maximumSize(int);
  public int size();
  public boolean add(E);
  public boolean addAll(java.util.Collection<? extends E>);
  public boolean offer(E);
  public E poll();
  public E peek();
  public E pollFirst();
  public E removeFirst();
  public E peekFirst();
  public E pollLast();
  public E removeLast();
  public E peekLast();
  public java.util.Iterator<E> iterator();
  public void clear();
  public java.lang.Object[] toArray();
  public java.util.Comparator<? super E> comparator();
}
```

## `com.google.common.collect.MinMaxPriorityQueue$Builder`

```java
public final class com.google.common.collect.MinMaxPriorityQueue$Builder<B> {
  public com.google.common.collect.MinMaxPriorityQueue$Builder<B> expectedSize(int);
  public com.google.common.collect.MinMaxPriorityQueue$Builder<B> maximumSize(int);
  public <T extends B> com.google.common.collect.MinMaxPriorityQueue<T> create();
  public <T extends B> com.google.common.collect.MinMaxPriorityQueue<T> create(java.lang.Iterable<? extends T>);
}
```

## `com.google.common.collect.MoreCollectors`

```java
public final class com.google.common.collect.MoreCollectors {
  public static <T> java.util.stream.Collector<T, ?, java.util.Optional<T>> toOptional();
  public static <T> java.util.stream.Collector<T, ?, T> onlyElement();
}
```

## `com.google.common.collect.Multimap`

```java
public interface com.google.common.collect.Multimap<K, V> {
  public abstract int size();
  public abstract boolean isEmpty();
  public abstract boolean containsKey(java.lang.Object);
  public abstract boolean containsValue(java.lang.Object);
  public abstract boolean containsEntry(java.lang.Object, java.lang.Object);
  public abstract boolean put(K, V);
  public abstract boolean remove(java.lang.Object, java.lang.Object);
  public abstract boolean putAll(K, java.lang.Iterable<? extends V>);
  public abstract boolean putAll(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public abstract java.util.Collection<V> replaceValues(K, java.lang.Iterable<? extends V>);
  public abstract java.util.Collection<V> removeAll(java.lang.Object);
  public abstract void clear();
  public abstract java.util.Collection<V> get(K);
  public abstract java.util.Set<K> keySet();
  public abstract com.google.common.collect.Multiset<K> keys();
  public abstract java.util.Collection<V> values();
  public abstract java.util.Collection<java.util.Map$Entry<K, V>> entries();
  public default void forEach(java.util.function.BiConsumer<? super K, ? super V>);
  public abstract java.util.Map<K, java.util.Collection<V>> asMap();
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
}
```

## `com.google.common.collect.MultimapBuilder`

```java
public abstract class com.google.common.collect.MultimapBuilder<K0, V0> {
  public static com.google.common.collect.MultimapBuilder$MultimapBuilderWithKeys<java.lang.Object> hashKeys();
  public static com.google.common.collect.MultimapBuilder$MultimapBuilderWithKeys<java.lang.Object> hashKeys(int);
  public static com.google.common.collect.MultimapBuilder$MultimapBuilderWithKeys<java.lang.Object> linkedHashKeys();
  public static com.google.common.collect.MultimapBuilder$MultimapBuilderWithKeys<java.lang.Object> linkedHashKeys(int);
  public static com.google.common.collect.MultimapBuilder$MultimapBuilderWithKeys<java.lang.Comparable> treeKeys();
  public static <K0> com.google.common.collect.MultimapBuilder$MultimapBuilderWithKeys<K0> treeKeys(java.util.Comparator<K0>);
  public static <K0 extends java.lang.Enum<K0>> com.google.common.collect.MultimapBuilder$MultimapBuilderWithKeys<K0> enumKeys(java.lang.Class<K0>);
  public abstract <K extends K0, V extends V0> com.google.common.collect.Multimap<K, V> build();
  public <K extends K0, V extends V0> com.google.common.collect.Multimap<K, V> build(com.google.common.collect.Multimap<? extends K, ? extends V>);
}
```

## `com.google.common.collect.MultimapBuilder$ListMultimapBuilder`

```java
public abstract class com.google.common.collect.MultimapBuilder$ListMultimapBuilder<K0, V0> extends com.google.common.collect.MultimapBuilder<K0, V0> {
  public abstract <K extends K0, V extends V0> com.google.common.collect.ListMultimap<K, V> build();
  public <K extends K0, V extends V0> com.google.common.collect.ListMultimap<K, V> build(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public com.google.common.collect.Multimap build(com.google.common.collect.Multimap);
  public com.google.common.collect.Multimap build();
}
```

## `com.google.common.collect.MultimapBuilder$MultimapBuilderWithKeys`

```java
public abstract class com.google.common.collect.MultimapBuilder$MultimapBuilderWithKeys<K0> {
  public com.google.common.collect.MultimapBuilder$ListMultimapBuilder<K0, java.lang.Object> arrayListValues();
  public com.google.common.collect.MultimapBuilder$ListMultimapBuilder<K0, java.lang.Object> arrayListValues(int);
  public com.google.common.collect.MultimapBuilder$ListMultimapBuilder<K0, java.lang.Object> linkedListValues();
  public com.google.common.collect.MultimapBuilder$SetMultimapBuilder<K0, java.lang.Object> hashSetValues();
  public com.google.common.collect.MultimapBuilder$SetMultimapBuilder<K0, java.lang.Object> hashSetValues(int);
  public com.google.common.collect.MultimapBuilder$SetMultimapBuilder<K0, java.lang.Object> linkedHashSetValues();
  public com.google.common.collect.MultimapBuilder$SetMultimapBuilder<K0, java.lang.Object> linkedHashSetValues(int);
  public com.google.common.collect.MultimapBuilder$SortedSetMultimapBuilder<K0, java.lang.Comparable> treeSetValues();
  public <V0> com.google.common.collect.MultimapBuilder$SortedSetMultimapBuilder<K0, V0> treeSetValues(java.util.Comparator<V0>);
  public <V0 extends java.lang.Enum<V0>> com.google.common.collect.MultimapBuilder$SetMultimapBuilder<K0, V0> enumSetValues(java.lang.Class<V0>);
}
```

## `com.google.common.collect.MultimapBuilder$SetMultimapBuilder`

```java
public abstract class com.google.common.collect.MultimapBuilder$SetMultimapBuilder<K0, V0> extends com.google.common.collect.MultimapBuilder<K0, V0> {
  public abstract <K extends K0, V extends V0> com.google.common.collect.SetMultimap<K, V> build();
  public <K extends K0, V extends V0> com.google.common.collect.SetMultimap<K, V> build(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public com.google.common.collect.Multimap build(com.google.common.collect.Multimap);
  public com.google.common.collect.Multimap build();
}
```

## `com.google.common.collect.MultimapBuilder$SortedSetMultimapBuilder`

```java
public abstract class com.google.common.collect.MultimapBuilder$SortedSetMultimapBuilder<K0, V0> extends com.google.common.collect.MultimapBuilder$SetMultimapBuilder<K0, V0> {
  public abstract <K extends K0, V extends V0> com.google.common.collect.SortedSetMultimap<K, V> build();
  public <K extends K0, V extends V0> com.google.common.collect.SortedSetMultimap<K, V> build(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public com.google.common.collect.SetMultimap build(com.google.common.collect.Multimap);
  public com.google.common.collect.SetMultimap build();
  public com.google.common.collect.Multimap build(com.google.common.collect.Multimap);
  public com.google.common.collect.Multimap build();
}
```

## `com.google.common.collect.Multimaps`

```java
public final class com.google.common.collect.Multimaps {
  public static <T, K, V, M extends com.google.common.collect.Multimap<K, V>> java.util.stream.Collector<T, ?, M> toMultimap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends V>, java.util.function.Supplier<M>);
  public static <T, K, V, M extends com.google.common.collect.Multimap<K, V>> java.util.stream.Collector<T, ?, M> flatteningToMultimap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends java.util.stream.Stream<? extends V>>, java.util.function.Supplier<M>);
  public static <K, V> com.google.common.collect.Multimap<K, V> newMultimap(java.util.Map<K, java.util.Collection<V>>, com.google.common.base.Supplier<? extends java.util.Collection<V>>);
  public static <K, V> com.google.common.collect.ListMultimap<K, V> newListMultimap(java.util.Map<K, java.util.Collection<V>>, com.google.common.base.Supplier<? extends java.util.List<V>>);
  public static <K, V> com.google.common.collect.SetMultimap<K, V> newSetMultimap(java.util.Map<K, java.util.Collection<V>>, com.google.common.base.Supplier<? extends java.util.Set<V>>);
  public static <K, V> com.google.common.collect.SortedSetMultimap<K, V> newSortedSetMultimap(java.util.Map<K, java.util.Collection<V>>, com.google.common.base.Supplier<? extends java.util.SortedSet<V>>);
  public static <K, V, M extends com.google.common.collect.Multimap<K, V>> M invertFrom(com.google.common.collect.Multimap<? extends V, ? extends K>, M);
  public static <K, V> com.google.common.collect.Multimap<K, V> synchronizedMultimap(com.google.common.collect.Multimap<K, V>);
  public static <K, V> com.google.common.collect.Multimap<K, V> unmodifiableMultimap(com.google.common.collect.Multimap<K, V>);
  public static <K, V> com.google.common.collect.Multimap<K, V> unmodifiableMultimap(com.google.common.collect.ImmutableMultimap<K, V>);
  public static <K, V> com.google.common.collect.SetMultimap<K, V> synchronizedSetMultimap(com.google.common.collect.SetMultimap<K, V>);
  public static <K, V> com.google.common.collect.SetMultimap<K, V> unmodifiableSetMultimap(com.google.common.collect.SetMultimap<K, V>);
  public static <K, V> com.google.common.collect.SetMultimap<K, V> unmodifiableSetMultimap(com.google.common.collect.ImmutableSetMultimap<K, V>);
  public static <K, V> com.google.common.collect.SortedSetMultimap<K, V> synchronizedSortedSetMultimap(com.google.common.collect.SortedSetMultimap<K, V>);
  public static <K, V> com.google.common.collect.SortedSetMultimap<K, V> unmodifiableSortedSetMultimap(com.google.common.collect.SortedSetMultimap<K, V>);
  public static <K, V> com.google.common.collect.ListMultimap<K, V> synchronizedListMultimap(com.google.common.collect.ListMultimap<K, V>);
  public static <K, V> com.google.common.collect.ListMultimap<K, V> unmodifiableListMultimap(com.google.common.collect.ListMultimap<K, V>);
  public static <K, V> com.google.common.collect.ListMultimap<K, V> unmodifiableListMultimap(com.google.common.collect.ImmutableListMultimap<K, V>);
  public static <K, V> java.util.Map<K, java.util.List<V>> asMap(com.google.common.collect.ListMultimap<K, V>);
  public static <K, V> java.util.Map<K, java.util.Set<V>> asMap(com.google.common.collect.SetMultimap<K, V>);
  public static <K, V> java.util.Map<K, java.util.SortedSet<V>> asMap(com.google.common.collect.SortedSetMultimap<K, V>);
  public static <K, V> java.util.Map<K, java.util.Collection<V>> asMap(com.google.common.collect.Multimap<K, V>);
  public static <K, V> com.google.common.collect.SetMultimap<K, V> forMap(java.util.Map<K, V>);
  public static <K, V1, V2> com.google.common.collect.Multimap<K, V2> transformValues(com.google.common.collect.Multimap<K, V1>, com.google.common.base.Function<? super V1, V2>);
  public static <K, V1, V2> com.google.common.collect.ListMultimap<K, V2> transformValues(com.google.common.collect.ListMultimap<K, V1>, com.google.common.base.Function<? super V1, V2>);
  public static <K, V1, V2> com.google.common.collect.Multimap<K, V2> transformEntries(com.google.common.collect.Multimap<K, V1>, com.google.common.collect.Maps$EntryTransformer<? super K, ? super V1, V2>);
  public static <K, V1, V2> com.google.common.collect.ListMultimap<K, V2> transformEntries(com.google.common.collect.ListMultimap<K, V1>, com.google.common.collect.Maps$EntryTransformer<? super K, ? super V1, V2>);
  public static <K, V> com.google.common.collect.ImmutableListMultimap<K, V> index(java.lang.Iterable<V>, com.google.common.base.Function<? super V, K>);
  public static <K, V> com.google.common.collect.ImmutableListMultimap<K, V> index(java.util.Iterator<V>, com.google.common.base.Function<? super V, K>);
  public static <K, V> com.google.common.collect.Multimap<K, V> filterKeys(com.google.common.collect.Multimap<K, V>, com.google.common.base.Predicate<? super K>);
  public static <K, V> com.google.common.collect.SetMultimap<K, V> filterKeys(com.google.common.collect.SetMultimap<K, V>, com.google.common.base.Predicate<? super K>);
  public static <K, V> com.google.common.collect.ListMultimap<K, V> filterKeys(com.google.common.collect.ListMultimap<K, V>, com.google.common.base.Predicate<? super K>);
  public static <K, V> com.google.common.collect.Multimap<K, V> filterValues(com.google.common.collect.Multimap<K, V>, com.google.common.base.Predicate<? super V>);
  public static <K, V> com.google.common.collect.SetMultimap<K, V> filterValues(com.google.common.collect.SetMultimap<K, V>, com.google.common.base.Predicate<? super V>);
  public static <K, V> com.google.common.collect.Multimap<K, V> filterEntries(com.google.common.collect.Multimap<K, V>, com.google.common.base.Predicate<? super java.util.Map$Entry<K, V>>);
  public static <K, V> com.google.common.collect.SetMultimap<K, V> filterEntries(com.google.common.collect.SetMultimap<K, V>, com.google.common.base.Predicate<? super java.util.Map$Entry<K, V>>);
}
```

## `com.google.common.collect.Multiset`

```java
public interface com.google.common.collect.Multiset<E> extends java.util.Collection<E> {
  public abstract int size();
  public abstract int count(java.lang.Object);
  public abstract int add(E, int);
  public abstract boolean add(E);
  public abstract int remove(java.lang.Object, int);
  public abstract boolean remove(java.lang.Object);
  public abstract int setCount(E, int);
  public abstract boolean setCount(E, int, int);
  public abstract java.util.Set<E> elementSet();
  public abstract java.util.Set<com.google.common.collect.Multiset$Entry<E>> entrySet();
  public default void forEachEntry(java.util.function.ObjIntConsumer<? super E>);
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
  public abstract java.lang.String toString();
  public abstract java.util.Iterator<E> iterator();
  public abstract boolean contains(java.lang.Object);
  public abstract boolean containsAll(java.util.Collection<?>);
  public abstract boolean removeAll(java.util.Collection<?>);
  public abstract boolean retainAll(java.util.Collection<?>);
  public default void forEach(java.util.function.Consumer<? super E>);
  public default java.util.Spliterator<E> spliterator();
}
```

## `com.google.common.collect.Multiset$Entry`

```java
public interface com.google.common.collect.Multiset$Entry<E> {
  public abstract E getElement();
  public abstract int getCount();
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
  public abstract java.lang.String toString();
}
```

## `com.google.common.collect.Multisets`

```java
public final class com.google.common.collect.Multisets {
  public static <T, E, M extends com.google.common.collect.Multiset<E>> java.util.stream.Collector<T, ?, M> toMultiset(java.util.function.Function<? super T, E>, java.util.function.ToIntFunction<? super T>, java.util.function.Supplier<M>);
  public static <E> com.google.common.collect.Multiset<E> unmodifiableMultiset(com.google.common.collect.Multiset<? extends E>);
  public static <E> com.google.common.collect.Multiset<E> unmodifiableMultiset(com.google.common.collect.ImmutableMultiset<E>);
  public static <E> com.google.common.collect.SortedMultiset<E> unmodifiableSortedMultiset(com.google.common.collect.SortedMultiset<E>);
  public static <E> com.google.common.collect.Multiset$Entry<E> immutableEntry(E, int);
  public static <E> com.google.common.collect.Multiset<E> filter(com.google.common.collect.Multiset<E>, com.google.common.base.Predicate<? super E>);
  public static <E> com.google.common.collect.Multiset<E> union(com.google.common.collect.Multiset<? extends E>, com.google.common.collect.Multiset<? extends E>);
  public static <E> com.google.common.collect.Multiset<E> intersection(com.google.common.collect.Multiset<E>, com.google.common.collect.Multiset<?>);
  public static <E> com.google.common.collect.Multiset<E> sum(com.google.common.collect.Multiset<? extends E>, com.google.common.collect.Multiset<? extends E>);
  public static <E> com.google.common.collect.Multiset<E> difference(com.google.common.collect.Multiset<E>, com.google.common.collect.Multiset<?>);
  public static boolean containsOccurrences(com.google.common.collect.Multiset<?>, com.google.common.collect.Multiset<?>);
  public static boolean retainOccurrences(com.google.common.collect.Multiset<?>, com.google.common.collect.Multiset<?>);
  public static boolean removeOccurrences(com.google.common.collect.Multiset<?>, java.lang.Iterable<?>);
  public static boolean removeOccurrences(com.google.common.collect.Multiset<?>, com.google.common.collect.Multiset<?>);
  public static <E> com.google.common.collect.ImmutableMultiset<E> copyHighestCountFirst(com.google.common.collect.Multiset<E>);
}
```

## `com.google.common.collect.MutableClassToInstanceMap`

```java
public final class com.google.common.collect.MutableClassToInstanceMap<B> extends com.google.common.collect.ForwardingMap<java.lang.Class<? extends B>, B> implements com.google.common.collect.ClassToInstanceMap<B>, java.io.Serializable {
  public static <B> com.google.common.collect.MutableClassToInstanceMap<B> create();
  public static <B> com.google.common.collect.MutableClassToInstanceMap<B> create(java.util.Map<java.lang.Class<? extends B>, B>);
  public java.util.Set<java.util.Map$Entry<java.lang.Class<? extends B>, B>> entrySet();
  public B put(java.lang.Class<? extends B>, B);
  public void putAll(java.util.Map<? extends java.lang.Class<? extends B>, ? extends B>);
  public <T extends B> T putInstance(java.lang.Class<T>, T);
  public <T extends B> T getInstance(java.lang.Class<T>);
  public java.lang.Object put(java.lang.Object, java.lang.Object);
}
```

## `com.google.common.collect.ObjectArrays`

```java
public final class com.google.common.collect.ObjectArrays {
  public static <T> T[] newArray(java.lang.Class<T>, int);
  public static <T> T[] newArray(T[], int);
  public static <T> T[] concat(T[], T[], java.lang.Class<T>);
  public static <T> T[] concat(T, T[]);
  public static <T> T[] concat(T[], T);
}
```

## `com.google.common.collect.Ordering`

```java
public abstract class com.google.common.collect.Ordering<T> implements java.util.Comparator<T> {
  public static <C extends java.lang.Comparable> com.google.common.collect.Ordering<C> natural();
  public static <T> com.google.common.collect.Ordering<T> from(java.util.Comparator<T>);
  public static <T> com.google.common.collect.Ordering<T> from(com.google.common.collect.Ordering<T>);
  public static <T> com.google.common.collect.Ordering<T> explicit(java.util.List<T>);
  public static <T> com.google.common.collect.Ordering<T> explicit(T, T...);
  public static com.google.common.collect.Ordering<java.lang.Object> allEqual();
  public static com.google.common.collect.Ordering<java.lang.Object> usingToString();
  public static com.google.common.collect.Ordering<java.lang.Object> arbitrary();
  public <S extends T> com.google.common.collect.Ordering<S> reverse();
  public <S extends T> com.google.common.collect.Ordering<S> nullsFirst();
  public <S extends T> com.google.common.collect.Ordering<S> nullsLast();
  public <F> com.google.common.collect.Ordering<F> onResultOf(com.google.common.base.Function<F, ? extends T>);
  public <U extends T> com.google.common.collect.Ordering<U> compound(java.util.Comparator<? super U>);
  public static <T> com.google.common.collect.Ordering<T> compound(java.lang.Iterable<? extends java.util.Comparator<? super T>>);
  public <S extends T> com.google.common.collect.Ordering<java.lang.Iterable<S>> lexicographical();
  public abstract int compare(T, T);
  public <E extends T> E min(java.util.Iterator<E>);
  public <E extends T> E min(java.lang.Iterable<E>);
  public <E extends T> E min(E, E);
  public <E extends T> E min(E, E, E, E...);
  public <E extends T> E max(java.util.Iterator<E>);
  public <E extends T> E max(java.lang.Iterable<E>);
  public <E extends T> E max(E, E);
  public <E extends T> E max(E, E, E, E...);
  public <E extends T> java.util.List<E> leastOf(java.lang.Iterable<E>, int);
  public <E extends T> java.util.List<E> leastOf(java.util.Iterator<E>, int);
  public <E extends T> java.util.List<E> greatestOf(java.lang.Iterable<E>, int);
  public <E extends T> java.util.List<E> greatestOf(java.util.Iterator<E>, int);
  public <E extends T> java.util.List<E> sortedCopy(java.lang.Iterable<E>);
  public <E extends T> com.google.common.collect.ImmutableList<E> immutableSortedCopy(java.lang.Iterable<E>);
  public boolean isOrdered(java.lang.Iterable<? extends T>);
  public boolean isStrictlyOrdered(java.lang.Iterable<? extends T>);
  public int binarySearch(java.util.List<? extends T>, T);
}
```

## `com.google.common.collect.PeekingIterator`

```java
public interface com.google.common.collect.PeekingIterator<E> extends java.util.Iterator<E> {
  public abstract E peek();
  public abstract E next();
  public abstract void remove();
}
```

## `com.google.common.collect.Queues`

```java
public final class com.google.common.collect.Queues {
  public static <E> java.util.concurrent.ArrayBlockingQueue<E> newArrayBlockingQueue(int);
  public static <E> java.util.ArrayDeque<E> newArrayDeque();
  public static <E> java.util.ArrayDeque<E> newArrayDeque(java.lang.Iterable<? extends E>);
  public static <E> java.util.concurrent.ConcurrentLinkedQueue<E> newConcurrentLinkedQueue();
  public static <E> java.util.concurrent.ConcurrentLinkedQueue<E> newConcurrentLinkedQueue(java.lang.Iterable<? extends E>);
  public static <E> java.util.concurrent.LinkedBlockingDeque<E> newLinkedBlockingDeque();
  public static <E> java.util.concurrent.LinkedBlockingDeque<E> newLinkedBlockingDeque(int);
  public static <E> java.util.concurrent.LinkedBlockingDeque<E> newLinkedBlockingDeque(java.lang.Iterable<? extends E>);
  public static <E> java.util.concurrent.LinkedBlockingQueue<E> newLinkedBlockingQueue();
  public static <E> java.util.concurrent.LinkedBlockingQueue<E> newLinkedBlockingQueue(int);
  public static <E> java.util.concurrent.LinkedBlockingQueue<E> newLinkedBlockingQueue(java.lang.Iterable<? extends E>);
  public static <E extends java.lang.Comparable> java.util.concurrent.PriorityBlockingQueue<E> newPriorityBlockingQueue();
  public static <E extends java.lang.Comparable> java.util.concurrent.PriorityBlockingQueue<E> newPriorityBlockingQueue(java.lang.Iterable<? extends E>);
  public static <E extends java.lang.Comparable> java.util.PriorityQueue<E> newPriorityQueue();
  public static <E extends java.lang.Comparable> java.util.PriorityQueue<E> newPriorityQueue(java.lang.Iterable<? extends E>);
  public static <E> java.util.concurrent.SynchronousQueue<E> newSynchronousQueue();
  public static <E> int drain(java.util.concurrent.BlockingQueue<E>, java.util.Collection<? super E>, int, java.time.Duration) throws java.lang.InterruptedException;
  public static <E> int drain(java.util.concurrent.BlockingQueue<E>, java.util.Collection<? super E>, int, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public static <E> int drainUninterruptibly(java.util.concurrent.BlockingQueue<E>, java.util.Collection<? super E>, int, java.time.Duration);
  public static <E> int drainUninterruptibly(java.util.concurrent.BlockingQueue<E>, java.util.Collection<? super E>, int, long, java.util.concurrent.TimeUnit);
  public static <E> java.util.Queue<E> synchronizedQueue(java.util.Queue<E>);
  public static <E> java.util.Deque<E> synchronizedDeque(java.util.Deque<E>);
}
```

## `com.google.common.collect.Range`

```java
public final class com.google.common.collect.Range<C extends java.lang.Comparable> extends com.google.common.collect.RangeGwtSerializationDependencies implements com.google.common.base.Predicate<C>, java.io.Serializable {
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.Range<C> open(C, C);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.Range<C> closed(C, C);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.Range<C> closedOpen(C, C);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.Range<C> openClosed(C, C);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.Range<C> range(C, com.google.common.collect.BoundType, C, com.google.common.collect.BoundType);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.Range<C> lessThan(C);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.Range<C> atMost(C);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.Range<C> upTo(C, com.google.common.collect.BoundType);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.Range<C> greaterThan(C);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.Range<C> atLeast(C);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.Range<C> downTo(C, com.google.common.collect.BoundType);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.Range<C> all();
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.Range<C> singleton(C);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.Range<C> encloseAll(java.lang.Iterable<C>);
  public boolean hasLowerBound();
  public C lowerEndpoint();
  public com.google.common.collect.BoundType lowerBoundType();
  public boolean hasUpperBound();
  public C upperEndpoint();
  public com.google.common.collect.BoundType upperBoundType();
  public boolean isEmpty();
  public boolean contains(C);
  public boolean apply(C);
  public boolean test(C);
  public boolean containsAll(java.lang.Iterable<? extends C>);
  public boolean encloses(com.google.common.collect.Range<C>);
  public boolean isConnected(com.google.common.collect.Range<C>);
  public com.google.common.collect.Range<C> intersection(com.google.common.collect.Range<C>);
  public com.google.common.collect.Range<C> gap(com.google.common.collect.Range<C>);
  public com.google.common.collect.Range<C> span(com.google.common.collect.Range<C>);
  public com.google.common.collect.Range<C> canonical(com.google.common.collect.DiscreteDomain<C>);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public boolean test(java.lang.Object);
  public boolean apply(java.lang.Object);
}
```

## `com.google.common.collect.RangeMap`

```java
public interface com.google.common.collect.RangeMap<K extends java.lang.Comparable, V> {
  public abstract V get(K);
  public abstract java.util.Map$Entry<com.google.common.collect.Range<K>, V> getEntry(K);
  public abstract com.google.common.collect.Range<K> span();
  public abstract void put(com.google.common.collect.Range<K>, V);
  public abstract void putCoalescing(com.google.common.collect.Range<K>, V);
  public abstract void putAll(com.google.common.collect.RangeMap<K, ? extends V>);
  public abstract void clear();
  public abstract void remove(com.google.common.collect.Range<K>);
  public abstract void merge(com.google.common.collect.Range<K>, V, java.util.function.BiFunction<? super V, ? super V, ? extends V>);
  public abstract java.util.Map<com.google.common.collect.Range<K>, V> asMapOfRanges();
  public abstract java.util.Map<com.google.common.collect.Range<K>, V> asDescendingMapOfRanges();
  public abstract com.google.common.collect.RangeMap<K, V> subRangeMap(com.google.common.collect.Range<K>);
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
  public abstract java.lang.String toString();
}
```

## `com.google.common.collect.RangeSet`

```java
public interface com.google.common.collect.RangeSet<C extends java.lang.Comparable> {
  public abstract boolean contains(C);
  public abstract com.google.common.collect.Range<C> rangeContaining(C);
  public abstract boolean intersects(com.google.common.collect.Range<C>);
  public abstract boolean encloses(com.google.common.collect.Range<C>);
  public abstract boolean enclosesAll(com.google.common.collect.RangeSet<C>);
  public default boolean enclosesAll(java.lang.Iterable<com.google.common.collect.Range<C>>);
  public abstract boolean isEmpty();
  public abstract com.google.common.collect.Range<C> span();
  public abstract java.util.Set<com.google.common.collect.Range<C>> asRanges();
  public abstract java.util.Set<com.google.common.collect.Range<C>> asDescendingSetOfRanges();
  public abstract com.google.common.collect.RangeSet<C> complement();
  public abstract com.google.common.collect.RangeSet<C> subRangeSet(com.google.common.collect.Range<C>);
  public abstract void add(com.google.common.collect.Range<C>);
  public abstract void remove(com.google.common.collect.Range<C>);
  public abstract void clear();
  public abstract void addAll(com.google.common.collect.RangeSet<C>);
  public default void addAll(java.lang.Iterable<com.google.common.collect.Range<C>>);
  public abstract void removeAll(com.google.common.collect.RangeSet<C>);
  public default void removeAll(java.lang.Iterable<com.google.common.collect.Range<C>>);
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
  public abstract java.lang.String toString();
}
```

## `com.google.common.collect.RowSortedTable`

```java
public interface com.google.common.collect.RowSortedTable<R, C, V> extends com.google.common.collect.Table<R, C, V> {
  public abstract java.util.SortedSet<R> rowKeySet();
  public abstract java.util.SortedMap<R, java.util.Map<C, V>> rowMap();
  public default java.util.Map rowMap();
  public default java.util.Set rowKeySet();
}
```

## `com.google.common.collect.SetMultimap`

```java
public interface com.google.common.collect.SetMultimap<K, V> extends com.google.common.collect.Multimap<K, V> {
  public abstract java.util.Set<V> get(K);
  public abstract java.util.Set<V> removeAll(java.lang.Object);
  public abstract java.util.Set<V> replaceValues(K, java.lang.Iterable<? extends V>);
  public abstract java.util.Set<java.util.Map$Entry<K, V>> entries();
  public abstract java.util.Map<K, java.util.Collection<V>> asMap();
  public abstract boolean equals(java.lang.Object);
  public default java.util.Collection entries();
  public default java.util.Collection get(java.lang.Object);
  public default java.util.Collection removeAll(java.lang.Object);
  public default java.util.Collection replaceValues(java.lang.Object, java.lang.Iterable);
}
```

## `com.google.common.collect.Sets`

```java
public final class com.google.common.collect.Sets {
  public static <E extends java.lang.Enum<E>> com.google.common.collect.ImmutableSet<E> immutableEnumSet(E, E...);
  public static <E extends java.lang.Enum<E>> com.google.common.collect.ImmutableSet<E> immutableEnumSet(java.lang.Iterable<E>);
  public static <E extends java.lang.Enum<E>> java.util.stream.Collector<E, ?, com.google.common.collect.ImmutableSet<E>> toImmutableEnumSet();
  public static <E extends java.lang.Enum<E>> java.util.EnumSet<E> newEnumSet(java.lang.Iterable<E>, java.lang.Class<E>);
  public static <E> java.util.HashSet<E> newHashSet();
  public static <E> java.util.HashSet<E> newHashSet(E...);
  public static <E> java.util.HashSet<E> newHashSet(java.lang.Iterable<? extends E>);
  public static <E> java.util.HashSet<E> newHashSet(java.util.Iterator<? extends E>);
  public static <E> java.util.HashSet<E> newHashSetWithExpectedSize(int);
  public static <E> java.util.Set<E> newConcurrentHashSet();
  public static <E> java.util.Set<E> newConcurrentHashSet(java.lang.Iterable<? extends E>);
  public static <E> java.util.LinkedHashSet<E> newLinkedHashSet();
  public static <E> java.util.LinkedHashSet<E> newLinkedHashSet(java.lang.Iterable<? extends E>);
  public static <E> java.util.LinkedHashSet<E> newLinkedHashSetWithExpectedSize(int);
  public static <E extends java.lang.Comparable> java.util.TreeSet<E> newTreeSet();
  public static <E extends java.lang.Comparable> java.util.TreeSet<E> newTreeSet(java.lang.Iterable<? extends E>);
  public static <E> java.util.TreeSet<E> newTreeSet(java.util.Comparator<? super E>);
  public static <E> java.util.Set<E> newIdentityHashSet();
  public static <E> java.util.concurrent.CopyOnWriteArraySet<E> newCopyOnWriteArraySet();
  public static <E> java.util.concurrent.CopyOnWriteArraySet<E> newCopyOnWriteArraySet(java.lang.Iterable<? extends E>);
  public static <E extends java.lang.Enum<E>> java.util.EnumSet<E> complementOf(java.util.Collection<E>);
  public static <E extends java.lang.Enum<E>> java.util.EnumSet<E> complementOf(java.util.Collection<E>, java.lang.Class<E>);
  public static <E> java.util.Set<E> newSetFromMap(java.util.Map<E, java.lang.Boolean>);
  public static <E> com.google.common.collect.Sets$SetView<E> union(java.util.Set<? extends E>, java.util.Set<? extends E>);
  public static <E> com.google.common.collect.Sets$SetView<E> intersection(java.util.Set<E>, java.util.Set<?>);
  public static <E> com.google.common.collect.Sets$SetView<E> difference(java.util.Set<E>, java.util.Set<?>);
  public static <E> com.google.common.collect.Sets$SetView<E> symmetricDifference(java.util.Set<? extends E>, java.util.Set<? extends E>);
  public static <E> java.util.Set<E> filter(java.util.Set<E>, com.google.common.base.Predicate<? super E>);
  public static <E> java.util.SortedSet<E> filter(java.util.SortedSet<E>, com.google.common.base.Predicate<? super E>);
  public static <E> java.util.NavigableSet<E> filter(java.util.NavigableSet<E>, com.google.common.base.Predicate<? super E>);
  public static <B> java.util.Set<java.util.List<B>> cartesianProduct(java.util.List<? extends java.util.Set<? extends B>>);
  public static <B> java.util.Set<java.util.List<B>> cartesianProduct(java.util.Set<? extends B>...);
  public static <E> java.util.Set<java.util.Set<E>> powerSet(java.util.Set<E>);
  public static <E> java.util.Set<java.util.Set<E>> combinations(java.util.Set<E>, int);
  public static <E> java.util.NavigableSet<E> unmodifiableNavigableSet(java.util.NavigableSet<E>);
  public static <E> java.util.NavigableSet<E> synchronizedNavigableSet(java.util.NavigableSet<E>);
  public static <K extends java.lang.Comparable<? super K>> java.util.NavigableSet<K> subSet(java.util.NavigableSet<K>, com.google.common.collect.Range<K>);
}
```

## `com.google.common.collect.Sets$SetView`

```java
public abstract class com.google.common.collect.Sets$SetView<E> extends java.util.AbstractSet<E> {
  public com.google.common.collect.ImmutableSet<E> immutableCopy();
  public <S extends java.util.Set<E>> S copyInto(S);
  public final boolean add(E);
  public final boolean remove(java.lang.Object);
  public final boolean addAll(java.util.Collection<? extends E>);
  public final boolean removeAll(java.util.Collection<?>);
  public final boolean removeIf(java.util.function.Predicate<? super E>);
  public final boolean retainAll(java.util.Collection<?>);
  public final void clear();
  public abstract com.google.common.collect.UnmodifiableIterator<E> iterator();
  public java.util.Iterator iterator();
}
```

## `com.google.common.collect.SortedMapDifference`

```java
public interface com.google.common.collect.SortedMapDifference<K, V> extends com.google.common.collect.MapDifference<K, V> {
  public abstract java.util.SortedMap<K, V> entriesOnlyOnLeft();
  public abstract java.util.SortedMap<K, V> entriesOnlyOnRight();
  public abstract java.util.SortedMap<K, V> entriesInCommon();
  public abstract java.util.SortedMap<K, com.google.common.collect.MapDifference$ValueDifference<V>> entriesDiffering();
  public default java.util.Map entriesDiffering();
  public default java.util.Map entriesInCommon();
  public default java.util.Map entriesOnlyOnRight();
  public default java.util.Map entriesOnlyOnLeft();
}
```

## `com.google.common.collect.SortedMultiset`

```java
public interface com.google.common.collect.SortedMultiset<E> extends com.google.common.collect.SortedMultisetBridge<E>, com.google.common.collect.SortedIterable<E> {
  public abstract java.util.Comparator<? super E> comparator();
  public abstract com.google.common.collect.Multiset$Entry<E> firstEntry();
  public abstract com.google.common.collect.Multiset$Entry<E> lastEntry();
  public abstract com.google.common.collect.Multiset$Entry<E> pollFirstEntry();
  public abstract com.google.common.collect.Multiset$Entry<E> pollLastEntry();
  public abstract java.util.NavigableSet<E> elementSet();
  public abstract java.util.Set<com.google.common.collect.Multiset$Entry<E>> entrySet();
  public abstract java.util.Iterator<E> iterator();
  public abstract com.google.common.collect.SortedMultiset<E> descendingMultiset();
  public abstract com.google.common.collect.SortedMultiset<E> headMultiset(E, com.google.common.collect.BoundType);
  public abstract com.google.common.collect.SortedMultiset<E> subMultiset(E, com.google.common.collect.BoundType, E, com.google.common.collect.BoundType);
  public abstract com.google.common.collect.SortedMultiset<E> tailMultiset(E, com.google.common.collect.BoundType);
  public default java.util.SortedSet elementSet();
  public default java.util.Set elementSet();
}
```

## `com.google.common.collect.SortedSetMultimap`

```java
public interface com.google.common.collect.SortedSetMultimap<K, V> extends com.google.common.collect.SetMultimap<K, V> {
  public abstract java.util.SortedSet<V> get(K);
  public abstract java.util.SortedSet<V> removeAll(java.lang.Object);
  public abstract java.util.SortedSet<V> replaceValues(K, java.lang.Iterable<? extends V>);
  public abstract java.util.Map<K, java.util.Collection<V>> asMap();
  public abstract java.util.Comparator<? super V> valueComparator();
  public default java.util.Set replaceValues(java.lang.Object, java.lang.Iterable);
  public default java.util.Set removeAll(java.lang.Object);
  public default java.util.Set get(java.lang.Object);
  public default java.util.Collection get(java.lang.Object);
  public default java.util.Collection removeAll(java.lang.Object);
  public default java.util.Collection replaceValues(java.lang.Object, java.lang.Iterable);
}
```

## `com.google.common.collect.Streams`

```java
public final class com.google.common.collect.Streams {
  public static <T> java.util.stream.Stream<T> stream(java.lang.Iterable<T>);
  public static <T> java.util.stream.Stream<T> stream(java.util.Collection<T>);
  public static <T> java.util.stream.Stream<T> stream(java.util.Iterator<T>);
  public static <T> java.util.stream.Stream<T> stream(com.google.common.base.Optional<T>);
  public static <T> java.util.stream.Stream<T> stream(java.util.Optional<T>);
  public static java.util.stream.IntStream stream(java.util.OptionalInt);
  public static java.util.stream.LongStream stream(java.util.OptionalLong);
  public static java.util.stream.DoubleStream stream(java.util.OptionalDouble);
  public static <T> java.util.stream.Stream<T> concat(java.util.stream.Stream<? extends T>...);
  public static java.util.stream.IntStream concat(java.util.stream.IntStream...);
  public static java.util.stream.LongStream concat(java.util.stream.LongStream...);
  public static java.util.stream.DoubleStream concat(java.util.stream.DoubleStream...);
  public static <A, B, R> java.util.stream.Stream<R> zip(java.util.stream.Stream<A>, java.util.stream.Stream<B>, java.util.function.BiFunction<? super A, ? super B, R>);
  public static <A, B> void forEachPair(java.util.stream.Stream<A>, java.util.stream.Stream<B>, java.util.function.BiConsumer<? super A, ? super B>);
  public static <T, R> java.util.stream.Stream<R> mapWithIndex(java.util.stream.Stream<T>, com.google.common.collect.Streams$FunctionWithIndex<? super T, ? extends R>);
  public static <R> java.util.stream.Stream<R> mapWithIndex(java.util.stream.IntStream, com.google.common.collect.Streams$IntFunctionWithIndex<R>);
  public static <R> java.util.stream.Stream<R> mapWithIndex(java.util.stream.LongStream, com.google.common.collect.Streams$LongFunctionWithIndex<R>);
  public static <R> java.util.stream.Stream<R> mapWithIndex(java.util.stream.DoubleStream, com.google.common.collect.Streams$DoubleFunctionWithIndex<R>);
  public static <T> java.util.Optional<T> findLast(java.util.stream.Stream<T>);
  public static java.util.OptionalInt findLast(java.util.stream.IntStream);
  public static java.util.OptionalLong findLast(java.util.stream.LongStream);
  public static java.util.OptionalDouble findLast(java.util.stream.DoubleStream);
}
```

## `com.google.common.collect.Streams$DoubleFunctionWithIndex`

```java
public interface com.google.common.collect.Streams$DoubleFunctionWithIndex<R> {
  public abstract R apply(double, long);
}
```

## `com.google.common.collect.Streams$FunctionWithIndex`

```java
public interface com.google.common.collect.Streams$FunctionWithIndex<T, R> {
  public abstract R apply(T, long);
}
```

## `com.google.common.collect.Streams$IntFunctionWithIndex`

```java
public interface com.google.common.collect.Streams$IntFunctionWithIndex<R> {
  public abstract R apply(int, long);
}
```

## `com.google.common.collect.Streams$LongFunctionWithIndex`

```java
public interface com.google.common.collect.Streams$LongFunctionWithIndex<R> {
  public abstract R apply(long, long);
}
```

## `com.google.common.collect.Table`

```java
public interface com.google.common.collect.Table<R, C, V> {
  public abstract boolean contains(java.lang.Object, java.lang.Object);
  public abstract boolean containsRow(java.lang.Object);
  public abstract boolean containsColumn(java.lang.Object);
  public abstract boolean containsValue(java.lang.Object);
  public abstract V get(java.lang.Object, java.lang.Object);
  public abstract boolean isEmpty();
  public abstract int size();
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
  public abstract void clear();
  public abstract V put(R, C, V);
  public abstract void putAll(com.google.common.collect.Table<? extends R, ? extends C, ? extends V>);
  public abstract V remove(java.lang.Object, java.lang.Object);
  public abstract java.util.Map<C, V> row(R);
  public abstract java.util.Map<R, V> column(C);
  public abstract java.util.Set<com.google.common.collect.Table$Cell<R, C, V>> cellSet();
  public abstract java.util.Set<R> rowKeySet();
  public abstract java.util.Set<C> columnKeySet();
  public abstract java.util.Collection<V> values();
  public abstract java.util.Map<R, java.util.Map<C, V>> rowMap();
  public abstract java.util.Map<C, java.util.Map<R, V>> columnMap();
}
```

## `com.google.common.collect.Table$Cell`

```java
public interface com.google.common.collect.Table$Cell<R, C, V> {
  public abstract R getRowKey();
  public abstract C getColumnKey();
  public abstract V getValue();
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
}
```

## `com.google.common.collect.Tables`

```java
public final class com.google.common.collect.Tables {
  public static <T, R, C, V, I extends com.google.common.collect.Table<R, C, V>> java.util.stream.Collector<T, ?, I> toTable(java.util.function.Function<? super T, ? extends R>, java.util.function.Function<? super T, ? extends C>, java.util.function.Function<? super T, ? extends V>, java.util.function.Supplier<I>);
  public static <T, R, C, V, I extends com.google.common.collect.Table<R, C, V>> java.util.stream.Collector<T, ?, I> toTable(java.util.function.Function<? super T, ? extends R>, java.util.function.Function<? super T, ? extends C>, java.util.function.Function<? super T, ? extends V>, java.util.function.BinaryOperator<V>, java.util.function.Supplier<I>);
  public static <R, C, V> com.google.common.collect.Table$Cell<R, C, V> immutableCell(R, C, V);
  public static <R, C, V> com.google.common.collect.Table<C, R, V> transpose(com.google.common.collect.Table<R, C, V>);
  public static <R, C, V> com.google.common.collect.Table<R, C, V> newCustomTable(java.util.Map<R, java.util.Map<C, V>>, com.google.common.base.Supplier<? extends java.util.Map<C, V>>);
  public static <R, C, V1, V2> com.google.common.collect.Table<R, C, V2> transformValues(com.google.common.collect.Table<R, C, V1>, com.google.common.base.Function<? super V1, V2>);
  public static <R, C, V> com.google.common.collect.Table<R, C, V> unmodifiableTable(com.google.common.collect.Table<? extends R, ? extends C, ? extends V>);
  public static <R, C, V> com.google.common.collect.RowSortedTable<R, C, V> unmodifiableRowSortedTable(com.google.common.collect.RowSortedTable<R, ? extends C, ? extends V>);
  public static <R, C, V> com.google.common.collect.Table<R, C, V> synchronizedTable(com.google.common.collect.Table<R, C, V>);
}
```

## `com.google.common.collect.TreeBasedTable`

```java
public class com.google.common.collect.TreeBasedTable<R, C, V> extends com.google.common.collect.StandardRowSortedTable<R, C, V> {
  public static <R extends java.lang.Comparable, C extends java.lang.Comparable, V> com.google.common.collect.TreeBasedTable<R, C, V> create();
  public static <R, C, V> com.google.common.collect.TreeBasedTable<R, C, V> create(java.util.Comparator<? super R>, java.util.Comparator<? super C>);
  public static <R, C, V> com.google.common.collect.TreeBasedTable<R, C, V> create(com.google.common.collect.TreeBasedTable<R, C, ? extends V>);
  public final java.util.Comparator<? super R> rowComparator();
  public java.util.Comparator<? super C> columnComparator();
  public java.util.SortedMap<C, V> row(R);
  public java.util.SortedMap rowMap();
  public java.util.SortedSet rowKeySet();
  public java.util.Map row(java.lang.Object);
  public java.util.Map columnMap();
  public java.util.Collection values();
  public java.util.Set columnKeySet();
  public java.util.Map column(java.lang.Object);
  public java.util.Set cellSet();
  public java.lang.Object remove(java.lang.Object, java.lang.Object);
  public java.lang.Object put(java.lang.Object, java.lang.Object, java.lang.Object);
  public void clear();
  public int size();
  public boolean isEmpty();
  public java.lang.Object get(java.lang.Object, java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public boolean containsRow(java.lang.Object);
  public boolean containsColumn(java.lang.Object);
  public boolean contains(java.lang.Object, java.lang.Object);
  public java.lang.String toString();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public void putAll(com.google.common.collect.Table);
}
```

## `com.google.common.collect.TreeMultimap`

```java
public class com.google.common.collect.TreeMultimap<K, V> extends com.google.common.collect.AbstractSortedKeySortedSetMultimap<K, V> {
  public static <K extends java.lang.Comparable, V extends java.lang.Comparable> com.google.common.collect.TreeMultimap<K, V> create();
  public static <K, V> com.google.common.collect.TreeMultimap<K, V> create(java.util.Comparator<? super K>, java.util.Comparator<? super V>);
  public static <K extends java.lang.Comparable, V extends java.lang.Comparable> com.google.common.collect.TreeMultimap<K, V> create(com.google.common.collect.Multimap<? extends K, ? extends V>);
  public java.util.Comparator<? super K> keyComparator();
  public java.util.Comparator<? super V> valueComparator();
  public java.util.NavigableSet<V> get(K);
  public java.util.NavigableSet<K> keySet();
  public java.util.NavigableMap<K, java.util.Collection<V>> asMap();
  public java.util.SortedSet keySet();
  public java.util.SortedMap asMap();
  public java.util.Collection values();
  public java.util.Map asMap();
  public java.util.SortedSet replaceValues(java.lang.Object, java.lang.Iterable);
  public java.util.SortedSet removeAll(java.lang.Object);
  public java.util.SortedSet get(java.lang.Object);
  public java.util.Set get(java.lang.Object);
  public java.util.Set keySet();
  public java.util.Collection get(java.lang.Object);
  public boolean equals(java.lang.Object);
  public boolean put(java.lang.Object, java.lang.Object);
  public java.util.Set entries();
  public void forEach(java.util.function.BiConsumer);
  public void clear();
  public boolean containsKey(java.lang.Object);
  public int size();
  public java.lang.String toString();
  public int hashCode();
  public com.google.common.collect.Multiset keys();
  public boolean putAll(com.google.common.collect.Multimap);
  public boolean putAll(java.lang.Object, java.lang.Iterable);
  public boolean remove(java.lang.Object, java.lang.Object);
  public boolean containsEntry(java.lang.Object, java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public boolean isEmpty();
}
```

## `com.google.common.collect.TreeMultiset`

```java
public final class com.google.common.collect.TreeMultiset<E> extends com.google.common.collect.AbstractSortedMultiset<E> implements java.io.Serializable {
  public static <E extends java.lang.Comparable> com.google.common.collect.TreeMultiset<E> create();
  public static <E> com.google.common.collect.TreeMultiset<E> create(java.util.Comparator<? super E>);
  public static <E extends java.lang.Comparable> com.google.common.collect.TreeMultiset<E> create(java.lang.Iterable<? extends E>);
  public int size();
  public int count(java.lang.Object);
  public int add(E, int);
  public int remove(java.lang.Object, int);
  public int setCount(E, int);
  public boolean setCount(E, int, int);
  public void clear();
  public void forEachEntry(java.util.function.ObjIntConsumer<? super E>);
  public java.util.Iterator<E> iterator();
  public com.google.common.collect.SortedMultiset<E> headMultiset(E, com.google.common.collect.BoundType);
  public com.google.common.collect.SortedMultiset<E> tailMultiset(E, com.google.common.collect.BoundType);
  public com.google.common.collect.SortedMultiset descendingMultiset();
  public com.google.common.collect.SortedMultiset subMultiset(java.lang.Object, com.google.common.collect.BoundType, java.lang.Object, com.google.common.collect.BoundType);
  public com.google.common.collect.Multiset$Entry pollLastEntry();
  public com.google.common.collect.Multiset$Entry pollFirstEntry();
  public com.google.common.collect.Multiset$Entry lastEntry();
  public com.google.common.collect.Multiset$Entry firstEntry();
  public java.util.Comparator comparator();
  public java.util.NavigableSet elementSet();
  public java.util.Set entrySet();
  public boolean contains(java.lang.Object);
  public boolean isEmpty();
}
```

## `com.google.common.collect.TreeRangeMap`

```java
public final class com.google.common.collect.TreeRangeMap<K extends java.lang.Comparable, V> implements com.google.common.collect.RangeMap<K, V> {
  public static <K extends java.lang.Comparable, V> com.google.common.collect.TreeRangeMap<K, V> create();
  public static <K extends java.lang.Comparable<?>, V> com.google.common.collect.TreeRangeMap<K, V> copyOf(com.google.common.collect.RangeMap<K, ? extends V>);
  public V get(K);
  public java.util.Map$Entry<com.google.common.collect.Range<K>, V> getEntry(K);
  public void put(com.google.common.collect.Range<K>, V);
  public void putCoalescing(com.google.common.collect.Range<K>, V);
  public void putAll(com.google.common.collect.RangeMap<K, ? extends V>);
  public void clear();
  public com.google.common.collect.Range<K> span();
  public void remove(com.google.common.collect.Range<K>);
  public void merge(com.google.common.collect.Range<K>, V, java.util.function.BiFunction<? super V, ? super V, ? extends V>);
  public java.util.Map<com.google.common.collect.Range<K>, V> asMapOfRanges();
  public java.util.Map<com.google.common.collect.Range<K>, V> asDescendingMapOfRanges();
  public com.google.common.collect.RangeMap<K, V> subRangeMap(com.google.common.collect.Range<K>);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.google.common.collect.TreeRangeSet`

```java
public class com.google.common.collect.TreeRangeSet<C extends java.lang.Comparable<?>> extends com.google.common.collect.AbstractRangeSet<C> implements java.io.Serializable {
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.TreeRangeSet<C> create();
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.TreeRangeSet<C> create(com.google.common.collect.RangeSet<C>);
  public static <C extends java.lang.Comparable<?>> com.google.common.collect.TreeRangeSet<C> create(java.lang.Iterable<com.google.common.collect.Range<C>>);
  public java.util.Set<com.google.common.collect.Range<C>> asRanges();
  public java.util.Set<com.google.common.collect.Range<C>> asDescendingSetOfRanges();
  public com.google.common.collect.Range<C> rangeContaining(C);
  public boolean intersects(com.google.common.collect.Range<C>);
  public boolean encloses(com.google.common.collect.Range<C>);
  public com.google.common.collect.Range<C> span();
  public void add(com.google.common.collect.Range<C>);
  public void remove(com.google.common.collect.Range<C>);
  public com.google.common.collect.RangeSet<C> complement();
  public com.google.common.collect.RangeSet<C> subRangeSet(com.google.common.collect.Range<C>);
  public boolean equals(java.lang.Object);
  public void removeAll(com.google.common.collect.RangeSet);
  public void addAll(com.google.common.collect.RangeSet);
  public boolean enclosesAll(com.google.common.collect.RangeSet);
  public void clear();
  public boolean isEmpty();
  public boolean contains(java.lang.Comparable);
}
```

## `com.google.common.collect.TreeTraverser`

```java
public abstract class com.google.common.collect.TreeTraverser<T> {
  public com.google.common.collect.TreeTraverser();
  public static <T> com.google.common.collect.TreeTraverser<T> using(com.google.common.base.Function<T, ? extends java.lang.Iterable<T>>);
  public abstract java.lang.Iterable<T> children(T);
  public final com.google.common.collect.FluentIterable<T> preOrderTraversal(T);
  public final com.google.common.collect.FluentIterable<T> postOrderTraversal(T);
  public final com.google.common.collect.FluentIterable<T> breadthFirstTraversal(T);
}
```

## `com.google.common.collect.UnmodifiableIterator`

```java
public abstract class com.google.common.collect.UnmodifiableIterator<E> implements java.util.Iterator<E> {
  public final void remove();
}
```

## `com.google.common.collect.UnmodifiableListIterator`

```java
public abstract class com.google.common.collect.UnmodifiableListIterator<E> extends com.google.common.collect.UnmodifiableIterator<E> implements java.util.ListIterator<E> {
  public final void add(E);
  public final void set(E);
}
```
