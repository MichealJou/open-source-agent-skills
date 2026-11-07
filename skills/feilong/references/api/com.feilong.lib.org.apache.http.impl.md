# com.feilong.lib.org.apache.http.impl

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.impl.BHttpConnectionBase`

```java
public class com.feilong.lib.org.apache.http.impl.BHttpConnectionBase implements com.feilong.lib.org.apache.http.HttpInetConnection {
  public boolean isOpen();
  public java.net.InetAddress getLocalAddress();
  public int getLocalPort();
  public java.net.InetAddress getRemoteAddress();
  public int getRemotePort();
  public void setSocketTimeout(int);
  public int getSocketTimeout();
  public void shutdown() throws java.io.IOException;
  public void close() throws java.io.IOException;
  public boolean isStale();
  public com.feilong.lib.org.apache.http.HttpConnectionMetrics getMetrics();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.ConnSupport`

```java
public final class com.feilong.lib.org.apache.http.impl.ConnSupport {
  public com.feilong.lib.org.apache.http.impl.ConnSupport();
  public static java.nio.charset.CharsetDecoder createDecoder(com.feilong.lib.org.apache.http.config.ConnectionConfig);
  public static java.nio.charset.CharsetEncoder createEncoder(com.feilong.lib.org.apache.http.config.ConnectionConfig);
}
```

## `com.feilong.lib.org.apache.http.impl.DefaultBHttpClientConnection`

```java
public class com.feilong.lib.org.apache.http.impl.DefaultBHttpClientConnection extends com.feilong.lib.org.apache.http.impl.BHttpConnectionBase implements com.feilong.lib.org.apache.http.HttpClientConnection {
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpClientConnection(int, int, java.nio.charset.CharsetDecoder, java.nio.charset.CharsetEncoder, com.feilong.lib.org.apache.http.config.MessageConstraints, com.feilong.lib.org.apache.http.entity.ContentLengthStrategy, com.feilong.lib.org.apache.http.entity.ContentLengthStrategy, com.feilong.lib.org.apache.http.io.HttpMessageWriterFactory<com.feilong.lib.org.apache.http.HttpRequest>, com.feilong.lib.org.apache.http.io.HttpMessageParserFactory<com.feilong.lib.org.apache.http.HttpResponse>);
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpClientConnection(int, java.nio.charset.CharsetDecoder, java.nio.charset.CharsetEncoder, com.feilong.lib.org.apache.http.config.MessageConstraints);
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpClientConnection(int);
  public void bind(java.net.Socket) throws java.io.IOException;
  public boolean isResponseAvailable(int) throws java.io.IOException;
  public void sendRequestHeader(com.feilong.lib.org.apache.http.HttpRequest) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public void sendRequestEntity(com.feilong.lib.org.apache.http.HttpEntityEnclosingRequest) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public com.feilong.lib.org.apache.http.HttpResponse receiveResponseHeader() throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public void receiveResponseEntity(com.feilong.lib.org.apache.http.HttpResponse) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public void flush() throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.DefaultBHttpClientConnectionFactory`

```java
public class com.feilong.lib.org.apache.http.impl.DefaultBHttpClientConnectionFactory implements com.feilong.lib.org.apache.http.HttpConnectionFactory<com.feilong.lib.org.apache.http.impl.DefaultBHttpClientConnection> {
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpClientConnectionFactory(com.feilong.lib.org.apache.http.config.ConnectionConfig, com.feilong.lib.org.apache.http.entity.ContentLengthStrategy, com.feilong.lib.org.apache.http.entity.ContentLengthStrategy, com.feilong.lib.org.apache.http.io.HttpMessageWriterFactory<com.feilong.lib.org.apache.http.HttpRequest>, com.feilong.lib.org.apache.http.io.HttpMessageParserFactory<com.feilong.lib.org.apache.http.HttpResponse>);
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpClientConnectionFactory(com.feilong.lib.org.apache.http.config.ConnectionConfig, com.feilong.lib.org.apache.http.io.HttpMessageWriterFactory<com.feilong.lib.org.apache.http.HttpRequest>, com.feilong.lib.org.apache.http.io.HttpMessageParserFactory<com.feilong.lib.org.apache.http.HttpResponse>);
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpClientConnectionFactory(com.feilong.lib.org.apache.http.config.ConnectionConfig);
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpClientConnectionFactory();
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpClientConnection createConnection(java.net.Socket) throws java.io.IOException;
  public com.feilong.lib.org.apache.http.HttpConnection createConnection(java.net.Socket) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.DefaultBHttpServerConnection`

```java
public class com.feilong.lib.org.apache.http.impl.DefaultBHttpServerConnection extends com.feilong.lib.org.apache.http.impl.BHttpConnectionBase implements com.feilong.lib.org.apache.http.HttpServerConnection {
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpServerConnection(int, int, java.nio.charset.CharsetDecoder, java.nio.charset.CharsetEncoder, com.feilong.lib.org.apache.http.config.MessageConstraints, com.feilong.lib.org.apache.http.entity.ContentLengthStrategy, com.feilong.lib.org.apache.http.entity.ContentLengthStrategy, com.feilong.lib.org.apache.http.io.HttpMessageParserFactory<com.feilong.lib.org.apache.http.HttpRequest>, com.feilong.lib.org.apache.http.io.HttpMessageWriterFactory<com.feilong.lib.org.apache.http.HttpResponse>);
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpServerConnection(int, java.nio.charset.CharsetDecoder, java.nio.charset.CharsetEncoder, com.feilong.lib.org.apache.http.config.MessageConstraints);
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpServerConnection(int);
  public void bind(java.net.Socket) throws java.io.IOException;
  public com.feilong.lib.org.apache.http.HttpRequest receiveRequestHeader() throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public void receiveRequestEntity(com.feilong.lib.org.apache.http.HttpEntityEnclosingRequest) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public void sendResponseHeader(com.feilong.lib.org.apache.http.HttpResponse) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public void sendResponseEntity(com.feilong.lib.org.apache.http.HttpResponse) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public void flush() throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.DefaultBHttpServerConnectionFactory`

```java
public class com.feilong.lib.org.apache.http.impl.DefaultBHttpServerConnectionFactory implements com.feilong.lib.org.apache.http.HttpConnectionFactory<com.feilong.lib.org.apache.http.impl.DefaultBHttpServerConnection> {
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpServerConnectionFactory(com.feilong.lib.org.apache.http.config.ConnectionConfig, com.feilong.lib.org.apache.http.entity.ContentLengthStrategy, com.feilong.lib.org.apache.http.entity.ContentLengthStrategy, com.feilong.lib.org.apache.http.io.HttpMessageParserFactory<com.feilong.lib.org.apache.http.HttpRequest>, com.feilong.lib.org.apache.http.io.HttpMessageWriterFactory<com.feilong.lib.org.apache.http.HttpResponse>);
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpServerConnectionFactory(com.feilong.lib.org.apache.http.config.ConnectionConfig, com.feilong.lib.org.apache.http.io.HttpMessageParserFactory<com.feilong.lib.org.apache.http.HttpRequest>, com.feilong.lib.org.apache.http.io.HttpMessageWriterFactory<com.feilong.lib.org.apache.http.HttpResponse>);
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpServerConnectionFactory(com.feilong.lib.org.apache.http.config.ConnectionConfig);
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpServerConnectionFactory();
  public com.feilong.lib.org.apache.http.impl.DefaultBHttpServerConnection createConnection(java.net.Socket) throws java.io.IOException;
  public com.feilong.lib.org.apache.http.HttpConnection createConnection(java.net.Socket) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.DefaultConnectionReuseStrategy`

```java
public class com.feilong.lib.org.apache.http.impl.DefaultConnectionReuseStrategy implements com.feilong.lib.org.apache.http.ConnectionReuseStrategy {
  public com.feilong.lib.org.apache.http.impl.DefaultConnectionReuseStrategy();
  public boolean keepAlive(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.DefaultHttpRequestFactory`

```java
public class com.feilong.lib.org.apache.http.impl.DefaultHttpRequestFactory implements com.feilong.lib.org.apache.http.HttpRequestFactory {
  public com.feilong.lib.org.apache.http.impl.DefaultHttpRequestFactory();
  public com.feilong.lib.org.apache.http.HttpRequest newHttpRequest(com.feilong.lib.org.apache.http.RequestLine) throws com.feilong.lib.org.apache.http.MethodNotSupportedException;
  public com.feilong.lib.org.apache.http.HttpRequest newHttpRequest(java.lang.String, java.lang.String) throws com.feilong.lib.org.apache.http.MethodNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.impl.DefaultHttpResponseFactory`

```java
public class com.feilong.lib.org.apache.http.impl.DefaultHttpResponseFactory implements com.feilong.lib.org.apache.http.HttpResponseFactory {
  public com.feilong.lib.org.apache.http.impl.DefaultHttpResponseFactory(com.feilong.lib.org.apache.http.ReasonPhraseCatalog);
  public com.feilong.lib.org.apache.http.impl.DefaultHttpResponseFactory();
  public com.feilong.lib.org.apache.http.HttpResponse newHttpResponse(com.feilong.lib.org.apache.http.ProtocolVersion, int, com.feilong.lib.org.apache.http.protocol.HttpContext);
  public com.feilong.lib.org.apache.http.HttpResponse newHttpResponse(com.feilong.lib.org.apache.http.StatusLine, com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.EnglishReasonPhraseCatalog`

```java
public class com.feilong.lib.org.apache.http.impl.EnglishReasonPhraseCatalog implements com.feilong.lib.org.apache.http.ReasonPhraseCatalog {
  public java.lang.String getReason(int, java.util.Locale);
}
```

## `com.feilong.lib.org.apache.http.impl.HttpConnectionMetricsImpl`

```java
public class com.feilong.lib.org.apache.http.impl.HttpConnectionMetricsImpl implements com.feilong.lib.org.apache.http.HttpConnectionMetrics {
  public com.feilong.lib.org.apache.http.impl.HttpConnectionMetricsImpl(com.feilong.lib.org.apache.http.io.HttpTransportMetrics, com.feilong.lib.org.apache.http.io.HttpTransportMetrics);
  public long getReceivedBytesCount();
  public long getSentBytesCount();
  public long getRequestCount();
  public void incrementRequestCount();
  public long getResponseCount();
  public void incrementResponseCount();
  public java.lang.Object getMetric(java.lang.String);
  public void setMetric(java.lang.String, java.lang.Object);
  public void reset();
}
```

## `com.feilong.lib.org.apache.http.impl.NoConnectionReuseStrategy`

```java
public class com.feilong.lib.org.apache.http.impl.NoConnectionReuseStrategy implements com.feilong.lib.org.apache.http.ConnectionReuseStrategy {
  public com.feilong.lib.org.apache.http.impl.NoConnectionReuseStrategy();
  public boolean keepAlive(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```
