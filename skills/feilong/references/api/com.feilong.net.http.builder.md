# com.feilong.net.http.builder

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.net.http.builder.HttpClientBuilder`

```java
public class com.feilong.net.http.builder.HttpClientBuilder {
  public static com.feilong.lib.org.apache.http.client.HttpClient build(java.lang.String, com.feilong.net.http.ConnectionConfig);
}
```

## `com.feilong.net.http.builder.HttpRequestExecuter`

```java
public final class com.feilong.net.http.builder.HttpRequestExecuter {
  public static <T> T execute(com.feilong.net.http.HttpRequest, com.feilong.net.http.ConnectionConfig, com.feilong.net.http.callback.ResultCallback<T>);
}
```

## `com.feilong.net.http.builder.HttpResponseUtil`

```java
public final class com.feilong.net.http.builder.HttpResponseUtil {
  public static java.lang.String getResultString(com.feilong.lib.org.apache.http.HttpResponse);
}
```

## `com.feilong.net.http.builder.HttpUriRequestBuilder`

```java
public final class com.feilong.net.http.builder.HttpUriRequestBuilder {
  public static com.feilong.lib.org.apache.http.client.methods.HttpUriRequest build(com.feilong.net.http.HttpRequest, com.feilong.net.http.ConnectionConfig);
}
```

## `com.feilong.net.http.builder.RequestConfigBuilder`

```java
public final class com.feilong.net.http.builder.RequestConfigBuilder {
  public static com.feilong.lib.org.apache.http.client.config.RequestConfig build(com.feilong.net.http.ConnectionConfig);
}
```

## `com.feilong.net.http.builder.SpecialHttpRequestRetryHandler`

```java
public class com.feilong.net.http.builder.SpecialHttpRequestRetryHandler extends com.feilong.lib.org.apache.http.impl.client.DefaultHttpRequestRetryHandler {
  public com.feilong.net.http.builder.SpecialHttpRequestRetryHandler(java.lang.String, int);
  public boolean retryRequest(java.io.IOException, int, com.feilong.lib.org.apache.http.protocol.HttpContext);
  public void setLogTraceContext(java.lang.String);
}
```
