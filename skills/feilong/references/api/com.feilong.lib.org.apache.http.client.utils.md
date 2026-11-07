# com.feilong.lib.org.apache.http.client.utils

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.client.utils.CloneUtils`

```java
public class com.feilong.lib.org.apache.http.client.utils.CloneUtils {
  public static <T> T cloneObject(T) throws java.lang.CloneNotSupportedException;
  public static java.lang.Object clone(java.lang.Object) throws java.lang.CloneNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.client.utils.DateUtils`

```java
public final class com.feilong.lib.org.apache.http.client.utils.DateUtils {
  public static java.util.Date parseDate(java.lang.String);
  public static java.util.Date parseDate(java.lang.String, java.lang.String[]);
  public static java.util.Date parseDate(java.lang.String, java.lang.String[], java.util.Date);
  public static java.lang.String formatDate(java.util.Date);
  public static java.lang.String formatDate(java.util.Date, java.lang.String);
  public static void clearThreadLocal();
}
```

## `com.feilong.lib.org.apache.http.client.utils.HttpClientUtils`

```java
public class com.feilong.lib.org.apache.http.client.utils.HttpClientUtils {
  public static void closeQuietly(com.feilong.lib.org.apache.http.HttpResponse);
  public static void closeQuietly(com.feilong.lib.org.apache.http.client.methods.CloseableHttpResponse);
  public static void closeQuietly(com.feilong.lib.org.apache.http.client.HttpClient);
}
```

## `com.feilong.lib.org.apache.http.client.utils.URIBuilder`

```java
public class com.feilong.lib.org.apache.http.client.utils.URIBuilder {
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder();
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder(java.lang.String) throws java.net.URISyntaxException;
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder(java.net.URI);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder(java.lang.String, java.nio.charset.Charset) throws java.net.URISyntaxException;
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder(java.net.URI, java.nio.charset.Charset);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setCharset(java.nio.charset.Charset);
  public java.nio.charset.Charset getCharset();
  public java.net.URI build() throws java.net.URISyntaxException;
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setScheme(java.lang.String);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setUserInfo(java.lang.String);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setUserInfo(java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setHost(java.lang.String);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setPort(int);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setPath(java.lang.String);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setPathSegments(java.lang.String...);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setPathSegments(java.util.List<java.lang.String>);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder removeQuery();
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setQuery(java.lang.String);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setParameters(java.util.List<com.feilong.lib.org.apache.http.NameValuePair>);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder addParameters(java.util.List<com.feilong.lib.org.apache.http.NameValuePair>);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setParameters(com.feilong.lib.org.apache.http.NameValuePair...);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder addParameter(java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setParameter(java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder clearParameters();
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setCustomQuery(java.lang.String);
  public com.feilong.lib.org.apache.http.client.utils.URIBuilder setFragment(java.lang.String);
  public boolean isAbsolute();
  public boolean isOpaque();
  public java.lang.String getScheme();
  public java.lang.String getUserInfo();
  public java.lang.String getHost();
  public int getPort();
  public boolean isPathEmpty();
  public java.util.List<java.lang.String> getPathSegments();
  public java.lang.String getPath();
  public boolean isQueryEmpty();
  public java.util.List<com.feilong.lib.org.apache.http.NameValuePair> getQueryParams();
  public java.lang.String getFragment();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.client.utils.URIUtils`

```java
public class com.feilong.lib.org.apache.http.client.utils.URIUtils {
  public static java.net.URI createURI(java.lang.String, java.lang.String, int, java.lang.String, java.lang.String, java.lang.String) throws java.net.URISyntaxException;
  public static java.net.URI rewriteURI(java.net.URI, com.feilong.lib.org.apache.http.HttpHost, boolean) throws java.net.URISyntaxException;
  public static java.net.URI rewriteURI(java.net.URI, com.feilong.lib.org.apache.http.HttpHost, java.util.EnumSet<com.feilong.lib.org.apache.http.client.utils.URIUtils$UriFlag>) throws java.net.URISyntaxException;
  public static java.net.URI rewriteURI(java.net.URI, com.feilong.lib.org.apache.http.HttpHost) throws java.net.URISyntaxException;
  public static java.net.URI rewriteURI(java.net.URI) throws java.net.URISyntaxException;
  public static java.net.URI rewriteURIForRoute(java.net.URI, com.feilong.lib.org.apache.http.conn.routing.RouteInfo) throws java.net.URISyntaxException;
  public static java.net.URI rewriteURIForRoute(java.net.URI, com.feilong.lib.org.apache.http.conn.routing.RouteInfo, boolean) throws java.net.URISyntaxException;
  public static java.net.URI resolve(java.net.URI, java.lang.String);
  public static java.net.URI resolve(java.net.URI, java.net.URI);
  public static java.net.URI normalizeSyntax(java.net.URI) throws java.net.URISyntaxException;
  public static com.feilong.lib.org.apache.http.HttpHost extractHost(java.net.URI);
  public static java.net.URI resolve(java.net.URI, com.feilong.lib.org.apache.http.HttpHost, java.util.List<java.net.URI>) throws java.net.URISyntaxException;
}
```

## `com.feilong.lib.org.apache.http.client.utils.URIUtils$UriFlag`

```java
public final class com.feilong.lib.org.apache.http.client.utils.URIUtils$UriFlag extends java.lang.Enum<com.feilong.lib.org.apache.http.client.utils.URIUtils$UriFlag> {
  public static com.feilong.lib.org.apache.http.client.utils.URIUtils$UriFlag[] values();
  public static com.feilong.lib.org.apache.http.client.utils.URIUtils$UriFlag valueOf(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.client.utils.URLEncodedUtils`

```java
public class com.feilong.lib.org.apache.http.client.utils.URLEncodedUtils {
  public com.feilong.lib.org.apache.http.client.utils.URLEncodedUtils();
  public static java.util.List<com.feilong.lib.org.apache.http.NameValuePair> parse(java.net.URI, java.lang.String);
  public static java.util.List<com.feilong.lib.org.apache.http.NameValuePair> parse(java.net.URI, java.nio.charset.Charset);
  public static java.util.List<com.feilong.lib.org.apache.http.NameValuePair> parse(com.feilong.lib.org.apache.http.HttpEntity) throws java.io.IOException;
  public static boolean isEncoded(com.feilong.lib.org.apache.http.HttpEntity);
  public static void parse(java.util.List<com.feilong.lib.org.apache.http.NameValuePair>, java.util.Scanner, java.lang.String);
  public static void parse(java.util.List<com.feilong.lib.org.apache.http.NameValuePair>, java.util.Scanner, java.lang.String, java.lang.String);
  public static java.util.List<com.feilong.lib.org.apache.http.NameValuePair> parse(java.lang.String, java.nio.charset.Charset);
  public static java.util.List<com.feilong.lib.org.apache.http.NameValuePair> parse(java.lang.String, java.nio.charset.Charset, char...);
  public static java.util.List<com.feilong.lib.org.apache.http.NameValuePair> parse(com.feilong.lib.org.apache.http.util.CharArrayBuffer, java.nio.charset.Charset, char...);
  public static java.util.List<java.lang.String> parsePathSegments(java.lang.CharSequence, java.nio.charset.Charset);
  public static java.util.List<java.lang.String> parsePathSegments(java.lang.CharSequence);
  public static java.lang.String formatSegments(java.lang.Iterable<java.lang.String>, java.nio.charset.Charset);
  public static java.lang.String formatSegments(java.lang.String...);
  public static java.lang.String format(java.util.List<? extends com.feilong.lib.org.apache.http.NameValuePair>, java.lang.String);
  public static java.lang.String format(java.util.List<? extends com.feilong.lib.org.apache.http.NameValuePair>, char, java.lang.String);
  public static java.lang.String format(java.lang.Iterable<? extends com.feilong.lib.org.apache.http.NameValuePair>, java.nio.charset.Charset);
  public static java.lang.String format(java.lang.Iterable<? extends com.feilong.lib.org.apache.http.NameValuePair>, char, java.nio.charset.Charset);
}
```
