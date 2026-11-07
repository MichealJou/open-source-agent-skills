# com.feilong.lib.org.apache.http.impl.client

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.impl.client.AIMDBackoffManager`

```java
public class com.feilong.lib.org.apache.http.impl.client.AIMDBackoffManager implements com.feilong.lib.org.apache.http.client.BackoffManager {
  public com.feilong.lib.org.apache.http.impl.client.AIMDBackoffManager(com.feilong.lib.org.apache.http.pool.ConnPoolControl<com.feilong.lib.org.apache.http.conn.routing.HttpRoute>);
  public void backOff(com.feilong.lib.org.apache.http.conn.routing.HttpRoute);
  public void probe(com.feilong.lib.org.apache.http.conn.routing.HttpRoute);
  public void setBackoffFactor(double);
  public void setCooldownMillis(long);
  public void setPerHostConnectionCap(int);
}
```

## `com.feilong.lib.org.apache.http.impl.client.AbstractResponseHandler`

```java
public abstract class com.feilong.lib.org.apache.http.impl.client.AbstractResponseHandler<T> implements com.feilong.lib.org.apache.http.client.ResponseHandler<T> {
  public com.feilong.lib.org.apache.http.impl.client.AbstractResponseHandler();
  public T handleResponse(com.feilong.lib.org.apache.http.HttpResponse) throws com.feilong.lib.org.apache.http.client.HttpResponseException, java.io.IOException;
  public abstract T handleEntity(com.feilong.lib.org.apache.http.HttpEntity) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.client.BasicAuthCache`

```java
public class com.feilong.lib.org.apache.http.impl.client.BasicAuthCache implements com.feilong.lib.org.apache.http.client.AuthCache {
  public com.feilong.lib.org.apache.http.impl.client.BasicAuthCache(com.feilong.lib.org.apache.http.conn.SchemePortResolver);
  public com.feilong.lib.org.apache.http.impl.client.BasicAuthCache();
  public void put(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.auth.AuthScheme);
  public com.feilong.lib.org.apache.http.auth.AuthScheme get(com.feilong.lib.org.apache.http.HttpHost);
  public void remove(com.feilong.lib.org.apache.http.HttpHost);
  public void clear();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.client.BasicCookieStore`

```java
public class com.feilong.lib.org.apache.http.impl.client.BasicCookieStore implements com.feilong.lib.org.apache.http.client.CookieStore,java.io.Serializable {
  public com.feilong.lib.org.apache.http.impl.client.BasicCookieStore();
  public void addCookie(com.feilong.lib.org.apache.http.cookie.Cookie);
  public void addCookies(com.feilong.lib.org.apache.http.cookie.Cookie[]);
  public java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie> getCookies();
  public boolean clearExpired(java.util.Date);
  public void clear();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.client.BasicCredentialsProvider`

```java
public class com.feilong.lib.org.apache.http.impl.client.BasicCredentialsProvider implements com.feilong.lib.org.apache.http.client.CredentialsProvider {
  public com.feilong.lib.org.apache.http.impl.client.BasicCredentialsProvider();
  public void setCredentials(com.feilong.lib.org.apache.http.auth.AuthScope, com.feilong.lib.org.apache.http.auth.Credentials);
  public com.feilong.lib.org.apache.http.auth.Credentials getCredentials(com.feilong.lib.org.apache.http.auth.AuthScope);
  public void clear();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.client.BasicResponseHandler`

```java
public class com.feilong.lib.org.apache.http.impl.client.BasicResponseHandler extends com.feilong.lib.org.apache.http.impl.client.AbstractResponseHandler<java.lang.String> {
  public com.feilong.lib.org.apache.http.impl.client.BasicResponseHandler();
  public java.lang.String handleEntity(com.feilong.lib.org.apache.http.HttpEntity) throws java.io.IOException;
  public java.lang.String handleResponse(com.feilong.lib.org.apache.http.HttpResponse) throws com.feilong.lib.org.apache.http.client.HttpResponseException, java.io.IOException;
  public java.lang.Object handleEntity(com.feilong.lib.org.apache.http.HttpEntity) throws java.io.IOException;
  public java.lang.Object handleResponse(com.feilong.lib.org.apache.http.HttpResponse) throws com.feilong.lib.org.apache.http.client.HttpResponseException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.client.CloseableHttpClient`

```java
public abstract class com.feilong.lib.org.apache.http.impl.client.CloseableHttpClient implements com.feilong.lib.org.apache.http.client.HttpClient,java.io.Closeable {
  public com.feilong.lib.org.apache.http.impl.client.CloseableHttpClient();
  public com.feilong.lib.org.apache.http.client.methods.CloseableHttpResponse execute(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public com.feilong.lib.org.apache.http.client.methods.CloseableHttpResponse execute(com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public com.feilong.lib.org.apache.http.client.methods.CloseableHttpResponse execute(com.feilong.lib.org.apache.http.client.methods.HttpUriRequest) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public com.feilong.lib.org.apache.http.client.methods.CloseableHttpResponse execute(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpRequest) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public <T> T execute(com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.client.ResponseHandler<? extends T>) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public <T> T execute(com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.client.ResponseHandler<? extends T>, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public <T> T execute(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.client.ResponseHandler<? extends T>) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public <T> T execute(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.client.ResponseHandler<? extends T>, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public com.feilong.lib.org.apache.http.HttpResponse execute(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public com.feilong.lib.org.apache.http.HttpResponse execute(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpRequest) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public com.feilong.lib.org.apache.http.HttpResponse execute(com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public com.feilong.lib.org.apache.http.HttpResponse execute(com.feilong.lib.org.apache.http.client.methods.HttpUriRequest) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
}
```

## `com.feilong.lib.org.apache.http.impl.client.CookieSpecRegistries`

```java
public final class com.feilong.lib.org.apache.http.impl.client.CookieSpecRegistries {
  public static com.feilong.lib.org.apache.http.config.RegistryBuilder<com.feilong.lib.org.apache.http.cookie.CookieSpecProvider> createDefaultBuilder(com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher);
  public static com.feilong.lib.org.apache.http.config.RegistryBuilder<com.feilong.lib.org.apache.http.cookie.CookieSpecProvider> createDefaultBuilder();
  public static com.feilong.lib.org.apache.http.config.Lookup<com.feilong.lib.org.apache.http.cookie.CookieSpecProvider> createDefault();
  public static com.feilong.lib.org.apache.http.config.Lookup<com.feilong.lib.org.apache.http.cookie.CookieSpecProvider> createDefault(com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher);
}
```

## `com.feilong.lib.org.apache.http.impl.client.DefaultBackoffStrategy`

```java
public class com.feilong.lib.org.apache.http.impl.client.DefaultBackoffStrategy implements com.feilong.lib.org.apache.http.client.ConnectionBackoffStrategy {
  public com.feilong.lib.org.apache.http.impl.client.DefaultBackoffStrategy();
  public boolean shouldBackoff(java.lang.Throwable);
  public boolean shouldBackoff(com.feilong.lib.org.apache.http.HttpResponse);
}
```

## `com.feilong.lib.org.apache.http.impl.client.DefaultClientConnectionReuseStrategy`

```java
public class com.feilong.lib.org.apache.http.impl.client.DefaultClientConnectionReuseStrategy extends com.feilong.lib.org.apache.http.impl.DefaultConnectionReuseStrategy {
  public com.feilong.lib.org.apache.http.impl.client.DefaultClientConnectionReuseStrategy();
  public boolean keepAlive(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.client.DefaultConnectionKeepAliveStrategy`

```java
public class com.feilong.lib.org.apache.http.impl.client.DefaultConnectionKeepAliveStrategy implements com.feilong.lib.org.apache.http.conn.ConnectionKeepAliveStrategy {
  public com.feilong.lib.org.apache.http.impl.client.DefaultConnectionKeepAliveStrategy();
  public long getKeepAliveDuration(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.client.DefaultHttpRequestRetryHandler`

```java
public class com.feilong.lib.org.apache.http.impl.client.DefaultHttpRequestRetryHandler implements com.feilong.lib.org.apache.http.client.HttpRequestRetryHandler {
  public com.feilong.lib.org.apache.http.impl.client.DefaultHttpRequestRetryHandler(int, boolean);
  public com.feilong.lib.org.apache.http.impl.client.DefaultHttpRequestRetryHandler();
  public boolean retryRequest(java.io.IOException, int, com.feilong.lib.org.apache.http.protocol.HttpContext);
  public boolean isRequestSentRetryEnabled();
  public int getRetryCount();
}
```

## `com.feilong.lib.org.apache.http.impl.client.DefaultRedirectStrategy`

```java
public class com.feilong.lib.org.apache.http.impl.client.DefaultRedirectStrategy implements com.feilong.lib.org.apache.http.client.RedirectStrategy {
  public com.feilong.lib.org.apache.http.impl.client.DefaultRedirectStrategy();
  public com.feilong.lib.org.apache.http.impl.client.DefaultRedirectStrategy(java.lang.String[]);
  public boolean isRedirected(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.ProtocolException;
  public java.net.URI getLocationURI(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.ProtocolException;
  public com.feilong.lib.org.apache.http.client.methods.HttpUriRequest getRedirect(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.ProtocolException;
}
```

## `com.feilong.lib.org.apache.http.impl.client.DefaultServiceUnavailableRetryStrategy`

```java
public class com.feilong.lib.org.apache.http.impl.client.DefaultServiceUnavailableRetryStrategy implements com.feilong.lib.org.apache.http.client.ServiceUnavailableRetryStrategy {
  public com.feilong.lib.org.apache.http.impl.client.DefaultServiceUnavailableRetryStrategy(int, int);
  public com.feilong.lib.org.apache.http.impl.client.DefaultServiceUnavailableRetryStrategy();
  public boolean retryRequest(com.feilong.lib.org.apache.http.HttpResponse, int, com.feilong.lib.org.apache.http.protocol.HttpContext);
  public long getRetryInterval();
}
```

## `com.feilong.lib.org.apache.http.impl.client.DefaultUserTokenHandler`

```java
public class com.feilong.lib.org.apache.http.impl.client.DefaultUserTokenHandler implements com.feilong.lib.org.apache.http.client.UserTokenHandler {
  public com.feilong.lib.org.apache.http.impl.client.DefaultUserTokenHandler();
  public java.lang.Object getUserToken(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.client.FutureRequestExecutionMetrics`

```java
public final class com.feilong.lib.org.apache.http.impl.client.FutureRequestExecutionMetrics {
  public long getActiveConnectionCount();
  public long getScheduledConnectionCount();
  public long getSuccessfulConnectionCount();
  public long getSuccessfulConnectionAverageDuration();
  public long getFailedConnectionCount();
  public long getFailedConnectionAverageDuration();
  public long getRequestCount();
  public long getRequestAverageDuration();
  public long getTaskCount();
  public long getTaskAverageDuration();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.client.FutureRequestExecutionService`

```java
public class com.feilong.lib.org.apache.http.impl.client.FutureRequestExecutionService implements java.io.Closeable {
  public com.feilong.lib.org.apache.http.impl.client.FutureRequestExecutionService(com.feilong.lib.org.apache.http.client.HttpClient, java.util.concurrent.ExecutorService);
  public <T> com.feilong.lib.org.apache.http.impl.client.HttpRequestFutureTask<T> execute(com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.protocol.HttpContext, com.feilong.lib.org.apache.http.client.ResponseHandler<T>);
  public <T> com.feilong.lib.org.apache.http.impl.client.HttpRequestFutureTask<T> execute(com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.protocol.HttpContext, com.feilong.lib.org.apache.http.client.ResponseHandler<T>, com.feilong.lib.org.apache.http.concurrent.FutureCallback<T>);
  public com.feilong.lib.org.apache.http.impl.client.FutureRequestExecutionMetrics metrics();
  public void close() throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder`

```java
public class com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder {
  public static com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder create();
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setRequestExecutor(com.feilong.lib.org.apache.http.protocol.HttpRequestExecutor);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setHostnameVerifier(com.feilong.lib.org.apache.http.conn.ssl.X509HostnameVerifier);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setSSLHostnameVerifier(javax.net.ssl.HostnameVerifier);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setPublicSuffixMatcher(com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setSslcontext(javax.net.ssl.SSLContext);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setSSLContext(javax.net.ssl.SSLContext);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setSSLSocketFactory(com.feilong.lib.org.apache.http.conn.socket.LayeredConnectionSocketFactory);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setMaxConnTotal(int);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setMaxConnPerRoute(int);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setDefaultSocketConfig(com.feilong.lib.org.apache.http.config.SocketConfig);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setDefaultConnectionConfig(com.feilong.lib.org.apache.http.config.ConnectionConfig);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setConnectionTimeToLive(long, java.util.concurrent.TimeUnit);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setConnectionManager(com.feilong.lib.org.apache.http.conn.HttpClientConnectionManager);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setConnectionManagerShared(boolean);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setConnectionReuseStrategy(com.feilong.lib.org.apache.http.ConnectionReuseStrategy);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setKeepAliveStrategy(com.feilong.lib.org.apache.http.conn.ConnectionKeepAliveStrategy);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setTargetAuthenticationStrategy(com.feilong.lib.org.apache.http.client.AuthenticationStrategy);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setProxyAuthenticationStrategy(com.feilong.lib.org.apache.http.client.AuthenticationStrategy);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setUserTokenHandler(com.feilong.lib.org.apache.http.client.UserTokenHandler);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder disableConnectionState();
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setSchemePortResolver(com.feilong.lib.org.apache.http.conn.SchemePortResolver);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setUserAgent(java.lang.String);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setDefaultHeaders(java.util.Collection<? extends com.feilong.lib.org.apache.http.Header>);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder addInterceptorFirst(com.feilong.lib.org.apache.http.HttpResponseInterceptor);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder addInterceptorLast(com.feilong.lib.org.apache.http.HttpResponseInterceptor);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder addInterceptorFirst(com.feilong.lib.org.apache.http.HttpRequestInterceptor);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder addInterceptorLast(com.feilong.lib.org.apache.http.HttpRequestInterceptor);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder disableCookieManagement();
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder disableContentCompression();
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder disableAuthCaching();
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setHttpProcessor(com.feilong.lib.org.apache.http.protocol.HttpProcessor);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setDnsResolver(com.feilong.lib.org.apache.http.conn.DnsResolver);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setRetryHandler(com.feilong.lib.org.apache.http.client.HttpRequestRetryHandler);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder disableAutomaticRetries();
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setProxy(com.feilong.lib.org.apache.http.HttpHost);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setRoutePlanner(com.feilong.lib.org.apache.http.conn.routing.HttpRoutePlanner);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setRedirectStrategy(com.feilong.lib.org.apache.http.client.RedirectStrategy);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder disableRedirectHandling();
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setConnectionBackoffStrategy(com.feilong.lib.org.apache.http.client.ConnectionBackoffStrategy);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setBackoffManager(com.feilong.lib.org.apache.http.client.BackoffManager);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setServiceUnavailableRetryStrategy(com.feilong.lib.org.apache.http.client.ServiceUnavailableRetryStrategy);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setDefaultCookieStore(com.feilong.lib.org.apache.http.client.CookieStore);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setDefaultCredentialsProvider(com.feilong.lib.org.apache.http.client.CredentialsProvider);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setDefaultAuthSchemeRegistry(com.feilong.lib.org.apache.http.config.Lookup<com.feilong.lib.org.apache.http.auth.AuthSchemeProvider>);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setDefaultCookieSpecRegistry(com.feilong.lib.org.apache.http.config.Lookup<com.feilong.lib.org.apache.http.cookie.CookieSpecProvider>);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setContentDecoderRegistry(java.util.Map<java.lang.String, com.feilong.lib.org.apache.http.client.entity.InputStreamFactory>);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder setDefaultRequestConfig(com.feilong.lib.org.apache.http.client.config.RequestConfig);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder useSystemProperties();
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder evictExpiredConnections();
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder evictIdleConnections(java.lang.Long, java.util.concurrent.TimeUnit);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder evictIdleConnections(long, java.util.concurrent.TimeUnit);
  public final com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder disableDefaultUserAgent();
  public com.feilong.lib.org.apache.http.impl.client.CloseableHttpClient build();
}
```

## `com.feilong.lib.org.apache.http.impl.client.HttpClients`

```java
public class com.feilong.lib.org.apache.http.impl.client.HttpClients {
  public static com.feilong.lib.org.apache.http.impl.client.HttpClientBuilder custom();
  public static com.feilong.lib.org.apache.http.impl.client.CloseableHttpClient createDefault();
  public static com.feilong.lib.org.apache.http.impl.client.CloseableHttpClient createSystem();
  public static com.feilong.lib.org.apache.http.impl.client.CloseableHttpClient createMinimal();
  public static com.feilong.lib.org.apache.http.impl.client.CloseableHttpClient createMinimal(com.feilong.lib.org.apache.http.conn.HttpClientConnectionManager);
}
```

## `com.feilong.lib.org.apache.http.impl.client.HttpRequestFutureTask`

```java
public class com.feilong.lib.org.apache.http.impl.client.HttpRequestFutureTask<V> extends java.util.concurrent.FutureTask<V> {
  public com.feilong.lib.org.apache.http.impl.client.HttpRequestFutureTask(com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.impl.client.HttpRequestTaskCallable<V>);
  public boolean cancel(boolean);
  public long scheduledTime();
  public long startedTime();
  public long endedTime();
  public long requestDuration();
  public long taskDuration();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.client.IdleConnectionEvictor`

```java
public final class com.feilong.lib.org.apache.http.impl.client.IdleConnectionEvictor {
  public com.feilong.lib.org.apache.http.impl.client.IdleConnectionEvictor(com.feilong.lib.org.apache.http.conn.HttpClientConnectionManager, java.util.concurrent.ThreadFactory, long, java.util.concurrent.TimeUnit, long, java.util.concurrent.TimeUnit);
  public com.feilong.lib.org.apache.http.impl.client.IdleConnectionEvictor(com.feilong.lib.org.apache.http.conn.HttpClientConnectionManager, long, java.util.concurrent.TimeUnit, long, java.util.concurrent.TimeUnit);
  public com.feilong.lib.org.apache.http.impl.client.IdleConnectionEvictor(com.feilong.lib.org.apache.http.conn.HttpClientConnectionManager, long, java.util.concurrent.TimeUnit);
  public void start();
  public void shutdown();
  public boolean isRunning();
  public void awaitTermination(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
}
```

## `com.feilong.lib.org.apache.http.impl.client.LaxRedirectStrategy`

```java
public class com.feilong.lib.org.apache.http.impl.client.LaxRedirectStrategy extends com.feilong.lib.org.apache.http.impl.client.DefaultRedirectStrategy {
  public com.feilong.lib.org.apache.http.impl.client.LaxRedirectStrategy();
}
```

## `com.feilong.lib.org.apache.http.impl.client.NoopUserTokenHandler`

```java
public class com.feilong.lib.org.apache.http.impl.client.NoopUserTokenHandler implements com.feilong.lib.org.apache.http.client.UserTokenHandler {
  public com.feilong.lib.org.apache.http.impl.client.NoopUserTokenHandler();
  public java.lang.Object getUserToken(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.client.NullBackoffStrategy`

```java
public class com.feilong.lib.org.apache.http.impl.client.NullBackoffStrategy implements com.feilong.lib.org.apache.http.client.ConnectionBackoffStrategy {
  public com.feilong.lib.org.apache.http.impl.client.NullBackoffStrategy();
  public boolean shouldBackoff(java.lang.Throwable);
  public boolean shouldBackoff(com.feilong.lib.org.apache.http.HttpResponse);
}
```

## `com.feilong.lib.org.apache.http.impl.client.ProxyAuthenticationStrategy`

```java
public class com.feilong.lib.org.apache.http.impl.client.ProxyAuthenticationStrategy extends com.feilong.lib.org.apache.http.impl.client.AuthenticationStrategyImpl {
  public com.feilong.lib.org.apache.http.impl.client.ProxyAuthenticationStrategy();
  public void authFailed(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.auth.AuthScheme, com.feilong.lib.org.apache.http.protocol.HttpContext);
  public void authSucceeded(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.auth.AuthScheme, com.feilong.lib.org.apache.http.protocol.HttpContext);
  public java.util.Queue select(java.util.Map, com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.auth.MalformedChallengeException;
  public java.util.Map getChallenges(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.auth.MalformedChallengeException;
  public boolean isAuthenticationRequested(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.client.ProxyClient`

```java
public class com.feilong.lib.org.apache.http.impl.client.ProxyClient {
  public com.feilong.lib.org.apache.http.impl.client.ProxyClient(com.feilong.lib.org.apache.http.conn.HttpConnectionFactory<com.feilong.lib.org.apache.http.conn.routing.HttpRoute, com.feilong.lib.org.apache.http.conn.ManagedHttpClientConnection>, com.feilong.lib.org.apache.http.config.ConnectionConfig, com.feilong.lib.org.apache.http.client.config.RequestConfig);
  public com.feilong.lib.org.apache.http.impl.client.ProxyClient(com.feilong.lib.org.apache.http.client.config.RequestConfig);
  public com.feilong.lib.org.apache.http.impl.client.ProxyClient();
  public com.feilong.lib.org.apache.http.params.HttpParams getParams();
  public java.net.Socket tunnel(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.auth.Credentials) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.impl.client.RedirectLocations`

```java
public class com.feilong.lib.org.apache.http.impl.client.RedirectLocations extends java.util.AbstractList<java.lang.Object> {
  public com.feilong.lib.org.apache.http.impl.client.RedirectLocations();
  public boolean contains(java.net.URI);
  public void add(java.net.URI);
  public boolean remove(java.net.URI);
  public java.util.List<java.net.URI> getAll();
  public java.net.URI get(int);
  public int size();
  public java.lang.Object set(int, java.lang.Object);
  public void add(int, java.lang.Object);
  public java.net.URI remove(int);
  public boolean contains(java.lang.Object);
  public java.lang.Object remove(int);
  public java.lang.Object get(int);
}
```

## `com.feilong.lib.org.apache.http.impl.client.RequestWrapper`

```java
public class com.feilong.lib.org.apache.http.impl.client.RequestWrapper extends com.feilong.lib.org.apache.http.message.AbstractHttpMessage implements com.feilong.lib.org.apache.http.client.methods.HttpUriRequest {
  public com.feilong.lib.org.apache.http.impl.client.RequestWrapper(com.feilong.lib.org.apache.http.HttpRequest) throws com.feilong.lib.org.apache.http.ProtocolException;
  public void resetHeaders();
  public java.lang.String getMethod();
  public void setMethod(java.lang.String);
  public com.feilong.lib.org.apache.http.ProtocolVersion getProtocolVersion();
  public void setProtocolVersion(com.feilong.lib.org.apache.http.ProtocolVersion);
  public java.net.URI getURI();
  public void setURI(java.net.URI);
  public com.feilong.lib.org.apache.http.RequestLine getRequestLine();
  public void abort() throws java.lang.UnsupportedOperationException;
  public boolean isAborted();
  public com.feilong.lib.org.apache.http.HttpRequest getOriginal();
  public boolean isRepeatable();
  public int getExecCount();
  public void incrementExecCount();
}
```

## `com.feilong.lib.org.apache.http.impl.client.StandardHttpRequestRetryHandler`

```java
public class com.feilong.lib.org.apache.http.impl.client.StandardHttpRequestRetryHandler extends com.feilong.lib.org.apache.http.impl.client.DefaultHttpRequestRetryHandler {
  public com.feilong.lib.org.apache.http.impl.client.StandardHttpRequestRetryHandler(int, boolean);
  public com.feilong.lib.org.apache.http.impl.client.StandardHttpRequestRetryHandler();
}
```

## `com.feilong.lib.org.apache.http.impl.client.SystemDefaultCredentialsProvider`

```java
public class com.feilong.lib.org.apache.http.impl.client.SystemDefaultCredentialsProvider implements com.feilong.lib.org.apache.http.client.CredentialsProvider {
  public com.feilong.lib.org.apache.http.impl.client.SystemDefaultCredentialsProvider();
  public void setCredentials(com.feilong.lib.org.apache.http.auth.AuthScope, com.feilong.lib.org.apache.http.auth.Credentials);
  public com.feilong.lib.org.apache.http.auth.Credentials getCredentials(com.feilong.lib.org.apache.http.auth.AuthScope);
  public void clear();
}
```

## `com.feilong.lib.org.apache.http.impl.client.TargetAuthenticationStrategy`

```java
public class com.feilong.lib.org.apache.http.impl.client.TargetAuthenticationStrategy extends com.feilong.lib.org.apache.http.impl.client.AuthenticationStrategyImpl {
  public com.feilong.lib.org.apache.http.impl.client.TargetAuthenticationStrategy();
  public void authFailed(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.auth.AuthScheme, com.feilong.lib.org.apache.http.protocol.HttpContext);
  public void authSucceeded(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.auth.AuthScheme, com.feilong.lib.org.apache.http.protocol.HttpContext);
  public java.util.Queue select(java.util.Map, com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.auth.MalformedChallengeException;
  public java.util.Map getChallenges(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.auth.MalformedChallengeException;
  public boolean isAuthenticationRequested(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```
