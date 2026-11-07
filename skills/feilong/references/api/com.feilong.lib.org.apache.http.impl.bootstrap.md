# com.feilong.lib.org.apache.http.impl.bootstrap

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.impl.bootstrap.HttpServer`

```java
public class com.feilong.lib.org.apache.http.impl.bootstrap.HttpServer {
  public java.net.InetAddress getInetAddress();
  public int getLocalPort();
  public void start() throws java.io.IOException;
  public void stop();
  public void awaitTermination(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public void shutdown(long, java.util.concurrent.TimeUnit);
}
```

## `com.feilong.lib.org.apache.http.impl.bootstrap.SSLServerSetupHandler`

```java
public interface com.feilong.lib.org.apache.http.impl.bootstrap.SSLServerSetupHandler {
  public abstract void initialize(javax.net.ssl.SSLServerSocket) throws javax.net.ssl.SSLException;
}
```

## `com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap`

```java
public class com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap {
  public static com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap bootstrap();
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setListenerPort(int);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setLocalAddress(java.net.InetAddress);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setSocketConfig(com.feilong.lib.org.apache.http.config.SocketConfig);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setConnectionConfig(com.feilong.lib.org.apache.http.config.ConnectionConfig);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setHttpProcessor(com.feilong.lib.org.apache.http.protocol.HttpProcessor);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap addInterceptorFirst(com.feilong.lib.org.apache.http.HttpResponseInterceptor);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap addInterceptorLast(com.feilong.lib.org.apache.http.HttpResponseInterceptor);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap addInterceptorFirst(com.feilong.lib.org.apache.http.HttpRequestInterceptor);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap addInterceptorLast(com.feilong.lib.org.apache.http.HttpRequestInterceptor);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setServerInfo(java.lang.String);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setConnectionReuseStrategy(com.feilong.lib.org.apache.http.ConnectionReuseStrategy);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setResponseFactory(com.feilong.lib.org.apache.http.HttpResponseFactory);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setHandlerMapper(com.feilong.lib.org.apache.http.protocol.HttpRequestHandlerMapper);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap registerHandler(java.lang.String, com.feilong.lib.org.apache.http.protocol.HttpRequestHandler);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setExpectationVerifier(com.feilong.lib.org.apache.http.protocol.HttpExpectationVerifier);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setConnectionFactory(com.feilong.lib.org.apache.http.HttpConnectionFactory<? extends com.feilong.lib.org.apache.http.impl.DefaultBHttpServerConnection>);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setSslSetupHandler(com.feilong.lib.org.apache.http.impl.bootstrap.SSLServerSetupHandler);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setServerSocketFactory(javax.net.ServerSocketFactory);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setSslContext(javax.net.ssl.SSLContext);
  public final com.feilong.lib.org.apache.http.impl.bootstrap.ServerBootstrap setExceptionLogger(com.feilong.lib.org.apache.http.ExceptionLogger);
  public com.feilong.lib.org.apache.http.impl.bootstrap.HttpServer create();
}
```
