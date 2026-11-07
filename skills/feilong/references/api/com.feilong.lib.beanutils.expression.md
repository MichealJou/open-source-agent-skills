# com.feilong.lib.beanutils.expression

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.beanutils.expression.DefaultResolver`

```java
public class com.feilong.lib.beanutils.expression.DefaultResolver implements com.feilong.lib.beanutils.expression.Resolver {
  public com.feilong.lib.beanutils.expression.DefaultResolver();
  public int getIndex(java.lang.String);
  public java.lang.String getKey(java.lang.String);
  public java.lang.String getProperty(java.lang.String);
  public boolean hasNested(java.lang.String);
  public boolean isIndexed(java.lang.String);
  public boolean isMapped(java.lang.String);
  public java.lang.String next(java.lang.String);
  public java.lang.String remove(java.lang.String);
}
```

## `com.feilong.lib.beanutils.expression.Resolver`

```java
public interface com.feilong.lib.beanutils.expression.Resolver {
  public abstract int getIndex(java.lang.String);
  public abstract java.lang.String getKey(java.lang.String);
  public abstract java.lang.String getProperty(java.lang.String);
  public abstract boolean hasNested(java.lang.String);
  public abstract boolean isIndexed(java.lang.String);
  public abstract boolean isMapped(java.lang.String);
  public abstract java.lang.String next(java.lang.String);
  public abstract java.lang.String remove(java.lang.String);
}
```
