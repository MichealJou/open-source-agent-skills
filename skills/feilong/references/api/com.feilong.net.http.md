# com.feilong.net.http

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.net.http.ConnectionConfig`

```java
public final class com.feilong.net.http.ConnectionConfig {
  public com.feilong.net.http.ConnectionConfig();
  public com.feilong.net.http.ConnectionConfig(java.lang.String, java.lang.String);
  public com.feilong.net.http.ConnectionConfig(int);
  public com.feilong.net.http.ConnectionConfig(int, int);
  public com.feilong.net.http.ConnectionConfig(boolean);
  public int getConnectTimeout();
  public void setConnectTimeout(int);
  public int getReadTimeout();
  public void setReadTimeout(int);
  public java.lang.String getContentCharset();
  public void setContentCharset(java.lang.String);
  public java.lang.String getProxyAddress();
  public void setProxyAddress(java.lang.String);
  public java.lang.Integer getProxyPort();
  public void setProxyPort(java.lang.Integer);
  public java.lang.String getUserName();
  public void setUserName(java.lang.String);
  public java.lang.String getPassword();
  public void setPassword(java.lang.String);
  public boolean getTurnOffHostnameVerifier();
  public void setTurnOffHostnameVerifier(boolean);
  public int getMaxConnPerRoute();
  public void setMaxConnPerRoute(int);
  public int getMaxConnTotal();
  public void setMaxConnTotal(int);
  public boolean getIsTimeoutRetry();
  public int getTimeoutRetryCount();
  public void setIsTimeoutRetry(boolean);
  public void setTimeoutRetryCount(int);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.feilong.net.http.HttpClientUtil`

```java
public final class com.feilong.net.http.HttpClientUtil {
  public static int getResponseStatusCode(java.lang.String);
  public static int getResponseStatusCode(java.lang.String, com.feilong.net.http.ConnectionConfig);
  public static int getResponseStatusCode(com.feilong.net.http.HttpRequest, com.feilong.net.http.ConnectionConfig);
  public static com.feilong.net.http.HttpResponse getHttpResponse(java.lang.String);
  public static com.feilong.net.http.HttpResponse getHttpResponse(java.lang.String, com.feilong.net.http.ConnectionConfig);
  public static com.feilong.net.http.HttpResponse getHttpResponse(com.feilong.net.http.HttpRequest, com.feilong.net.http.ConnectionConfig);
  public static <T> com.feilong.net.http.HttpFullInfo<T> getHttpFullInfo(com.feilong.net.http.HttpRequest, com.feilong.net.http.ConnectionConfig, com.feilong.net.http.callback.ResultBeanConverter<T>);
  public static com.feilong.net.http.HttpResponse getHttpResponse(com.feilong.net.http.HttpRequest);
  public static java.lang.String get(java.lang.String);
  public static java.lang.String get(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String get(java.lang.String, java.util.Map<java.lang.String, java.lang.String>);
  public static java.lang.String get(java.lang.String, java.util.Map<java.lang.String, java.lang.String>, java.util.Map<java.lang.String, java.lang.String>);
  public static java.lang.String put(java.lang.String);
  public static java.lang.String put(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String put(java.lang.String, java.util.Map<java.lang.String, java.lang.String>);
  public static java.lang.String put(java.lang.String, java.util.Map<java.lang.String, java.lang.String>, java.util.Map<java.lang.String, java.lang.String>);
  public static java.lang.String post(java.lang.String);
  public static java.lang.String post(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String post(java.lang.String, java.util.Map<java.lang.String, java.lang.String>);
  public static java.lang.String post(java.lang.String, java.util.Map<java.lang.String, java.lang.String>, java.util.Map<java.lang.String, java.lang.String>);
  public static java.lang.String post(java.lang.String, java.lang.String);
  public static java.lang.String post(java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.lang.String>);
  public static java.lang.String patch(java.lang.String, java.lang.String);
  public static java.lang.String patch(java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.lang.String>);
  public static java.lang.String getResponseBodyAsString(com.feilong.net.http.HttpRequest);
  public static java.lang.String getResponseBodyAsString(java.lang.String, java.util.Map<java.lang.String, java.lang.String>, java.lang.String);
  public static java.lang.String getResponseBodyAsString(java.lang.String, java.util.Map<java.lang.String, java.lang.String>, com.feilong.net.http.HttpMethodType);
  public static java.lang.String getResponseBodyAsString(java.lang.String, com.feilong.net.http.ConnectionConfig);
  public static java.lang.String getResponseBodyAsString(com.feilong.net.http.HttpRequest, com.feilong.net.http.ConnectionConfig);
}
```

## `com.feilong.net.http.HttpFullInfo`

```java
public class com.feilong.net.http.HttpFullInfo<T> implements java.io.Serializable {
  public com.feilong.net.http.HttpFullInfo();
  public com.feilong.net.http.HttpFullInfo(com.feilong.net.http.HttpRequest, com.feilong.net.http.ConnectionConfig);
  public com.feilong.net.http.HttpRequest getHttpRequest();
  public void setHttpRequest(com.feilong.net.http.HttpRequest);
  public com.feilong.net.http.ConnectionConfig getConnectionConfig();
  public void setConnectionConfig(com.feilong.net.http.ConnectionConfig);
  public com.feilong.net.http.HttpResponse getHttpResponse();
  public void setHttpResponse(com.feilong.net.http.HttpResponse);
  public com.feilong.net.UncheckedHttpException getUncheckedHttpException();
  public void setUncheckedHttpException(com.feilong.net.UncheckedHttpException);
  public T getResultBean();
  public void setResultBean(T);
}
```

## `com.feilong.net.http.HttpLogHelper`

```java
public class com.feilong.net.http.HttpLogHelper {
  public com.feilong.net.http.HttpLogHelper();
  public static java.lang.String autoLog(com.feilong.net.http.HttpRequest, java.lang.String, java.lang.Object...);
  public static java.lang.String autoLog(com.feilong.net.http.HttpRequest, com.feilong.net.http.ConnectionConfig, java.lang.String, java.lang.Object...);
  public static java.lang.String autoLog(com.feilong.net.http.HttpRequest, com.feilong.net.http.HttpResponse, com.feilong.net.http.ConnectionConfig, java.lang.String, java.lang.Object...);
}
```

## `com.feilong.net.http.HttpMethodType`

```java
public final class com.feilong.net.http.HttpMethodType extends java.lang.Enum<com.feilong.net.http.HttpMethodType> {
  public static com.feilong.net.http.HttpMethodType[] values();
  public static com.feilong.net.http.HttpMethodType valueOf(java.lang.String);
  public java.lang.String getMethod();
  public static com.feilong.net.http.HttpMethodType getByMethodValueIgnoreCase(java.lang.String);
}
```

## `com.feilong.net.http.HttpRequest`

```java
public class com.feilong.net.http.HttpRequest {
  public com.feilong.net.http.HttpRequest();
  public com.feilong.net.http.HttpRequest(java.lang.String);
  public com.feilong.net.http.HttpRequest(java.lang.String, com.feilong.net.http.HttpMethodType);
  public com.feilong.net.http.HttpRequest(java.lang.String, java.util.Map<java.lang.String, java.lang.String>, com.feilong.net.http.HttpMethodType);
  public com.feilong.net.http.HttpRequest(java.lang.String, java.util.Map<java.lang.String, java.lang.String>, java.lang.String);
  public java.lang.String getFullEncodedUrl();
  public java.lang.String getUri();
  public void setUri(java.lang.String);
  public com.feilong.net.http.HttpMethodType getHttpMethodType();
  public void setHttpMethodType(com.feilong.net.http.HttpMethodType);
  public java.util.Map<java.lang.String, java.lang.String> getParamMap();
  public void setParamMap(java.util.Map<java.lang.String, java.lang.String>);
  public java.util.Map<java.lang.String, java.lang.String> getHeaderMap();
  public void setHeaderMap(java.util.Map<java.lang.String, java.lang.String>);
  public java.lang.String getRequestBody();
  public void setRequestBody(java.lang.String);
  public void setIsTrimUri(boolean);
  public boolean getIsTrimUri();
  public com.feilong.net.http.RequestByteArrayBody getRequestByteArrayBody();
  public void setRequestByteArrayBody(com.feilong.net.http.RequestByteArrayBody);
  public java.lang.String getLogTraceContext();
  public void setLogTraceContext(java.lang.String);
  public java.lang.String toString();
}
```

## `com.feilong.net.http.HttpResponse`

```java
public class com.feilong.net.http.HttpResponse implements java.io.Serializable {
  public com.feilong.net.http.HttpResponse();
  public long getUseTime();
  public void setUseTime(long);
  public int getStatusCode();
  public void setStatusCode(int);
  public java.lang.String getResultString();
  public void setResultString(java.lang.String);
  public java.util.Map<java.lang.String, java.lang.String> getHeaderMap();
  public void setHeaderMap(java.util.Map<java.lang.String, java.lang.String>);
  public java.lang.String toString();
}
```

## `com.feilong.net.http.RequestByteArrayBody`

```java
public class com.feilong.net.http.RequestByteArrayBody {
  public com.feilong.net.http.RequestByteArrayBody(byte[]);
  public com.feilong.net.http.RequestByteArrayBody(byte[], java.lang.Integer, java.lang.Integer, com.feilong.io.entity.MimeType);
  public com.feilong.net.http.RequestByteArrayBody(byte[], java.lang.Integer, java.lang.Integer, java.lang.String);
  public com.feilong.net.http.RequestByteArrayBody(byte[], com.feilong.io.entity.MimeType);
  public com.feilong.net.http.RequestByteArrayBody(byte[], java.lang.String);
  public byte[] getBuf();
  public void setBuf(byte[]);
  public java.lang.Integer getOff();
  public void setOff(java.lang.Integer);
  public java.lang.Integer getLength();
  public void setLength(java.lang.Integer);
  public java.lang.String getMimeType();
  public void setMimeType(java.lang.String);
}
```
