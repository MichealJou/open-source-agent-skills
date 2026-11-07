# cn.hutool.core.stream

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.stream.CollectorUtil`

```java
public class cn.hutool.core.stream.CollectorUtil {
  public cn.hutool.core.stream.CollectorUtil();
  public static <T> java.util.stream.Collector<T, ?, java.lang.String> joining(java.lang.CharSequence);
  public static <T> java.util.stream.Collector<T, ?, java.lang.String> joining(java.lang.CharSequence, java.util.function.Function<T, ? extends java.lang.CharSequence>);
  public static <T> java.util.stream.Collector<T, ?, java.lang.String> joining(java.lang.CharSequence, java.lang.CharSequence, java.lang.CharSequence, java.util.function.Function<T, ? extends java.lang.CharSequence>);
  public static <T, K, D, A, M extends java.util.Map<K, D>> java.util.stream.Collector<T, ?, M> groupingBy(java.util.function.Function<? super T, ? extends K>, java.util.function.Supplier<M>, java.util.stream.Collector<? super T, A, D>);
  public static <T, K, A, D> java.util.stream.Collector<T, ?, java.util.Map<K, D>> groupingBy(java.util.function.Function<? super T, ? extends K>, java.util.stream.Collector<? super T, A, D>);
  public static <T, K> java.util.stream.Collector<T, ?, java.util.Map<K, java.util.List<T>>> groupingBy(java.util.function.Function<? super T, ? extends K>);
  public static <T, K, U> java.util.stream.Collector<T, ?, java.util.Map<K, U>> toMap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends U>, java.util.function.BinaryOperator<U>);
  public static <T, K, U, M extends java.util.Map<K, U>> java.util.stream.Collector<T, ?, M> toMap(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends U>, java.util.function.BinaryOperator<U>, java.util.function.Supplier<M>);
  public static <K, V, M extends java.util.Map<K, V>> java.util.function.BinaryOperator<M> mapMerger(java.util.function.BinaryOperator<V>);
  public static <K, V> java.util.stream.Collector<java.util.Map<K, V>, ?, java.util.Map<K, java.util.List<V>>> reduceListMap();
  public static <K, V, R extends java.util.Map<K, java.util.List<V>>> java.util.stream.Collector<java.util.Map<K, V>, ?, R> reduceListMap(java.util.function.Supplier<R>);
  public static <T, K, R, C extends java.util.Collection<R>, M extends java.util.Map<K, C>> java.util.stream.Collector<T, ?, M> groupingBy(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends R>, java.util.function.Supplier<C>, java.util.function.Supplier<M>);
  public static <T, K, R, C extends java.util.Collection<R>> java.util.stream.Collector<T, ?, java.util.Map<K, C>> groupingBy(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends R>, java.util.function.Supplier<C>);
  public static <T, K, R> java.util.stream.Collector<T, ?, java.util.Map<K, java.util.List<R>>> groupingBy(java.util.function.Function<? super T, ? extends K>, java.util.function.Function<? super T, ? extends R>);
}
```

## `cn.hutool.core.stream.SimpleCollector`

```java
public class cn.hutool.core.stream.SimpleCollector<T, A, R> implements java.util.stream.Collector<T, A, R> {
  public cn.hutool.core.stream.SimpleCollector(java.util.function.Supplier<A>, java.util.function.BiConsumer<A, T>, java.util.function.BinaryOperator<A>, java.util.function.Function<A, R>, java.util.Set<java.util.stream.Collector$Characteristics>);
  public cn.hutool.core.stream.SimpleCollector(java.util.function.Supplier<A>, java.util.function.BiConsumer<A, T>, java.util.function.BinaryOperator<A>, java.util.Set<java.util.stream.Collector$Characteristics>);
  public java.util.function.BiConsumer<A, T> accumulator();
  public java.util.function.Supplier<A> supplier();
  public java.util.function.BinaryOperator<A> combiner();
  public java.util.function.Function<A, R> finisher();
  public java.util.Set<java.util.stream.Collector$Characteristics> characteristics();
}
```

## `cn.hutool.core.stream.StreamUtil`

```java
public class cn.hutool.core.stream.StreamUtil {
  public cn.hutool.core.stream.StreamUtil();
  public static <T> java.util.stream.Stream<T> of(T...);
  public static <T> java.util.stream.Stream<T> of(java.lang.Iterable<T>);
  public static <T> java.util.stream.Stream<T> of(java.lang.Iterable<T>, boolean);
  public static <T> java.util.stream.Stream<T> of(java.util.Iterator<T>);
  public static <T> java.util.stream.Stream<T> of(java.util.Iterator<T>, boolean);
  public static java.util.stream.Stream<java.lang.String> of(java.io.File);
  public static java.util.stream.Stream<java.lang.String> of(java.nio.file.Path);
  public static java.util.stream.Stream<java.lang.String> of(java.io.File, java.nio.charset.Charset);
  public static java.util.stream.Stream<java.lang.String> of(java.nio.file.Path, java.nio.charset.Charset);
  public static <T> java.util.stream.Stream<T> of(T, java.util.function.UnaryOperator<T>, int);
  public static <T> java.lang.String join(java.util.stream.Stream<T>, java.lang.CharSequence);
  public static <T> java.lang.String join(java.util.stream.Stream<T>, java.lang.CharSequence, java.util.function.Function<T, ? extends java.lang.CharSequence>);
}
```
