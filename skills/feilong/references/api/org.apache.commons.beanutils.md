# org.apache.commons.beanutils

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `org.apache.commons.beanutils.DynaBean`

```java
public interface org.apache.commons.beanutils.DynaBean {
  public abstract boolean contains(java.lang.String, java.lang.String);
  public abstract java.lang.Object get(java.lang.String);
  public abstract java.lang.Object get(java.lang.String, int);
  public abstract java.lang.Object get(java.lang.String, java.lang.String);
  public abstract com.feilong.lib.beanutils.DynaClass getDynaClass();
  public abstract void remove(java.lang.String, java.lang.String);
  public abstract void set(java.lang.String, java.lang.Object);
  public abstract void set(java.lang.String, int, java.lang.Object);
  public abstract void set(java.lang.String, java.lang.String, java.lang.Object);
}
```
