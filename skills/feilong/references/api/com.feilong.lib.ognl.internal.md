# com.feilong.lib.ognl.internal

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.ognl.internal.ClassCache`

```java
public interface com.feilong.lib.ognl.internal.ClassCache {
  public abstract void setClassInspector(com.feilong.lib.ognl.ClassCacheInspector);
  public abstract void clear();
  public abstract int getSize();
  public abstract java.lang.Object get(java.lang.Class);
  public abstract java.lang.Object put(java.lang.Class, java.lang.Object);
}
```

## `com.feilong.lib.ognl.internal.ClassCacheImpl`

```java
public class com.feilong.lib.ognl.internal.ClassCacheImpl implements com.feilong.lib.ognl.internal.ClassCache {
  public com.feilong.lib.ognl.internal.ClassCacheImpl();
  public void setClassInspector(com.feilong.lib.ognl.ClassCacheInspector);
  public void clear();
  public int getSize();
  public final java.lang.Object get(java.lang.Class);
  public final java.lang.Object put(java.lang.Class, java.lang.Object);
  public java.lang.String toString();
}
```
