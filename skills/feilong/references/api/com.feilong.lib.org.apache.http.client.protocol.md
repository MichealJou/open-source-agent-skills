# com.feilong.lib.org.apache.http.client.protocol

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.client.protocol.HttpClientContext`

```java
public class com.feilong.lib.org.apache.http.client.protocol.HttpClientContext extends com.feilong.lib.org.apache.http.protocol.HttpCoreContext {
  public static com.feilong.lib.org.apache.http.client.protocol.HttpClientContext adapt(com.feilong.lib.org.apache.http.protocol.HttpContext);
  public static com.feilong.lib.org.apache.http.client.protocol.HttpClientContext create();
  public com.feilong.lib.org.apache.http.client.protocol.HttpClientContext(com.feilong.lib.org.apache.http.protocol.HttpContext);
  public com.feilong.lib.org.apache.http.client.protocol.HttpClientContext();
  public com.feilong.lib.org.apache.http.conn.routing.RouteInfo getHttpRoute();
  public java.util.List<java.net.URI> getRedirectLocations();
  public com.feilong.lib.org.apache.http.client.CookieStore getCookieStore();
  public void setCookieStore(com.feilong.lib.org.apache.http.client.CookieStore);
  public com.feilong.lib.org.apache.http.cookie.CookieSpec getCookieSpec();
  public com.feilong.lib.org.apache.http.cookie.CookieOrigin getCookieOrigin();
  public com.feilong.lib.org.apache.http.config.Lookup<com.feilong.lib.org.apache.http.cookie.CookieSpecProvider> getCookieSpecRegistry();
  public void setCookieSpecRegistry(com.feilong.lib.org.apache.http.config.Lookup<com.feilong.lib.org.apache.http.cookie.CookieSpecProvider>);
  public com.feilong.lib.org.apache.http.config.Lookup<com.feilong.lib.org.apache.http.auth.AuthSchemeProvider> getAuthSchemeRegistry();
  public void setAuthSchemeRegistry(com.feilong.lib.org.apache.http.config.Lookup<com.feilong.lib.org.apache.http.auth.AuthSchemeProvider>);
  public com.feilong.lib.org.apache.http.client.CredentialsProvider getCredentialsProvider();
  public void setCredentialsProvider(com.feilong.lib.org.apache.http.client.CredentialsProvider);
  public com.feilong.lib.org.apache.http.client.AuthCache getAuthCache();
  public void setAuthCache(com.feilong.lib.org.apache.http.client.AuthCache);
  public com.feilong.lib.org.apache.http.auth.AuthState getTargetAuthState();
  public com.feilong.lib.org.apache.http.auth.AuthState getProxyAuthState();
  public <T> T getUserToken(java.lang.Class<T>);
  public java.lang.Object getUserToken();
  public void setUserToken(java.lang.Object);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig getRequestConfig();
  public void setRequestConfig(com.feilong.lib.org.apache.http.client.config.RequestConfig);
}
```

## `com.feilong.lib.org.apache.http.client.protocol.RequestAcceptEncoding`

```java
public class com.feilong.lib.org.apache.http.client.protocol.RequestAcceptEncoding implements com.feilong.lib.org.apache.http.HttpRequestInterceptor {
  public com.feilong.lib.org.apache.http.client.protocol.RequestAcceptEncoding(java.util.List<java.lang.String>);
  public com.feilong.lib.org.apache.http.client.protocol.RequestAcceptEncoding();
  public void process(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.client.protocol.RequestAddCookies`

```java
public class com.feilong.lib.org.apache.http.client.protocol.RequestAddCookies implements com.feilong.lib.org.apache.http.HttpRequestInterceptor {
  public com.feilong.lib.org.apache.http.client.protocol.RequestAddCookies();
  public void process(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.client.protocol.RequestAuthCache`

```java
public class com.feilong.lib.org.apache.http.client.protocol.RequestAuthCache implements com.feilong.lib.org.apache.http.HttpRequestInterceptor {
  public com.feilong.lib.org.apache.http.client.protocol.RequestAuthCache();
  public void process(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.client.protocol.RequestClientConnControl`

```java
public class com.feilong.lib.org.apache.http.client.protocol.RequestClientConnControl implements com.feilong.lib.org.apache.http.HttpRequestInterceptor {
  public com.feilong.lib.org.apache.http.client.protocol.RequestClientConnControl();
  public void process(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.client.protocol.RequestDefaultHeaders`

```java
public class com.feilong.lib.org.apache.http.client.protocol.RequestDefaultHeaders implements com.feilong.lib.org.apache.http.HttpRequestInterceptor {
  public com.feilong.lib.org.apache.http.client.protocol.RequestDefaultHeaders(java.util.Collection<? extends com.feilong.lib.org.apache.http.Header>);
  public com.feilong.lib.org.apache.http.client.protocol.RequestDefaultHeaders();
  public void process(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.client.protocol.RequestExpectContinue`

```java
public class com.feilong.lib.org.apache.http.client.protocol.RequestExpectContinue implements com.feilong.lib.org.apache.http.HttpRequestInterceptor {
  public com.feilong.lib.org.apache.http.client.protocol.RequestExpectContinue();
  public void process(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.client.protocol.ResponseContentEncoding`

```java
public class com.feilong.lib.org.apache.http.client.protocol.ResponseContentEncoding implements com.feilong.lib.org.apache.http.HttpResponseInterceptor {
  public com.feilong.lib.org.apache.http.client.protocol.ResponseContentEncoding(com.feilong.lib.org.apache.http.config.Lookup<com.feilong.lib.org.apache.http.client.entity.InputStreamFactory>, boolean);
  public com.feilong.lib.org.apache.http.client.protocol.ResponseContentEncoding(boolean);
  public com.feilong.lib.org.apache.http.client.protocol.ResponseContentEncoding(com.feilong.lib.org.apache.http.config.Lookup<com.feilong.lib.org.apache.http.client.entity.InputStreamFactory>);
  public com.feilong.lib.org.apache.http.client.protocol.ResponseContentEncoding();
  public void process(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.client.protocol.ResponseProcessCookies`

```java
public class com.feilong.lib.org.apache.http.client.protocol.ResponseProcessCookies implements com.feilong.lib.org.apache.http.HttpResponseInterceptor {
  public com.feilong.lib.org.apache.http.client.protocol.ResponseProcessCookies();
  public void process(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```
