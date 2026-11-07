# cn.hutool.core.comparator

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.comparator.BaseFieldComparator`

```java
public abstract class cn.hutool.core.comparator.BaseFieldComparator<T> implements java.util.Comparator<T>, java.io.Serializable {
  public cn.hutool.core.comparator.BaseFieldComparator();
}
```

## `cn.hutool.core.comparator.ComparableComparator`

```java
public class cn.hutool.core.comparator.ComparableComparator<E extends java.lang.Comparable<? super E>> implements java.util.Comparator<E>, java.io.Serializable {
  public cn.hutool.core.comparator.ComparableComparator();
  public int compare(E, E);
  public int hashCode();
  public boolean equals(java.lang.Object);
  public int compare(java.lang.Object, java.lang.Object);
}
```

## `cn.hutool.core.comparator.ComparatorChain`

```java
public class cn.hutool.core.comparator.ComparatorChain<E> implements cn.hutool.core.lang.Chain<java.util.Comparator<E>, cn.hutool.core.comparator.ComparatorChain<E>>, java.util.Comparator<E>, java.io.Serializable {
  public static <E> cn.hutool.core.comparator.ComparatorChain<E> of(java.util.Comparator<E>);
  public static <E> cn.hutool.core.comparator.ComparatorChain<E> of(java.util.Comparator<E>, boolean);
  public static <E> cn.hutool.core.comparator.ComparatorChain<E> of(java.util.Comparator<E>...);
  public static <E> cn.hutool.core.comparator.ComparatorChain<E> of(java.util.List<java.util.Comparator<E>>);
  public static <E> cn.hutool.core.comparator.ComparatorChain<E> of(java.util.List<java.util.Comparator<E>>, java.util.BitSet);
  public cn.hutool.core.comparator.ComparatorChain();
  public cn.hutool.core.comparator.ComparatorChain(java.util.Comparator<E>);
  public cn.hutool.core.comparator.ComparatorChain(java.util.Comparator<E>, boolean);
  public cn.hutool.core.comparator.ComparatorChain(java.util.List<java.util.Comparator<E>>);
  public cn.hutool.core.comparator.ComparatorChain(java.util.List<java.util.Comparator<E>>, java.util.BitSet);
  public cn.hutool.core.comparator.ComparatorChain<E> addComparator(java.util.Comparator<E>);
  public cn.hutool.core.comparator.ComparatorChain<E> addComparator(java.util.Comparator<E>, boolean);
  public cn.hutool.core.comparator.ComparatorChain<E> setComparator(int, java.util.Comparator<E>) throws java.lang.IndexOutOfBoundsException;
  public cn.hutool.core.comparator.ComparatorChain<E> setComparator(int, java.util.Comparator<E>, boolean);
  public cn.hutool.core.comparator.ComparatorChain<E> setForwardSort(int);
  public cn.hutool.core.comparator.ComparatorChain<E> setReverseSort(int);
  public int size();
  public boolean isLocked();
  public java.util.Iterator<java.util.Comparator<E>> iterator();
  public cn.hutool.core.comparator.ComparatorChain<E> addChain(java.util.Comparator<E>);
  public int compare(E, E) throws java.lang.UnsupportedOperationException;
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.Object addChain(java.lang.Object);
}
```

## `cn.hutool.core.comparator.ComparatorException`

```java
public class cn.hutool.core.comparator.ComparatorException extends java.lang.RuntimeException {
  public cn.hutool.core.comparator.ComparatorException(java.lang.Throwable);
  public cn.hutool.core.comparator.ComparatorException(java.lang.String);
  public cn.hutool.core.comparator.ComparatorException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.comparator.ComparatorException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.comparator.ComparatorException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.core.comparator.CompareUtil`

```java
public class cn.hutool.core.comparator.CompareUtil {
  public cn.hutool.core.comparator.CompareUtil();
  public static <E extends java.lang.Comparable<? super E>> java.util.Comparator<E> naturalComparator();
  public static <T> int compare(T, T, java.util.Comparator<T>);
  public static <T extends java.lang.Comparable<? super T>> int compare(T, T);
  public static <T extends java.lang.Comparable<? super T>> int compare(T, T, boolean);
  public static <T> int compare(T, T, boolean);
  public static <T> java.util.Comparator<T> comparingPinyin(java.util.function.Function<T, java.lang.String>);
  public static <T> java.util.Comparator<T> comparingPinyin(java.util.function.Function<T, java.lang.String>, boolean);
  public static <T, U> java.util.Comparator<T> comparingIndexed(java.util.function.Function<? super T, ? extends U>, U...);
  public static <T, U> java.util.Comparator<T> comparingIndexed(java.util.function.Function<? super T, ? extends U>, boolean, U...);
}
```

## `cn.hutool.core.comparator.FieldComparator`

```java
public class cn.hutool.core.comparator.FieldComparator<T> extends cn.hutool.core.comparator.FuncComparator<T> {
  public cn.hutool.core.comparator.FieldComparator(java.lang.Class<T>, java.lang.String);
  public cn.hutool.core.comparator.FieldComparator(java.lang.reflect.Field);
  public cn.hutool.core.comparator.FieldComparator(boolean, boolean, java.lang.reflect.Field);
}
```

## `cn.hutool.core.comparator.FieldsComparator`

```java
public class cn.hutool.core.comparator.FieldsComparator<T> extends cn.hutool.core.comparator.NullComparator<T> {
  public cn.hutool.core.comparator.FieldsComparator(java.lang.Class<T>, java.lang.String...);
  public cn.hutool.core.comparator.FieldsComparator(boolean, java.lang.Class<T>, java.lang.String...);
}
```

## `cn.hutool.core.comparator.FuncComparator`

```java
public class cn.hutool.core.comparator.FuncComparator<T> extends cn.hutool.core.comparator.NullComparator<T> {
  public cn.hutool.core.comparator.FuncComparator(boolean, java.util.function.Function<T, java.lang.Comparable<?>>);
  public cn.hutool.core.comparator.FuncComparator(boolean, boolean, java.util.function.Function<T, java.lang.Comparable<?>>);
}
```

## `cn.hutool.core.comparator.IndexedComparator`

```java
public class cn.hutool.core.comparator.IndexedComparator<T> implements java.util.Comparator<T> {
  public cn.hutool.core.comparator.IndexedComparator(T...);
  public cn.hutool.core.comparator.IndexedComparator(boolean, T...);
  public int compare(T, T);
}
```

## `cn.hutool.core.comparator.InstanceComparator`

```java
public class cn.hutool.core.comparator.InstanceComparator<T> implements java.util.Comparator<T> {
  public cn.hutool.core.comparator.InstanceComparator(java.lang.Class<?>...);
  public cn.hutool.core.comparator.InstanceComparator(boolean, java.lang.Class<?>...);
  public int compare(T, T);
}
```

## `cn.hutool.core.comparator.LengthComparator`

```java
public class cn.hutool.core.comparator.LengthComparator implements java.util.Comparator<java.lang.CharSequence> {
  public cn.hutool.core.comparator.LengthComparator();
  public int compare(java.lang.CharSequence, java.lang.CharSequence);
  public int compare(java.lang.Object, java.lang.Object);
}
```

## `cn.hutool.core.comparator.NullComparator`

```java
public class cn.hutool.core.comparator.NullComparator<T> implements java.util.Comparator<T>, java.io.Serializable {
  public cn.hutool.core.comparator.NullComparator(boolean, java.util.Comparator<? super T>);
  public int compare(T, T);
  public java.util.Comparator<T> thenComparing(java.util.Comparator<? super T>);
}
```

## `cn.hutool.core.comparator.PinyinComparator`

```java
public class cn.hutool.core.comparator.PinyinComparator implements java.util.Comparator<java.lang.String>, java.io.Serializable {
  public cn.hutool.core.comparator.PinyinComparator();
  public int compare(java.lang.String, java.lang.String);
  public int compare(java.lang.Object, java.lang.Object);
}
```

## `cn.hutool.core.comparator.PropertyComparator`

```java
public class cn.hutool.core.comparator.PropertyComparator<T> extends cn.hutool.core.comparator.FuncComparator<T> {
  public cn.hutool.core.comparator.PropertyComparator(java.lang.String);
  public cn.hutool.core.comparator.PropertyComparator(java.lang.String, boolean);
  public cn.hutool.core.comparator.PropertyComparator(java.lang.String, boolean, boolean);
}
```

## `cn.hutool.core.comparator.ReverseComparator`

```java
public class cn.hutool.core.comparator.ReverseComparator<E> implements java.util.Comparator<E>, java.io.Serializable {
  public cn.hutool.core.comparator.ReverseComparator(java.util.Comparator<? super E>);
  public int compare(E, E);
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```

## `cn.hutool.core.comparator.VersionComparator`

```java
public class cn.hutool.core.comparator.VersionComparator implements java.util.Comparator<java.lang.String>, java.io.Serializable {
  public cn.hutool.core.comparator.VersionComparator();
  public int compare(java.lang.String, java.lang.String);
  public int compare(java.lang.Object, java.lang.Object);
}
```

## `cn.hutool.core.comparator.WindowsExplorerStringComparator`

```java
public class cn.hutool.core.comparator.WindowsExplorerStringComparator implements java.util.Comparator<java.lang.CharSequence> {
  public cn.hutool.core.comparator.WindowsExplorerStringComparator();
  public int compare(java.lang.CharSequence, java.lang.CharSequence);
  public int compare(java.lang.Object, java.lang.Object);
}
```
