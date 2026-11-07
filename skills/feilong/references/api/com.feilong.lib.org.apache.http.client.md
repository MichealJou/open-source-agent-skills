# com.feilong.lib.org.apache.http.client

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.client.AuthCache`

```java
public interface com.feilong.lib.org.apache.http.client.AuthCache {
  public abstract void put(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.auth.AuthScheme);
  public abstract com.feilong.lib.org.apache.http.auth.AuthScheme get(com.feilong.lib.org.apache.http.HttpHost);
  public abstract void remove(com.feilong.lib.org.apache.http.HttpHost);
  public abstract void clear();
}
```

## `com.feilong.lib.org.apache.http.client.AuthenticationStrategy`

```java
public interface com.feilong.lib.org.apache.http.client.AuthenticationStrategy {
  public abstract boolean isAuthenticationRequested(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext);
  public abstract java.util.Map<java.lang.String, com.feilong.lib.org.apache.http.Header> getChallenges(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.auth.MalformedChallengeException;
  public abstract java.util.Queue<com.feilong.lib.org.apache.http.auth.AuthOption> select(java.util.Map<java.lang.String, com.feilong.lib.org.apache.http.Header>, com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.auth.MalformedChallengeException;
  public abstract void authSucceeded(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.auth.AuthScheme, com.feilong.lib.org.apache.http.protocol.HttpContext);
  public abstract void authFailed(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.auth.AuthScheme, com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.client.BackoffManager`

```java
public interface com.feilong.lib.org.apache.http.client.BackoffManager {
  public abstract void backOff(com.feilong.lib.org.apache.http.conn.routing.HttpRoute);
  public abstract void probe(com.feilong.lib.org.apache.http.conn.routing.HttpRoute);
}
```

## `com.feilong.lib.org.apache.http.client.CircularRedirectException`

```java
public class com.feilong.lib.org.apache.http.client.CircularRedirectException extends com.feilong.lib.org.apache.http.client.RedirectException {
  public com.feilong.lib.org.apache.http.client.CircularRedirectException();
  public com.feilong.lib.org.apache.http.client.CircularRedirectException(java.lang.String);
  public com.feilong.lib.org.apache.http.client.CircularRedirectException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.client.ClientProtocolException`

```java
public class com.feilong.lib.org.apache.http.client.ClientProtocolException extends java.io.IOException {
  public com.feilong.lib.org.apache.http.client.ClientProtocolException();
  public com.feilong.lib.org.apache.http.client.ClientProtocolException(java.lang.String);
  public com.feilong.lib.org.apache.http.client.ClientProtocolException(java.lang.Throwable);
  public com.feilong.lib.org.apache.http.client.ClientProtocolException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.client.ConnectionBackoffStrategy`

```java
public interface com.feilong.lib.org.apache.http.client.ConnectionBackoffStrategy {
  public abstract boolean shouldBackoff(java.lang.Throwable);
  public abstract boolean shouldBackoff(com.feilong.lib.org.apache.http.HttpResponse);
}
```

## `com.feilong.lib.org.apache.http.client.CookieStore`

```java
public interface com.feilong.lib.org.apache.http.client.CookieStore {
  public abstract void addCookie(com.feilong.lib.org.apache.http.cookie.Cookie);
  public abstract java.util.List<com.feilong.lib.org.apache.http.cookie.Cookie> getCookies();
  public abstract boolean clearExpired(java.util.Date);
  public abstract void clear();
}
```

## `com.feilong.lib.org.apache.http.client.CredentialsProvider`

```java
public interface com.feilong.lib.org.apache.http.client.CredentialsProvider {
  public abstract void setCredentials(com.feilong.lib.org.apache.http.auth.AuthScope, com.feilong.lib.org.apache.http.auth.Credentials);
  public abstract com.feilong.lib.org.apache.http.auth.Credentials getCredentials(com.feilong.lib.org.apache.http.auth.AuthScope);
  public abstract void clear();
}
```

## `com.feilong.lib.org.apache.http.client.HttpClient`

```java
public interface com.feilong.lib.org.apache.http.client.HttpClient {
  public abstract com.feilong.lib.org.apache.http.HttpResponse execute(com.feilong.lib.org.apache.http.client.methods.HttpUriRequest) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public abstract com.feilong.lib.org.apache.http.HttpResponse execute(com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public abstract com.feilong.lib.org.apache.http.HttpResponse execute(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpRequest) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public abstract com.feilong.lib.org.apache.http.HttpResponse execute(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public abstract <T> T execute(com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.client.ResponseHandler<? extends T>) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public abstract <T> T execute(com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.client.ResponseHandler<? extends T>, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public abstract <T> T execute(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.client.ResponseHandler<? extends T>) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
  public abstract <T> T execute(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.client.ResponseHandler<? extends T>, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, com.feilong.lib.org.apache.http.client.ClientProtocolException;
}
```

## `com.feilong.lib.org.apache.http.client.HttpRequestRetryHandler`

```java
public interface com.feilong.lib.org.apache.http.client.HttpRequestRetryHandler {
  public abstract boolean retryRequest(java.io.IOException, int, com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.client.HttpResponseException`

```java
public class com.feilong.lib.org.apache.http.client.HttpResponseException extends com.feilong.lib.org.apache.http.client.ClientProtocolException {
  public com.feilong.lib.org.apache.http.client.HttpResponseException(int, java.lang.String);
  public int getStatusCode();
  public java.lang.String getReasonPhrase();
}
```

## `com.feilong.lib.org.apache.http.client.NonRepeatableRequestException`

```java
public class com.feilong.lib.org.apache.http.client.NonRepeatableRequestException extends com.feilong.lib.org.apache.http.ProtocolException {
  public com.feilong.lib.org.apache.http.client.NonRepeatableRequestException();
  public com.feilong.lib.org.apache.http.client.NonRepeatableRequestException(java.lang.String);
  public com.feilong.lib.org.apache.http.client.NonRepeatableRequestException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.client.RedirectException`

```java
public class com.feilong.lib.org.apache.http.client.RedirectException extends com.feilong.lib.org.apache.http.ProtocolException {
  public com.feilong.lib.org.apache.http.client.RedirectException();
  public com.feilong.lib.org.apache.http.client.RedirectException(java.lang.String);
  public com.feilong.lib.org.apache.http.client.RedirectException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.client.RedirectStrategy`

```java
public interface com.feilong.lib.org.apache.http.client.RedirectStrategy {
  public abstract boolean isRedirected(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.ProtocolException;
  public abstract com.feilong.lib.org.apache.http.client.methods.HttpUriRequest getRedirect(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.ProtocolException;
}
```

## `com.feilong.lib.org.apache.http.client.ResponseHandler`

```java
public interface com.feilong.lib.org.apache.http.client.ResponseHandler<T> {
  public abstract T handleResponse(com.feilong.lib.org.apache.http.HttpResponse) throws com.feilong.lib.org.apache.http.client.ClientProtocolException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.client.ServiceUnavailableRetryStrategy`

```java
public interface com.feilong.lib.org.apache.http.client.ServiceUnavailableRetryStrategy {
  public abstract boolean retryRequest(com.feilong.lib.org.apache.http.HttpResponse, int, com.feilong.lib.org.apache.http.protocol.HttpContext);
  public abstract long getRetryInterval();
}
```

## `com.feilong.lib.org.apache.http.client.UserTokenHandler`

```java
public interface com.feilong.lib.org.apache.http.client.UserTokenHandler {
  public abstract java.lang.Object getUserToken(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```
