# com.feilong.lib.collection4

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.collection4.ClosureUtils`

```java
public class com.feilong.lib.collection4.ClosureUtils {
  public static <E> org.apache.commons.collections4.Closure<E> exceptionClosure();
  public static <E> org.apache.commons.collections4.Closure<E> nopClosure();
  public static <E> org.apache.commons.collections4.Closure<E> asClosure(org.apache.commons.collections4.Transformer<? super E, ?>);
  public static <E> org.apache.commons.collections4.Closure<E> forClosure(int, org.apache.commons.collections4.Closure<? super E>);
  public static <E> org.apache.commons.collections4.Closure<E> whileClosure(org.apache.commons.collections4.Predicate<? super E>, org.apache.commons.collections4.Closure<? super E>);
  public static <E> org.apache.commons.collections4.Closure<E> doWhileClosure(org.apache.commons.collections4.Closure<? super E>, org.apache.commons.collections4.Predicate<? super E>);
  public static <E> org.apache.commons.collections4.Closure<E> invokerClosure(java.lang.String);
  public static <E> org.apache.commons.collections4.Closure<E> invokerClosure(java.lang.String, java.lang.Class<?>[], java.lang.Object[]);
  public static <E> org.apache.commons.collections4.Closure<E> chainedClosure(org.apache.commons.collections4.Closure<? super E>...);
  public static <E> org.apache.commons.collections4.Closure<E> chainedClosure(java.util.Collection<? extends org.apache.commons.collections4.Closure<? super E>>);
  public static <E> org.apache.commons.collections4.Closure<E> ifClosure(org.apache.commons.collections4.Predicate<? super E>, org.apache.commons.collections4.Closure<? super E>);
  public static <E> org.apache.commons.collections4.Closure<E> ifClosure(org.apache.commons.collections4.Predicate<? super E>, org.apache.commons.collections4.Closure<? super E>, org.apache.commons.collections4.Closure<? super E>);
  public static <E> org.apache.commons.collections4.Closure<E> switchClosure(org.apache.commons.collections4.Predicate<? super E>[], org.apache.commons.collections4.Closure<? super E>[]);
  public static <E> org.apache.commons.collections4.Closure<E> switchClosure(org.apache.commons.collections4.Predicate<? super E>[], org.apache.commons.collections4.Closure<? super E>[], org.apache.commons.collections4.Closure<? super E>);
  public static <E> org.apache.commons.collections4.Closure<E> switchClosure(java.util.Map<org.apache.commons.collections4.Predicate<E>, org.apache.commons.collections4.Closure<E>>);
  public static <E> org.apache.commons.collections4.Closure<E> switchMapClosure(java.util.Map<? extends E, org.apache.commons.collections4.Closure<E>>);
}
```

## `com.feilong.lib.collection4.CollectionUtils`

```java
public class com.feilong.lib.collection4.CollectionUtils {
  public static <T> java.util.Collection<T> emptyCollection();
  public static <T> java.util.Collection<T> emptyIfNull(java.util.Collection<T>);
  public static <O> java.util.Collection<O> union(java.lang.Iterable<? extends O>, java.lang.Iterable<? extends O>);
  public static <O> java.util.Collection<O> intersection(java.lang.Iterable<? extends O>, java.lang.Iterable<? extends O>);
  public static <O> java.util.Collection<O> disjunction(java.lang.Iterable<? extends O>, java.lang.Iterable<? extends O>);
  public static boolean containsAll(java.util.Collection<?>, java.util.Collection<?>);
  public static <O> java.util.Map<O, java.lang.Integer> getCardinalityMap(java.lang.Iterable<? extends O>);
  public static boolean isSubCollection(java.util.Collection<?>, java.util.Collection<?>);
  public static boolean isProperSubCollection(java.util.Collection<?>, java.util.Collection<?>);
  public static boolean isEqualCollection(java.util.Collection<?>, java.util.Collection<?>);
  public static <E> boolean isEqualCollection(java.util.Collection<? extends E>, java.util.Collection<? extends E>, org.apache.commons.collections4.Equator<? super E>);
  public static <T> boolean filter(java.lang.Iterable<T>, org.apache.commons.collections4.Predicate<? super T>);
  public static <T> boolean filterInverse(java.lang.Iterable<T>, org.apache.commons.collections4.Predicate<? super T>);
  public static <C> void transform(java.util.Collection<C>, org.apache.commons.collections4.Transformer<? super C, ? extends C>);
  public static <O> java.util.Collection<O> select(java.lang.Iterable<? extends O>, org.apache.commons.collections4.Predicate<? super O>);
  public static <O, R extends java.util.Collection<? super O>> R select(java.lang.Iterable<? extends O>, org.apache.commons.collections4.Predicate<? super O>, R);
  public static <O, R extends java.util.Collection<? super O>> R select(java.lang.Iterable<? extends O>, org.apache.commons.collections4.Predicate<? super O>, R, R);
  public static <O> java.util.Collection<O> selectRejected(java.lang.Iterable<? extends O>, org.apache.commons.collections4.Predicate<? super O>);
  public static <O, R extends java.util.Collection<? super O>> R selectRejected(java.lang.Iterable<? extends O>, org.apache.commons.collections4.Predicate<? super O>, R);
  public static <I, O> java.util.Collection<O> collect(java.lang.Iterable<I>, org.apache.commons.collections4.Transformer<? super I, ? extends O>);
  public static <I, O> java.util.Collection<O> collect(java.util.Iterator<I>, org.apache.commons.collections4.Transformer<? super I, ? extends O>);
  public static <I, O, R extends java.util.Collection<? super O>> R collect(java.lang.Iterable<? extends I>, org.apache.commons.collections4.Transformer<? super I, ? extends O>, R);
  public static <I, O, R extends java.util.Collection<? super O>> R collect(java.util.Iterator<? extends I>, org.apache.commons.collections4.Transformer<? super I, ? extends O>, R);
  public static <T> boolean addIgnoreNull(java.util.Collection<T>, T);
  public static <C> boolean addAll(java.util.Collection<C>, java.lang.Iterable<? extends C>);
  public static <C> boolean addAll(java.util.Collection<C>, java.util.Iterator<? extends C>);
  public static <C> boolean addAll(java.util.Collection<C>, java.util.Enumeration<? extends C>);
  public static <C> boolean addAll(java.util.Collection<C>, C...);
  public static java.lang.Object get(java.lang.Object, int);
  public static <K, V> java.util.Map$Entry<K, V> get(java.util.Map<K, V>, int);
  public static int size(java.lang.Object);
  public static boolean sizeIsEmpty(java.lang.Object);
  public static boolean isEmpty(java.util.Collection<?>);
  public static boolean isNotEmpty(java.util.Collection<?>);
  public static void reverseArray(java.lang.Object[]);
  public static <C> java.util.Collection<C> retainAll(java.util.Collection<C>, java.util.Collection<?>);
  public static <E> java.util.Collection<E> retainAll(java.lang.Iterable<E>, java.lang.Iterable<? extends E>, org.apache.commons.collections4.Equator<? super E>);
  public static <E> java.util.Collection<E> removeAll(java.util.Collection<E>, java.util.Collection<?>);
  public static <E> java.util.Collection<E> removeAll(java.lang.Iterable<E>, java.lang.Iterable<? extends E>, org.apache.commons.collections4.Equator<? super E>);
  public static <E> E extractSingleton(java.util.Collection<E>);
}
```

## `com.feilong.lib.collection4.ComparatorUtils`

```java
public class com.feilong.lib.collection4.ComparatorUtils {
  public static <E extends java.lang.Comparable<? super E>> java.util.Comparator<E> naturalComparator();
  public static <E> java.util.Comparator<E> chainedComparator(java.util.Comparator<E>...);
  public static <E> java.util.Comparator<E> chainedComparator(java.util.Collection<java.util.Comparator<E>>);
  public static <E> java.util.Comparator<E> reversedComparator(java.util.Comparator<E>);
  public static java.util.Comparator<java.lang.Boolean> booleanComparator(boolean);
  public static <E> java.util.Comparator<E> nullLowComparator(java.util.Comparator<E>);
  public static <E> java.util.Comparator<E> nullHighComparator(java.util.Comparator<E>);
  public static <I, O> java.util.Comparator<I> transformedComparator(java.util.Comparator<O>, org.apache.commons.collections4.Transformer<? super I, ? extends O>);
  public static <E> E min(E, E, java.util.Comparator<E>);
  public static <E> E max(E, E, java.util.Comparator<E>);
}
```

## `com.feilong.lib.collection4.EnumerationUtils`

```java
public class com.feilong.lib.collection4.EnumerationUtils {
  public static <T> T get(java.util.Enumeration<T>, int);
  public static <E> java.util.List<E> toList(java.util.Enumeration<? extends E>);
  public static java.util.List<java.lang.String> toList(java.util.StringTokenizer);
}
```

## `com.feilong.lib.collection4.FunctorException`

```java
public class com.feilong.lib.collection4.FunctorException extends java.lang.RuntimeException {
  public com.feilong.lib.collection4.FunctorException();
  public com.feilong.lib.collection4.FunctorException(java.lang.String);
  public com.feilong.lib.collection4.FunctorException(java.lang.Throwable);
  public com.feilong.lib.collection4.FunctorException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.collection4.IterableUtils`

```java
public class com.feilong.lib.collection4.IterableUtils {
  public com.feilong.lib.collection4.IterableUtils();
  public static <E> void forEach(java.lang.Iterable<E>, org.apache.commons.collections4.Closure<? super E>);
  public static <E> E forEachButLast(java.lang.Iterable<E>, org.apache.commons.collections4.Closure<? super E>);
  public static <E> E find(java.lang.Iterable<E>, org.apache.commons.collections4.Predicate<? super E>);
  public static <E> int indexOf(java.lang.Iterable<E>, org.apache.commons.collections4.Predicate<? super E>);
  public static <E> boolean matchesAll(java.lang.Iterable<E>, org.apache.commons.collections4.Predicate<? super E>);
  public static <E> boolean matchesAny(java.lang.Iterable<E>, org.apache.commons.collections4.Predicate<? super E>);
  public static boolean isEmpty(java.lang.Iterable<?>);
  public static <E> boolean contains(java.lang.Iterable<E>, java.lang.Object);
  public static <E> boolean contains(java.lang.Iterable<? extends E>, E, org.apache.commons.collections4.Equator<? super E>);
  public static <T> T get(java.lang.Iterable<T>, int);
  public static <T> T first(java.lang.Iterable<T>);
  public static int size(java.lang.Iterable<?>);
  public static <E> java.util.List<E> toList(java.lang.Iterable<E>);
  public static <E> java.lang.String toString(java.lang.Iterable<E>);
  public static <E> java.lang.String toString(java.lang.Iterable<E>, org.apache.commons.collections4.Transformer<? super E, java.lang.String>);
  public static <E> java.lang.String toString(java.lang.Iterable<E>, org.apache.commons.collections4.Transformer<? super E, java.lang.String>, java.lang.String, java.lang.String, java.lang.String);
}
```

## `com.feilong.lib.collection4.IteratorUtils`

```java
public class com.feilong.lib.collection4.IteratorUtils {
  public static <E> org.apache.commons.collections4.ResettableIterator<E> emptyIterator();
  public static <E> java.util.Iterator<E> chainedIterator(java.util.Iterator<? extends E>, java.util.Iterator<? extends E>);
  public static <E> java.util.Iterator<E> chainedIterator(java.util.Iterator<? extends E>...);
  public static <E> java.util.Iterator<E> chainedIterator(java.util.Collection<java.util.Iterator<? extends E>>);
  public static <I, O> java.util.Iterator<O> transformedIterator(java.util.Iterator<? extends I>, org.apache.commons.collections4.Transformer<? super I, ? extends O>);
  public static <E> java.util.Iterator<E> filteredIterator(java.util.Iterator<? extends E>, org.apache.commons.collections4.Predicate<? super E>);
  public static com.feilong.lib.collection4.iterators.NodeListIterator nodeListIterator(org.w3c.dom.NodeList);
  public static com.feilong.lib.collection4.iterators.NodeListIterator nodeListIterator(org.w3c.dom.Node);
  public static <E> java.util.Iterator<E> asIterator(java.util.Enumeration<? extends E>);
  public static <E> java.util.Iterator<E> asIterator(java.util.Enumeration<? extends E>, java.util.Collection<? super E>);
  public static <E> java.util.Enumeration<E> asEnumeration(java.util.Iterator<? extends E>);
  public static java.lang.Object[] toArray(java.util.Iterator<?>);
  public static <E> E[] toArray(java.util.Iterator<? extends E>, java.lang.Class<E>);
  public static <E> java.util.List<E> toList(java.util.Iterator<? extends E>);
  public static <E> java.util.List<E> toList(java.util.Iterator<? extends E>, int);
  public static java.util.Iterator<?> getIterator(java.lang.Object);
  public static <E> org.apache.commons.collections4.ResettableIterator<E> singletonIterator(E);
  public static <E> void forEach(java.util.Iterator<E>, org.apache.commons.collections4.Closure<? super E>);
  public static <E> E forEachButLast(java.util.Iterator<E>, org.apache.commons.collections4.Closure<? super E>);
  public static <E> E find(java.util.Iterator<E>, org.apache.commons.collections4.Predicate<? super E>);
  public static <E> int indexOf(java.util.Iterator<E>, org.apache.commons.collections4.Predicate<? super E>);
  public static <E> boolean matchesAny(java.util.Iterator<E>, org.apache.commons.collections4.Predicate<? super E>);
  public static <E> boolean matchesAll(java.util.Iterator<E>, org.apache.commons.collections4.Predicate<? super E>);
  public static boolean isEmpty(java.util.Iterator<?>);
  public static <E> boolean contains(java.util.Iterator<E>, java.lang.Object);
  public static <E> E get(java.util.Iterator<E>, int);
  public static <E> E first(java.util.Iterator<E>);
  public static int size(java.util.Iterator<?>);
  public static <E> java.lang.String toString(java.util.Iterator<E>);
  public static <E> java.lang.String toString(java.util.Iterator<E>, org.apache.commons.collections4.Transformer<? super E, java.lang.String>);
  public static <E> java.lang.String toString(java.util.Iterator<E>, org.apache.commons.collections4.Transformer<? super E, java.lang.String>, java.lang.String, java.lang.String, java.lang.String);
}
```

## `com.feilong.lib.collection4.ListUtils`

```java
public class com.feilong.lib.collection4.ListUtils {
  public static <T> java.util.List<T> emptyIfNull(java.util.List<T>);
  public static <E> java.util.List<E> intersection(java.util.List<? extends E>, java.util.List<? extends E>);
  public static <E> java.util.List<E> union(java.util.List<? extends E>, java.util.List<? extends E>);
  public static <E> java.util.List<E> select(java.util.Collection<? extends E>, org.apache.commons.collections4.Predicate<? super E>);
  public static <E> java.util.List<E> selectRejected(java.util.Collection<? extends E>, org.apache.commons.collections4.Predicate<? super E>);
  public static <E> java.util.List<E> retainAll(java.util.Collection<E>, java.util.Collection<?>);
  public static <E> java.util.List<E> removeAll(java.util.Collection<E>, java.util.Collection<?>);
  public static <E> java.util.List<E> synchronizedList(java.util.List<E>);
  public static <E> int indexOf(java.util.List<E>, org.apache.commons.collections4.Predicate<E>);
  public static <T> java.util.List<java.util.List<T>> partition(java.util.List<T>, int);
}
```

## `com.feilong.lib.collection4.MapUtils`

```java
public class com.feilong.lib.collection4.MapUtils {
  public static <K, V> V getObject(java.util.Map<? super K, V>, K);
  public static <K, V> java.util.Properties toProperties(java.util.Map<K, V>);
  public static java.util.Map<java.lang.String, java.lang.Object> toMap(java.util.ResourceBundle);
  public static <K, V> java.util.Map<V, K> invertMap(java.util.Map<K, V>);
  public static <K, V> java.util.Map<K, V> synchronizedMap(java.util.Map<K, V>);
  public static <K, V> java.util.SortedMap<K, V> synchronizedSortedMap(java.util.SortedMap<K, V>);
  public static <K, V> void populateMap(java.util.Map<K, V>, java.lang.Iterable<? extends V>, org.apache.commons.collections4.Transformer<V, K>);
  public static <K, V, E> void populateMap(java.util.Map<K, V>, java.lang.Iterable<? extends E>, org.apache.commons.collections4.Transformer<E, K>, org.apache.commons.collections4.Transformer<E, V>);
}
```

## `com.feilong.lib.collection4.PredicateUtils`

```java
public class com.feilong.lib.collection4.PredicateUtils {
  public static <T> org.apache.commons.collections4.Predicate<T> exceptionPredicate();
  public static <T> org.apache.commons.collections4.Predicate<T> truePredicate();
  public static <T> org.apache.commons.collections4.Predicate<T> falsePredicate();
  public static <T> org.apache.commons.collections4.Predicate<T> nullPredicate();
  public static <T> org.apache.commons.collections4.Predicate<T> notNullPredicate();
  public static <T> org.apache.commons.collections4.Predicate<T> equalPredicate(T);
  public static <T> org.apache.commons.collections4.Predicate<T> identityPredicate(T);
  public static org.apache.commons.collections4.Predicate<java.lang.Object> instanceofPredicate(java.lang.Class<?>);
  public static <T> org.apache.commons.collections4.Predicate<T> uniquePredicate();
  public static <T> org.apache.commons.collections4.Predicate<T> invokerPredicate(java.lang.String);
  public static <T> org.apache.commons.collections4.Predicate<T> invokerPredicate(java.lang.String, java.lang.Class<?>[], java.lang.Object[]);
  public static <T> org.apache.commons.collections4.Predicate<T> andPredicate(org.apache.commons.collections4.Predicate<? super T>, org.apache.commons.collections4.Predicate<? super T>);
  public static <T> org.apache.commons.collections4.Predicate<T> allPredicate(org.apache.commons.collections4.Predicate<? super T>...);
  public static <T> org.apache.commons.collections4.Predicate<T> allPredicate(java.util.Collection<? extends org.apache.commons.collections4.Predicate<? super T>>);
  public static <T> org.apache.commons.collections4.Predicate<T> orPredicate(org.apache.commons.collections4.Predicate<? super T>, org.apache.commons.collections4.Predicate<? super T>);
  public static <T> org.apache.commons.collections4.Predicate<T> anyPredicate(org.apache.commons.collections4.Predicate<? super T>...);
  public static <T> org.apache.commons.collections4.Predicate<T> anyPredicate(java.util.Collection<? extends org.apache.commons.collections4.Predicate<? super T>>);
  public static <T> org.apache.commons.collections4.Predicate<T> eitherPredicate(org.apache.commons.collections4.Predicate<? super T>, org.apache.commons.collections4.Predicate<? super T>);
  public static <T> org.apache.commons.collections4.Predicate<T> onePredicate(org.apache.commons.collections4.Predicate<? super T>...);
  public static <T> org.apache.commons.collections4.Predicate<T> onePredicate(java.util.Collection<? extends org.apache.commons.collections4.Predicate<? super T>>);
  public static <T> org.apache.commons.collections4.Predicate<T> neitherPredicate(org.apache.commons.collections4.Predicate<? super T>, org.apache.commons.collections4.Predicate<? super T>);
  public static <T> org.apache.commons.collections4.Predicate<T> nonePredicate(org.apache.commons.collections4.Predicate<? super T>...);
  public static <T> org.apache.commons.collections4.Predicate<T> nonePredicate(java.util.Collection<? extends org.apache.commons.collections4.Predicate<? super T>>);
  public static <T> org.apache.commons.collections4.Predicate<T> notPredicate(org.apache.commons.collections4.Predicate<? super T>);
  public static <T> org.apache.commons.collections4.Predicate<T> asPredicate(org.apache.commons.collections4.Transformer<? super T, java.lang.Boolean>);
  public static <T> org.apache.commons.collections4.Predicate<T> nullIsExceptionPredicate(org.apache.commons.collections4.Predicate<? super T>);
  public static <T> org.apache.commons.collections4.Predicate<T> nullIsFalsePredicate(org.apache.commons.collections4.Predicate<? super T>);
  public static <T> org.apache.commons.collections4.Predicate<T> nullIsTruePredicate(org.apache.commons.collections4.Predicate<? super T>);
  public static <T> org.apache.commons.collections4.Predicate<T> transformedPredicate(org.apache.commons.collections4.Transformer<? super T, ? extends T>, org.apache.commons.collections4.Predicate<? super T>);
}
```

## `com.feilong.lib.collection4.SetUtils`

```java
public class com.feilong.lib.collection4.SetUtils {
  public static <T> java.util.Set<T> emptyIfNull(java.util.Set<T>);
  public static <E> java.util.Set<E> emptySet();
  public static boolean isEqualSet(java.util.Collection<?>, java.util.Collection<?>);
  public static <E> java.util.Set<E> newIdentityHashSet();
  public static <E> java.util.Set<E> synchronizedSet(java.util.Set<E>);
  public static <E> java.util.SortedSet<E> synchronizedSortedSet(java.util.SortedSet<E>);
}
```

## `com.feilong.lib.collection4.TransformerUtils`

```java
public class com.feilong.lib.collection4.TransformerUtils {
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> exceptionTransformer();
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> nullTransformer();
  public static <T> org.apache.commons.collections4.Transformer<T, T> nopTransformer();
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> constantTransformer(O);
  public static <T> org.apache.commons.collections4.Transformer<T, T> asTransformer(org.apache.commons.collections4.Closure<? super T>);
  public static <T> org.apache.commons.collections4.Transformer<T, java.lang.Boolean> asTransformer(org.apache.commons.collections4.Predicate<? super T>);
  public static <T> org.apache.commons.collections4.Transformer<T, T> chainedTransformer(org.apache.commons.collections4.Transformer<? super T, ? extends T>...);
  public static <T> org.apache.commons.collections4.Transformer<T, T> chainedTransformer(java.util.Collection<? extends org.apache.commons.collections4.Transformer<? super T, ? extends T>>);
  public static <T> org.apache.commons.collections4.Transformer<T, T> ifTransformer(org.apache.commons.collections4.Predicate<? super T>, org.apache.commons.collections4.Transformer<? super T, ? extends T>);
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> ifTransformer(org.apache.commons.collections4.Predicate<? super I>, org.apache.commons.collections4.Transformer<? super I, ? extends O>, org.apache.commons.collections4.Transformer<? super I, ? extends O>);
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> switchTransformer(org.apache.commons.collections4.Predicate<? super I>[], org.apache.commons.collections4.Transformer<? super I, ? extends O>[]);
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> switchTransformer(org.apache.commons.collections4.Predicate<? super I>[], org.apache.commons.collections4.Transformer<? super I, ? extends O>[], org.apache.commons.collections4.Transformer<? super I, ? extends O>);
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> switchTransformer(java.util.Map<org.apache.commons.collections4.Predicate<I>, org.apache.commons.collections4.Transformer<I, O>>);
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> switchMapTransformer(java.util.Map<I, org.apache.commons.collections4.Transformer<I, O>>);
  public static <T> org.apache.commons.collections4.Transformer<java.lang.Class<? extends T>, T> instantiateTransformer();
  public static <T> org.apache.commons.collections4.Transformer<java.lang.Class<? extends T>, T> instantiateTransformer(java.lang.Class<?>[], java.lang.Object[]);
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> mapTransformer(java.util.Map<? super I, ? extends O>);
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> invokerTransformer(java.lang.String);
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> invokerTransformer(java.lang.String, java.lang.Class<?>[], java.lang.Object[]);
  public static <T> org.apache.commons.collections4.Transformer<T, java.lang.String> stringValueTransformer();
}
```
