# com.feilong.lib.org.apache.http.impl.cookie

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.impl.cookie.AbstractCookieAttributeHandler`

```java
public abstract class com.feilong.lib.org.apache.http.impl.cookie.AbstractCookieAttributeHandler implements com.feilong.lib.org.apache.http.cookie.CookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.AbstractCookieAttributeHandler();
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.AbstractCookieSpec`

```java
public abstract class com.feilong.lib.org.apache.http.impl.cookie.AbstractCookieSpec implements com.feilong.lib.org.apache.http.cookie.CookieSpec {
  public com.feilong.lib.org.apache.http.impl.cookie.AbstractCookieSpec();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.BasicClientCookie`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.BasicClientCookie implements com.feilong.lib.org.apache.http.cookie.SetCookie,com.feilong.lib.org.apache.http.cookie.ClientCookie,java.lang.Cloneable,java.io.Serializable {
  public com.feilong.lib.org.apache.http.impl.cookie.BasicClientCookie(java.lang.String, java.lang.String);
  public java.lang.String getName();
  public java.lang.String getValue();
  public void setValue(java.lang.String);
  public java.lang.String getComment();
  public void setComment(java.lang.String);
  public java.lang.String getCommentURL();
  public java.util.Date getExpiryDate();
  public void setExpiryDate(java.util.Date);
  public boolean isPersistent();
  public java.lang.String getDomain();
  public void setDomain(java.lang.String);
  public java.lang.String getPath();
  public void setPath(java.lang.String);
  public boolean isSecure();
  public void setSecure(boolean);
  public int[] getPorts();
  public int getVersion();
  public void setVersion(int);
  public boolean isExpired(java.util.Date);
  public java.util.Date getCreationDate();
  public void setCreationDate(java.util.Date);
  public void setAttribute(java.lang.String, java.lang.String);
  public java.lang.String getAttribute(java.lang.String);
  public boolean containsAttribute(java.lang.String);
  public boolean removeAttribute(java.lang.String);
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.BasicClientCookie2`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.BasicClientCookie2 extends com.feilong.lib.org.apache.http.impl.cookie.BasicClientCookie implements com.feilong.lib.org.apache.http.cookie.SetCookie2 {
  public com.feilong.lib.org.apache.http.impl.cookie.BasicClientCookie2(java.lang.String, java.lang.String);
  public int[] getPorts();
  public void setPorts(int[]);
  public java.lang.String getCommentURL();
  public void setCommentURL(java.lang.String);
  public void setDiscard(boolean);
  public boolean isPersistent();
  public boolean isExpired(java.util.Date);
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.BasicCommentHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.BasicCommentHandler extends com.feilong.lib.org.apache.http.impl.cookie.AbstractCookieAttributeHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.BasicCommentHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.BasicDomainHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.BasicDomainHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.BasicDomainHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.BasicExpiresHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.BasicExpiresHandler extends com.feilong.lib.org.apache.http.impl.cookie.AbstractCookieAttributeHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.BasicExpiresHandler(java.lang.String[]);
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.BasicMaxAgeHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.BasicMaxAgeHandler extends com.feilong.lib.org.apache.http.impl.cookie.AbstractCookieAttributeHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.BasicMaxAgeHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.BasicPathHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.BasicPathHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.BasicPathHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.BasicSecureHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.BasicSecureHandler extends com.feilong.lib.org.apache.http.impl.cookie.AbstractCookieAttributeHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.BasicSecureHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.CookieSpecBase`

```java
public abstract class com.feilong.lib.org.apache.http.impl.cookie.CookieSpecBase extends com.feilong.lib.org.apache.http.impl.cookie.AbstractCookieSpec {
  public com.feilong.lib.org.apache.http.impl.cookie.CookieSpecBase();
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpec`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpec implements com.feilong.lib.org.apache.http.cookie.CookieSpec {
  public com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpec(java.lang.String[], boolean);
  public com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpec();
  public java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie> parse(com.feilong.lib.org.apache.http.Header, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public java.util.List<com.feilong.lib.org.apache.http.Header> formatCookies(java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie>);
  public int getVersion();
  public com.feilong.lib.org.apache.http.Header getVersionHeader();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpecProvider`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpecProvider implements com.feilong.lib.org.apache.http.cookie.CookieSpecProvider {
  public com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpecProvider(com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpecProvider$CompatibilityLevel, com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher, java.lang.String[], boolean);
  public com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpecProvider(com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpecProvider$CompatibilityLevel, com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher);
  public com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpecProvider(com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher);
  public com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpecProvider();
  public com.feilong.lib.org.apache.http.cookie.CookieSpec create(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpecProvider$CompatibilityLevel`

```java
public final class com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpecProvider$CompatibilityLevel extends java.lang.Enum<com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpecProvider$CompatibilityLevel> {
  public static com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpecProvider$CompatibilityLevel[] values();
  public static com.feilong.lib.org.apache.http.impl.cookie.DefaultCookieSpecProvider$CompatibilityLevel valueOf(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.IgnoreSpec`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.IgnoreSpec extends com.feilong.lib.org.apache.http.impl.cookie.CookieSpecBase {
  public com.feilong.lib.org.apache.http.impl.cookie.IgnoreSpec();
  public int getVersion();
  public java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie> parse(com.feilong.lib.org.apache.http.Header, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public java.util.List<com.feilong.lib.org.apache.http.Header> formatCookies(java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie>);
  public com.feilong.lib.org.apache.http.Header getVersionHeader();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.IgnoreSpecProvider`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.IgnoreSpecProvider implements com.feilong.lib.org.apache.http.cookie.CookieSpecProvider {
  public com.feilong.lib.org.apache.http.impl.cookie.IgnoreSpecProvider();
  public com.feilong.lib.org.apache.http.cookie.CookieSpec create(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.LaxExpiresHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.LaxExpiresHandler extends com.feilong.lib.org.apache.http.impl.cookie.AbstractCookieAttributeHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.LaxExpiresHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.LaxMaxAgeHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.LaxMaxAgeHandler extends com.feilong.lib.org.apache.http.impl.cookie.AbstractCookieAttributeHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.LaxMaxAgeHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.NetscapeDomainHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.NetscapeDomainHandler extends com.feilong.lib.org.apache.http.impl.cookie.BasicDomainHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.NetscapeDomainHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.NetscapeDraftHeaderParser`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.NetscapeDraftHeaderParser {
  public com.feilong.lib.org.apache.http.impl.cookie.NetscapeDraftHeaderParser();
  public com.feilong.lib.org.apache.http.HeaderElement parseHeader(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor) throws com.feilong.lib.org.apache.http.ParseException;
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.NetscapeDraftSpec`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.NetscapeDraftSpec extends com.feilong.lib.org.apache.http.impl.cookie.CookieSpecBase {
  public com.feilong.lib.org.apache.http.impl.cookie.NetscapeDraftSpec(java.lang.String[]);
  public com.feilong.lib.org.apache.http.impl.cookie.NetscapeDraftSpec();
  public java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie> parse(com.feilong.lib.org.apache.http.Header, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public java.util.List<com.feilong.lib.org.apache.http.Header> formatCookies(java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie>);
  public int getVersion();
  public com.feilong.lib.org.apache.http.Header getVersionHeader();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.NetscapeDraftSpecProvider`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.NetscapeDraftSpecProvider implements com.feilong.lib.org.apache.http.cookie.CookieSpecProvider {
  public com.feilong.lib.org.apache.http.impl.cookie.NetscapeDraftSpecProvider(java.lang.String[]);
  public com.feilong.lib.org.apache.http.impl.cookie.NetscapeDraftSpecProvider();
  public com.feilong.lib.org.apache.http.cookie.CookieSpec create(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.PublicSuffixDomainFilter`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.PublicSuffixDomainFilter implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.PublicSuffixDomainFilter(com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler, com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher);
  public com.feilong.lib.org.apache.http.impl.cookie.PublicSuffixDomainFilter(com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler, com.feilong.lib.org.apache.http.conn.util.PublicSuffixList);
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public java.lang.String getAttributeName();
  public static com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler decorate(com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler, com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher);
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC2109DomainHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC2109DomainHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2109DomainHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC2109Spec`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC2109Spec extends com.feilong.lib.org.apache.http.impl.cookie.CookieSpecBase {
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2109Spec(java.lang.String[], boolean);
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2109Spec();
  public java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie> parse(com.feilong.lib.org.apache.http.Header, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public java.util.List<com.feilong.lib.org.apache.http.Header> formatCookies(java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie>);
  public int getVersion();
  public com.feilong.lib.org.apache.http.Header getVersionHeader();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC2109SpecProvider`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC2109SpecProvider implements com.feilong.lib.org.apache.http.cookie.CookieSpecProvider {
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2109SpecProvider(com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher, boolean);
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2109SpecProvider(com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher);
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2109SpecProvider();
  public com.feilong.lib.org.apache.http.cookie.CookieSpec create(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC2109VersionHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC2109VersionHandler extends com.feilong.lib.org.apache.http.impl.cookie.AbstractCookieAttributeHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2109VersionHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC2965CommentUrlAttributeHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC2965CommentUrlAttributeHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2965CommentUrlAttributeHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC2965DiscardAttributeHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC2965DiscardAttributeHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2965DiscardAttributeHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC2965DomainAttributeHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC2965DomainAttributeHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2965DomainAttributeHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean domainMatch(java.lang.String, java.lang.String);
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC2965PortAttributeHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC2965PortAttributeHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2965PortAttributeHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC2965Spec`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC2965Spec extends com.feilong.lib.org.apache.http.impl.cookie.RFC2109Spec {
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2965Spec();
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2965Spec(java.lang.String[], boolean);
  public java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie> parse(com.feilong.lib.org.apache.http.Header, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public int getVersion();
  public com.feilong.lib.org.apache.http.Header getVersionHeader();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC2965SpecProvider`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC2965SpecProvider implements com.feilong.lib.org.apache.http.cookie.CookieSpecProvider {
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2965SpecProvider(com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher, boolean);
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2965SpecProvider(com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher);
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2965SpecProvider();
  public com.feilong.lib.org.apache.http.cookie.CookieSpec create(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC2965VersionAttributeHandler`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC2965VersionAttributeHandler implements com.feilong.lib.org.apache.http.cookie.CommonCookieAttributeHandler {
  public com.feilong.lib.org.apache.http.impl.cookie.RFC2965VersionAttributeHandler();
  public void parse(com.feilong.lib.org.apache.http.cookie.SetCookie, java.lang.String) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public java.lang.String getAttributeName();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpec`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpec implements com.feilong.lib.org.apache.http.cookie.CookieSpec {
  public final java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie> parse(com.feilong.lib.org.apache.http.Header, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public final void validate(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin) throws com.feilong.lib.org.apache.http.cookie.MalformedCookieException;
  public final boolean match(com.feilong.lib.org.apache.http.cookie.Cookie, com.feilong.lib.org.apache.http.cookie.CookieOrigin);
  public java.util.List<com.feilong.lib.org.apache.http.Header> formatCookies(java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie>);
  public final int getVersion();
  public final com.feilong.lib.org.apache.http.Header getVersionHeader();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpecProvider`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpecProvider implements com.feilong.lib.org.apache.http.cookie.CookieSpecProvider {
  public com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpecProvider(com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpecProvider$CompatibilityLevel, com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher);
  public com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpecProvider(com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher);
  public com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpecProvider();
  public com.feilong.lib.org.apache.http.cookie.CookieSpec create(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpecProvider$CompatibilityLevel`

```java
public final class com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpecProvider$CompatibilityLevel extends java.lang.Enum<com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpecProvider$CompatibilityLevel> {
  public static com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpecProvider$CompatibilityLevel[] values();
  public static com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpecProvider$CompatibilityLevel valueOf(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC6265LaxSpec`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC6265LaxSpec extends com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpecBase {
  public com.feilong.lib.org.apache.http.impl.cookie.RFC6265LaxSpec();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.cookie.RFC6265StrictSpec`

```java
public class com.feilong.lib.org.apache.http.impl.cookie.RFC6265StrictSpec extends com.feilong.lib.org.apache.http.impl.cookie.RFC6265CookieSpecBase {
  public com.feilong.lib.org.apache.http.impl.cookie.RFC6265StrictSpec();
  public java.lang.String toString();
}
```
