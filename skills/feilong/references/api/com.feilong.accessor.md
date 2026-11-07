# com.feilong.accessor

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.accessor.Accessor`

```java
public interface com.feilong.accessor.Accessor {
  public abstract <T extends java.io.Serializable> T get(java.lang.String, javax.servlet.http.HttpServletRequest);
  public abstract void remove(java.lang.String, javax.servlet.http.HttpServletRequest);
}
```

## `com.feilong.accessor.AutoKeyAccessor`

```java
public interface com.feilong.accessor.AutoKeyAccessor extends com.feilong.accessor.Accessor {
  public abstract java.lang.String save(java.io.Serializable, javax.servlet.http.HttpServletRequest);
}
```

## `com.feilong.accessor.KeyAccessor`

```java
public interface com.feilong.accessor.KeyAccessor extends com.feilong.accessor.Accessor {
  public abstract void save(java.lang.String, java.io.Serializable, javax.servlet.http.HttpServletRequest);
}
```
