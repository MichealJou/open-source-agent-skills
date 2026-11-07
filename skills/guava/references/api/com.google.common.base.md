# com.google.common.base

版本：33.4.8-jre。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.google.common.base.Ascii`

```java
public final class com.google.common.base.Ascii {
  public static java.lang.String toLowerCase(java.lang.String);
  public static java.lang.String toLowerCase(java.lang.CharSequence);
  public static char toLowerCase(char);
  public static java.lang.String toUpperCase(java.lang.String);
  public static java.lang.String toUpperCase(java.lang.CharSequence);
  public static char toUpperCase(char);
  public static boolean isLowerCase(char);
  public static boolean isUpperCase(char);
  public static java.lang.String truncate(java.lang.CharSequence, int, java.lang.String);
  public static boolean equalsIgnoreCase(java.lang.CharSequence, java.lang.CharSequence);
}
```

## `com.google.common.base.CaseFormat`

```java
public abstract class com.google.common.base.CaseFormat extends java.lang.Enum<com.google.common.base.CaseFormat> {
  public static com.google.common.base.CaseFormat[] values();
  public static com.google.common.base.CaseFormat valueOf(java.lang.String);
  public final java.lang.String to(com.google.common.base.CaseFormat, java.lang.String);
  public com.google.common.base.Converter<java.lang.String, java.lang.String> converterTo(com.google.common.base.CaseFormat);
}
```

## `com.google.common.base.CharMatcher`

```java
public abstract class com.google.common.base.CharMatcher implements com.google.common.base.Predicate<java.lang.Character> {
  public static com.google.common.base.CharMatcher any();
  public static com.google.common.base.CharMatcher none();
  public static com.google.common.base.CharMatcher whitespace();
  public static com.google.common.base.CharMatcher breakingWhitespace();
  public static com.google.common.base.CharMatcher ascii();
  public static com.google.common.base.CharMatcher digit();
  public static com.google.common.base.CharMatcher javaDigit();
  public static com.google.common.base.CharMatcher javaLetter();
  public static com.google.common.base.CharMatcher javaLetterOrDigit();
  public static com.google.common.base.CharMatcher javaUpperCase();
  public static com.google.common.base.CharMatcher javaLowerCase();
  public static com.google.common.base.CharMatcher javaIsoControl();
  public static com.google.common.base.CharMatcher invisible();
  public static com.google.common.base.CharMatcher singleWidth();
  public static com.google.common.base.CharMatcher is(char);
  public static com.google.common.base.CharMatcher isNot(char);
  public static com.google.common.base.CharMatcher anyOf(java.lang.CharSequence);
  public static com.google.common.base.CharMatcher noneOf(java.lang.CharSequence);
  public static com.google.common.base.CharMatcher inRange(char, char);
  public static com.google.common.base.CharMatcher forPredicate(com.google.common.base.Predicate<? super java.lang.Character>);
  public abstract boolean matches(char);
  public com.google.common.base.CharMatcher negate();
  public com.google.common.base.CharMatcher and(com.google.common.base.CharMatcher);
  public com.google.common.base.CharMatcher or(com.google.common.base.CharMatcher);
  public com.google.common.base.CharMatcher precomputed();
  public boolean matchesAnyOf(java.lang.CharSequence);
  public boolean matchesAllOf(java.lang.CharSequence);
  public boolean matchesNoneOf(java.lang.CharSequence);
  public int indexIn(java.lang.CharSequence);
  public int indexIn(java.lang.CharSequence, int);
  public int lastIndexIn(java.lang.CharSequence);
  public int countIn(java.lang.CharSequence);
  public java.lang.String removeFrom(java.lang.CharSequence);
  public java.lang.String retainFrom(java.lang.CharSequence);
  public java.lang.String replaceFrom(java.lang.CharSequence, char);
  public java.lang.String replaceFrom(java.lang.CharSequence, java.lang.CharSequence);
  public java.lang.String trimFrom(java.lang.CharSequence);
  public java.lang.String trimLeadingFrom(java.lang.CharSequence);
  public java.lang.String trimTrailingFrom(java.lang.CharSequence);
  public java.lang.String collapseFrom(java.lang.CharSequence, char);
  public java.lang.String trimAndCollapseFrom(java.lang.CharSequence, char);
  public boolean apply(java.lang.Character);
  public boolean test(java.lang.Character);
  public java.lang.String toString();
  public boolean test(java.lang.Object);
  public boolean apply(java.lang.Object);
  public java.util.function.Predicate negate();
}
```

## `com.google.common.base.Converter`

```java
public abstract class com.google.common.base.Converter<A, B> implements com.google.common.base.Function<A, B> {
  public final B convert(A);
  public java.lang.Iterable<B> convertAll(java.lang.Iterable<? extends A>);
  public com.google.common.base.Converter<B, A> reverse();
  public final <C> com.google.common.base.Converter<A, C> andThen(com.google.common.base.Converter<B, C>);
  public final B apply(A);
  public boolean equals(java.lang.Object);
  public static <A, B> com.google.common.base.Converter<A, B> from(com.google.common.base.Function<? super A, ? extends B>, com.google.common.base.Function<? super B, ? extends A>);
  public static <T> com.google.common.base.Converter<T, T> identity();
}
```

## `com.google.common.base.Defaults`

```java
public final class com.google.common.base.Defaults {
  public static <T> T defaultValue(java.lang.Class<T>);
}
```

## `com.google.common.base.Enums`

```java
public final class com.google.common.base.Enums {
  public static java.lang.reflect.Field getField(java.lang.Enum<?>);
  public static <T extends java.lang.Enum<T>> com.google.common.base.Optional<T> getIfPresent(java.lang.Class<T>, java.lang.String);
  public static <T extends java.lang.Enum<T>> com.google.common.base.Converter<java.lang.String, T> stringConverter(java.lang.Class<T>);
}
```

## `com.google.common.base.Equivalence`

```java
public abstract class com.google.common.base.Equivalence<T> implements java.util.function.BiPredicate<T, T> {
  public final boolean equivalent(T, T);
  public final boolean test(T, T);
  public final int hash(T);
  public final <F> com.google.common.base.Equivalence<F> onResultOf(com.google.common.base.Function<? super F, ? extends T>);
  public final <S extends T> com.google.common.base.Equivalence$Wrapper<S> wrap(S);
  public final <S extends T> com.google.common.base.Equivalence<java.lang.Iterable<S>> pairwise();
  public final com.google.common.base.Predicate<T> equivalentTo(T);
  public static com.google.common.base.Equivalence<java.lang.Object> equals();
  public static com.google.common.base.Equivalence<java.lang.Object> identity();
}
```

## `com.google.common.base.Equivalence$Wrapper`

```java
public final class com.google.common.base.Equivalence$Wrapper<T> implements java.io.Serializable {
  public T get();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.google.common.base.FinalizableReference`

```java
public interface com.google.common.base.FinalizableReference {
  public abstract void finalizeReferent();
}
```

## `com.google.common.base.FinalizableReferenceQueue`

```java
public class com.google.common.base.FinalizableReferenceQueue implements java.io.Closeable {
  public com.google.common.base.FinalizableReferenceQueue();
  public void close();
}
```

## `com.google.common.base.Function`

```java
public interface com.google.common.base.Function<F, T> extends java.util.function.Function<F, T> {
  public abstract T apply(F);
  public abstract boolean equals(java.lang.Object);
}
```

## `com.google.common.base.Functions`

```java
public final class com.google.common.base.Functions {
  public static com.google.common.base.Function<java.lang.Object, java.lang.String> toStringFunction();
  public static <E> com.google.common.base.Function<E, E> identity();
  public static <K, V> com.google.common.base.Function<K, V> forMap(java.util.Map<K, V>);
  public static <K, V> com.google.common.base.Function<K, V> forMap(java.util.Map<K, ? extends V>, V);
  public static <A, B, C> com.google.common.base.Function<A, C> compose(com.google.common.base.Function<B, C>, com.google.common.base.Function<A, ? extends B>);
  public static <T> com.google.common.base.Function<T, java.lang.Boolean> forPredicate(com.google.common.base.Predicate<T>);
  public static <E> com.google.common.base.Function<java.lang.Object, E> constant(E);
  public static <F, T> com.google.common.base.Function<F, T> forSupplier(com.google.common.base.Supplier<T>);
}
```

## `com.google.common.base.Joiner`

```java
public class com.google.common.base.Joiner {
  public static com.google.common.base.Joiner on(java.lang.String);
  public static com.google.common.base.Joiner on(char);
  public <A extends java.lang.Appendable> A appendTo(A, java.lang.Iterable<?>) throws java.io.IOException;
  public <A extends java.lang.Appendable> A appendTo(A, java.util.Iterator<?>) throws java.io.IOException;
  public final <A extends java.lang.Appendable> A appendTo(A, java.lang.Object[]) throws java.io.IOException;
  public final <A extends java.lang.Appendable> A appendTo(A, java.lang.Object, java.lang.Object, java.lang.Object...) throws java.io.IOException;
  public final java.lang.StringBuilder appendTo(java.lang.StringBuilder, java.lang.Iterable<?>);
  public final java.lang.StringBuilder appendTo(java.lang.StringBuilder, java.util.Iterator<?>);
  public final java.lang.StringBuilder appendTo(java.lang.StringBuilder, java.lang.Object[]);
  public final java.lang.StringBuilder appendTo(java.lang.StringBuilder, java.lang.Object, java.lang.Object, java.lang.Object...);
  public java.lang.String join(java.lang.Iterable<?>);
  public final java.lang.String join(java.util.Iterator<?>);
  public final java.lang.String join(java.lang.Object[]);
  public final java.lang.String join(java.lang.Object, java.lang.Object, java.lang.Object...);
  public com.google.common.base.Joiner useForNull(java.lang.String);
  public com.google.common.base.Joiner skipNulls();
  public com.google.common.base.Joiner$MapJoiner withKeyValueSeparator(char);
  public com.google.common.base.Joiner$MapJoiner withKeyValueSeparator(java.lang.String);
}
```

## `com.google.common.base.Joiner$MapJoiner`

```java
public final class com.google.common.base.Joiner$MapJoiner {
  public <A extends java.lang.Appendable> A appendTo(A, java.util.Map<?, ?>) throws java.io.IOException;
  public java.lang.StringBuilder appendTo(java.lang.StringBuilder, java.util.Map<?, ?>);
  public <A extends java.lang.Appendable> A appendTo(A, java.lang.Iterable<? extends java.util.Map$Entry<?, ?>>) throws java.io.IOException;
  public <A extends java.lang.Appendable> A appendTo(A, java.util.Iterator<? extends java.util.Map$Entry<?, ?>>) throws java.io.IOException;
  public java.lang.StringBuilder appendTo(java.lang.StringBuilder, java.lang.Iterable<? extends java.util.Map$Entry<?, ?>>);
  public java.lang.StringBuilder appendTo(java.lang.StringBuilder, java.util.Iterator<? extends java.util.Map$Entry<?, ?>>);
  public java.lang.String join(java.util.Map<?, ?>);
  public java.lang.String join(java.lang.Iterable<? extends java.util.Map$Entry<?, ?>>);
  public java.lang.String join(java.util.Iterator<? extends java.util.Map$Entry<?, ?>>);
  public com.google.common.base.Joiner$MapJoiner useForNull(java.lang.String);
}
```

## `com.google.common.base.MoreObjects`

```java
public final class com.google.common.base.MoreObjects {
  public static <T> T firstNonNull(T, T);
  public static com.google.common.base.MoreObjects$ToStringHelper toStringHelper(java.lang.Object);
  public static com.google.common.base.MoreObjects$ToStringHelper toStringHelper(java.lang.Class<?>);
  public static com.google.common.base.MoreObjects$ToStringHelper toStringHelper(java.lang.String);
}
```

## `com.google.common.base.MoreObjects$ToStringHelper`

```java
public final class com.google.common.base.MoreObjects$ToStringHelper {
  public com.google.common.base.MoreObjects$ToStringHelper omitNullValues();
  public com.google.common.base.MoreObjects$ToStringHelper omitEmptyValues();
  public com.google.common.base.MoreObjects$ToStringHelper add(java.lang.String, java.lang.Object);
  public com.google.common.base.MoreObjects$ToStringHelper add(java.lang.String, boolean);
  public com.google.common.base.MoreObjects$ToStringHelper add(java.lang.String, char);
  public com.google.common.base.MoreObjects$ToStringHelper add(java.lang.String, double);
  public com.google.common.base.MoreObjects$ToStringHelper add(java.lang.String, float);
  public com.google.common.base.MoreObjects$ToStringHelper add(java.lang.String, int);
  public com.google.common.base.MoreObjects$ToStringHelper add(java.lang.String, long);
  public com.google.common.base.MoreObjects$ToStringHelper addValue(java.lang.Object);
  public com.google.common.base.MoreObjects$ToStringHelper addValue(boolean);
  public com.google.common.base.MoreObjects$ToStringHelper addValue(char);
  public com.google.common.base.MoreObjects$ToStringHelper addValue(double);
  public com.google.common.base.MoreObjects$ToStringHelper addValue(float);
  public com.google.common.base.MoreObjects$ToStringHelper addValue(int);
  public com.google.common.base.MoreObjects$ToStringHelper addValue(long);
  public java.lang.String toString();
}
```

## `com.google.common.base.Objects`

```java
public final class com.google.common.base.Objects extends com.google.common.base.ExtraObjectsMethodsForWeb {
  public static boolean equal(java.lang.Object, java.lang.Object);
  public static int hashCode(java.lang.Object...);
}
```

## `com.google.common.base.Optional`

```java
public abstract class com.google.common.base.Optional<T> implements java.io.Serializable {
  public static <T> com.google.common.base.Optional<T> absent();
  public static <T> com.google.common.base.Optional<T> of(T);
  public static <T> com.google.common.base.Optional<T> fromNullable(T);
  public static <T> com.google.common.base.Optional<T> fromJavaUtil(java.util.Optional<T>);
  public static <T> java.util.Optional<T> toJavaUtil(com.google.common.base.Optional<T>);
  public java.util.Optional<T> toJavaUtil();
  public abstract boolean isPresent();
  public abstract T get();
  public abstract T or(T);
  public abstract com.google.common.base.Optional<T> or(com.google.common.base.Optional<? extends T>);
  public abstract T or(com.google.common.base.Supplier<? extends T>);
  public abstract T orNull();
  public abstract java.util.Set<T> asSet();
  public abstract <V> com.google.common.base.Optional<V> transform(com.google.common.base.Function<? super T, V>);
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
  public abstract java.lang.String toString();
  public static <T> java.lang.Iterable<T> presentInstances(java.lang.Iterable<? extends com.google.common.base.Optional<? extends T>>);
}
```

## `com.google.common.base.Preconditions`

```java
public final class com.google.common.base.Preconditions {
  public static void checkArgument(boolean);
  public static void checkArgument(boolean, java.lang.Object);
  public static void checkArgument(boolean, java.lang.String, java.lang.Object...);
  public static void checkArgument(boolean, java.lang.String, char);
  public static void checkArgument(boolean, java.lang.String, int);
  public static void checkArgument(boolean, java.lang.String, long);
  public static void checkArgument(boolean, java.lang.String, java.lang.Object);
  public static void checkArgument(boolean, java.lang.String, char, char);
  public static void checkArgument(boolean, java.lang.String, char, int);
  public static void checkArgument(boolean, java.lang.String, char, long);
  public static void checkArgument(boolean, java.lang.String, char, java.lang.Object);
  public static void checkArgument(boolean, java.lang.String, int, char);
  public static void checkArgument(boolean, java.lang.String, int, int);
  public static void checkArgument(boolean, java.lang.String, int, long);
  public static void checkArgument(boolean, java.lang.String, int, java.lang.Object);
  public static void checkArgument(boolean, java.lang.String, long, char);
  public static void checkArgument(boolean, java.lang.String, long, int);
  public static void checkArgument(boolean, java.lang.String, long, long);
  public static void checkArgument(boolean, java.lang.String, long, java.lang.Object);
  public static void checkArgument(boolean, java.lang.String, java.lang.Object, char);
  public static void checkArgument(boolean, java.lang.String, java.lang.Object, int);
  public static void checkArgument(boolean, java.lang.String, java.lang.Object, long);
  public static void checkArgument(boolean, java.lang.String, java.lang.Object, java.lang.Object);
  public static void checkArgument(boolean, java.lang.String, java.lang.Object, java.lang.Object, java.lang.Object);
  public static void checkArgument(boolean, java.lang.String, java.lang.Object, java.lang.Object, java.lang.Object, java.lang.Object);
  public static void checkState(boolean);
  public static void checkState(boolean, java.lang.Object);
  public static void checkState(boolean, java.lang.String, java.lang.Object...);
  public static void checkState(boolean, java.lang.String, char);
  public static void checkState(boolean, java.lang.String, int);
  public static void checkState(boolean, java.lang.String, long);
  public static void checkState(boolean, java.lang.String, java.lang.Object);
  public static void checkState(boolean, java.lang.String, char, char);
  public static void checkState(boolean, java.lang.String, char, int);
  public static void checkState(boolean, java.lang.String, char, long);
  public static void checkState(boolean, java.lang.String, char, java.lang.Object);
  public static void checkState(boolean, java.lang.String, int, char);
  public static void checkState(boolean, java.lang.String, int, int);
  public static void checkState(boolean, java.lang.String, int, long);
  public static void checkState(boolean, java.lang.String, int, java.lang.Object);
  public static void checkState(boolean, java.lang.String, long, char);
  public static void checkState(boolean, java.lang.String, long, int);
  public static void checkState(boolean, java.lang.String, long, long);
  public static void checkState(boolean, java.lang.String, long, java.lang.Object);
  public static void checkState(boolean, java.lang.String, java.lang.Object, char);
  public static void checkState(boolean, java.lang.String, java.lang.Object, int);
  public static void checkState(boolean, java.lang.String, java.lang.Object, long);
  public static void checkState(boolean, java.lang.String, java.lang.Object, java.lang.Object);
  public static void checkState(boolean, java.lang.String, java.lang.Object, java.lang.Object, java.lang.Object);
  public static void checkState(boolean, java.lang.String, java.lang.Object, java.lang.Object, java.lang.Object, java.lang.Object);
  public static <T> T checkNotNull(T);
  public static <T> T checkNotNull(T, java.lang.Object);
  public static <T> T checkNotNull(T, java.lang.String, java.lang.Object...);
  public static <T> T checkNotNull(T, java.lang.String, char);
  public static <T> T checkNotNull(T, java.lang.String, int);
  public static <T> T checkNotNull(T, java.lang.String, long);
  public static <T> T checkNotNull(T, java.lang.String, java.lang.Object);
  public static <T> T checkNotNull(T, java.lang.String, char, char);
  public static <T> T checkNotNull(T, java.lang.String, char, int);
  public static <T> T checkNotNull(T, java.lang.String, char, long);
  public static <T> T checkNotNull(T, java.lang.String, char, java.lang.Object);
  public static <T> T checkNotNull(T, java.lang.String, int, char);
  public static <T> T checkNotNull(T, java.lang.String, int, int);
  public static <T> T checkNotNull(T, java.lang.String, int, long);
  public static <T> T checkNotNull(T, java.lang.String, int, java.lang.Object);
  public static <T> T checkNotNull(T, java.lang.String, long, char);
  public static <T> T checkNotNull(T, java.lang.String, long, int);
  public static <T> T checkNotNull(T, java.lang.String, long, long);
  public static <T> T checkNotNull(T, java.lang.String, long, java.lang.Object);
  public static <T> T checkNotNull(T, java.lang.String, java.lang.Object, char);
  public static <T> T checkNotNull(T, java.lang.String, java.lang.Object, int);
  public static <T> T checkNotNull(T, java.lang.String, java.lang.Object, long);
  public static <T> T checkNotNull(T, java.lang.String, java.lang.Object, java.lang.Object);
  public static <T> T checkNotNull(T, java.lang.String, java.lang.Object, java.lang.Object, java.lang.Object);
  public static <T> T checkNotNull(T, java.lang.String, java.lang.Object, java.lang.Object, java.lang.Object, java.lang.Object);
  public static int checkElementIndex(int, int);
  public static int checkElementIndex(int, int, java.lang.String);
  public static int checkPositionIndex(int, int);
  public static int checkPositionIndex(int, int, java.lang.String);
  public static void checkPositionIndexes(int, int, int);
}
```

## `com.google.common.base.Predicate`

```java
public interface com.google.common.base.Predicate<T> extends java.util.function.Predicate<T> {
  public abstract boolean apply(T);
  public abstract boolean equals(java.lang.Object);
  public default boolean test(T);
}
```

## `com.google.common.base.Predicates`

```java
public final class com.google.common.base.Predicates {
  public static <T> com.google.common.base.Predicate<T> alwaysTrue();
  public static <T> com.google.common.base.Predicate<T> alwaysFalse();
  public static <T> com.google.common.base.Predicate<T> isNull();
  public static <T> com.google.common.base.Predicate<T> notNull();
  public static <T> com.google.common.base.Predicate<T> not(com.google.common.base.Predicate<T>);
  public static <T> com.google.common.base.Predicate<T> and(java.lang.Iterable<? extends com.google.common.base.Predicate<? super T>>);
  public static <T> com.google.common.base.Predicate<T> and(com.google.common.base.Predicate<? super T>...);
  public static <T> com.google.common.base.Predicate<T> and(com.google.common.base.Predicate<? super T>, com.google.common.base.Predicate<? super T>);
  public static <T> com.google.common.base.Predicate<T> or(java.lang.Iterable<? extends com.google.common.base.Predicate<? super T>>);
  public static <T> com.google.common.base.Predicate<T> or(com.google.common.base.Predicate<? super T>...);
  public static <T> com.google.common.base.Predicate<T> or(com.google.common.base.Predicate<? super T>, com.google.common.base.Predicate<? super T>);
  public static <T> com.google.common.base.Predicate<T> equalTo(T);
  public static <T> com.google.common.base.Predicate<T> instanceOf(java.lang.Class<?>);
  public static com.google.common.base.Predicate<java.lang.Class<?>> subtypeOf(java.lang.Class<?>);
  public static <T> com.google.common.base.Predicate<T> in(java.util.Collection<? extends T>);
  public static <A, B> com.google.common.base.Predicate<A> compose(com.google.common.base.Predicate<B>, com.google.common.base.Function<A, ? extends B>);
  public static com.google.common.base.Predicate<java.lang.CharSequence> containsPattern(java.lang.String);
  public static com.google.common.base.Predicate<java.lang.CharSequence> contains(java.util.regex.Pattern);
}
```

## `com.google.common.base.Splitter`

```java
public final class com.google.common.base.Splitter {
  public static com.google.common.base.Splitter on(char);
  public static com.google.common.base.Splitter on(com.google.common.base.CharMatcher);
  public static com.google.common.base.Splitter on(java.lang.String);
  public static com.google.common.base.Splitter on(java.util.regex.Pattern);
  public static com.google.common.base.Splitter onPattern(java.lang.String);
  public static com.google.common.base.Splitter fixedLength(int);
  public com.google.common.base.Splitter omitEmptyStrings();
  public com.google.common.base.Splitter limit(int);
  public com.google.common.base.Splitter trimResults();
  public com.google.common.base.Splitter trimResults(com.google.common.base.CharMatcher);
  public java.lang.Iterable<java.lang.String> split(java.lang.CharSequence);
  public java.util.List<java.lang.String> splitToList(java.lang.CharSequence);
  public java.util.stream.Stream<java.lang.String> splitToStream(java.lang.CharSequence);
  public com.google.common.base.Splitter$MapSplitter withKeyValueSeparator(java.lang.String);
  public com.google.common.base.Splitter$MapSplitter withKeyValueSeparator(char);
  public com.google.common.base.Splitter$MapSplitter withKeyValueSeparator(com.google.common.base.Splitter);
}
```

## `com.google.common.base.Splitter$MapSplitter`

```java
public final class com.google.common.base.Splitter$MapSplitter {
  public java.util.Map<java.lang.String, java.lang.String> split(java.lang.CharSequence);
}
```

## `com.google.common.base.StandardSystemProperty`

```java
public final class com.google.common.base.StandardSystemProperty extends java.lang.Enum<com.google.common.base.StandardSystemProperty> {
  public static com.google.common.base.StandardSystemProperty[] values();
  public static com.google.common.base.StandardSystemProperty valueOf(java.lang.String);
  public java.lang.String key();
  public java.lang.String value();
  public java.lang.String toString();
}
```

## `com.google.common.base.Stopwatch`

```java
public final class com.google.common.base.Stopwatch {
  public static com.google.common.base.Stopwatch createUnstarted();
  public static com.google.common.base.Stopwatch createUnstarted(com.google.common.base.Ticker);
  public static com.google.common.base.Stopwatch createStarted();
  public static com.google.common.base.Stopwatch createStarted(com.google.common.base.Ticker);
  public boolean isRunning();
  public com.google.common.base.Stopwatch start();
  public com.google.common.base.Stopwatch stop();
  public com.google.common.base.Stopwatch reset();
  public long elapsed(java.util.concurrent.TimeUnit);
  public java.time.Duration elapsed();
  public java.lang.String toString();
}
```

## `com.google.common.base.Strings`

```java
public final class com.google.common.base.Strings {
  public static java.lang.String nullToEmpty(java.lang.String);
  public static java.lang.String emptyToNull(java.lang.String);
  public static boolean isNullOrEmpty(java.lang.String);
  public static java.lang.String padStart(java.lang.String, int, char);
  public static java.lang.String padEnd(java.lang.String, int, char);
  public static java.lang.String repeat(java.lang.String, int);
  public static java.lang.String commonPrefix(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String commonSuffix(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String lenientFormat(java.lang.String, java.lang.Object...);
}
```

## `com.google.common.base.Supplier`

```java
public interface com.google.common.base.Supplier<T> extends java.util.function.Supplier<T> {
  public abstract T get();
}
```

## `com.google.common.base.Suppliers`

```java
public final class com.google.common.base.Suppliers {
  public static <F, T> com.google.common.base.Supplier<T> compose(com.google.common.base.Function<? super F, T>, com.google.common.base.Supplier<F>);
  public static <T> com.google.common.base.Supplier<T> memoize(com.google.common.base.Supplier<T>);
  public static <T> com.google.common.base.Supplier<T> memoizeWithExpiration(com.google.common.base.Supplier<T>, long, java.util.concurrent.TimeUnit);
  public static <T> com.google.common.base.Supplier<T> memoizeWithExpiration(com.google.common.base.Supplier<T>, java.time.Duration);
  public static <T> com.google.common.base.Supplier<T> ofInstance(T);
  public static <T> com.google.common.base.Supplier<T> synchronizedSupplier(com.google.common.base.Supplier<T>);
  public static <T> com.google.common.base.Function<com.google.common.base.Supplier<T>, T> supplierFunction();
}
```

## `com.google.common.base.Throwables`

```java
public final class com.google.common.base.Throwables {
  public static <X extends java.lang.Throwable> void throwIfInstanceOf(java.lang.Throwable, java.lang.Class<X>) throws X;
  public static <X extends java.lang.Throwable> void propagateIfInstanceOf(java.lang.Throwable, java.lang.Class<X>) throws X;
  public static void throwIfUnchecked(java.lang.Throwable);
  public static void propagateIfPossible(java.lang.Throwable);
  public static <X extends java.lang.Throwable> void propagateIfPossible(java.lang.Throwable, java.lang.Class<X>) throws X;
  public static <X1 extends java.lang.Throwable, X2 extends java.lang.Throwable> void propagateIfPossible(java.lang.Throwable, java.lang.Class<X1>, java.lang.Class<X2>) throws X1, X2;
  public static java.lang.RuntimeException propagate(java.lang.Throwable);
  public static java.lang.Throwable getRootCause(java.lang.Throwable);
  public static java.util.List<java.lang.Throwable> getCausalChain(java.lang.Throwable);
  public static <X extends java.lang.Throwable> X getCauseAs(java.lang.Throwable, java.lang.Class<X>);
  public static java.lang.String getStackTraceAsString(java.lang.Throwable);
  public static java.util.List<java.lang.StackTraceElement> lazyStackTrace(java.lang.Throwable);
  public static boolean lazyStackTraceIsLazy();
}
```

## `com.google.common.base.Ticker`

```java
public abstract class com.google.common.base.Ticker {
  public abstract long read();
  public static com.google.common.base.Ticker systemTicker();
}
```

## `com.google.common.base.Utf8`

```java
public final class com.google.common.base.Utf8 {
  public static int encodedLength(java.lang.CharSequence);
  public static boolean isWellFormed(byte[]);
  public static boolean isWellFormed(byte[], int, int);
}
```

## `com.google.common.base.Verify`

```java
public final class com.google.common.base.Verify {
  public static void verify(boolean);
  public static void verify(boolean, java.lang.String, java.lang.Object...);
  public static void verify(boolean, java.lang.String, char);
  public static void verify(boolean, java.lang.String, int);
  public static void verify(boolean, java.lang.String, long);
  public static void verify(boolean, java.lang.String, java.lang.Object);
  public static void verify(boolean, java.lang.String, char, char);
  public static void verify(boolean, java.lang.String, int, char);
  public static void verify(boolean, java.lang.String, long, char);
  public static void verify(boolean, java.lang.String, java.lang.Object, char);
  public static void verify(boolean, java.lang.String, char, int);
  public static void verify(boolean, java.lang.String, int, int);
  public static void verify(boolean, java.lang.String, long, int);
  public static void verify(boolean, java.lang.String, java.lang.Object, int);
  public static void verify(boolean, java.lang.String, char, long);
  public static void verify(boolean, java.lang.String, int, long);
  public static void verify(boolean, java.lang.String, long, long);
  public static void verify(boolean, java.lang.String, java.lang.Object, long);
  public static void verify(boolean, java.lang.String, char, java.lang.Object);
  public static void verify(boolean, java.lang.String, int, java.lang.Object);
  public static void verify(boolean, java.lang.String, long, java.lang.Object);
  public static void verify(boolean, java.lang.String, java.lang.Object, java.lang.Object);
  public static void verify(boolean, java.lang.String, java.lang.Object, java.lang.Object, java.lang.Object);
  public static void verify(boolean, java.lang.String, java.lang.Object, java.lang.Object, java.lang.Object, java.lang.Object);
  public static <T> T verifyNotNull(T);
  public static <T> T verifyNotNull(T, java.lang.String, java.lang.Object...);
}
```

## `com.google.common.base.VerifyException`

```java
public class com.google.common.base.VerifyException extends java.lang.RuntimeException {
  public com.google.common.base.VerifyException();
  public com.google.common.base.VerifyException(java.lang.String);
  public com.google.common.base.VerifyException(java.lang.Throwable);
  public com.google.common.base.VerifyException(java.lang.String, java.lang.Throwable);
}
```
