# com.google.common.annotations

版本：33.4.8-jre。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.google.common.annotations.GwtCompatible`

```java
public interface com.google.common.annotations.GwtCompatible extends java.lang.annotation.Annotation {
  public abstract boolean serializable();
  public abstract boolean emulated();
}
```

## `com.google.common.annotations.GwtIncompatible`

```java
public interface com.google.common.annotations.GwtIncompatible extends java.lang.annotation.Annotation {
  public abstract java.lang.String value();
}
```
