# com.feilong.lib.lang3.compare

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.lang3.compare.ComparableUtils`

```java
public class com.feilong.lib.lang3.compare.ComparableUtils {
  public static <A extends java.lang.Comparable<A>> java.util.function.Predicate<A> between(A, A);
  public static <A extends java.lang.Comparable<A>> java.util.function.Predicate<A> betweenExclusive(A, A);
  public static <A extends java.lang.Comparable<A>> java.util.function.Predicate<A> ge(A);
  public static <A extends java.lang.Comparable<A>> java.util.function.Predicate<A> gt(A);
  public static <A extends java.lang.Comparable<A>> com.feilong.lib.lang3.compare.ComparableUtils$ComparableCheckBuilder<A> is(A);
  public static <A extends java.lang.Comparable<A>> java.util.function.Predicate<A> le(A);
  public static <A extends java.lang.Comparable<A>> java.util.function.Predicate<A> lt(A);
}
```

## `com.feilong.lib.lang3.compare.ComparableUtils$ComparableCheckBuilder`

```java
public class com.feilong.lib.lang3.compare.ComparableUtils$ComparableCheckBuilder<A extends java.lang.Comparable<A>> {
  public boolean between(A, A);
  public boolean betweenExclusive(A, A);
  public boolean equalTo(A);
  public boolean greaterThan(A);
  public boolean greaterThanOrEqualTo(A);
  public boolean lessThan(A);
  public boolean lessThanOrEqualTo(A);
}
```
