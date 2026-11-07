# com.feilong.lib.org.apache.http.conn

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.conn.ConnectTimeoutException`

```java
public class com.feilong.lib.org.apache.http.conn.ConnectTimeoutException extends java.io.InterruptedIOException {
  public com.feilong.lib.org.apache.http.conn.ConnectTimeoutException();
  public com.feilong.lib.org.apache.http.conn.ConnectTimeoutException(java.lang.String);
  public com.feilong.lib.org.apache.http.conn.ConnectTimeoutException(java.io.IOException, com.feilong.lib.org.apache.http.HttpHost, java.net.InetAddress...);
  public com.feilong.lib.org.apache.http.HttpHost getHost();
}
```

## `com.feilong.lib.org.apache.http.conn.ConnectionKeepAliveStrategy`

```java
public interface com.feilong.lib.org.apache.http.conn.ConnectionKeepAliveStrategy {
  public abstract long getKeepAliveDuration(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.conn.ConnectionPoolTimeoutException`

```java
public class com.feilong.lib.org.apache.http.conn.ConnectionPoolTimeoutException extends com.feilong.lib.org.apache.http.conn.ConnectTimeoutException {
  public com.feilong.lib.org.apache.http.conn.ConnectionPoolTimeoutException();
  public com.feilong.lib.org.apache.http.conn.ConnectionPoolTimeoutException(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.conn.ConnectionReleaseTrigger`

```java
public interface com.feilong.lib.org.apache.http.conn.ConnectionReleaseTrigger {
  public abstract void releaseConnection() throws java.io.IOException;
  public abstract void abortConnection() throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.conn.ConnectionRequest`

```java
public interface com.feilong.lib.org.apache.http.conn.ConnectionRequest extends com.feilong.lib.org.apache.http.concurrent.Cancellable {
  public abstract com.feilong.lib.org.apache.http.HttpClientConnection get(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException, java.util.concurrent.ExecutionException, com.feilong.lib.org.apache.http.conn.ConnectionPoolTimeoutException;
}
```

## `com.feilong.lib.org.apache.http.conn.DnsResolver`

```java
public interface com.feilong.lib.org.apache.http.conn.DnsResolver {
  public abstract java.net.InetAddress[] resolve(java.lang.String) throws java.net.UnknownHostException;
}
```

## `com.feilong.lib.org.apache.http.conn.EofSensorInputStream`

```java
public class com.feilong.lib.org.apache.http.conn.EofSensorInputStream extends java.io.InputStream implements com.feilong.lib.org.apache.http.conn.ConnectionReleaseTrigger {
  public com.feilong.lib.org.apache.http.conn.EofSensorInputStream(java.io.InputStream, com.feilong.lib.org.apache.http.conn.EofSensorWatcher);
  public int read() throws java.io.IOException;
  public int read(byte[], int, int) throws java.io.IOException;
  public int read(byte[]) throws java.io.IOException;
  public int available() throws java.io.IOException;
  public void close() throws java.io.IOException;
  public void releaseConnection() throws java.io.IOException;
  public void abortConnection() throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.conn.EofSensorWatcher`

```java
public interface com.feilong.lib.org.apache.http.conn.EofSensorWatcher {
  public abstract boolean eofDetected(java.io.InputStream) throws java.io.IOException;
  public abstract boolean streamClosed(java.io.InputStream) throws java.io.IOException;
  public abstract boolean streamAbort(java.io.InputStream) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.conn.HttpClientConnectionManager`

```java
public interface com.feilong.lib.org.apache.http.conn.HttpClientConnectionManager {
  public abstract com.feilong.lib.org.apache.http.conn.ConnectionRequest requestConnection(com.feilong.lib.org.apache.http.conn.routing.HttpRoute, java.lang.Object);
  public abstract void releaseConnection(com.feilong.lib.org.apache.http.HttpClientConnection, java.lang.Object, long, java.util.concurrent.TimeUnit);
  public abstract void connect(com.feilong.lib.org.apache.http.HttpClientConnection, com.feilong.lib.org.apache.http.conn.routing.HttpRoute, int, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public abstract void upgrade(com.feilong.lib.org.apache.http.HttpClientConnection, com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public abstract void routeComplete(com.feilong.lib.org.apache.http.HttpClientConnection, com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public abstract void closeIdleConnections(long, java.util.concurrent.TimeUnit);
  public abstract void closeExpiredConnections();
  public abstract void shutdown();
}
```

## `com.feilong.lib.org.apache.http.conn.HttpClientConnectionOperator`

```java
public interface com.feilong.lib.org.apache.http.conn.HttpClientConnectionOperator {
  public abstract void connect(com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection, com.feilong.lib.org.apache.http.HttpHost, java.net.InetSocketAddress, int, com.feilong.lib.org.apache.http.config.SocketConfig, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public abstract void upgrade(com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection, com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.conn.HttpConnectionFactory`

```java
public interface com.feilong.lib.org.apache.http.conn.HttpConnectionFactory<T, C extends com.feilong.lib.org.apache.http.HttpConnection> {
  public abstract C create(T, com.feilong.lib.org.apache.http.config.ConnectionConfig);
}
```

## `com.feilong.lib.org.apache.http.conn.HttpHostConnectException`

```java
public class com.feilong.lib.org.apache.http.conn.HttpHostConnectException extends java.net.ConnectException {
  public com.feilong.lib.org.apache.http.conn.HttpHostConnectException(com.feilong.lib.org.apache.http.HttpHost, java.net.ConnectException);
  public com.feilong.lib.org.apache.http.conn.HttpHostConnectException(java.io.IOException, com.feilong.lib.org.apache.http.HttpHost, java.net.InetAddress...);
  public com.feilong.lib.org.apache.http.HttpHost getHost();
}
```

## `com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection`

```java
public interface com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection extends com.feilong.lib.org.apache.http.HttpClientConnection,com.feilong.lib.org.apache.http.HttpInetConnection {
  public abstract java.lang.String getId();
  public abstract void bind(java.net.Socket) throws java.io.IOException;
  public abstract java.net.Socket getSocket();
  public abstract javax.net.ssl.SSLSession getSSLSession();
}
```

## `com.feilong.lib.org.apache.http.conn.SchemePortResolver`

```java
public interface com.feilong.lib.org.apache.http.conn.SchemePortResolver {
  public abstract int resolve(com.feilong.lib.org.apache.http.HttpHost) throws com.feilong.lib.org.apache.http.conn.UnsupportedSchemeException;
}
```

## `com.feilong.lib.org.apache.http.conn.UnsupportedSchemeException`

```java
public class com.feilong.lib.org.apache.http.conn.UnsupportedSchemeException extends java.io.IOException {
  public com.feilong.lib.org.apache.http.conn.UnsupportedSchemeException(java.lang.String);
}
```
