# com.feilong.accessor.session

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.accessor.session.AbstractSessionKeyAccessor`

```java
public abstract class com.feilong.accessor.session.AbstractSessionKeyAccessor {
  public com.feilong.accessor.session.AbstractSessionKeyAccessor();
  public <T extends java.io.Serializable> T get(java.lang.String, javax.servlet.http.HttpServletRequest);
  public void remove(java.lang.String, javax.servlet.http.HttpServletRequest);
}
```

## `com.feilong.accessor.session.SessionAccessor`

```java
public class com.feilong.accessor.session.SessionAccessor extends com.feilong.accessor.session.AbstractSessionKeyAccessor {
  public com.feilong.accessor.session.SessionAccessor();
  public com.feilong.accessor.session.SessionAccessor(java.lang.String);
  public void save(java.io.Serializable, javax.servlet.http.HttpServletRequest);
  public <T extends java.io.Serializable> T get(javax.servlet.http.HttpServletRequest);
  public void remove(javax.servlet.http.HttpServletRequest);
  public void setKey(java.lang.String);
  public java.lang.String getKey();
}
```

## `com.feilong.accessor.session.SessionAutoKeyAccessor`

```java
public class com.feilong.accessor.session.SessionAutoKeyAccessor extends com.feilong.accessor.session.AbstractSessionKeyAccessor implements com.feilong.accessor.AutoKeyAccessor {
  public com.feilong.accessor.session.SessionAutoKeyAccessor();
  public com.feilong.accessor.session.SessionAutoKeyAccessor(com.feilong.accessor.keygenerator.KeyGenerator);
  public java.lang.String save(java.io.Serializable, javax.servlet.http.HttpServletRequest);
  public void setKeyGenerator(com.feilong.accessor.keygenerator.KeyGenerator);
}
```

## `com.feilong.accessor.session.SessionKeyAccessor`

```java
public class com.feilong.accessor.session.SessionKeyAccessor extends com.feilong.accessor.session.AbstractSessionKeyAccessor implements com.feilong.accessor.KeyAccessor {
  public com.feilong.accessor.session.SessionKeyAccessor();
  public void save(java.lang.String, java.io.Serializable, javax.servlet.http.HttpServletRequest);
}
```
