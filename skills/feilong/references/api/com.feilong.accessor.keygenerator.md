# com.feilong.accessor.keygenerator

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.accessor.keygenerator.FixValueKeyGenerator`

```java
public class com.feilong.accessor.keygenerator.FixValueKeyGenerator implements com.feilong.accessor.keygenerator.KeyGenerator {
  public com.feilong.accessor.keygenerator.FixValueKeyGenerator();
  public java.lang.String generator(java.io.Serializable, javax.servlet.http.HttpServletRequest);
  public void setKey(java.lang.String);
}
```

## `com.feilong.accessor.keygenerator.KeyGenerator`

```java
public interface com.feilong.accessor.keygenerator.KeyGenerator {
  public abstract java.lang.String generator(java.io.Serializable, javax.servlet.http.HttpServletRequest);
}
```

## `com.feilong.accessor.keygenerator.UUIDKeyGenerator`

```java
public class com.feilong.accessor.keygenerator.UUIDKeyGenerator implements com.feilong.accessor.keygenerator.KeyGenerator {
  public com.feilong.accessor.keygenerator.UUIDKeyGenerator();
  public java.lang.String generator(java.io.Serializable, javax.servlet.http.HttpServletRequest);
}
```
