# cn.hutool.core.clone

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.clone.CloneRuntimeException`

```java
public class cn.hutool.core.clone.CloneRuntimeException extends java.lang.RuntimeException {
  public cn.hutool.core.clone.CloneRuntimeException(java.lang.Throwable);
  public cn.hutool.core.clone.CloneRuntimeException(java.lang.String);
  public cn.hutool.core.clone.CloneRuntimeException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.clone.CloneRuntimeException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.clone.CloneRuntimeException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.core.clone.CloneSupport`

```java
public class cn.hutool.core.clone.CloneSupport<T> implements cn.hutool.core.clone.Cloneable<T> {
  public cn.hutool.core.clone.CloneSupport();
  public T clone();
}
```

## `cn.hutool.core.clone.Cloneable`

```java
public interface cn.hutool.core.clone.Cloneable<T> extends java.lang.Cloneable {
  public abstract T clone();
}
```

## `cn.hutool.core.clone.DefaultCloneable`

```java
public interface cn.hutool.core.clone.DefaultCloneable<T> extends java.lang.Cloneable {
  public default T clone0();
}
```
