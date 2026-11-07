# cn.hutool.core.lang

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.lang.Assert`

```java
public class cn.hutool.core.lang.Assert {
  public cn.hutool.core.lang.Assert();
  public static <X extends java.lang.Throwable> void isTrue(boolean, java.util.function.Supplier<? extends X>) throws X;
  public static void isTrue(boolean, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static void isTrue(boolean) throws java.lang.IllegalArgumentException;
  public static <X extends java.lang.Throwable> void isFalse(boolean, java.util.function.Supplier<X>) throws X;
  public static void isFalse(boolean, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static void isFalse(boolean) throws java.lang.IllegalArgumentException;
  public static <X extends java.lang.Throwable> void isNull(java.lang.Object, java.util.function.Supplier<X>) throws X;
  public static void isNull(java.lang.Object, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static void isNull(java.lang.Object) throws java.lang.IllegalArgumentException;
  public static <T, X extends java.lang.Throwable> T notNull(T, java.util.function.Supplier<X>) throws X;
  public static <T> T notNull(T, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static <T> T notNull(T) throws java.lang.IllegalArgumentException;
  public static <T extends java.lang.CharSequence, X extends java.lang.Throwable> T notEmpty(T, java.util.function.Supplier<X>) throws X;
  public static <T extends java.lang.CharSequence> T notEmpty(T, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static <T extends java.lang.CharSequence> T notEmpty(T) throws java.lang.IllegalArgumentException;
  public static <T extends java.lang.CharSequence, X extends java.lang.Throwable> T notBlank(T, java.util.function.Supplier<X>) throws X;
  public static <T extends java.lang.CharSequence> T notBlank(T, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static <T extends java.lang.CharSequence> T notBlank(T) throws java.lang.IllegalArgumentException;
  public static <T extends java.lang.CharSequence, X extends java.lang.Throwable> T notContain(java.lang.CharSequence, T, java.util.function.Supplier<X>) throws X;
  public static java.lang.String notContain(java.lang.String, java.lang.String, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static java.lang.String notContain(java.lang.String, java.lang.String) throws java.lang.IllegalArgumentException;
  public static <T, X extends java.lang.Throwable> T[] notEmpty(T[], java.util.function.Supplier<X>) throws X;
  public static <T> T[] notEmpty(T[], java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static <T> T[] notEmpty(T[]) throws java.lang.IllegalArgumentException;
  public static <T, X extends java.lang.Throwable> T[] noNullElements(T[], java.util.function.Supplier<X>) throws X;
  public static <T> T[] noNullElements(T[], java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static <T> T[] noNullElements(T[]) throws java.lang.IllegalArgumentException;
  public static <E, T extends java.lang.Iterable<E>, X extends java.lang.Throwable> void empty(T, java.util.function.Supplier<X>) throws X;
  public static <E, T extends java.lang.Iterable<E>> void empty(T, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static <E, T extends java.lang.Iterable<E>> void empty(T) throws java.lang.IllegalArgumentException;
  public static <E, T extends java.lang.Iterable<E>, X extends java.lang.Throwable> T notEmpty(T, java.util.function.Supplier<X>) throws X;
  public static <E, T extends java.lang.Iterable<E>> T notEmpty(T, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static <E, T extends java.lang.Iterable<E>> T notEmpty(T) throws java.lang.IllegalArgumentException;
  public static <K, V, T extends java.util.Map<K, V>, X extends java.lang.Throwable> T notEmpty(T, java.util.function.Supplier<X>) throws X;
  public static <K, V, T extends java.util.Map<K, V>> T notEmpty(T, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static <K, V, T extends java.util.Map<K, V>> T notEmpty(T) throws java.lang.IllegalArgumentException;
  public static <T> T isInstanceOf(java.lang.Class<?>, T);
  public static <T> T isInstanceOf(java.lang.Class<?>, T, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static void isAssignable(java.lang.Class<?>, java.lang.Class<?>) throws java.lang.IllegalArgumentException;
  public static void isAssignable(java.lang.Class<?>, java.lang.Class<?>, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static void state(boolean, java.util.function.Supplier<java.lang.String>) throws java.lang.IllegalStateException;
  public static void state(boolean, java.lang.String, java.lang.Object...) throws java.lang.IllegalStateException;
  public static void state(boolean) throws java.lang.IllegalStateException;
  public static int checkIndex(int, int) throws java.lang.IllegalArgumentException, java.lang.IndexOutOfBoundsException;
  public static int checkIndex(int, int, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException, java.lang.IndexOutOfBoundsException;
  public static <X extends java.lang.Throwable> int checkBetween(int, int, int, java.util.function.Supplier<? extends X>) throws X;
  public static int checkBetween(int, int, int, java.lang.String, java.lang.Object...);
  public static int checkBetween(int, int, int);
  public static <X extends java.lang.Throwable> long checkBetween(long, long, long, java.util.function.Supplier<? extends X>) throws X;
  public static long checkBetween(long, long, long, java.lang.String, java.lang.Object...);
  public static long checkBetween(long, long, long);
  public static <X extends java.lang.Throwable> double checkBetween(double, double, double, java.util.function.Supplier<? extends X>) throws X;
  public static double checkBetween(double, double, double, java.lang.String, java.lang.Object...);
  public static double checkBetween(double, double, double);
  public static java.lang.Number checkBetween(java.lang.Number, java.lang.Number, java.lang.Number);
  public static void notEquals(java.lang.Object, java.lang.Object);
  public static void notEquals(java.lang.Object, java.lang.Object, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static <X extends java.lang.Throwable> void notEquals(java.lang.Object, java.lang.Object, java.util.function.Supplier<X>) throws X;
  public static void equals(java.lang.Object, java.lang.Object);
  public static void equals(java.lang.Object, java.lang.Object, java.lang.String, java.lang.Object...) throws java.lang.IllegalArgumentException;
  public static <X extends java.lang.Throwable> void equals(java.lang.Object, java.lang.Object, java.util.function.Supplier<X>) throws X;
}
```

## `cn.hutool.core.lang.Chain`

```java
public interface cn.hutool.core.lang.Chain<E, T> extends java.lang.Iterable<E> {
  public abstract T addChain(E);
}
```

## `cn.hutool.core.lang.ClassScanner`

```java
public class cn.hutool.core.lang.ClassScanner implements java.io.Serializable {
  public static java.util.Set<java.lang.Class<?>> scanAllPackageByAnnotation(java.lang.String, java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static java.util.Set<java.lang.Class<?>> scanPackageByAnnotation(java.lang.String, java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static java.util.Set<java.lang.Class<?>> scanAllPackageBySuper(java.lang.String, java.lang.Class<?>);
  public static java.util.Set<java.lang.Class<?>> scanPackageBySuper(java.lang.String, java.lang.Class<?>);
  public static java.util.Set<java.lang.Class<?>> scanAllPackage();
  public static java.util.Set<java.lang.Class<?>> scanPackage();
  public static java.util.Set<java.lang.Class<?>> scanPackage(java.lang.String);
  public static java.util.Set<java.lang.Class<?>> scanAllPackage(java.lang.String, cn.hutool.core.lang.Filter<java.lang.Class<?>>);
  public static java.util.Set<java.lang.Class<?>> scanPackage(java.lang.String, cn.hutool.core.lang.Filter<java.lang.Class<?>>);
  public cn.hutool.core.lang.ClassScanner();
  public cn.hutool.core.lang.ClassScanner(java.lang.String);
  public cn.hutool.core.lang.ClassScanner(java.lang.String, cn.hutool.core.lang.Filter<java.lang.Class<?>>);
  public cn.hutool.core.lang.ClassScanner(java.lang.String, cn.hutool.core.lang.Filter<java.lang.Class<?>>, java.nio.charset.Charset);
  public cn.hutool.core.lang.ClassScanner setIgnoreLoadError(boolean);
  public java.util.Set<java.lang.Class<?>> scan();
  public java.util.Set<java.lang.Class<?>> scan(boolean);
  public void setInitialize(boolean);
  public void setClassLoader(java.lang.ClassLoader);
  public java.util.Set<java.lang.String> getClassesOfLoadError();
}
```

## `cn.hutool.core.lang.ConsistentHash`

```java
public class cn.hutool.core.lang.ConsistentHash<T> implements java.io.Serializable {
  public cn.hutool.core.lang.ConsistentHash(int, java.util.Collection<T>);
  public cn.hutool.core.lang.ConsistentHash(cn.hutool.core.lang.hash.Hash32<java.lang.Object>, int, java.util.Collection<T>);
  public void add(T);
  public void remove(T);
  public T get(java.lang.Object);
}
```

## `cn.hutool.core.lang.Console`

```java
public class cn.hutool.core.lang.Console {
  public cn.hutool.core.lang.Console();
  public static void log();
  public static void log(java.lang.Object);
  public static void log(java.lang.Object, java.lang.Object...);
  public static void log(java.lang.String, java.lang.Object...);
  public static void log(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public static void table(cn.hutool.core.lang.ConsoleTable);
  public static void print(java.lang.Object);
  public static void print(java.lang.Object, java.lang.Object...);
  public static void print(java.lang.String, java.lang.Object...);
  public static void printProgress(char, int);
  public static void printProgress(char, int, double);
  public static void error();
  public static void error(java.lang.Object);
  public static void error(java.lang.Object, java.lang.Object...);
  public static void error(java.lang.String, java.lang.Object...);
  public static void error(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public static java.util.Scanner scanner();
  public static java.lang.String input();
  public static java.lang.String where();
  public static java.lang.Integer lineNumber();
}
```

## `cn.hutool.core.lang.ConsoleTable`

```java
public class cn.hutool.core.lang.ConsoleTable {
  public cn.hutool.core.lang.ConsoleTable();
  public static cn.hutool.core.lang.ConsoleTable create();
  public cn.hutool.core.lang.ConsoleTable setSBCMode(boolean);
  public cn.hutool.core.lang.ConsoleTable addHeader(java.lang.String...);
  public cn.hutool.core.lang.ConsoleTable addBody(java.lang.String...);
  public java.lang.String toString();
  public void print();
}
```

## `cn.hutool.core.lang.DefaultSegment`

```java
public class cn.hutool.core.lang.DefaultSegment<T extends java.lang.Number> implements cn.hutool.core.lang.Segment<T> {
  public cn.hutool.core.lang.DefaultSegment(T, T);
  public T getStartIndex();
  public T getEndIndex();
}
```

## `cn.hutool.core.lang.Dict`

```java
public class cn.hutool.core.lang.Dict extends java.util.LinkedHashMap<java.lang.String, java.lang.Object> implements cn.hutool.core.getter.BasicTypeGetter<java.lang.String> {
  public static cn.hutool.core.lang.Dict create();
  public static <T> cn.hutool.core.lang.Dict parse(T);
  public static cn.hutool.core.lang.Dict of(cn.hutool.core.lang.Pair<java.lang.String, java.lang.Object>...);
  public static cn.hutool.core.lang.Dict of(java.lang.Object...);
  public cn.hutool.core.lang.Dict();
  public cn.hutool.core.lang.Dict(boolean);
  public cn.hutool.core.lang.Dict(int);
  public cn.hutool.core.lang.Dict(int, boolean);
  public cn.hutool.core.lang.Dict(int, float);
  public cn.hutool.core.lang.Dict(int, float, boolean);
  public cn.hutool.core.lang.Dict(java.util.Map<java.lang.String, java.lang.Object>);
  public <T> T toBean(T);
  public <T> T toBeanIgnoreCase(T);
  public <T> T toBean(T, boolean);
  public <T> T toBeanWithCamelCase(T);
  public <T> T toBean(java.lang.Class<T>);
  public <T> T toBeanIgnoreCase(java.lang.Class<T>);
  public <T> cn.hutool.core.lang.Dict parseBean(T);
  public <T> cn.hutool.core.lang.Dict parseBean(T, boolean, boolean);
  public <T extends cn.hutool.core.lang.Dict> void removeEqual(T, java.lang.String...);
  public cn.hutool.core.lang.Dict filter(java.lang.String...);
  public cn.hutool.core.lang.Dict set(java.lang.String, java.lang.Object);
  public cn.hutool.core.lang.Dict setIgnoreNull(java.lang.String, java.lang.Object);
  public java.lang.Object getObj(java.lang.String);
  public <T> T getBean(java.lang.String);
  public <T> T get(java.lang.String, T);
  public java.lang.String getStr(java.lang.String);
  public java.lang.Integer getInt(java.lang.String);
  public java.lang.Long getLong(java.lang.String);
  public java.lang.Float getFloat(java.lang.String);
  public java.lang.Short getShort(java.lang.String);
  public java.lang.Character getChar(java.lang.String);
  public java.lang.Double getDouble(java.lang.String);
  public java.lang.Byte getByte(java.lang.String);
  public java.lang.Boolean getBool(java.lang.String);
  public java.math.BigDecimal getBigDecimal(java.lang.String);
  public java.math.BigInteger getBigInteger(java.lang.String);
  public <E extends java.lang.Enum<E>> E getEnum(java.lang.Class<E>, java.lang.String);
  public byte[] getBytes(java.lang.String);
  public java.util.Date getDate(java.lang.String);
  public java.sql.Time getTime(java.lang.String);
  public java.sql.Timestamp getTimestamp(java.lang.String);
  public java.lang.Number getNumber(java.lang.String);
  public <T> T getByPath(java.lang.String);
  public <T> T getByPath(java.lang.String, java.lang.Class<T>);
  public boolean containsKey(java.lang.Object);
  public java.lang.Object get(java.lang.Object);
  public java.lang.Object put(java.lang.String, java.lang.Object);
  public void putAll(java.util.Map<? extends java.lang.String, ?>);
  public cn.hutool.core.lang.Dict clone();
  public java.lang.Object remove(java.lang.Object);
  public boolean remove(java.lang.Object, java.lang.Object);
  public boolean replace(java.lang.String, java.lang.Object, java.lang.Object);
  public java.lang.Object replace(java.lang.String, java.lang.Object);
  public java.lang.Object getOrDefault(java.lang.Object, java.lang.Object);
  public java.lang.Object computeIfPresent(java.lang.String, java.util.function.BiFunction<? super java.lang.String, ? super java.lang.Object, ?>);
  public java.lang.Object compute(java.lang.String, java.util.function.BiFunction<? super java.lang.String, ? super java.lang.Object, ?>);
  public java.lang.Object merge(java.lang.String, java.lang.Object, java.util.function.BiFunction<? super java.lang.Object, ? super java.lang.Object, ?>);
  public java.lang.Object putIfAbsent(java.lang.String, java.lang.Object);
  public java.lang.Object computeIfAbsent(java.lang.String, java.util.function.Function<? super java.lang.String, ?>);
  public cn.hutool.core.lang.Dict setFields(cn.hutool.core.lang.func.Func0<?>...);
  public java.lang.Object merge(java.lang.Object, java.lang.Object, java.util.function.BiFunction);
  public java.lang.Object compute(java.lang.Object, java.util.function.BiFunction);
  public java.lang.Object computeIfPresent(java.lang.Object, java.util.function.BiFunction);
  public java.lang.Object computeIfAbsent(java.lang.Object, java.util.function.Function);
  public java.lang.Object replace(java.lang.Object, java.lang.Object);
  public boolean replace(java.lang.Object, java.lang.Object, java.lang.Object);
  public java.lang.Object putIfAbsent(java.lang.Object, java.lang.Object);
  public java.lang.Object put(java.lang.Object, java.lang.Object);
  public java.lang.Object clone();
  public java.util.Date getDate(java.lang.Object);
  public java.lang.Enum getEnum(java.lang.Class, java.lang.Object);
  public java.math.BigInteger getBigInteger(java.lang.Object);
  public java.math.BigDecimal getBigDecimal(java.lang.Object);
  public java.lang.Byte getByte(java.lang.Object);
  public java.lang.Double getDouble(java.lang.Object);
  public java.lang.Float getFloat(java.lang.Object);
  public java.lang.Character getChar(java.lang.Object);
  public java.lang.Long getLong(java.lang.Object);
  public java.lang.Boolean getBool(java.lang.Object);
  public java.lang.Short getShort(java.lang.Object);
  public java.lang.Integer getInt(java.lang.Object);
  public java.lang.String getStr(java.lang.Object);
  public java.lang.Object getObj(java.lang.Object);
}
```

## `cn.hutool.core.lang.Editor`

```java
public interface cn.hutool.core.lang.Editor<T> {
  public abstract T edit(T);
}
```

## `cn.hutool.core.lang.EnumItem`

```java
public interface cn.hutool.core.lang.EnumItem<E extends cn.hutool.core.lang.EnumItem<E>> extends java.io.Serializable {
  public abstract java.lang.String name();
  public default java.lang.String text();
  public abstract int intVal();
  public default E[] items();
  public default E fromInt(java.lang.Integer);
  public default E fromStr(java.lang.String);
}
```

## `cn.hutool.core.lang.Filter`

```java
public interface cn.hutool.core.lang.Filter<T> {
  public abstract boolean accept(T);
}
```

## `cn.hutool.core.lang.JarClassLoader`

```java
public class cn.hutool.core.lang.JarClassLoader extends java.net.URLClassLoader {
  public static cn.hutool.core.lang.JarClassLoader load(java.io.File);
  public static cn.hutool.core.lang.JarClassLoader loadJar(java.io.File);
  public static void loadJar(java.net.URLClassLoader, java.io.File) throws cn.hutool.core.exceptions.UtilException;
  public static java.net.URLClassLoader loadJarToSystemClassLoader(java.io.File);
  public cn.hutool.core.lang.JarClassLoader();
  public cn.hutool.core.lang.JarClassLoader(java.net.URL[]);
  public cn.hutool.core.lang.JarClassLoader(java.net.URL[], java.lang.ClassLoader);
  public cn.hutool.core.lang.JarClassLoader addJar(java.io.File);
  public void addURL(java.net.URL);
  public cn.hutool.core.lang.JarClassLoader addURL(java.io.File);
}
```

## `cn.hutool.core.lang.Matcher`

```java
public interface cn.hutool.core.lang.Matcher<T> {
  public abstract boolean match(T);
}
```

## `cn.hutool.core.lang.ObjectId`

```java
public class cn.hutool.core.lang.ObjectId {
  public cn.hutool.core.lang.ObjectId();
  public static boolean isValid(java.lang.String);
  public static byte[] nextBytes();
  public static java.lang.String next();
  public static java.lang.String next(boolean);
}
```

## `cn.hutool.core.lang.Opt`

```java
public class cn.hutool.core.lang.Opt<T> {
  public static <T> cn.hutool.core.lang.Opt<T> empty();
  public static <T> cn.hutool.core.lang.Opt<T> of(T);
  public static <T> cn.hutool.core.lang.Opt<T> ofNullable(T);
  public static <T> cn.hutool.core.lang.Opt<T> ofBlankAble(T);
  public static <T, R extends java.util.Collection<T>> cn.hutool.core.lang.Opt<R> ofEmptyAble(R);
  public static <T> cn.hutool.core.lang.Opt<T> ofTry(cn.hutool.core.lang.func.Func0<T>);
  public T get();
  public boolean isEmpty();
  public java.lang.Exception getException();
  public boolean isFail();
  public cn.hutool.core.lang.Opt<T> ifFail(java.util.function.Consumer<? super java.lang.Throwable>) throws java.lang.NullPointerException;
  public boolean isPresent();
  public cn.hutool.core.lang.Opt<T> ifPresent(java.util.function.Consumer<? super T>);
  public cn.hutool.core.lang.Opt<T> ifPresentOrElse(java.util.function.Consumer<? super T>, cn.hutool.core.lang.func.VoidFunc0);
  public <U> cn.hutool.core.lang.Opt<U> mapOrElse(java.util.function.Function<? super T, ? extends U>, cn.hutool.core.lang.func.VoidFunc0);
  public cn.hutool.core.lang.Opt<T> filter(java.util.function.Predicate<? super T>);
  public <U> cn.hutool.core.lang.Opt<U> map(java.util.function.Function<? super T, ? extends U>);
  public <U> cn.hutool.core.lang.Opt<U> flatMap(java.util.function.Function<? super T, ? extends cn.hutool.core.lang.Opt<? extends U>>);
  public <U> cn.hutool.core.lang.Opt<U> flattedMap(java.util.function.Function<? super T, ? extends java.util.Optional<? extends U>>);
  public cn.hutool.core.lang.Opt<T> peek(java.util.function.Consumer<T>) throws java.lang.NullPointerException;
  public final cn.hutool.core.lang.Opt<T> peeks(java.util.function.Consumer<T>...) throws java.lang.NullPointerException;
  public cn.hutool.core.lang.Opt<T> or(java.util.function.Supplier<? extends cn.hutool.core.lang.Opt<? extends T>>);
  public java.util.stream.Stream<T> stream();
  public T orElse(T);
  public T exceptionOrElse(T);
  public T orElseGet(java.util.function.Supplier<? extends T>);
  public T orElseThrow();
  public <X extends java.lang.Throwable> T orElseThrow(java.util.function.Supplier<? extends X>) throws X;
  public <X extends java.lang.Throwable> T orElseThrow(java.util.function.Function<java.lang.String, ? extends X>, java.lang.String) throws X;
  public java.util.Optional<T> toOptional();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `cn.hutool.core.lang.Pair`

```java
public class cn.hutool.core.lang.Pair<K, V> extends cn.hutool.core.clone.CloneSupport<cn.hutool.core.lang.Pair<K, V>> implements java.io.Serializable {
  public static <K, V> cn.hutool.core.lang.Pair<K, V> of(K, V);
  public cn.hutool.core.lang.Pair(K, V);
  public K getKey();
  public V getValue();
  public java.lang.String toString();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `cn.hutool.core.lang.ParameterizedTypeImpl`

```java
public class cn.hutool.core.lang.ParameterizedTypeImpl implements java.lang.reflect.ParameterizedType,java.io.Serializable {
  public cn.hutool.core.lang.ParameterizedTypeImpl(java.lang.reflect.Type[], java.lang.reflect.Type, java.lang.reflect.Type);
  public java.lang.reflect.Type[] getActualTypeArguments();
  public java.lang.reflect.Type getOwnerType();
  public java.lang.reflect.Type getRawType();
  public java.lang.String toString();
}
```

## `cn.hutool.core.lang.PatternPool`

```java
public class cn.hutool.core.lang.PatternPool {
  public cn.hutool.core.lang.PatternPool();
  public static java.util.regex.Pattern get(java.lang.String);
  public static java.util.regex.Pattern get(java.lang.String, int);
  public static java.util.regex.Pattern remove(java.lang.String, int);
  public static void clear();
}
```

## `cn.hutool.core.lang.Pid`

```java
public final class cn.hutool.core.lang.Pid extends java.lang.Enum<cn.hutool.core.lang.Pid> {
  public static cn.hutool.core.lang.Pid[] values();
  public static cn.hutool.core.lang.Pid valueOf(java.lang.String);
  public int get();
}
```

## `cn.hutool.core.lang.Range`

```java
public class cn.hutool.core.lang.Range<T> implements java.lang.Iterable<T>, java.util.Iterator<T>, java.io.Serializable {
  public cn.hutool.core.lang.Range(T, cn.hutool.core.lang.Range$Stepper<T>);
  public cn.hutool.core.lang.Range(T, T, cn.hutool.core.lang.Range$Stepper<T>);
  public cn.hutool.core.lang.Range(T, T, cn.hutool.core.lang.Range$Stepper<T>, boolean, boolean);
  public cn.hutool.core.lang.Range<T> disableLock();
  public boolean hasNext();
  public T next();
  public void remove();
  public java.util.Iterator<T> iterator();
  public cn.hutool.core.lang.Range<T> reset();
}
```

## `cn.hutool.core.lang.Range$Stepper`

```java
public interface cn.hutool.core.lang.Range$Stepper<T> {
  public abstract T step(T, T, int);
}
```

## `cn.hutool.core.lang.Replacer`

```java
public interface cn.hutool.core.lang.Replacer<T> {
  public abstract T replace(T);
}
```

## `cn.hutool.core.lang.ResourceClassLoader`

```java
public class cn.hutool.core.lang.ResourceClassLoader<T extends cn.hutool.core.io.resource.Resource> extends java.security.SecureClassLoader {
  public cn.hutool.core.lang.ResourceClassLoader(java.lang.ClassLoader, java.util.Map<java.lang.String, T>);
  public cn.hutool.core.lang.ResourceClassLoader<T> addResource(T);
}
```

## `cn.hutool.core.lang.Segment`

```java
public interface cn.hutool.core.lang.Segment<T extends java.lang.Number> {
  public abstract T getStartIndex();
  public abstract T getEndIndex();
  public default T length();
}
```

## `cn.hutool.core.lang.SimpleCache`

```java
public class cn.hutool.core.lang.SimpleCache<K, V> implements java.lang.Iterable<java.util.Map$Entry<K, V>>, java.io.Serializable {
  public cn.hutool.core.lang.SimpleCache();
  public cn.hutool.core.lang.SimpleCache(java.util.Map<cn.hutool.core.lang.mutable.Mutable<K>, V>);
  public V get(K);
  public V get(K, cn.hutool.core.lang.func.Func0<V>);
  public V get(K, java.util.function.Predicate<V>, cn.hutool.core.lang.func.Func0<V>);
  public V put(K, V);
  public V remove(K);
  public void clear();
  public java.util.Iterator<java.util.Map$Entry<K, V>> iterator();
}
```

## `cn.hutool.core.lang.Singleton`

```java
public final class cn.hutool.core.lang.Singleton {
  public static <T> T get(java.lang.Class<T>, java.lang.Object...);
  public static <T> T get(java.lang.String, cn.hutool.core.lang.func.Func0<T>);
  public static <T> T get(java.lang.String, java.lang.Object...);
  public static void put(java.lang.Object);
  public static void put(java.lang.String, java.lang.Object);
  public static boolean exists(java.lang.Class<?>, java.lang.Object...);
  public static java.util.Set<java.lang.Class<?>> getExistClass();
  public static void remove(java.lang.Class<?>);
  public static void remove(java.lang.String);
  public static void destroy();
}
```

## `cn.hutool.core.lang.Snowflake`

```java
public class cn.hutool.core.lang.Snowflake implements java.io.Serializable {
  public cn.hutool.core.lang.Snowflake();
  public cn.hutool.core.lang.Snowflake(long);
  public cn.hutool.core.lang.Snowflake(long, long);
  public cn.hutool.core.lang.Snowflake(long, long, boolean);
  public cn.hutool.core.lang.Snowflake(java.util.Date, long, long, boolean);
  public cn.hutool.core.lang.Snowflake(java.util.Date, long, long, boolean, long);
  public cn.hutool.core.lang.Snowflake(java.util.Date, long, long, boolean, long, long);
  public long getWorkerId(long);
  public long getDataCenterId(long);
  public long getGenerateDateTime(long);
  public cn.hutool.core.lang.Pair<java.lang.Long, java.lang.Long> getIdScopeByTimestamp(long, long);
  public cn.hutool.core.lang.Pair<java.lang.Long, java.lang.Long> getIdScopeByTimestamp(long, long, boolean);
  public synchronized long nextId();
  public java.lang.String nextIdStr();
}
```

## `cn.hutool.core.lang.Tuple`

```java
public class cn.hutool.core.lang.Tuple extends cn.hutool.core.clone.CloneSupport<cn.hutool.core.lang.Tuple> implements java.lang.Iterable<java.lang.Object>, java.io.Serializable {
  public cn.hutool.core.lang.Tuple(java.lang.Object...);
  public <T> T get(int);
  public java.lang.Object[] getMembers();
  public final java.util.List<java.lang.Object> toList();
  public cn.hutool.core.lang.Tuple setCacheHash(boolean);
  public int size();
  public boolean contains(java.lang.Object);
  public final java.util.stream.Stream<java.lang.Object> stream();
  public final java.util.stream.Stream<java.lang.Object> parallelStream();
  public final cn.hutool.core.lang.Tuple sub(int, int);
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
  public java.util.Iterator<java.lang.Object> iterator();
  public final java.util.Spliterator<java.lang.Object> spliterator();
}
```

## `cn.hutool.core.lang.TypeReference`

```java
public abstract class cn.hutool.core.lang.TypeReference<T> implements java.lang.reflect.Type {
  public cn.hutool.core.lang.TypeReference();
  public java.lang.reflect.Type getType();
  public java.lang.String toString();
}
```

## `cn.hutool.core.lang.UUID`

```java
public final class cn.hutool.core.lang.UUID implements java.io.Serializable, java.lang.Comparable<cn.hutool.core.lang.UUID> {
  public cn.hutool.core.lang.UUID(long, long);
  public static cn.hutool.core.lang.UUID fastUUID();
  public static cn.hutool.core.lang.UUID randomUUID();
  public static cn.hutool.core.lang.UUID randomUUID(boolean);
  public static cn.hutool.core.lang.UUID nameUUIDFromBytes(byte[]);
  public static cn.hutool.core.lang.UUID fromString(java.lang.String);
  public long getLeastSignificantBits();
  public long getMostSignificantBits();
  public int version();
  public int variant();
  public long timestamp() throws java.lang.UnsupportedOperationException;
  public int clockSequence() throws java.lang.UnsupportedOperationException;
  public long node() throws java.lang.UnsupportedOperationException;
  public java.lang.String toString();
  public java.lang.String toString(boolean);
  public int hashCode();
  public boolean equals(java.lang.Object);
  public int compareTo(cn.hutool.core.lang.UUID);
  public int compareTo(java.lang.Object);
}
```

## `cn.hutool.core.lang.Validator`

```java
public class cn.hutool.core.lang.Validator {
  public cn.hutool.core.lang.Validator();
  public static boolean isTrue(boolean);
  public static boolean isFalse(boolean);
  public static boolean validateTrue(boolean, java.lang.String, java.lang.Object...) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean validateFalse(boolean, java.lang.String, java.lang.Object...) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isNull(java.lang.Object);
  public static boolean isNotNull(java.lang.Object);
  public static <T> T validateNull(T, java.lang.String, java.lang.Object...) throws cn.hutool.core.exceptions.ValidateException;
  public static <T> T validateNotNull(T, java.lang.String, java.lang.Object...) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isEmpty(java.lang.Object);
  public static boolean isNotEmpty(java.lang.Object);
  public static <T> T validateEmpty(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static <T> T validateNotEmpty(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean equal(java.lang.Object, java.lang.Object);
  public static java.lang.Object validateEqual(java.lang.Object, java.lang.Object, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static void validateNotEqual(java.lang.Object, java.lang.Object, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static void validateNotEmptyAndEqual(java.lang.Object, java.lang.Object, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static void validateNotEmptyAndNotEqual(java.lang.Object, java.lang.Object, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static <T extends java.lang.CharSequence> T validateMatchRegex(java.lang.String, T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isMatchRegex(java.util.regex.Pattern, java.lang.CharSequence);
  public static boolean isMatchRegex(java.lang.String, java.lang.CharSequence);
  public static boolean isGeneral(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateGeneral(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isGeneral(java.lang.CharSequence, int, int);
  public static <T extends java.lang.CharSequence> T validateGeneral(T, int, int, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isGeneral(java.lang.CharSequence, int);
  public static <T extends java.lang.CharSequence> T validateGeneral(T, int, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isLetter(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateLetter(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isUpperCase(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateUpperCase(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isLowerCase(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateLowerCase(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isNumber(java.lang.CharSequence);
  public static boolean hasNumber(java.lang.CharSequence);
  public static java.lang.String validateNumber(java.lang.String, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isWord(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateWord(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isMoney(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateMoney(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isZipCode(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateZipCode(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isEmail(java.lang.CharSequence);
  public static boolean isEmail(java.lang.CharSequence, boolean);
  public static <T extends java.lang.CharSequence> T validateEmail(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isMobile(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateMobile(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isCitizenId(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateCitizenIdNumber(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isBirthday(int, int, int);
  public static boolean isBirthday(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateBirthday(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isIpv4(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateIpv4(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isIpv6(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateIpv6(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isMac(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateMac(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isPlateNumber(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validatePlateNumber(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isUrl(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateUrl(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isChinese(java.lang.CharSequence);
  public static boolean hasChinese(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateChinese(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isGeneralWithChinese(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateGeneralWithChinese(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isUUID(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateUUID(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isHex(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateHex(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isBetween(java.lang.Number, java.lang.Number, java.lang.Number);
  public static void validateBetween(java.lang.Number, java.lang.Number, java.lang.Number, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isCreditCode(java.lang.CharSequence);
  public static boolean isCarVin(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateCarVin(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static boolean isCarDrivingLicence(java.lang.CharSequence);
  public static boolean isChineseName(java.lang.CharSequence);
  public static <T extends java.lang.CharSequence> T validateCarDrivingLicence(T, java.lang.String) throws cn.hutool.core.exceptions.ValidateException;
  public static void checkIndexLimit(int, int);
}
```

## `cn.hutool.core.lang.Version`

```java
public class cn.hutool.core.lang.Version implements java.lang.Comparable<cn.hutool.core.lang.Version>, java.io.Serializable {
  public static cn.hutool.core.lang.Version of(java.lang.String);
  public cn.hutool.core.lang.Version(java.lang.String);
  public int compareTo(cn.hutool.core.lang.Version);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public int compareTo(java.lang.Object);
}
```

## `cn.hutool.core.lang.WeightListRandom`

```java
public class cn.hutool.core.lang.WeightListRandom<E> implements java.io.Serializable {
  public cn.hutool.core.lang.WeightListRandom();
  public cn.hutool.core.lang.WeightListRandom(int);
  public void add(E, double);
  public boolean remove(E);
  public E next();
  public E randomByWeight(double);
  public boolean isEmpty();
}
```

## `cn.hutool.core.lang.WeightRandom`

```java
public class cn.hutool.core.lang.WeightRandom<T> implements java.io.Serializable {
  public static <T> cn.hutool.core.lang.WeightRandom<T> create();
  public cn.hutool.core.lang.WeightRandom();
  public cn.hutool.core.lang.WeightRandom(cn.hutool.core.lang.WeightRandom$WeightObj<T>);
  public cn.hutool.core.lang.WeightRandom(java.lang.Iterable<cn.hutool.core.lang.WeightRandom$WeightObj<T>>);
  public cn.hutool.core.lang.WeightRandom(cn.hutool.core.lang.WeightRandom$WeightObj<T>[]);
  public cn.hutool.core.lang.WeightRandom<T> add(T, double);
  public cn.hutool.core.lang.WeightRandom<T> add(cn.hutool.core.lang.WeightRandom$WeightObj<T>);
  public cn.hutool.core.lang.WeightRandom<T> clear();
  public T next();
}
```

## `cn.hutool.core.lang.WeightRandom$WeightObj`

```java
public class cn.hutool.core.lang.WeightRandom$WeightObj<T> {
  public cn.hutool.core.lang.WeightRandom$WeightObj(T, double);
  public T getObj();
  public void setObj(T);
  public double getWeight();
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```
