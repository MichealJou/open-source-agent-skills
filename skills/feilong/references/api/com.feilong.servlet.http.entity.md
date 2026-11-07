# com.feilong.servlet.http.entity

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.servlet.http.entity.CookieEntity`

```java
public class com.feilong.servlet.http.entity.CookieEntity implements java.io.Serializable {
  public com.feilong.servlet.http.entity.CookieEntity();
  public com.feilong.servlet.http.entity.CookieEntity(java.lang.String, java.lang.String);
  public com.feilong.servlet.http.entity.CookieEntity(java.lang.String, java.lang.String, int);
  public java.lang.String getName();
  public void setName(java.lang.String);
  public java.lang.String getValue();
  public void setValue(java.lang.String);
  public int getMaxAge();
  public void setMaxAge(int);
  public java.lang.String getComment();
  public void setComment(java.lang.String);
  public java.lang.String getDomain();
  public void setDomain(java.lang.String);
  public java.lang.String getPath();
  public void setPath(java.lang.String);
  public boolean getSecure();
  public void setSecure(boolean);
  public int getVersion();
  public void setVersion(int);
  public boolean getHttpOnly();
  public void setHttpOnly(boolean);
}
```

## `com.feilong.servlet.http.entity.RequestIdentity`

```java
public class com.feilong.servlet.http.entity.RequestIdentity implements java.io.Serializable {
  public com.feilong.servlet.http.entity.RequestIdentity();
  public java.lang.String getClientIP();
  public void setClientIP(java.lang.String);
  public java.lang.String getUserAgent();
  public void setUserAgent(java.lang.String);
  public java.lang.String getSessionId();
  public void setSessionId(java.lang.String);
}
```

## `com.feilong.servlet.http.entity.RequestLogSwitch`

```java
public abstract class com.feilong.servlet.http.entity.RequestLogSwitch implements java.io.Serializable {
  public com.feilong.servlet.http.entity.RequestLogSwitch();
  public boolean getShowParams();
  public boolean getShowCookies();
  public boolean getShowIPs();
  public boolean getShowURLs();
  public boolean getShowPorts();
  public boolean getShowElses();
  public boolean getShowHeaders();
  public boolean getShowErrors();
  public boolean getShowFullURL();
  public boolean getShowMethod();
  public boolean getShowForwardInfos();
  public boolean getShowIncludeInfos();
  public boolean getShowIdentity();
}
```
