# com.feilong.lib.ognl.security

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.ognl.security.OgnlSecurityManager`

```java
public class com.feilong.lib.ognl.security.OgnlSecurityManager extends java.lang.SecurityManager {
  public com.feilong.lib.ognl.security.OgnlSecurityManager(java.lang.SecurityManager);
  public void checkPermission(java.security.Permission);
  public void checkPermission(java.security.Permission, java.lang.Object);
  public java.lang.Long enter();
  public void leave(long) throws java.lang.SecurityException;
}
```

## `com.feilong.lib.ognl.security.OgnlSecurityManagerFactory`

```java
public class com.feilong.lib.ognl.security.OgnlSecurityManagerFactory extends java.security.SecureClassLoader {
  public static java.lang.Object getOgnlSecurityManager();
}
```

## `com.feilong.lib.ognl.security.UserMethod`

```java
public class com.feilong.lib.ognl.security.UserMethod implements java.security.PrivilegedExceptionAction<java.lang.Object> {
  public com.feilong.lib.ognl.security.UserMethod(java.lang.Object, java.lang.reflect.Method, java.lang.Object[]);
  public java.lang.Object run() throws java.lang.Exception;
}
```
