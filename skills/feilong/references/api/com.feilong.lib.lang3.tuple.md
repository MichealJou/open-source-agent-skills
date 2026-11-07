# com.feilong.lib.lang3.tuple

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.lang3.tuple.ImmutablePair`

```java
public final class com.feilong.lib.lang3.tuple.ImmutablePair<L, R> extends com.feilong.lib.lang3.tuple.Pair<L, R> {
  public static <L, R> com.feilong.lib.lang3.tuple.ImmutablePair<L, R>[] emptyArray();
  public static <L, R> com.feilong.lib.lang3.tuple.ImmutablePair<L, R> nullPair();
  public static <L, R> com.feilong.lib.lang3.tuple.ImmutablePair<L, R> of(L, R);
  public static <L, R> com.feilong.lib.lang3.tuple.ImmutablePair<L, R> of(java.util.Map$Entry<L, R>);
  public com.feilong.lib.lang3.tuple.ImmutablePair(L, R);
  public L getLeft();
  public R getRight();
  public R setValue(R);
}
```

## `com.feilong.lib.lang3.tuple.ImmutableTriple`

```java
public final class com.feilong.lib.lang3.tuple.ImmutableTriple<L, M, R> extends com.feilong.lib.lang3.tuple.Triple<L, M, R> {
  public static <L, M, R> com.feilong.lib.lang3.tuple.ImmutableTriple<L, M, R>[] emptyArray();
  public static <L, M, R> com.feilong.lib.lang3.tuple.ImmutableTriple<L, M, R> nullTriple();
  public static <L, M, R> com.feilong.lib.lang3.tuple.ImmutableTriple<L, M, R> of(L, M, R);
  public com.feilong.lib.lang3.tuple.ImmutableTriple(L, M, R);
  public L getLeft();
  public M getMiddle();
  public R getRight();
}
```

## `com.feilong.lib.lang3.tuple.Pair`

```java
public abstract class com.feilong.lib.lang3.tuple.Pair<L, R> implements java.util.Map$Entry<L, R>, java.lang.Comparable<com.feilong.lib.lang3.tuple.Pair<L, R>>, java.io.Serializable {
  public com.feilong.lib.lang3.tuple.Pair();
  public static <L, R> com.feilong.lib.lang3.tuple.Pair<L, R>[] emptyArray();
  public static <L, R> com.feilong.lib.lang3.tuple.Pair<L, R> of(L, R);
  public static <L, R> com.feilong.lib.lang3.tuple.Pair<L, R> of(java.util.Map$Entry<L, R>);
  public int compareTo(com.feilong.lib.lang3.tuple.Pair<L, R>);
  public boolean equals(java.lang.Object);
  public final L getKey();
  public abstract L getLeft();
  public abstract R getRight();
  public R getValue();
  public int hashCode();
  public java.lang.String toString();
  public java.lang.String toString(java.lang.String);
  public int compareTo(java.lang.Object);
}
```

## `com.feilong.lib.lang3.tuple.Triple`

```java
public abstract class com.feilong.lib.lang3.tuple.Triple<L, M, R> implements java.lang.Comparable<com.feilong.lib.lang3.tuple.Triple<L, M, R>>, java.io.Serializable {
  public com.feilong.lib.lang3.tuple.Triple();
  public static <L, M, R> com.feilong.lib.lang3.tuple.Triple<L, M, R>[] emptyArray();
  public static <L, M, R> com.feilong.lib.lang3.tuple.Triple<L, M, R> of(L, M, R);
  public int compareTo(com.feilong.lib.lang3.tuple.Triple<L, M, R>);
  public boolean equals(java.lang.Object);
  public abstract L getLeft();
  public abstract M getMiddle();
  public abstract R getRight();
  public int hashCode();
  public java.lang.String toString();
  public java.lang.String toString(java.lang.String);
  public int compareTo(java.lang.Object);
}
```
