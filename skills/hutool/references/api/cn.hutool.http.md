# cn.hutool.http

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.http.ContentType`

```java
public final class cn.hutool.http.ContentType extends java.lang.Enum<cn.hutool.http.ContentType> {
  public static cn.hutool.http.ContentType[] values();
  public static cn.hutool.http.ContentType valueOf(java.lang.String);
  public java.lang.String getValue();
  public java.lang.String toString();
  public java.lang.String toString(java.nio.charset.Charset);
  public static boolean isDefault(java.lang.String);
  public static boolean isFormUrlEncode(java.lang.String);
  public static cn.hutool.http.ContentType get(java.lang.String);
  public static java.lang.String build(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String build(cn.hutool.http.ContentType, java.nio.charset.Charset);
}
```

## `cn.hutool.http.GlobalHeaders`

```java
public final class cn.hutool.http.GlobalHeaders extends java.lang.Enum<cn.hutool.http.GlobalHeaders> {
  public static cn.hutool.http.GlobalHeaders[] values();
  public static cn.hutool.http.GlobalHeaders valueOf(java.lang.String);
  public cn.hutool.http.GlobalHeaders putDefault(boolean);
  public java.lang.String header(java.lang.String);
  public java.util.List<java.lang.String> headerList(java.lang.String);
  public java.lang.String header(cn.hutool.http.Header);
  public synchronized cn.hutool.http.GlobalHeaders header(java.lang.String, java.lang.String, boolean);
  public cn.hutool.http.GlobalHeaders header(cn.hutool.http.Header, java.lang.String, boolean);
  public cn.hutool.http.GlobalHeaders header(cn.hutool.http.Header, java.lang.String);
  public cn.hutool.http.GlobalHeaders header(java.lang.String, java.lang.String);
  public cn.hutool.http.GlobalHeaders header(java.util.Map<java.lang.String, java.util.List<java.lang.String>>);
  public synchronized cn.hutool.http.GlobalHeaders removeHeader(java.lang.String);
  public cn.hutool.http.GlobalHeaders removeHeader(cn.hutool.http.Header);
  public java.util.Map<java.lang.String, java.util.List<java.lang.String>> headers();
  public synchronized cn.hutool.http.GlobalHeaders clearHeaders();
}
```

## `cn.hutool.http.GlobalInterceptor`

```java
public final class cn.hutool.http.GlobalInterceptor extends java.lang.Enum<cn.hutool.http.GlobalInterceptor> {
  public static cn.hutool.http.GlobalInterceptor[] values();
  public static cn.hutool.http.GlobalInterceptor valueOf(java.lang.String);
  public synchronized cn.hutool.http.GlobalInterceptor addRequestInterceptor(cn.hutool.http.HttpInterceptor<cn.hutool.http.HttpRequest>);
  public synchronized cn.hutool.http.GlobalInterceptor addResponseInterceptor(cn.hutool.http.HttpInterceptor<cn.hutool.http.HttpResponse>);
  public cn.hutool.http.GlobalInterceptor clear();
  public synchronized cn.hutool.http.GlobalInterceptor clearRequest();
  public synchronized cn.hutool.http.GlobalInterceptor clearResponse();
}
```

## `cn.hutool.http.HTMLFilter`

```java
public final class cn.hutool.http.HTMLFilter {
  public cn.hutool.http.HTMLFilter();
  public cn.hutool.http.HTMLFilter(boolean);
  public cn.hutool.http.HTMLFilter(java.util.Map<java.lang.String, java.lang.Object>);
  public static java.lang.String chr(int);
  public static java.lang.String htmlSpecialChars(java.lang.String);
  public java.lang.String filter(java.lang.String);
  public boolean isAlwaysMakeTags();
  public boolean isStripComments();
}
```

## `cn.hutool.http.Header`

```java
public final class cn.hutool.http.Header extends java.lang.Enum<cn.hutool.http.Header> {
  public static cn.hutool.http.Header[] values();
  public static cn.hutool.http.Header valueOf(java.lang.String);
  public java.lang.String getValue();
  public java.lang.String toString();
}
```

## `cn.hutool.http.HtmlUtil`

```java
public class cn.hutool.http.HtmlUtil {
  public cn.hutool.http.HtmlUtil();
  public static java.lang.String escape(java.lang.String);
  public static java.lang.String unescape(java.lang.String);
  public static java.lang.String cleanHtmlTag(java.lang.String);
  public static java.lang.String cleanEmptyTag(java.lang.String);
  public static java.lang.String removeHtmlTag(java.lang.String, java.lang.String...);
  public static java.lang.String unwrapHtmlTag(java.lang.String, java.lang.String...);
  public static java.lang.String removeHtmlTag(java.lang.String, boolean, java.lang.String...);
  public static java.lang.String removeHtmlAttr(java.lang.String, java.lang.String...);
  public static java.lang.String removeAllHtmlAttr(java.lang.String, java.lang.String...);
  public static java.lang.String filter(java.lang.String);
}
```

## `cn.hutool.http.HttpBase`

```java
public abstract class cn.hutool.http.HttpBase<T> {
  public cn.hutool.http.HttpBase();
  public java.lang.String header(java.lang.String);
  public java.util.List<java.lang.String> headerList(java.lang.String);
  public java.lang.String header(cn.hutool.http.Header);
  public T header(java.lang.String, java.lang.String, boolean);
  public T header(cn.hutool.http.Header, java.lang.String, boolean);
  public T header(cn.hutool.http.Header, java.lang.String);
  public T header(java.lang.String, java.lang.String);
  public T headerMap(java.util.Map<java.lang.String, java.lang.String>, boolean);
  public T header(java.util.Map<java.lang.String, java.util.List<java.lang.String>>);
  public T header(java.util.Map<java.lang.String, java.util.List<java.lang.String>>, boolean);
  public T addHeaders(java.util.Map<java.lang.String, java.lang.String>);
  public T removeHeader(java.lang.String);
  public T removeHeader(cn.hutool.http.Header);
  public java.util.Map<java.lang.String, java.util.List<java.lang.String>> headers();
  public T clearHeaders();
  public T headerAggregation(boolean);
  public boolean isHeaderAggregated();
  public java.lang.String httpVersion();
  public T httpVersion(java.lang.String);
  public byte[] bodyBytes();
  public java.lang.String charset();
  public T charset(java.lang.String);
  public T charset(java.nio.charset.Charset);
  public java.lang.String toString();
}
```

## `cn.hutool.http.HttpConfig`

```java
public class cn.hutool.http.HttpConfig {
  public cn.hutool.http.HttpConfig();
  public static cn.hutool.http.HttpConfig create();
  public cn.hutool.http.HttpConfig timeout(int);
  public cn.hutool.http.HttpConfig setConnectionTimeout(int);
  public cn.hutool.http.HttpConfig setReadTimeout(int);
  public cn.hutool.http.HttpConfig disableCache();
  public cn.hutool.http.HttpConfig setMaxRedirectCount(int);
  public cn.hutool.http.HttpConfig setHostnameVerifier(javax.net.ssl.HostnameVerifier);
  public cn.hutool.http.HttpConfig setHttpProxy(java.lang.String, int);
  public cn.hutool.http.HttpConfig setProxy(java.net.Proxy);
  public cn.hutool.http.HttpConfig setSSLSocketFactory(javax.net.ssl.SSLSocketFactory);
  public cn.hutool.http.HttpConfig setSSLProtocol(java.lang.String);
  public cn.hutool.http.HttpConfig setBlockSize(int);
  public cn.hutool.http.HttpConfig setIgnoreEOFError(boolean);
  public cn.hutool.http.HttpConfig setDecodeUrl(boolean);
  public cn.hutool.http.HttpConfig addRequestInterceptor(cn.hutool.http.HttpInterceptor<cn.hutool.http.HttpRequest>);
  public cn.hutool.http.HttpConfig addResponseInterceptor(cn.hutool.http.HttpInterceptor<cn.hutool.http.HttpResponse>);
  public cn.hutool.http.HttpConfig setInterceptorOnRedirect(boolean);
  public cn.hutool.http.HttpConfig setFollowRedirectsCookie(boolean);
  public cn.hutool.http.HttpConfig setUseDefaultContentTypeIfNull(boolean);
  public cn.hutool.http.HttpConfig setIgnoreContentLength(boolean);
}
```

## `cn.hutool.http.HttpConnection`

```java
public class cn.hutool.http.HttpConnection {
  public static cn.hutool.http.HttpConnection create(java.lang.String, java.net.Proxy);
  public static cn.hutool.http.HttpConnection create(java.net.URL, java.net.Proxy);
  public cn.hutool.http.HttpConnection(java.net.URL, java.net.Proxy);
  public cn.hutool.http.HttpConnection initConn();
  public cn.hutool.http.Method getMethod();
  public cn.hutool.http.HttpConnection setMethod(cn.hutool.http.Method);
  public java.net.URL getUrl();
  public java.net.Proxy getProxy();
  public java.net.HttpURLConnection getHttpURLConnection();
  public cn.hutool.http.HttpConnection header(java.lang.String, java.lang.String, boolean);
  public cn.hutool.http.HttpConnection header(cn.hutool.http.Header, java.lang.String, boolean);
  public cn.hutool.http.HttpConnection header(java.util.Map<java.lang.String, java.util.List<java.lang.String>>, boolean);
  public cn.hutool.http.HttpConnection header(java.util.Map<java.lang.String, java.util.List<java.lang.String>>, boolean, boolean);
  public java.lang.String header(java.lang.String);
  public java.lang.String header(cn.hutool.http.Header);
  public java.util.Map<java.lang.String, java.util.List<java.lang.String>> headers();
  public cn.hutool.http.HttpConnection setHttpsInfo(javax.net.ssl.HostnameVerifier, javax.net.ssl.SSLSocketFactory) throws cn.hutool.http.HttpException;
  public cn.hutool.http.HttpConnection disableCache();
  public cn.hutool.http.HttpConnection setConnectTimeout(int);
  public cn.hutool.http.HttpConnection setReadTimeout(int);
  public cn.hutool.http.HttpConnection setConnectionAndReadTimeout(int);
  public cn.hutool.http.HttpConnection setCookie(java.lang.String);
  public cn.hutool.http.HttpConnection setFixedLengthStreamingMode(long);
  public cn.hutool.http.HttpConnection setChunkedStreamingMode(int);
  public cn.hutool.http.HttpConnection setInstanceFollowRedirects(boolean);
  public cn.hutool.http.HttpConnection connect() throws java.io.IOException;
  public cn.hutool.http.HttpConnection disconnectQuietly();
  public cn.hutool.http.HttpConnection disconnect();
  public java.io.InputStream getInputStream() throws java.io.IOException;
  public java.io.InputStream getErrorStream();
  public java.io.OutputStream getOutputStream() throws java.io.IOException;
  public int responseCode() throws java.io.IOException;
  public java.lang.String getCharsetName();
  public java.nio.charset.Charset getCharset();
  public java.lang.String toString();
}
```

## `cn.hutool.http.HttpDownloader`

```java
public class cn.hutool.http.HttpDownloader {
  public cn.hutool.http.HttpDownloader();
  public static java.lang.String downloadString(java.lang.String, java.nio.charset.Charset, cn.hutool.core.io.StreamProgress);
  public static byte[] downloadBytes(java.lang.String);
  public static byte[] downloadBytes(java.lang.String, int);
  public static long downloadFile(java.lang.String, java.io.File, int, cn.hutool.core.io.StreamProgress);
  public static long downloadFile(java.lang.String, java.io.File, java.lang.String, int, cn.hutool.core.io.StreamProgress);
  public static java.io.File downloadForFile(java.lang.String, java.io.File, int, cn.hutool.core.io.StreamProgress);
  public static long download(java.lang.String, java.io.OutputStream, boolean, cn.hutool.core.io.StreamProgress);
}
```

## `cn.hutool.http.HttpException`

```java
public class cn.hutool.http.HttpException extends java.lang.RuntimeException {
  public cn.hutool.http.HttpException(java.lang.Throwable);
  public cn.hutool.http.HttpException(java.lang.String);
  public cn.hutool.http.HttpException(java.lang.String, java.lang.Object...);
  public cn.hutool.http.HttpException(java.lang.String, java.lang.Throwable);
  public cn.hutool.http.HttpException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.http.HttpException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.http.HttpGlobalConfig`

```java
public class cn.hutool.http.HttpGlobalConfig implements java.io.Serializable {
  public cn.hutool.http.HttpGlobalConfig();
  public static int getTimeout();
  public static synchronized void setTimeout(int);
  public static java.lang.String getBoundary();
  public static synchronized void setBoundary(java.lang.String);
  public static int getMaxRedirectCount();
  public static synchronized void setMaxRedirectCount(int);
  public static boolean isIgnoreEOFError();
  public static synchronized void setIgnoreEOFError(boolean);
  public static boolean isDecodeUrl();
  public static synchronized void setDecodeUrl(boolean);
  public static java.net.CookieManager getCookieManager();
  public static synchronized void setCookieManager(java.net.CookieManager);
  public static synchronized void closeCookie();
  public static synchronized void allowPatch();
  public static boolean isTrustAnyHost();
  public static void setTrustAnyHost(boolean);
}
```

## `cn.hutool.http.HttpInputStream`

```java
public class cn.hutool.http.HttpInputStream extends java.io.InputStream {
  public cn.hutool.http.HttpInputStream(cn.hutool.http.HttpResponse);
  public int read() throws java.io.IOException;
  public int read(byte[], int, int) throws java.io.IOException;
  public long skip(long) throws java.io.IOException;
  public int available() throws java.io.IOException;
  public void close() throws java.io.IOException;
  public synchronized void mark(int);
  public synchronized void reset() throws java.io.IOException;
  public boolean markSupported();
}
```

## `cn.hutool.http.HttpInterceptor`

```java
public interface cn.hutool.http.HttpInterceptor<T extends cn.hutool.http.HttpBase<T>> {
  public abstract void process(T);
}
```

## `cn.hutool.http.HttpInterceptor$Chain`

```java
public class cn.hutool.http.HttpInterceptor$Chain<T extends cn.hutool.http.HttpBase<T>> implements cn.hutool.core.lang.Chain<cn.hutool.http.HttpInterceptor<T>, cn.hutool.http.HttpInterceptor$Chain<T>> {
  public cn.hutool.http.HttpInterceptor$Chain();
  public cn.hutool.http.HttpInterceptor$Chain<T> addChain(cn.hutool.http.HttpInterceptor<T>);
  public java.util.Iterator<cn.hutool.http.HttpInterceptor<T>> iterator();
  public cn.hutool.http.HttpInterceptor$Chain<T> clear();
  public java.lang.Object addChain(java.lang.Object);
}
```

## `cn.hutool.http.HttpRequest`

```java
public class cn.hutool.http.HttpRequest extends cn.hutool.http.HttpBase<cn.hutool.http.HttpRequest> {
  public static cn.hutool.http.HttpRequest post(java.lang.String);
  public static cn.hutool.http.HttpRequest get(java.lang.String);
  public static cn.hutool.http.HttpRequest head(java.lang.String);
  public static cn.hutool.http.HttpRequest options(java.lang.String);
  public static cn.hutool.http.HttpRequest put(java.lang.String);
  public static cn.hutool.http.HttpRequest patch(java.lang.String);
  public static cn.hutool.http.HttpRequest delete(java.lang.String);
  public static cn.hutool.http.HttpRequest trace(java.lang.String);
  public static cn.hutool.http.HttpRequest of(java.lang.String);
  public static cn.hutool.http.HttpRequest of(java.lang.String, java.nio.charset.Charset);
  public static cn.hutool.http.HttpRequest of(cn.hutool.core.net.url.UrlBuilder);
  public static void setGlobalTimeout(int);
  public static java.net.CookieManager getCookieManager();
  public static void setCookieManager(java.net.CookieManager);
  public static void closeCookie();
  public cn.hutool.http.HttpRequest(java.lang.String);
  public cn.hutool.http.HttpRequest(cn.hutool.core.net.url.UrlBuilder);
  public java.lang.String getUrl();
  public cn.hutool.http.HttpRequest setUrl(java.lang.String);
  public cn.hutool.http.HttpRequest setUrl(cn.hutool.core.net.url.UrlBuilder);
  public cn.hutool.http.HttpRequest setUrlHandler(java.net.URLStreamHandler);
  public cn.hutool.http.Method getMethod();
  public cn.hutool.http.HttpRequest setMethod(cn.hutool.http.Method);
  public cn.hutool.http.HttpConnection getConnection();
  public cn.hutool.http.HttpRequest setFixedContentLength(long);
  public cn.hutool.http.HttpRequest method(cn.hutool.http.Method);
  public cn.hutool.http.HttpRequest contentType(java.lang.String);
  public cn.hutool.http.HttpRequest keepAlive(boolean);
  public boolean isKeepAlive();
  public java.lang.String contentLength();
  public cn.hutool.http.HttpRequest contentLength(int);
  public cn.hutool.http.HttpRequest cookie(java.util.Collection<java.net.HttpCookie>);
  public cn.hutool.http.HttpRequest cookie(java.net.HttpCookie...);
  public cn.hutool.http.HttpRequest cookie(java.lang.String);
  public cn.hutool.http.HttpRequest disableCookie();
  public cn.hutool.http.HttpRequest enableDefaultCookie();
  public cn.hutool.http.HttpRequest form(java.lang.String, java.lang.Object);
  public cn.hutool.http.HttpRequest form(java.lang.String, java.lang.Object, java.lang.Object...);
  public cn.hutool.http.HttpRequest form(java.util.Map<java.lang.String, java.lang.Object>);
  public cn.hutool.http.HttpRequest formStr(java.util.Map<java.lang.String, java.lang.String>);
  public cn.hutool.http.HttpRequest form(java.lang.String, java.io.File...);
  public cn.hutool.http.HttpRequest form(java.lang.String, java.io.File);
  public cn.hutool.http.HttpRequest form(java.lang.String, java.io.File, java.lang.String);
  public cn.hutool.http.HttpRequest form(java.lang.String, byte[], java.lang.String);
  public cn.hutool.http.HttpRequest form(java.lang.String, cn.hutool.core.io.resource.Resource);
  public java.util.Map<java.lang.String, java.lang.Object> form();
  public java.util.Map<java.lang.String, cn.hutool.core.io.resource.Resource> fileForm();
  public cn.hutool.http.HttpRequest body(java.lang.String);
  public cn.hutool.http.HttpRequest body(java.lang.String, java.lang.String);
  public cn.hutool.http.HttpRequest body(byte[]);
  public cn.hutool.http.HttpRequest body(cn.hutool.core.io.resource.Resource);
  public cn.hutool.http.HttpRequest setConfig(cn.hutool.http.HttpConfig);
  public cn.hutool.http.HttpRequest timeout(int);
  public cn.hutool.http.HttpRequest setConnectionTimeout(int);
  public cn.hutool.http.HttpRequest setReadTimeout(int);
  public cn.hutool.http.HttpRequest disableCache();
  public cn.hutool.http.HttpRequest setFollowRedirects(boolean);
  public cn.hutool.http.HttpRequest setFollowRedirectsCookie(boolean);
  public cn.hutool.http.HttpRequest setMaxRedirectCount(int);
  public cn.hutool.http.HttpRequest setHostnameVerifier(javax.net.ssl.HostnameVerifier);
  public cn.hutool.http.HttpRequest setHttpProxy(java.lang.String, int);
  public cn.hutool.http.HttpRequest setProxy(java.net.Proxy);
  public cn.hutool.http.HttpRequest setSSLSocketFactory(javax.net.ssl.SSLSocketFactory);
  public cn.hutool.http.HttpRequest setSSLProtocol(java.lang.String);
  public cn.hutool.http.HttpRequest setRest(boolean);
  public cn.hutool.http.HttpRequest setChunkedStreamingMode(int);
  public cn.hutool.http.HttpRequest addInterceptor(cn.hutool.http.HttpInterceptor<cn.hutool.http.HttpRequest>);
  public cn.hutool.http.HttpRequest addRequestInterceptor(cn.hutool.http.HttpInterceptor<cn.hutool.http.HttpRequest>);
  public cn.hutool.http.HttpRequest addResponseInterceptor(cn.hutool.http.HttpInterceptor<cn.hutool.http.HttpResponse>);
  public cn.hutool.http.HttpResponse execute();
  public cn.hutool.http.HttpResponse executeAsync();
  public cn.hutool.http.HttpResponse execute(boolean);
  public void then(java.util.function.Consumer<cn.hutool.http.HttpResponse>);
  public <T> T thenFunction(java.util.function.Function<cn.hutool.http.HttpResponse, T>);
  public cn.hutool.http.HttpRequest basicAuth(java.lang.String, java.lang.String);
  public cn.hutool.http.HttpRequest basicProxyAuth(java.lang.String, java.lang.String);
  public cn.hutool.http.HttpRequest bearerAuth(java.lang.String);
  public cn.hutool.http.HttpRequest auth(java.lang.String);
  public cn.hutool.http.HttpRequest proxyAuth(java.lang.String);
  public java.lang.String toString();
}
```

## `cn.hutool.http.HttpResource`

```java
public class cn.hutool.http.HttpResource implements cn.hutool.core.io.resource.Resource,java.io.Serializable {
  public cn.hutool.http.HttpResource(cn.hutool.core.io.resource.Resource, java.lang.String);
  public java.lang.String getName();
  public java.net.URL getUrl();
  public java.io.InputStream getStream();
  public java.lang.String getContentType();
}
```

## `cn.hutool.http.HttpResponse`

```java
public class cn.hutool.http.HttpResponse extends cn.hutool.http.HttpBase<cn.hutool.http.HttpResponse> implements java.io.Closeable {
  public int getStatus();
  public boolean isOk();
  public cn.hutool.http.HttpResponse sync();
  public java.lang.String contentEncoding();
  public long contentLength();
  public boolean isGzip();
  public boolean isDeflate();
  public boolean isChunked();
  public java.lang.String getCookieStr();
  public java.util.List<java.net.HttpCookie> getCookies();
  public java.net.HttpCookie getCookie(java.lang.String);
  public java.lang.String getCookieValue(java.lang.String);
  public java.io.InputStream bodyStream();
  public byte[] bodyBytes();
  public cn.hutool.http.HttpResponse body(byte[]);
  public java.lang.String body() throws cn.hutool.http.HttpException;
  public long writeBody(java.io.OutputStream, boolean, cn.hutool.core.io.StreamProgress);
  public long writeBody(java.io.File, cn.hutool.core.io.StreamProgress);
  public long writeBody(java.io.File, java.lang.String, cn.hutool.core.io.StreamProgress);
  public java.io.File writeBodyForFile(java.io.File, cn.hutool.core.io.StreamProgress);
  public long writeBody(java.io.File);
  public long writeBody(java.lang.String);
  public void close();
  public java.lang.String toString();
  public java.io.File completeFileNameFromHeader(java.io.File);
  public java.lang.String getFileNameFromDisposition();
  public java.lang.String getFileNameFromDisposition(java.lang.String);
}
```

## `cn.hutool.http.HttpStatus`

```java
public class cn.hutool.http.HttpStatus {
  public cn.hutool.http.HttpStatus();
  public static boolean isRedirected(int);
}
```

## `cn.hutool.http.HttpUtil`

```java
public class cn.hutool.http.HttpUtil {
  public cn.hutool.http.HttpUtil();
  public static boolean isHttps(java.lang.String);
  public static boolean isHttp(java.lang.String);
  public static cn.hutool.http.HttpRequest createRequest(cn.hutool.http.Method, java.lang.String);
  public static cn.hutool.http.HttpRequest createGet(java.lang.String);
  public static cn.hutool.http.HttpRequest createGet(java.lang.String, boolean);
  public static cn.hutool.http.HttpRequest createPost(java.lang.String);
  public static java.lang.String get(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String get(java.lang.String);
  public static java.lang.String get(java.lang.String, int);
  public static java.lang.String get(java.lang.String, java.util.Map<java.lang.String, java.lang.Object>);
  public static java.lang.String get(java.lang.String, java.util.Map<java.lang.String, java.lang.Object>, int);
  public static java.lang.String post(java.lang.String, java.util.Map<java.lang.String, java.lang.Object>);
  public static java.lang.String post(java.lang.String, java.util.Map<java.lang.String, java.lang.Object>, int);
  public static java.lang.String post(java.lang.String, java.lang.String);
  public static java.lang.String post(java.lang.String, java.lang.String, int);
  public static java.lang.String downloadString(java.lang.String, java.lang.String);
  public static java.lang.String downloadString(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String downloadString(java.lang.String, java.nio.charset.Charset, cn.hutool.core.io.StreamProgress);
  public static long downloadFile(java.lang.String, java.lang.String);
  public static long downloadFile(java.lang.String, java.io.File);
  public static long downloadFile(java.lang.String, java.io.File, int);
  public static long downloadFile(java.lang.String, java.io.File, cn.hutool.core.io.StreamProgress);
  public static long downloadFile(java.lang.String, java.io.File, int, cn.hutool.core.io.StreamProgress);
  public static java.io.File downloadFileFromUrl(java.lang.String, java.lang.String);
  public static java.io.File downloadFileFromUrl(java.lang.String, java.io.File);
  public static java.io.File downloadFileFromUrl(java.lang.String, java.io.File, int);
  public static java.io.File downloadFileFromUrl(java.lang.String, java.io.File, cn.hutool.core.io.StreamProgress);
  public static java.io.File downloadFileFromUrl(java.lang.String, java.io.File, int, cn.hutool.core.io.StreamProgress);
  public static long download(java.lang.String, java.io.OutputStream, boolean);
  public static long download(java.lang.String, java.io.OutputStream, boolean, cn.hutool.core.io.StreamProgress);
  public static byte[] downloadBytes(java.lang.String);
  public static java.lang.String toParams(java.util.Map<java.lang.String, ?>);
  public static java.lang.String toParams(java.util.Map<java.lang.String, java.lang.Object>, java.lang.String);
  public static java.lang.String toParams(java.util.Map<java.lang.String, ?>, java.nio.charset.Charset);
  public static java.lang.String toParams(java.util.Map<java.lang.String, ?>, java.nio.charset.Charset, boolean);
  public static java.lang.String encodeParams(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String normalizeParams(java.lang.String, java.nio.charset.Charset);
  public static java.util.Map<java.lang.String, java.lang.String> decodeParamMap(java.lang.String, java.nio.charset.Charset);
  public static java.util.Map<java.lang.String, java.util.List<java.lang.String>> decodeParams(java.lang.String, java.lang.String);
  public static java.util.Map<java.lang.String, java.util.List<java.lang.String>> decodeParams(java.lang.String, java.lang.String, boolean);
  public static java.util.Map<java.lang.String, java.util.List<java.lang.String>> decodeParams(java.lang.String, java.nio.charset.Charset);
  public static java.util.Map<java.lang.String, java.util.List<java.lang.String>> decodeParams(java.lang.String, java.nio.charset.Charset, boolean);
  public static java.lang.String urlWithForm(java.lang.String, java.util.Map<java.lang.String, java.lang.Object>, java.nio.charset.Charset, boolean);
  public static java.lang.String urlWithFormUrlEncoded(java.lang.String, java.util.Map<java.lang.String, java.lang.Object>, java.nio.charset.Charset);
  public static java.lang.String urlWithForm(java.lang.String, java.lang.String, java.nio.charset.Charset, boolean);
  public static java.lang.String getCharset(java.net.HttpURLConnection);
  public static java.lang.String getCharset(java.lang.String);
  public static java.lang.String getString(java.io.InputStream, java.nio.charset.Charset, boolean);
  public static java.lang.String getString(byte[], java.nio.charset.Charset, boolean);
  public static java.lang.String getMimeType(java.lang.String, java.lang.String);
  public static java.lang.String getMimeType(java.lang.String);
  public static java.lang.String getContentTypeByRequestBody(java.lang.String);
  public static cn.hutool.http.server.SimpleServer createServer(int);
  public static java.lang.String buildBasicAuth(java.lang.String, java.lang.String, java.nio.charset.Charset);
  public static void closeCookie();
}
```

## `cn.hutool.http.Method`

```java
public final class cn.hutool.http.Method extends java.lang.Enum<cn.hutool.http.Method> {
  public static cn.hutool.http.Method[] values();
  public static cn.hutool.http.Method valueOf(java.lang.String);
}
```

## `cn.hutool.http.MultipartOutputStream`

```java
public class cn.hutool.http.MultipartOutputStream extends java.io.OutputStream {
  public cn.hutool.http.MultipartOutputStream(java.io.OutputStream, java.nio.charset.Charset);
  public cn.hutool.http.MultipartOutputStream(java.io.OutputStream, java.nio.charset.Charset, java.lang.String);
  public cn.hutool.http.MultipartOutputStream write(java.lang.String, java.lang.Object) throws cn.hutool.core.io.IORuntimeException;
  public void write(int) throws java.io.IOException;
  public void finish() throws cn.hutool.core.io.IORuntimeException;
  public void close();
}
```
