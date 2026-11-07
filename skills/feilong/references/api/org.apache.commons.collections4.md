# org.apache.commons.collections4

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `org.apache.commons.collections4.Closure`

```java
public interface org.apache.commons.collections4.Closure<T> {
  public abstract void execute(T);
}
```

## `org.apache.commons.collections4.Equator`

```java
public interface org.apache.commons.collections4.Equator<T> {
  public abstract boolean equate(T, T);
  public abstract int hash(T);
}
```

## `org.apache.commons.collections4.Predicate`

```java
public interface org.apache.commons.collections4.Predicate<T> {
  public abstract boolean evaluate(T);
}
```

## `org.apache.commons.collections4.ResettableIterator`

```java
public interface org.apache.commons.collections4.ResettableIterator<E> extends java.util.Iterator<E> {
  public abstract void reset();
}
```

## `org.apache.commons.collections4.Transformer`

```java
public interface org.apache.commons.collections4.Transformer<I, O> {
  public abstract O transform(I);
}
```
