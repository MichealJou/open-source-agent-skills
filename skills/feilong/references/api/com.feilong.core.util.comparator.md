# com.feilong.core.util.comparator

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.core.util.comparator.BeanComparatorUtil`

```java
public final class com.feilong.core.util.comparator.BeanComparatorUtil {
  public static <T> java.util.Comparator<T> chainedComparator(java.lang.String...);
  public static <T> java.util.Comparator<T> propertyComparator(java.lang.String);
  public static <T, V> java.util.Comparator<T> propertyComparator(java.lang.String, V...);
  public static <T, V> java.util.Comparator<T> propertyComparator(java.lang.String, java.util.List<V>);
  public static <T, V> java.util.Comparator<T> propertyComparator(java.lang.String, java.util.List<V>, com.feilong.lib.collection4.comparators.FixedOrderComparator$UnknownObjectBehavior);
}
```

## `com.feilong.core.util.comparator.ComparatorUtil`

```java
public final class com.feilong.core.util.comparator.ComparatorUtil {
  public static <T> com.feilong.lib.collection4.comparators.FixedOrderComparator<T> buildFixedOrderComparator(java.util.List<T>);
  public static <T> com.feilong.lib.collection4.comparators.FixedOrderComparator<T> buildFixedOrderComparator(java.util.List<T>, com.feilong.lib.collection4.comparators.FixedOrderComparator$UnknownObjectBehavior);
}
```

## `com.feilong.core.util.comparator.PropertyComparator`

```java
public class com.feilong.core.util.comparator.PropertyComparator<T> implements java.util.Comparator<T>, java.io.Serializable {
  public com.feilong.core.util.comparator.PropertyComparator(java.lang.String);
  public com.feilong.core.util.comparator.PropertyComparator(java.lang.String, java.util.Comparator);
  public com.feilong.core.util.comparator.PropertyComparator(java.lang.String, java.lang.Class<? extends java.lang.Comparable>);
  public com.feilong.core.util.comparator.PropertyComparator(java.lang.String, java.lang.Class<? extends java.lang.Comparable>, java.util.Comparator);
  public int compare(T, T);
}
```

## `com.feilong.core.util.comparator.RegexGroupNumberComparator`

```java
public class com.feilong.core.util.comparator.RegexGroupNumberComparator implements java.util.Comparator<java.lang.String>, java.io.Serializable {
  public com.feilong.core.util.comparator.RegexGroupNumberComparator(java.lang.String);
  public int compare(java.lang.String, java.lang.String);
  public int compare(java.lang.Object, java.lang.Object);
}
```

## `com.feilong.core.util.comparator.SortHelper`

```java
public final class com.feilong.core.util.comparator.SortHelper {
  public static java.lang.String[] parsePropertyNameAndOrder(java.lang.String);
  public static boolean isAsc(java.lang.String[]);
}
```
