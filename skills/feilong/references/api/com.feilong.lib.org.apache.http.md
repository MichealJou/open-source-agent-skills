# com.feilong.lib.org.apache.http

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.ConnectionClosedException`

```java
public class com.feilong.lib.org.apache.http.ConnectionClosedException extends java.io.IOException {
  public com.feilong.lib.org.apache.http.ConnectionClosedException();
  public com.feilong.lib.org.apache.http.ConnectionClosedException(java.lang.String);
  public com.feilong.lib.org.apache.http.ConnectionClosedException(java.lang.String, java.lang.Object...);
}
```

## `com.feilong.lib.org.apache.http.ConnectionReuseStrategy`

```java
public interface com.feilong.lib.org.apache.http.ConnectionReuseStrategy {
  public abstract boolean keepAlive(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.ContentTooLongException`

```java
public class com.feilong.lib.org.apache.http.ContentTooLongException extends java.io.IOException {
  public com.feilong.lib.org.apache.http.ContentTooLongException(java.lang.String);
  public com.feilong.lib.org.apache.http.ContentTooLongException(java.lang.String, java.lang.Object...);
}
```

## `com.feilong.lib.org.apache.http.ExceptionLogger`

```java
public interface com.feilong.lib.org.apache.http.ExceptionLogger {
  public abstract void log(java.lang.Exception);
}
```

## `com.feilong.lib.org.apache.http.FormattedHeader`

```java
public interface com.feilong.lib.org.apache.http.FormattedHeader extends com.feilong.lib.org.apache.http.Header {
  public abstract com.feilong.lib.org.apache.http.util.CharArrayBuffer getBuffer();
  public abstract int getValuePos();
}
```

## `com.feilong.lib.org.apache.http.Header`

```java
public interface com.feilong.lib.org.apache.http.Header extends com.feilong.lib.org.apache.http.NameValuePair {
  public abstract com.feilong.lib.org.apache.http.HeaderElement[] getElements() throws com.feilong.lib.org.apache.http.ParseException;
}
```

## `com.feilong.lib.org.apache.http.HeaderElement`

```java
public interface com.feilong.lib.org.apache.http.HeaderElement {
  public abstract java.lang.String getName();
  public abstract java.lang.String getValue();
  public abstract com.feilong.lib.org.apache.http.NameValuePair[] getParameters();
  public abstract com.feilong.lib.org.apache.http.NameValuePair getParameterByName(java.lang.String);
  public abstract int getParameterCount();
  public abstract com.feilong.lib.org.apache.http.NameValuePair getParameter(int);
}
```

## `com.feilong.lib.org.apache.http.HeaderElementIterator`

```java
public interface com.feilong.lib.org.apache.http.HeaderElementIterator extends java.util.Iterator<java.lang.Object> {
  public abstract boolean hasNext();
  public abstract com.feilong.lib.org.apache.http.HeaderElement nextElement();
}
```

## `com.feilong.lib.org.apache.http.HeaderIterator`

```java
public interface com.feilong.lib.org.apache.http.HeaderIterator extends java.util.Iterator<java.lang.Object> {
  public abstract boolean hasNext();
  public abstract com.feilong.lib.org.apache.http.Header nextHeader();
}
```

## `com.feilong.lib.org.apache.http.HttpClientConnection`

```java
public interface com.feilong.lib.org.apache.http.HttpClientConnection extends com.feilong.lib.org.apache.http.HttpConnection {
  public abstract boolean isResponseAvailable(int) throws java.io.IOException;
  public abstract void sendRequestHeader(com.feilong.lib.org.apache.http.HttpRequest) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public abstract void sendRequestEntity(com.feilong.lib.org.apache.http.HttpEntityEnclosingRequest) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public abstract com.feilong.lib.org.apache.http.HttpResponse receiveResponseHeader() throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public abstract void receiveResponseEntity(com.feilong.lib.org.apache.http.HttpResponse) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public abstract void flush() throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.HttpConnection`

```java
public interface com.feilong.lib.org.apache.http.HttpConnection extends java.io.Closeable {
  public abstract void close() throws java.io.IOException;
  public abstract boolean isOpen();
  public abstract boolean isStale();
  public abstract void setSocketTimeout(int);
  public abstract int getSocketTimeout();
  public abstract void shutdown() throws java.io.IOException;
  public abstract com.feilong.lib.org.apache.http.HttpConnectionMetrics getMetrics();
}
```

## `com.feilong.lib.org.apache.http.HttpConnectionFactory`

```java
public interface com.feilong.lib.org.apache.http.HttpConnectionFactory<T extends com.feilong.lib.org.apache.http.HttpConnection> {
  public abstract T createConnection(java.net.Socket) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.HttpConnectionMetrics`

```java
public interface com.feilong.lib.org.apache.http.HttpConnectionMetrics {
  public abstract long getRequestCount();
  public abstract long getResponseCount();
  public abstract long getSentBytesCount();
  public abstract long getReceivedBytesCount();
  public abstract java.lang.Object getMetric(java.lang.String);
  public abstract void reset();
}
```

## `com.feilong.lib.org.apache.http.HttpEntity`

```java
public interface com.feilong.lib.org.apache.http.HttpEntity {
  public abstract boolean isRepeatable();
  public abstract boolean isChunked();
  public abstract long getContentLength();
  public abstract com.feilong.lib.org.apache.http.Header getContentType();
  public abstract com.feilong.lib.org.apache.http.Header getContentEncoding();
  public abstract java.io.InputStream getContent() throws java.io.IOException, java.lang.UnsupportedOperationException;
  public abstract void writeTo(java.io.OutputStream) throws java.io.IOException;
  public abstract boolean isStreaming();
}
```

## `com.feilong.lib.org.apache.http.HttpEntityEnclosingRequest`

```java
public interface com.feilong.lib.org.apache.http.HttpEntityEnclosingRequest extends com.feilong.lib.org.apache.http.HttpRequest {
  public abstract boolean expectContinue();
  public abstract void setEntity(com.feilong.lib.org.apache.http.HttpEntity);
  public abstract com.feilong.lib.org.apache.http.HttpEntity getEntity();
}
```

## `com.feilong.lib.org.apache.http.HttpException`

```java
public class com.feilong.lib.org.apache.http.HttpException extends java.lang.Exception {
  public com.feilong.lib.org.apache.http.HttpException();
  public com.feilong.lib.org.apache.http.HttpException(java.lang.String);
  public com.feilong.lib.org.apache.http.HttpException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.HttpHost`

```java
public final class com.feilong.lib.org.apache.http.HttpHost implements java.lang.Cloneable,java.io.Serializable {
  public com.feilong.lib.org.apache.http.HttpHost(java.lang.String, int, java.lang.String);
  public com.feilong.lib.org.apache.http.HttpHost(java.lang.String, int);
  public static com.feilong.lib.org.apache.http.HttpHost create(java.lang.String);
  public com.feilong.lib.org.apache.http.HttpHost(java.lang.String);
  public com.feilong.lib.org.apache.http.HttpHost(java.net.InetAddress, int, java.lang.String);
  public com.feilong.lib.org.apache.http.HttpHost(java.net.InetAddress, java.lang.String, int, java.lang.String);
  public com.feilong.lib.org.apache.http.HttpHost(java.net.InetAddress, int);
  public com.feilong.lib.org.apache.http.HttpHost(java.net.InetAddress);
  public com.feilong.lib.org.apache.http.HttpHost(com.feilong.lib.org.apache.http.HttpHost);
  public java.lang.String getHostName();
  public int getPort();
  public java.lang.String getSchemeName();
  public java.net.InetAddress getAddress();
  public java.lang.String toURI();
  public java.lang.String toHostString();
  public java.lang.String toString();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.HttpInetConnection`

```java
public interface com.feilong.lib.org.apache.http.HttpInetConnection extends com.feilong.lib.org.apache.http.HttpConnection {
  public abstract java.net.InetAddress getLocalAddress();
  public abstract int getLocalPort();
  public abstract java.net.InetAddress getRemoteAddress();
  public abstract int getRemotePort();
}
```

## `com.feilong.lib.org.apache.http.HttpMessage`

```java
public interface com.feilong.lib.org.apache.http.HttpMessage {
  public abstract com.feilong.lib.org.apache.http.ProtocolVersion getProtocolVersion();
  public abstract boolean containsHeader(java.lang.String);
  public abstract com.feilong.lib.org.apache.http.Header[] getHeaders(java.lang.String);
  public abstract com.feilong.lib.org.apache.http.Header getFirstHeader(java.lang.String);
  public abstract com.feilong.lib.org.apache.http.Header getLastHeader(java.lang.String);
  public abstract com.feilong.lib.org.apache.http.Header[] getAllHeaders();
  public abstract void addHeader(com.feilong.lib.org.apache.http.Header);
  public abstract void addHeader(java.lang.String, java.lang.String);
  public abstract void setHeader(com.feilong.lib.org.apache.http.Header);
  public abstract void setHeader(java.lang.String, java.lang.String);
  public abstract void setHeaders(com.feilong.lib.org.apache.http.Header[]);
  public abstract void removeHeader(com.feilong.lib.org.apache.http.Header);
  public abstract void removeHeaders(java.lang.String);
  public abstract com.feilong.lib.org.apache.http.HeaderIterator headerIterator();
  public abstract com.feilong.lib.org.apache.http.HeaderIterator headerIterator(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.HttpRequest`

```java
public interface com.feilong.lib.org.apache.http.HttpRequest extends com.feilong.lib.org.apache.http.HttpMessage {
  public abstract com.feilong.lib.org.apache.http.RequestLine getRequestLine();
}
```

## `com.feilong.lib.org.apache.http.HttpRequestFactory`

```java
public interface com.feilong.lib.org.apache.http.HttpRequestFactory {
  public abstract com.feilong.lib.org.apache.http.HttpRequest newHttpRequest(com.feilong.lib.org.apache.http.RequestLine) throws com.feilong.lib.org.apache.http.MethodNotSupportedException;
  public abstract com.feilong.lib.org.apache.http.HttpRequest newHttpRequest(java.lang.String, java.lang.String) throws com.feilong.lib.org.apache.http.MethodNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.HttpRequestInterceptor`

```java
public interface com.feilong.lib.org.apache.http.HttpRequestInterceptor {
  public abstract void process(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.HttpResponse`

```java
public interface com.feilong.lib.org.apache.http.HttpResponse extends com.feilong.lib.org.apache.http.HttpMessage {
  public abstract com.feilong.lib.org.apache.http.StatusLine getStatusLine();
  public abstract void setStatusLine(com.feilong.lib.org.apache.http.StatusLine);
  public abstract void setStatusLine(com.feilong.lib.org.apache.http.ProtocolVersion, int);
  public abstract void setStatusLine(com.feilong.lib.org.apache.http.ProtocolVersion, int, java.lang.String);
  public abstract void setStatusCode(int) throws java.lang.IllegalStateException;
  public abstract void setReasonPhrase(java.lang.String) throws java.lang.IllegalStateException;
  public abstract com.feilong.lib.org.apache.http.HttpEntity getEntity();
  public abstract void setEntity(com.feilong.lib.org.apache.http.HttpEntity);
  public abstract java.util.Locale getLocale();
  public abstract void setLocale(java.util.Locale);
}
```

## `com.feilong.lib.org.apache.http.HttpResponseFactory`

```java
public interface com.feilong.lib.org.apache.http.HttpResponseFactory {
  public abstract com.feilong.lib.org.apache.http.HttpResponse newHttpResponse(com.feilong.lib.org.apache.http.ProtocolVersion, int, com.feilong.lib.org.apache.http.protocol.HttpContext);
  public abstract com.feilong.lib.org.apache.http.HttpResponse newHttpResponse(com.feilong.lib.org.apache.http.StatusLine, com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.HttpResponseInterceptor`

```java
public interface com.feilong.lib.org.apache.http.HttpResponseInterceptor {
  public abstract void process(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.HttpServerConnection`

```java
public interface com.feilong.lib.org.apache.http.HttpServerConnection extends com.feilong.lib.org.apache.http.HttpConnection {
  public abstract com.feilong.lib.org.apache.http.HttpRequest receiveRequestHeader() throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public abstract void receiveRequestEntity(com.feilong.lib.org.apache.http.HttpEntityEnclosingRequest) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public abstract void sendResponseHeader(com.feilong.lib.org.apache.http.HttpResponse) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public abstract void sendResponseEntity(com.feilong.lib.org.apache.http.HttpResponse) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public abstract void flush() throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.HttpVersion`

```java
public final class com.feilong.lib.org.apache.http.HttpVersion extends com.feilong.lib.org.apache.http.ProtocolVersion {
  public com.feilong.lib.org.apache.http.HttpVersion(int, int);
  public com.feilong.lib.org.apache.http.ProtocolVersion forVersion(int, int);
}
```

## `com.feilong.lib.org.apache.http.MalformedChunkCodingException`

```java
public class com.feilong.lib.org.apache.http.MalformedChunkCodingException extends java.io.IOException {
  public com.feilong.lib.org.apache.http.MalformedChunkCodingException();
  public com.feilong.lib.org.apache.http.MalformedChunkCodingException(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.MessageConstraintException`

```java
public class com.feilong.lib.org.apache.http.MessageConstraintException extends java.nio.charset.CharacterCodingException {
  public com.feilong.lib.org.apache.http.MessageConstraintException(java.lang.String);
  public java.lang.String getMessage();
}
```

## `com.feilong.lib.org.apache.http.MethodNotSupportedException`

```java
public class com.feilong.lib.org.apache.http.MethodNotSupportedException extends com.feilong.lib.org.apache.http.HttpException {
  public com.feilong.lib.org.apache.http.MethodNotSupportedException(java.lang.String);
  public com.feilong.lib.org.apache.http.MethodNotSupportedException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.NameValuePair`

```java
public interface com.feilong.lib.org.apache.http.NameValuePair {
  public abstract java.lang.String getName();
  public abstract java.lang.String getValue();
}
```

## `com.feilong.lib.org.apache.http.NoHttpResponseException`

```java
public class com.feilong.lib.org.apache.http.NoHttpResponseException extends java.io.IOException {
  public com.feilong.lib.org.apache.http.NoHttpResponseException(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.ParseException`

```java
public class com.feilong.lib.org.apache.http.ParseException extends java.lang.RuntimeException {
  public com.feilong.lib.org.apache.http.ParseException();
  public com.feilong.lib.org.apache.http.ParseException(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.ProtocolException`

```java
public class com.feilong.lib.org.apache.http.ProtocolException extends com.feilong.lib.org.apache.http.HttpException {
  public com.feilong.lib.org.apache.http.ProtocolException();
  public com.feilong.lib.org.apache.http.ProtocolException(java.lang.String);
  public com.feilong.lib.org.apache.http.ProtocolException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.ProtocolVersion`

```java
public class com.feilong.lib.org.apache.http.ProtocolVersion implements java.io.Serializable,java.lang.Cloneable {
  public com.feilong.lib.org.apache.http.ProtocolVersion(java.lang.String, int, int);
  public final java.lang.String getProtocol();
  public final int getMajor();
  public final int getMinor();
  public com.feilong.lib.org.apache.http.ProtocolVersion forVersion(int, int);
  public final int hashCode();
  public final boolean equals(java.lang.Object);
  public boolean isComparable(com.feilong.lib.org.apache.http.ProtocolVersion);
  public int compareToVersion(com.feilong.lib.org.apache.http.ProtocolVersion);
  public final boolean greaterEquals(com.feilong.lib.org.apache.http.ProtocolVersion);
  public final boolean lessEquals(com.feilong.lib.org.apache.http.ProtocolVersion);
  public java.lang.String toString();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.ReasonPhraseCatalog`

```java
public interface com.feilong.lib.org.apache.http.ReasonPhraseCatalog {
  public abstract java.lang.String getReason(int, java.util.Locale);
}
```

## `com.feilong.lib.org.apache.http.RequestLine`

```java
public interface com.feilong.lib.org.apache.http.RequestLine {
  public abstract java.lang.String getMethod();
  public abstract com.feilong.lib.org.apache.http.ProtocolVersion getProtocolVersion();
  public abstract java.lang.String getUri();
}
```

## `com.feilong.lib.org.apache.http.StatusLine`

```java
public interface com.feilong.lib.org.apache.http.StatusLine {
  public abstract com.feilong.lib.org.apache.http.ProtocolVersion getProtocolVersion();
  public abstract int getStatusCode();
  public abstract java.lang.String getReasonPhrase();
}
```

## `com.feilong.lib.org.apache.http.TokenIterator`

```java
public interface com.feilong.lib.org.apache.http.TokenIterator extends java.util.Iterator<java.lang.Object> {
  public abstract boolean hasNext();
  public abstract java.lang.String nextToken();
}
```

## `com.feilong.lib.org.apache.http.TruncatedChunkException`

```java
public class com.feilong.lib.org.apache.http.TruncatedChunkException extends com.feilong.lib.org.apache.http.MalformedChunkCodingException {
  public com.feilong.lib.org.apache.http.TruncatedChunkException(java.lang.String);
  public com.feilong.lib.org.apache.http.TruncatedChunkException(java.lang.String, java.lang.Object...);
}
```

## `com.feilong.lib.org.apache.http.UnsupportedHttpVersionException`

```java
public class com.feilong.lib.org.apache.http.UnsupportedHttpVersionException extends com.feilong.lib.org.apache.http.ProtocolException {
  public com.feilong.lib.org.apache.http.UnsupportedHttpVersionException();
  public com.feilong.lib.org.apache.http.UnsupportedHttpVersionException(java.lang.String);
}
```
