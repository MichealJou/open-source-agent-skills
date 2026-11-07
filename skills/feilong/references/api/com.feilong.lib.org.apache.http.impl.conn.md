# com.feilong.lib.org.apache.http.impl.conn

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.impl.conn.BasicHttpClientConnectionManager`

```java
public class com.feilong.lib.org.apache.http.impl.conn.BasicHttpClientConnectionManager implements com.feilong.lib.org.apache.http.conn.HttpClientConnectionManager,java.io.Closeable {
  public com.feilong.lib.org.apache.http.impl.conn.BasicHttpClientConnectionManager(com.feilong.lib.org.apache.http.config.Lookup<com.feilong.lib.org.apache.http.conn.socket.ConnectionSocketFactory>, com.feilong.lib.org.apache.http.conn.HttpConnectionFactory<com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection>, com.feilong.lib.org.apache.http.conn.SchemePortResolver, com.feilong.lib.org.apache.http.conn.DnsResolver);
  public com.feilong.lib.org.apache.http.impl.conn.BasicHttpClientConnectionManager(com.feilong.lib.org.apache.http.conn.HttpClientConnectionOperator, com.feilong.lib.org.apache.http.conn.HttpConnectionFactory<com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection>);
  public com.feilong.lib.org.apache.http.impl.conn.BasicHttpClientConnectionManager(com.feilong.lib.org.apache.http.config.Lookup<com.feilong.lib.org.apache.http.conn.socket.ConnectionSocketFactory>, com.feilong.lib.org.apache.http.conn.HttpConnectionFactory<com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection>);
  public com.feilong.lib.org.apache.http.impl.conn.BasicHttpClientConnectionManager(com.feilong.lib.org.apache.http.config.Lookup<com.feilong.lib.org.apache.http.conn.socket.ConnectionSocketFactory>);
  public com.feilong.lib.org.apache.http.impl.conn.BasicHttpClientConnectionManager();
  public void close();
  public synchronized com.feilong.lib.org.apache.http.config.SocketConfig getSocketConfig();
  public synchronized void setSocketConfig(com.feilong.lib.org.apache.http.config.SocketConfig);
  public synchronized com.feilong.lib.org.apache.http.config.ConnectionConfig getConnectionConfig();
  public synchronized void setConnectionConfig(com.feilong.lib.org.apache.http.config.ConnectionConfig);
  public final com.feilong.lib.org.apache.http.conn.ConnectionRequest requestConnection(com.feilong.lib.org.apache.http.conn.routing.HttpRoute, java.lang.Object);
  public synchronized void releaseConnection(com.feilong.lib.org.apache.http.HttpClientConnection, java.lang.Object, long, java.util.concurrent.TimeUnit);
  public void connect(com.feilong.lib.org.apache.http.HttpClientConnection, com.feilong.lib.org.apache.http.conn.routing.HttpRoute, int, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public void upgrade(com.feilong.lib.org.apache.http.HttpClientConnection, com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public void routeComplete(com.feilong.lib.org.apache.http.HttpClientConnection, com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public synchronized void closeExpiredConnections();
  public synchronized void closeIdleConnections(long, java.util.concurrent.TimeUnit);
  public void shutdown();
}
```

## `com.feilong.lib.org.apache.http.impl.conn.ConnectionShutdownException`

```java
public class com.feilong.lib.org.apache.http.impl.conn.ConnectionShutdownException extends java.lang.IllegalStateException {
  public com.feilong.lib.org.apache.http.impl.conn.ConnectionShutdownException();
}
```

## `com.feilong.lib.org.apache.http.impl.conn.DefaultHttpClientConnectionOperator`

```java
public class com.feilong.lib.org.apache.http.impl.conn.DefaultHttpClientConnectionOperator implements com.feilong.lib.org.apache.http.conn.HttpClientConnectionOperator {
  public com.feilong.lib.org.apache.http.impl.conn.DefaultHttpClientConnectionOperator(com.feilong.lib.org.apache.http.config.Lookup<com.feilong.lib.org.apache.http.conn.socket.ConnectionSocketFactory>, com.feilong.lib.org.apache.http.conn.SchemePortResolver, com.feilong.lib.org.apache.http.conn.DnsResolver);
  public void connect(com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection, com.feilong.lib.org.apache.http.HttpHost, java.net.InetSocketAddress, int, com.feilong.lib.org.apache.http.config.SocketConfig, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public void upgrade(com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection, com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.conn.DefaultHttpResponseParser`

```java
public class com.feilong.lib.org.apache.http.impl.conn.DefaultHttpResponseParser extends com.feilong.lib.org.apache.http.impl.io.AbstractMessageParser<com.feilong.lib.org.apache.http.HttpResponse> {
  public com.feilong.lib.org.apache.http.impl.conn.DefaultHttpResponseParser(com.feilong.lib.org.apache.http.io.SessionInputBuffer, com.feilong.lib.org.apache.http.message.LineParser, com.feilong.lib.org.apache.http.HttpResponseFactory, com.feilong.lib.org.apache.http.config.MessageConstraints);
  public com.feilong.lib.org.apache.http.impl.conn.DefaultHttpResponseParser(com.feilong.lib.org.apache.http.io.SessionInputBuffer, com.feilong.lib.org.apache.http.config.MessageConstraints);
  public com.feilong.lib.org.apache.http.impl.conn.DefaultHttpResponseParser(com.feilong.lib.org.apache.http.io.SessionInputBuffer);
}
```

## `com.feilong.lib.org.apache.http.impl.conn.DefaultHttpResponseParserFactory`

```java
public class com.feilong.lib.org.apache.http.impl.conn.DefaultHttpResponseParserFactory implements com.feilong.lib.org.apache.http.io.HttpMessageParserFactory<com.feilong.lib.org.apache.http.HttpResponse> {
  public com.feilong.lib.org.apache.http.impl.conn.DefaultHttpResponseParserFactory(com.feilong.lib.org.apache.http.message.LineParser, com.feilong.lib.org.apache.http.HttpResponseFactory);
  public com.feilong.lib.org.apache.http.impl.conn.DefaultHttpResponseParserFactory(com.feilong.lib.org.apache.http.HttpResponseFactory);
  public com.feilong.lib.org.apache.http.impl.conn.DefaultHttpResponseParserFactory();
  public com.feilong.lib.org.apache.http.io.HttpMessageParser<com.feilong.lib.org.apache.http.HttpResponse> create(com.feilong.lib.org.apache.http.io.SessionInputBuffer, com.feilong.lib.org.apache.http.config.MessageConstraints);
}
```

## `com.feilong.lib.org.apache.http.impl.conn.DefaultManagedHttpClientConnection`

```java
public class com.feilong.lib.org.apache.http.impl.conn.DefaultManagedHttpClientConnection extends com.feilong.lib.org.apache.http.impl.DefaultBHttpClientConnection implements com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection,com.feilong.lib.org.apache.http.protocol.HttpContext {
  public com.feilong.lib.org.apache.http.impl.conn.DefaultManagedHttpClientConnection(java.lang.String, int, int, java.nio.charset.CharsetDecoder, java.nio.charset.CharsetEncoder, com.feilong.lib.org.apache.http.config.MessageConstraints, com.feilong.lib.org.apache.http.entity.ContentLengthStrategy, com.feilong.lib.org.apache.http.entity.ContentLengthStrategy, com.feilong.lib.org.apache.http.io.HttpMessageWriterFactory<com.feilong.lib.org.apache.http.HttpRequest>, com.feilong.lib.org.apache.http.io.HttpMessageParserFactory<com.feilong.lib.org.apache.http.HttpResponse>);
  public com.feilong.lib.org.apache.http.impl.conn.DefaultManagedHttpClientConnection(java.lang.String, int);
  public java.lang.String getId();
  public void shutdown() throws java.io.IOException;
  public java.lang.Object getAttribute(java.lang.String);
  public java.lang.Object removeAttribute(java.lang.String);
  public void setAttribute(java.lang.String, java.lang.Object);
  public void bind(java.net.Socket) throws java.io.IOException;
  public java.net.Socket getSocket();
  public javax.net.ssl.SSLSession getSSLSession();
}
```

## `com.feilong.lib.org.apache.http.impl.conn.DefaultProxyRoutePlanner`

```java
public class com.feilong.lib.org.apache.http.impl.conn.DefaultProxyRoutePlanner extends com.feilong.lib.org.apache.http.impl.conn.DefaultRoutePlanner {
  public com.feilong.lib.org.apache.http.impl.conn.DefaultProxyRoutePlanner(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.conn.SchemePortResolver);
  public com.feilong.lib.org.apache.http.impl.conn.DefaultProxyRoutePlanner(com.feilong.lib.org.apache.http.HttpHost);
}
```

## `com.feilong.lib.org.apache.http.impl.conn.DefaultRoutePlanner`

```java
public class com.feilong.lib.org.apache.http.impl.conn.DefaultRoutePlanner implements com.feilong.lib.org.apache.http.conn.routing.HttpRoutePlanner {
  public com.feilong.lib.org.apache.http.impl.conn.DefaultRoutePlanner(com.feilong.lib.org.apache.http.conn.SchemePortResolver);
  public com.feilong.lib.org.apache.http.conn.routing.HttpRoute determineRoute(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.impl.conn.DefaultSchemePortResolver`

```java
public class com.feilong.lib.org.apache.http.impl.conn.DefaultSchemePortResolver implements com.feilong.lib.org.apache.http.conn.SchemePortResolver {
  public com.feilong.lib.org.apache.http.impl.conn.DefaultSchemePortResolver();
  public int resolve(com.feilong.lib.org.apache.http.HttpHost) throws com.feilong.lib.org.apache.http.conn.UnsupportedSchemeException;
}
```

## `com.feilong.lib.org.apache.http.impl.conn.InMemoryDnsResolver`

```java
public class com.feilong.lib.org.apache.http.impl.conn.InMemoryDnsResolver implements com.feilong.lib.org.apache.http.conn.DnsResolver {
  public com.feilong.lib.org.apache.http.impl.conn.InMemoryDnsResolver();
  public void add(java.lang.String, java.net.InetAddress...);
  public java.net.InetAddress[] resolve(java.lang.String) throws java.net.UnknownHostException;
}
```

## `com.feilong.lib.org.apache.http.impl.conn.ManagedHttpClientConnectionFactory`

```java
public class com.feilong.lib.org.apache.http.impl.conn.ManagedHttpClientConnectionFactory implements com.feilong.lib.org.apache.http.conn.HttpConnectionFactory<com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection> {
  public com.feilong.lib.org.apache.http.impl.conn.ManagedHttpClientConnectionFactory(com.feilong.lib.org.apache.http.io.HttpMessageWriterFactory<com.feilong.lib.org.apache.http.HttpRequest>, com.feilong.lib.org.apache.http.io.HttpMessageParserFactory<com.feilong.lib.org.apache.http.HttpResponse>, com.feilong.lib.org.apache.http.entity.ContentLengthStrategy, com.feilong.lib.org.apache.http.entity.ContentLengthStrategy);
  public com.feilong.lib.org.apache.http.impl.conn.ManagedHttpClientConnectionFactory(com.feilong.lib.org.apache.http.io.HttpMessageWriterFactory<com.feilong.lib.org.apache.http.HttpRequest>, com.feilong.lib.org.apache.http.io.HttpMessageParserFactory<com.feilong.lib.org.apache.http.HttpResponse>);
  public com.feilong.lib.org.apache.http.impl.conn.ManagedHttpClientConnectionFactory(com.feilong.lib.org.apache.http.io.HttpMessageParserFactory<com.feilong.lib.org.apache.http.HttpResponse>);
  public com.feilong.lib.org.apache.http.impl.conn.ManagedHttpClientConnectionFactory();
  public com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection create(com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.config.ConnectionConfig);
  public com.feilong.lib.org.apache.http.HttpConnection create(java.lang.Object, com.feilong.lib.org.apache.http.config.ConnectionConfig);
}
```

## `com.feilong.lib.org.apache.http.impl.conn.PoolingHttpClientConnectionManager`

```java
public class com.feilong.lib.org.apache.http.impl.conn.PoolingHttpClientConnectionManager implements com.feilong.lib.org.apache.http.conn.HttpClientConnectionManager, com.feilong.lib.org.apache.http.pool.ConnPoolControl<com.feilong.lib.org.apache.http.conn.routing.HttpRoute>, java.io.Closeable {
  public com.feilong.lib.org.apache.http.impl.conn.PoolingHttpClientConnectionManager();
  public com.feilong.lib.org.apache.http.impl.conn.PoolingHttpClientConnectionManager(long, java.util.concurrent.TimeUnit);
  public com.feilong.lib.org.apache.http.impl.conn.PoolingHttpClientConnectionManager(com.feilong.lib.org.apache.http.config.Registry<com.feilong.lib.org.apache.http.conn.socket.ConnectionSocketFactory>);
  public com.feilong.lib.org.apache.http.impl.conn.PoolingHttpClientConnectionManager(com.feilong.lib.org.apache.http.config.Registry<com.feilong.lib.org.apache.http.conn.socket.ConnectionSocketFactory>, com.feilong.lib.org.apache.http.conn.DnsResolver);
  public com.feilong.lib.org.apache.http.impl.conn.PoolingHttpClientConnectionManager(com.feilong.lib.org.apache.http.config.Registry<com.feilong.lib.org.apache.http.conn.socket.ConnectionSocketFactory>, com.feilong.lib.org.apache.http.conn.HttpConnectionFactory<com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection>);
  public com.feilong.lib.org.apache.http.impl.conn.PoolingHttpClientConnectionManager(com.feilong.lib.org.apache.http.conn.HttpConnectionFactory<com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection>);
  public com.feilong.lib.org.apache.http.impl.conn.PoolingHttpClientConnectionManager(com.feilong.lib.org.apache.http.config.Registry<com.feilong.lib.org.apache.http.conn.socket.ConnectionSocketFactory>, com.feilong.lib.org.apache.http.conn.HttpConnectionFactory<com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection>, com.feilong.lib.org.apache.http.conn.DnsResolver);
  public com.feilong.lib.org.apache.http.impl.conn.PoolingHttpClientConnectionManager(com.feilong.lib.org.apache.http.config.Registry<com.feilong.lib.org.apache.http.conn.socket.ConnectionSocketFactory>, com.feilong.lib.org.apache.http.conn.HttpConnectionFactory<com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection>, com.feilong.lib.org.apache.http.conn.SchemePortResolver, com.feilong.lib.org.apache.http.conn.DnsResolver, long, java.util.concurrent.TimeUnit);
  public com.feilong.lib.org.apache.http.impl.conn.PoolingHttpClientConnectionManager(com.feilong.lib.org.apache.http.conn.HttpClientConnectionOperator, com.feilong.lib.org.apache.http.conn.HttpConnectionFactory<com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection>, long, java.util.concurrent.TimeUnit);
  public void close();
  public com.feilong.lib.org.apache.http.conn.ConnectionRequest requestConnection(com.feilong.lib.org.apache.http.conn.routing.HttpRoute, java.lang.Object);
  public void releaseConnection(com.feilong.lib.org.apache.http.HttpClientConnection, java.lang.Object, long, java.util.concurrent.TimeUnit);
  public void connect(com.feilong.lib.org.apache.http.HttpClientConnection, com.feilong.lib.org.apache.http.conn.routing.HttpRoute, int, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public void upgrade(com.feilong.lib.org.apache.http.HttpClientConnection, com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public void routeComplete(com.feilong.lib.org.apache.http.HttpClientConnection, com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public void shutdown();
  public void closeIdleConnections(long, java.util.concurrent.TimeUnit);
  public void closeExpiredConnections();
  public int getMaxTotal();
  public void setMaxTotal(int);
  public int getDefaultMaxPerRoute();
  public void setDefaultMaxPerRoute(int);
  public int getMaxPerRoute(com.feilong.lib.org.apache.http.conn.routing.HttpRoute);
  public void setMaxPerRoute(com.feilong.lib.org.apache.http.conn.routing.HttpRoute, int);
  public com.feilong.lib.org.apache.http.pool.PoolStats getTotalStats();
  public com.feilong.lib.org.apache.http.pool.PoolStats getStats(com.feilong.lib.org.apache.http.conn.routing.HttpRoute);
  public java.util.Set<com.feilong.lib.org.apache.http.conn.routing.HttpRoute> getRoutes();
  public com.feilong.lib.org.apache.http.config.SocketConfig getDefaultSocketConfig();
  public void setDefaultSocketConfig(com.feilong.lib.org.apache.http.config.SocketConfig);
  public com.feilong.lib.org.apache.http.config.ConnectionConfig getDefaultConnectionConfig();
  public void setDefaultConnectionConfig(com.feilong.lib.org.apache.http.config.ConnectionConfig);
  public com.feilong.lib.org.apache.http.config.SocketConfig getSocketConfig(com.feilong.lib.org.apache.http.HttpHost);
  public void setSocketConfig(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.config.SocketConfig);
  public com.feilong.lib.org.apache.http.config.ConnectionConfig getConnectionConfig(com.feilong.lib.org.apache.http.HttpHost);
  public void setConnectionConfig(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.config.ConnectionConfig);
  public int getValidateAfterInactivity();
  public void setValidateAfterInactivity(int);
  public com.feilong.lib.org.apache.http.pool.PoolStats getStats(java.lang.Object);
  public int getMaxPerRoute(java.lang.Object);
  public void setMaxPerRoute(java.lang.Object, int);
}
```

## `com.feilong.lib.org.apache.http.impl.conn.SystemDefaultDnsResolver`

```java
public class com.feilong.lib.org.apache.http.impl.conn.SystemDefaultDnsResolver implements com.feilong.lib.org.apache.http.conn.DnsResolver {
  public com.feilong.lib.org.apache.http.impl.conn.SystemDefaultDnsResolver();
  public java.net.InetAddress[] resolve(java.lang.String) throws java.net.UnknownHostException;
}
```

## `com.feilong.lib.org.apache.http.impl.conn.SystemDefaultRoutePlanner`

```java
public class com.feilong.lib.org.apache.http.impl.conn.SystemDefaultRoutePlanner extends com.feilong.lib.org.apache.http.impl.conn.DefaultRoutePlanner {
  public com.feilong.lib.org.apache.http.impl.conn.SystemDefaultRoutePlanner(com.feilong.lib.org.apache.http.conn.SchemePortResolver, java.net.ProxySelector);
  public com.feilong.lib.org.apache.http.impl.conn.SystemDefaultRoutePlanner(java.net.ProxySelector);
}
```

## `com.feilong.lib.org.apache.http.impl.conn.Wire`

```java
public class com.feilong.lib.org.apache.http.impl.conn.Wire {
  public com.feilong.lib.org.apache.http.impl.conn.Wire(java.lang.String);
  public boolean enabled();
  public void output(java.io.InputStream) throws java.io.IOException;
  public void input(java.io.InputStream) throws java.io.IOException;
  public void output(byte[], int, int) throws java.io.IOException;
  public void input(byte[], int, int) throws java.io.IOException;
  public void output(byte[]) throws java.io.IOException;
  public void input(byte[]) throws java.io.IOException;
  public void output(int) throws java.io.IOException;
  public void input(int) throws java.io.IOException;
  public void output(java.lang.String) throws java.io.IOException;
  public void input(java.lang.String) throws java.io.IOException;
}
```
