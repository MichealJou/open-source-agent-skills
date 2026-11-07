# com.feilong.lib.org.apache.http.impl.execchain

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.impl.execchain.BackoffStrategyExec`

```java
public class com.feilong.lib.org.apache.http.impl.execchain.BackoffStrategyExec implements com.feilong.lib.org.apache.http.impl.execchain.ClientExecChain {
  public com.feilong.lib.org.apache.http.impl.execchain.BackoffStrategyExec(com.feilong.lib.org.apache.http.impl.execchain.ClientExecChain, com.feilong.lib.org.apache.http.client.ConnectionBackoffStrategy, com.feilong.lib.org.apache.http.client.BackoffManager);
  public com.feilong.lib.org.apache.http.client.methods.CloseableHttpResponse execute(com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.client.methods.HttpRequestWrapper, com.feilong.lib.org.apache.http.client.protocol.HttpClientContext, com.feilong.lib.org.apache.http.client.methods.HttpExecutionAware) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.impl.execchain.ClientExecChain`

```java
public interface com.feilong.lib.org.apache.http.impl.execchain.ClientExecChain {
  public abstract com.feilong.lib.org.apache.http.client.methods.CloseableHttpResponse execute(com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.client.methods.HttpRequestWrapper, com.feilong.lib.org.apache.http.client.protocol.HttpClientContext, com.feilong.lib.org.apache.http.client.methods.HttpExecutionAware) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.impl.execchain.MainClientExec`

```java
public class com.feilong.lib.org.apache.http.impl.execchain.MainClientExec implements com.feilong.lib.org.apache.http.impl.execchain.ClientExecChain {
  public com.feilong.lib.org.apache.http.impl.execchain.MainClientExec(com.feilong.lib.org.apache.http.protocol.HttpRequestExecutor, com.feilong.lib.org.apache.http.conn.HttpClientConnectionManager, com.feilong.lib.org.apache.http.ConnectionReuseStrategy, com.feilong.lib.org.apache.http.conn.ConnectionKeepAliveStrategy, com.feilong.lib.org.apache.http.protocol.HttpProcessor, com.feilong.lib.org.apache.http.client.AuthenticationStrategy, com.feilong.lib.org.apache.http.client.AuthenticationStrategy, com.feilong.lib.org.apache.http.client.UserTokenHandler);
  public com.feilong.lib.org.apache.http.impl.execchain.MainClientExec(com.feilong.lib.org.apache.http.protocol.HttpRequestExecutor, com.feilong.lib.org.apache.http.conn.HttpClientConnectionManager, com.feilong.lib.org.apache.http.ConnectionReuseStrategy, com.feilong.lib.org.apache.http.conn.ConnectionKeepAliveStrategy, com.feilong.lib.org.apache.http.client.AuthenticationStrategy, com.feilong.lib.org.apache.http.client.AuthenticationStrategy, com.feilong.lib.org.apache.http.client.UserTokenHandler);
  public com.feilong.lib.org.apache.http.client.methods.CloseableHttpResponse execute(com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.client.methods.HttpRequestWrapper, com.feilong.lib.org.apache.http.client.protocol.HttpClientContext, com.feilong.lib.org.apache.http.client.methods.HttpExecutionAware) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.impl.execchain.MinimalClientExec`

```java
public class com.feilong.lib.org.apache.http.impl.execchain.MinimalClientExec implements com.feilong.lib.org.apache.http.impl.execchain.ClientExecChain {
  public com.feilong.lib.org.apache.http.impl.execchain.MinimalClientExec(com.feilong.lib.org.apache.http.protocol.HttpRequestExecutor, com.feilong.lib.org.apache.http.conn.HttpClientConnectionManager, com.feilong.lib.org.apache.http.ConnectionReuseStrategy, com.feilong.lib.org.apache.http.conn.ConnectionKeepAliveStrategy);
  public com.feilong.lib.org.apache.http.client.methods.CloseableHttpResponse execute(com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.client.methods.HttpRequestWrapper, com.feilong.lib.org.apache.http.client.protocol.HttpClientContext, com.feilong.lib.org.apache.http.client.methods.HttpExecutionAware) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.impl.execchain.ProtocolExec`

```java
public class com.feilong.lib.org.apache.http.impl.execchain.ProtocolExec implements com.feilong.lib.org.apache.http.impl.execchain.ClientExecChain {
  public com.feilong.lib.org.apache.http.impl.execchain.ProtocolExec(com.feilong.lib.org.apache.http.impl.execchain.ClientExecChain, com.feilong.lib.org.apache.http.protocol.HttpProcessor);
  public com.feilong.lib.org.apache.http.client.methods.CloseableHttpResponse execute(com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.client.methods.HttpRequestWrapper, com.feilong.lib.org.apache.http.client.protocol.HttpClientContext, com.feilong.lib.org.apache.http.client.methods.HttpExecutionAware) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.impl.execchain.RedirectExec`

```java
public class com.feilong.lib.org.apache.http.impl.execchain.RedirectExec implements com.feilong.lib.org.apache.http.impl.execchain.ClientExecChain {
  public com.feilong.lib.org.apache.http.impl.execchain.RedirectExec(com.feilong.lib.org.apache.http.impl.execchain.ClientExecChain, com.feilong.lib.org.apache.http.conn.routing.HttpRoutePlanner, com.feilong.lib.org.apache.http.client.RedirectStrategy);
  public com.feilong.lib.org.apache.http.client.methods.CloseableHttpResponse execute(com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.client.methods.HttpRequestWrapper, com.feilong.lib.org.apache.http.client.protocol.HttpClientContext, com.feilong.lib.org.apache.http.client.methods.HttpExecutionAware) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.impl.execchain.RequestAbortedException`

```java
public class com.feilong.lib.org.apache.http.impl.execchain.RequestAbortedException extends java.io.InterruptedIOException {
  public com.feilong.lib.org.apache.http.impl.execchain.RequestAbortedException(java.lang.String);
  public com.feilong.lib.org.apache.http.impl.execchain.RequestAbortedException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.impl.execchain.RetryExec`

```java
public class com.feilong.lib.org.apache.http.impl.execchain.RetryExec implements com.feilong.lib.org.apache.http.impl.execchain.ClientExecChain {
  public com.feilong.lib.org.apache.http.impl.execchain.RetryExec(com.feilong.lib.org.apache.http.impl.execchain.ClientExecChain, com.feilong.lib.org.apache.http.client.HttpRequestRetryHandler);
  public com.feilong.lib.org.apache.http.client.methods.CloseableHttpResponse execute(com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.client.methods.HttpRequestWrapper, com.feilong.lib.org.apache.http.client.protocol.HttpClientContext, com.feilong.lib.org.apache.http.client.methods.HttpExecutionAware) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.impl.execchain.ServiceUnavailableRetryExec`

```java
public class com.feilong.lib.org.apache.http.impl.execchain.ServiceUnavailableRetryExec implements com.feilong.lib.org.apache.http.impl.execchain.ClientExecChain {
  public com.feilong.lib.org.apache.http.impl.execchain.ServiceUnavailableRetryExec(com.feilong.lib.org.apache.http.impl.execchain.ClientExecChain, com.feilong.lib.org.apache.http.client.ServiceUnavailableRetryStrategy);
  public com.feilong.lib.org.apache.http.client.methods.CloseableHttpResponse execute(com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.client.methods.HttpRequestWrapper, com.feilong.lib.org.apache.http.client.protocol.HttpClientContext, com.feilong.lib.org.apache.http.client.methods.HttpExecutionAware) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.impl.execchain.TunnelRefusedException`

```java
public class com.feilong.lib.org.apache.http.impl.execchain.TunnelRefusedException extends com.feilong.lib.org.apache.http.HttpException {
  public com.feilong.lib.org.apache.http.impl.execchain.TunnelRefusedException(java.lang.String, com.feilong.lib.org.apache.http.HttpResponse);
  public com.feilong.lib.org.apache.http.HttpResponse getResponse();
}
```
