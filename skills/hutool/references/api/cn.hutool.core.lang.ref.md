# cn.hutool.core.lang.ref

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.lang.ref.PhantomObj`

```java
public class cn.hutool.core.lang.ref.PhantomObj<T> extends java.lang.ref.PhantomReference<T> implements cn.hutool.core.lang.ref.Ref<T> {
  public cn.hutool.core.lang.ref.PhantomObj(T, java.lang.ref.ReferenceQueue<? super T>);
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```

## `cn.hutool.core.lang.ref.Ref`

```java
public interface cn.hutool.core.lang.ref.Ref<T> {
  public abstract T get();
}
```

## `cn.hutool.core.lang.ref.ReferenceType`

```java
public final class cn.hutool.core.lang.ref.ReferenceType extends java.lang.Enum<cn.hutool.core.lang.ref.ReferenceType> {
  public static cn.hutool.core.lang.ref.ReferenceType[] values();
  public static cn.hutool.core.lang.ref.ReferenceType valueOf(java.lang.String);
}
```

## `cn.hutool.core.lang.ref.SoftObj`

```java
public class cn.hutool.core.lang.ref.SoftObj<T> extends java.lang.ref.SoftReference<T> implements cn.hutool.core.lang.ref.Ref<T> {
  public cn.hutool.core.lang.ref.SoftObj(T, java.lang.ref.ReferenceQueue<? super T>);
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```

## `cn.hutool.core.lang.ref.StrongObj`

```java
public class cn.hutool.core.lang.ref.StrongObj<T> implements cn.hutool.core.lang.ref.Ref<T> {
  public cn.hutool.core.lang.ref.StrongObj(T);
  public T get();
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```

## `cn.hutool.core.lang.ref.WeakObj`

```java
public class cn.hutool.core.lang.ref.WeakObj<T> extends java.lang.ref.WeakReference<T> implements cn.hutool.core.lang.ref.Ref<T> {
  public cn.hutool.core.lang.ref.WeakObj(T, java.lang.ref.ReferenceQueue<? super T>);
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```
