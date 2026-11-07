# cn.hutool.core.net.url

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.net.url.UrlBuilder`

```java
public final class cn.hutool.core.net.url.UrlBuilder implements cn.hutool.core.builder.Builder<java.lang.String> {
  public static cn.hutool.core.net.url.UrlBuilder of(java.net.URI, java.nio.charset.Charset);
  public static cn.hutool.core.net.url.UrlBuilder ofHttpWithoutEncode(java.lang.String);
  public static cn.hutool.core.net.url.UrlBuilder ofHttp(java.lang.String);
  public static cn.hutool.core.net.url.UrlBuilder ofHttp(java.lang.String, java.nio.charset.Charset);
  public static cn.hutool.core.net.url.UrlBuilder of(java.lang.String);
  public static cn.hutool.core.net.url.UrlBuilder of(java.lang.String, java.nio.charset.Charset);
  public static cn.hutool.core.net.url.UrlBuilder of(java.net.URL, java.nio.charset.Charset);
  public static cn.hutool.core.net.url.UrlBuilder of(java.lang.String, java.lang.String, int, java.lang.String, java.lang.String, java.lang.String, java.nio.charset.Charset);
  public static cn.hutool.core.net.url.UrlBuilder of(java.lang.String, java.lang.String, int, cn.hutool.core.net.url.UrlPath, cn.hutool.core.net.url.UrlQuery, java.lang.String, java.nio.charset.Charset);
  public static cn.hutool.core.net.url.UrlBuilder create();
  public static cn.hutool.core.net.url.UrlBuilder of();
  public cn.hutool.core.net.url.UrlBuilder();
  public cn.hutool.core.net.url.UrlBuilder(java.lang.String, java.lang.String, int, cn.hutool.core.net.url.UrlPath, cn.hutool.core.net.url.UrlQuery, java.lang.String, java.nio.charset.Charset);
  public java.lang.String getScheme();
  public java.lang.String getSchemeWithDefault();
  public cn.hutool.core.net.url.UrlBuilder setScheme(java.lang.String);
  public java.lang.String getHost();
  public cn.hutool.core.net.url.UrlBuilder setHost(java.lang.String);
  public int getPort();
  public int getPortWithDefault();
  public cn.hutool.core.net.url.UrlBuilder setPort(int);
  public java.lang.String getAuthority();
  public cn.hutool.core.net.url.UrlPath getPath();
  public java.lang.String getPathStr();
  public cn.hutool.core.net.url.UrlBuilder setWithEndTag(boolean);
  public cn.hutool.core.net.url.UrlBuilder setPath(cn.hutool.core.net.url.UrlPath);
  public cn.hutool.core.net.url.UrlBuilder addPath(java.lang.CharSequence);
  public cn.hutool.core.net.url.UrlBuilder addPathSegment(java.lang.CharSequence);
  public cn.hutool.core.net.url.UrlBuilder appendPath(java.lang.CharSequence);
  public cn.hutool.core.net.url.UrlQuery getQuery();
  public java.lang.String getQueryStr();
  public cn.hutool.core.net.url.UrlBuilder setQuery(cn.hutool.core.net.url.UrlQuery);
  public cn.hutool.core.net.url.UrlBuilder addQuery(java.lang.String, java.lang.Object);
  public java.lang.String getFragment();
  public java.lang.String getFragmentEncoded();
  public cn.hutool.core.net.url.UrlBuilder setFragment(java.lang.String);
  public java.nio.charset.Charset getCharset();
  public cn.hutool.core.net.url.UrlBuilder setCharset(java.nio.charset.Charset);
  public java.lang.String build();
  public java.net.URL toURL();
  public java.net.URL toURL(java.net.URLStreamHandler);
  public java.net.URI toURI();
  public java.lang.String toString();
  public java.lang.Object build();
}
```

## `cn.hutool.core.net.url.UrlPath`

```java
public class cn.hutool.core.net.url.UrlPath {
  public cn.hutool.core.net.url.UrlPath();
  public static cn.hutool.core.net.url.UrlPath of(java.lang.CharSequence, java.nio.charset.Charset);
  public cn.hutool.core.net.url.UrlPath setWithEndTag(boolean);
  public java.util.List<java.lang.String> getSegments();
  public java.lang.String getSegment(int);
  public cn.hutool.core.net.url.UrlPath add(java.lang.CharSequence);
  public cn.hutool.core.net.url.UrlPath addBefore(java.lang.CharSequence);
  public cn.hutool.core.net.url.UrlPath parse(java.lang.CharSequence, java.nio.charset.Charset);
  public java.lang.String build(java.nio.charset.Charset);
  public java.lang.String build(java.nio.charset.Charset, boolean);
  public java.lang.String toString();
}
```

## `cn.hutool.core.net.url.UrlQuery`

```java
public class cn.hutool.core.net.url.UrlQuery {
  public static cn.hutool.core.net.url.UrlQuery of(java.util.Map<? extends java.lang.CharSequence, ?>);
  public static cn.hutool.core.net.url.UrlQuery of(java.util.Map<? extends java.lang.CharSequence, ?>, boolean);
  public static cn.hutool.core.net.url.UrlQuery of(java.lang.String, java.nio.charset.Charset);
  public static cn.hutool.core.net.url.UrlQuery of(java.lang.String, java.nio.charset.Charset, boolean);
  public static cn.hutool.core.net.url.UrlQuery of(java.lang.String, java.nio.charset.Charset, boolean, boolean);
  public cn.hutool.core.net.url.UrlQuery();
  public cn.hutool.core.net.url.UrlQuery(boolean);
  public cn.hutool.core.net.url.UrlQuery(java.util.Map<? extends java.lang.CharSequence, ?>);
  public cn.hutool.core.net.url.UrlQuery(java.util.Map<? extends java.lang.CharSequence, ?>, boolean);
  public cn.hutool.core.net.url.UrlQuery setStrict(boolean);
  public cn.hutool.core.net.url.UrlQuery add(java.lang.CharSequence, java.lang.Object);
  public cn.hutool.core.net.url.UrlQuery addAll(java.util.Map<? extends java.lang.CharSequence, ?>);
  public cn.hutool.core.net.url.UrlQuery remove(java.lang.CharSequence);
  public cn.hutool.core.net.url.UrlQuery parse(java.lang.String, java.nio.charset.Charset);
  public cn.hutool.core.net.url.UrlQuery parse(java.lang.String, java.nio.charset.Charset, boolean);
  public java.util.Map<java.lang.CharSequence, java.lang.CharSequence> getQueryMap();
  public java.lang.CharSequence get(java.lang.CharSequence);
  public java.lang.String build(java.nio.charset.Charset);
  public java.lang.String build(java.nio.charset.Charset, boolean);
  public java.lang.String build(cn.hutool.core.codec.PercentCodec, cn.hutool.core.codec.PercentCodec, java.nio.charset.Charset);
  public java.lang.String build(cn.hutool.core.codec.PercentCodec, cn.hutool.core.codec.PercentCodec, java.nio.charset.Charset, boolean);
  public java.lang.String toString();
}
```
