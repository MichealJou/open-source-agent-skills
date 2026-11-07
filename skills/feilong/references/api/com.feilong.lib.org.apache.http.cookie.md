# com.feilong.lib.org.apache.http.cookie

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.cookie.ClientCookie`

```java
public interface com.feilong.lib.org.apache.http.cookie.ClientCookie extends com.feilong.lib.org.apache.http.cookie.Cookie {
  public abstract java.lang.String getAttribute(java.lang.String);
  public abstract boolean containsAttribute(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler`

```java
public interface com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler extends com.feilong.lib.org.apache.http.cookie.CookieAttributeHandler {
  public abstract java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.cookie.Cookie`

```java
public interface com.feilong.lib.org.apache.http.cookie.Cookie {
  public abstract java.lang.String getName();
  public abstract java.lang.String getValue();
  public abstract java.lang.String getComment();
  public abstract java.lang.String getCommentURL();
  public abstract java.util.Date getExpiryDate();
  public abstract boolean isPersistent();
  public abstract java.lang.String getDomain();
  public abstract java.lang.String getPath();
  public abstract int[] getPorts();
  public abstract boolean isSecure();
  public abstract int getVersion();
  public abstract boolean isExpired(java.util.Date);
}
```

## `com.feilong.lib.org.apache.http.cookie.CookieAttributeHandler`

```java
public interface com.feilong.lib.org.apache.http.cookie.CookieAttributeHandler {
  public abstract void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public abstract void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public abstract boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
}
```

## `com.feilong.lib.org.apache.http.cookie.CookieIdentityComparator`

```java
public class com.feilong.lib.org.apache.http.cookie.CookieIdentityComparator implements java.io.Serializable, java.util.Comparator<com.feilong.lib.org.apache.http.cookie.Cookie> {
  public com.feilong.lib.org.apache.http.cookie.CookieIdentityComparator();
  public int compare(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.Cookie);
  public int compare(java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.org.apache.http.cookie.CookieOrigin`

```java
public final class com.feilong.lib.org.apache.http.cookie.CookieOrigin {
  public com.feilong.lib.org.apache.http.cookie.CookieOrigin(java.lang.String, int, java.lang.String, boolean);
  public java.lang.String getHost();
  public java.lang.String getPath();
  public int getPort();
  public boolean isSecure();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.cookie.CookiePathComparator`

```java
public class com.feilong.lib.org.apache.http.cookie.CookiePathComparator implements java.io.Serializable, java.util.Comparator<com.feilong.lib.org.apache.http.cookie.Cookie> {
  public com.feilong.lib.org.apache.http.cookie.CookiePathComparator();
  public int compare(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.Cookie);
  public int compare(java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.org.apache.http.cookie.CookiePriorityComparator`

```java
public class com.feilong.lib.org.apache.http.cookie.CookiePriorityComparator implements java.util.Comparator<com.feilong.lib.org.apache.http.cookie.Cookie> {
  public com.feilong.lib.org.apache.http.cookie.CookiePriorityComparator();
  public int compare(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.Cookie);
  public int compare(java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.org.apache.http.cookie.CookieRestrictionViolationException`

```java
public class com.feilong.lib.org.apache.http.cookie.CookieRestrictionViolationException extends com.feilong.lib.org.apache.http.cookie.MalformedCookieException {
  public com.feilong.lib.org.apache.http.cookie.CookieRestrictionViolationException();
  public com.feilong.lib.org.apache.http.cookie.CookieRestrictionViolationException(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.cookie.CookieSpec`

```java
public interface com.feilong.lib.org.apache.http.cookie.CookieSpec {
  public abstract int getVersion();
  public abstract java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie> parse(com.feilong.lib.org.apache.http.Header, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public abstract void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public abstract boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public abstract java.util.List<com.feilong.lib.org.apache.http.Header> formatCookies(java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie>);
  public abstract com.feilong.lib.org.apache.http.Header getVersionHeader();
}
```

## `com.feilong.lib.org.apache.http.cookie.CookieSpecProvider`

```java
public interface com.feilong.lib.org.apache.http.cookie.CookieSpecProvider {
  public abstract com.feilong.lib.org.apache.http.cookie.CookieSpec create(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.cookie.MalformedCookieException`

```java
public class com.feilong.lib.org.apache.http.cookie.MalformedCookieException extends com.feilong.lib.org.apache.http.ProtocolException {
  public com.feilong.lib.org.apache.http.cookie.MalformedCookieException();
  public com.feilong.lib.org.apache.http.cookie.MalformedCookieException(java.lang.String);
  public com.feilong.lib.org.apache.http.cookie.MalformedCookieException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.cookie.SetCookie`

```java
public interface com.feilong.lib.org.apache.http.cookie.SetCookie extends com.feilong.lib.org.apache.http.cookie.Cookie {
  public abstract void setValue(java.lang.String);
  public abstract void setComment(java.lang.String);
  public abstract void setExpiryDate(java.util.Date);
  public abstract void setDomain(java.lang.String);
  public abstract void setPath(java.lang.String);
  public abstract void setSecure(boolean);
  public abstract void setVersion(int);
}
```

## `com.feilong.lib.org.apache.http.cookie.SetCookie2`

```java
public interface com.feilong.lib.org.apache.http.cookie.SetCookie2 extends com.feilong.lib.org.apache.http.cookie.SetCookie {
  public abstract void setCommentURL(java.lang.String);
  public abstract void setPorts(int[]);
  public abstract void setDiscard(boolean);
}
```
