# com.feilong.lib.collection4.comparators

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.collection4.comparators.BooleanComparator`

```java
public final class com.feilong.lib.collection4.comparators.BooleanComparator implements java.util.Comparator<java.lang.Boolean>, java.io.Serializable {
  public static com.feilong.lib.collection4.comparators.BooleanComparator getTrueFirstComparator();
  public static com.feilong.lib.collection4.comparators.BooleanComparator getFalseFirstComparator();
  public static com.feilong.lib.collection4.comparators.BooleanComparator booleanComparator(boolean);
  public com.feilong.lib.collection4.comparators.BooleanComparator();
  public com.feilong.lib.collection4.comparators.BooleanComparator(boolean);
  public int compare(java.lang.Boolean, java.lang.Boolean);
  public int hashCode();
  public boolean equals(java.lang.Object);
  public boolean sortsTrueFirst();
  public int compare(java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.collection4.comparators.ComparableComparator`

```java
public class com.feilong.lib.collection4.comparators.ComparableComparator<E extends java.lang.Comparable<? super E>> implements java.util.Comparator<E>, java.io.Serializable {
  public static <E extends java.lang.Comparable<? super E>> com.feilong.lib.collection4.comparators.ComparableComparator<E> comparableComparator();
  public com.feilong.lib.collection4.comparators.ComparableComparator();
  public int compare(E, E);
  public int hashCode();
  public boolean equals(java.lang.Object);
  public int compare(java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.collection4.comparators.ComparatorChain`

```java
public class com.feilong.lib.collection4.comparators.ComparatorChain<E> implements java.util.Comparator<E>, java.io.Serializable {
  public com.feilong.lib.collection4.comparators.ComparatorChain();
  public com.feilong.lib.collection4.comparators.ComparatorChain(java.util.Comparator<E>);
  public com.feilong.lib.collection4.comparators.ComparatorChain(java.util.Comparator<E>, boolean);
  public com.feilong.lib.collection4.comparators.ComparatorChain(java.util.List<java.util.Comparator<E>>);
  public com.feilong.lib.collection4.comparators.ComparatorChain(java.util.List<java.util.Comparator<E>>, java.util.BitSet);
  public void addComparator(java.util.Comparator<E>);
  public void addComparator(java.util.Comparator<E>, boolean);
  public void setComparator(int, java.util.Comparator<E>) throws java.lang.IndexOutOfBoundsException;
  public void setComparator(int, java.util.Comparator<E>, boolean);
  public void setForwardSort(int);
  public void setReverseSort(int);
  public int size();
  public boolean isLocked();
  public int compare(E, E) throws java.lang.UnsupportedOperationException;
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```

## `com.feilong.lib.collection4.comparators.FixedOrderComparator`

```java
public class com.feilong.lib.collection4.comparators.FixedOrderComparator<T> implements java.util.Comparator<T>, java.io.Serializable {
  public com.feilong.lib.collection4.comparators.FixedOrderComparator();
  public com.feilong.lib.collection4.comparators.FixedOrderComparator(T...);
  public com.feilong.lib.collection4.comparators.FixedOrderComparator(java.util.List<T>);
  public boolean isLocked();
  public com.feilong.lib.collection4.comparators.FixedOrderComparator$UnknownObjectBehavior getUnknownObjectBehavior();
  public void setUnknownObjectBehavior(com.feilong.lib.collection4.comparators.FixedOrderComparator$UnknownObjectBehavior);
  public boolean add(T);
  public boolean addAsEqual(T, T);
  public int compare(T, T);
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```

## `com.feilong.lib.collection4.comparators.FixedOrderComparator$UnknownObjectBehavior`

```java
public final class com.feilong.lib.collection4.comparators.FixedOrderComparator$UnknownObjectBehavior extends java.lang.Enum<com.feilong.lib.collection4.comparators.FixedOrderComparator$UnknownObjectBehavior> {
  public static com.feilong.lib.collection4.comparators.FixedOrderComparator$UnknownObjectBehavior[] values();
  public static com.feilong.lib.collection4.comparators.FixedOrderComparator$UnknownObjectBehavior valueOf(java.lang.String);
}
```

## `com.feilong.lib.collection4.comparators.NullComparator`

```java
public class com.feilong.lib.collection4.comparators.NullComparator<E> implements java.util.Comparator<E>, java.io.Serializable {
  public com.feilong.lib.collection4.comparators.NullComparator();
  public com.feilong.lib.collection4.comparators.NullComparator(java.util.Comparator<? super E>);
  public com.feilong.lib.collection4.comparators.NullComparator(boolean);
  public com.feilong.lib.collection4.comparators.NullComparator(java.util.Comparator<? super E>, boolean);
  public int compare(E, E);
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```

## `com.feilong.lib.collection4.comparators.ReverseComparator`

```java
public class com.feilong.lib.collection4.comparators.ReverseComparator<E> implements java.util.Comparator<E>, java.io.Serializable {
  public com.feilong.lib.collection4.comparators.ReverseComparator();
  public com.feilong.lib.collection4.comparators.ReverseComparator(java.util.Comparator<? super E>);
  public int compare(E, E);
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```

## `com.feilong.lib.collection4.comparators.TransformingComparator`

```java
public class com.feilong.lib.collection4.comparators.TransformingComparator<I, O> implements java.util.Comparator<I>, java.io.Serializable {
  public com.feilong.lib.collection4.comparators.TransformingComparator(org.apache.commons.collections4.Transformer<? super I, ? extends O>);
  public com.feilong.lib.collection4.comparators.TransformingComparator(org.apache.commons.collections4.Transformer<? super I, ? extends O>, java.util.Comparator<O>);
  public int compare(I, I);
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```
