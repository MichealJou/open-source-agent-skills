# com.feilong.lib.collection4.iterators

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.collection4.iterators.ArrayIterator`

```java
public class com.feilong.lib.collection4.iterators.ArrayIterator<E> implements org.apache.commons.collections4.ResettableIterator<E> {
  public com.feilong.lib.collection4.iterators.ArrayIterator(java.lang.Object);
  public com.feilong.lib.collection4.iterators.ArrayIterator(java.lang.Object, int);
  public com.feilong.lib.collection4.iterators.ArrayIterator(java.lang.Object, int, int);
  public boolean hasNext();
  public E next();
  public void remove();
  public java.lang.Object getArray();
  public int getStartIndex();
  public int getEndIndex();
  public void reset();
}
```

## `com.feilong.lib.collection4.iterators.EmptyIterator`

```java
public class com.feilong.lib.collection4.iterators.EmptyIterator<E> extends com.feilong.lib.collection4.iterators.AbstractEmptyIterator<E> implements org.apache.commons.collections4.ResettableIterator<E> {
  public static <E> org.apache.commons.collections4.ResettableIterator<E> resettableEmptyIterator();
  public static <E> java.util.Iterator<E> emptyIterator();
  public void reset();
  public void remove();
  public void set(java.lang.Object);
  public void add(java.lang.Object);
  public int previousIndex();
  public int nextIndex();
  public java.lang.Object previous();
  public boolean hasPrevious();
  public java.lang.Object next();
  public boolean hasNext();
}
```

## `com.feilong.lib.collection4.iterators.EnumerationIterator`

```java
public class com.feilong.lib.collection4.iterators.EnumerationIterator<E> implements java.util.Iterator<E> {
  public com.feilong.lib.collection4.iterators.EnumerationIterator();
  public com.feilong.lib.collection4.iterators.EnumerationIterator(java.util.Enumeration<? extends E>);
  public com.feilong.lib.collection4.iterators.EnumerationIterator(java.util.Enumeration<? extends E>, java.util.Collection<? super E>);
  public boolean hasNext();
  public E next();
  public void remove();
  public java.util.Enumeration<? extends E> getEnumeration();
  public void setEnumeration(java.util.Enumeration<? extends E>);
}
```

## `com.feilong.lib.collection4.iterators.FilterIterator`

```java
public class com.feilong.lib.collection4.iterators.FilterIterator<E> implements java.util.Iterator<E> {
  public com.feilong.lib.collection4.iterators.FilterIterator();
  public com.feilong.lib.collection4.iterators.FilterIterator(java.util.Iterator<? extends E>);
  public com.feilong.lib.collection4.iterators.FilterIterator(java.util.Iterator<? extends E>, org.apache.commons.collections4.Predicate<? super E>);
  public boolean hasNext();
  public E next();
  public void remove();
  public java.util.Iterator<? extends E> getIterator();
  public void setIterator(java.util.Iterator<? extends E>);
  public org.apache.commons.collections4.Predicate<? super E> getPredicate();
  public void setPredicate(org.apache.commons.collections4.Predicate<? super E>);
}
```

## `com.feilong.lib.collection4.iterators.IteratorChain`

```java
public class com.feilong.lib.collection4.iterators.IteratorChain<E> implements java.util.Iterator<E> {
  public com.feilong.lib.collection4.iterators.IteratorChain();
  public com.feilong.lib.collection4.iterators.IteratorChain(java.util.Iterator<? extends E>);
  public com.feilong.lib.collection4.iterators.IteratorChain(java.util.Iterator<? extends E>, java.util.Iterator<? extends E>);
  public com.feilong.lib.collection4.iterators.IteratorChain(java.util.Iterator<? extends E>...);
  public com.feilong.lib.collection4.iterators.IteratorChain(java.util.Collection<java.util.Iterator<? extends E>>);
  public void addIterator(java.util.Iterator<? extends E>);
  public int size();
  public boolean isLocked();
  public boolean hasNext();
  public E next();
  public void remove();
}
```

## `com.feilong.lib.collection4.iterators.IteratorEnumeration`

```java
public class com.feilong.lib.collection4.iterators.IteratorEnumeration<E> implements java.util.Enumeration<E> {
  public com.feilong.lib.collection4.iterators.IteratorEnumeration();
  public com.feilong.lib.collection4.iterators.IteratorEnumeration(java.util.Iterator<? extends E>);
  public boolean hasMoreElements();
  public E nextElement();
  public java.util.Iterator<? extends E> getIterator();
  public void setIterator(java.util.Iterator<? extends E>);
}
```

## `com.feilong.lib.collection4.iterators.NodeListIterator`

```java
public class com.feilong.lib.collection4.iterators.NodeListIterator implements java.util.Iterator<org.w3c.dom.Node> {
  public com.feilong.lib.collection4.iterators.NodeListIterator(org.w3c.dom.Node);
  public com.feilong.lib.collection4.iterators.NodeListIterator(org.w3c.dom.NodeList);
  public boolean hasNext();
  public org.w3c.dom.Node next();
  public void remove();
  public java.lang.Object next();
}
```

## `com.feilong.lib.collection4.iterators.ObjectArrayIterator`

```java
public class com.feilong.lib.collection4.iterators.ObjectArrayIterator<E> implements org.apache.commons.collections4.ResettableIterator<E> {
  public com.feilong.lib.collection4.iterators.ObjectArrayIterator(E...);
  public com.feilong.lib.collection4.iterators.ObjectArrayIterator(E[], int);
  public com.feilong.lib.collection4.iterators.ObjectArrayIterator(E[], int, int);
  public boolean hasNext();
  public E next();
  public void remove();
  public E[] getArray();
  public int getStartIndex();
  public int getEndIndex();
  public void reset();
}
```

## `com.feilong.lib.collection4.iterators.SingletonIterator`

```java
public class com.feilong.lib.collection4.iterators.SingletonIterator<E> implements org.apache.commons.collections4.ResettableIterator<E> {
  public com.feilong.lib.collection4.iterators.SingletonIterator(E);
  public com.feilong.lib.collection4.iterators.SingletonIterator(E, boolean);
  public boolean hasNext();
  public E next();
  public void remove();
  public void reset();
}
```

## `com.feilong.lib.collection4.iterators.TransformIterator`

```java
public class com.feilong.lib.collection4.iterators.TransformIterator<I, O> implements java.util.Iterator<O> {
  public com.feilong.lib.collection4.iterators.TransformIterator();
  public com.feilong.lib.collection4.iterators.TransformIterator(java.util.Iterator<? extends I>);
  public com.feilong.lib.collection4.iterators.TransformIterator(java.util.Iterator<? extends I>, org.apache.commons.collections4.Transformer<? super I, ? extends O>);
  public boolean hasNext();
  public O next();
  public void remove();
  public java.util.Iterator<? extends I> getIterator();
  public void setIterator(java.util.Iterator<? extends I>);
  public org.apache.commons.collections4.Transformer<? super I, ? extends O> getTransformer();
  public void setTransformer(org.apache.commons.collections4.Transformer<? super I, ? extends O>);
}
```
