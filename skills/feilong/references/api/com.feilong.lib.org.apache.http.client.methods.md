# com.feilong.lib.org.apache.http.client.methods

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.client.methods.AbstractExecutionAwareRequest`

```java
public abstract class com.feilong.lib.org.apache.http.client.methods.AbstractExecutionAwareRequest extends com.feilong.lib.org.apache.http.message.AbstractHttpMessage implements com.feilong.lib.org.apache.http.client.methods.HttpExecutionAware,java.lang.Cloneable,com.feilong.lib.org.apache.http.HttpRequest {
  public void abort();
  public boolean isAborted();
  public void setCancellable(com.feilong.lib.org.apache.http.concurrent.Cancellable);
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
  public void reset();
}
```

## `com.feilong.lib.org.apache.http.client.methods.Configurable`

```java
public interface com.feilong.lib.org.apache.http.client.methods.Configurable {
  public abstract com.feilong.lib.org.apache.http.client.config.RequestConfig getConfig();
}
```

## `com.feilong.lib.org.apache.http.client.methods.HttpDelete`

```java
public class com.feilong.lib.org.apache.http.client.methods.HttpDelete extends com.feilong.lib.org.apache.http.client.methods.HttpRequestBase {
  public com.feilong.lib.org.apache.http.client.methods.HttpDelete();
  public com.feilong.lib.org.apache.http.client.methods.HttpDelete(java.net.URI);
  public com.feilong.lib.org.apache.http.client.methods.HttpDelete(java.lang.String);
  public java.lang.String getMethod();
}
```

## `com.feilong.lib.org.apache.http.client.methods.HttpEntityEnclosingRequestBase`

```java
public abstract class com.feilong.lib.org.apache.http.client.methods.HttpEntityEnclosingRequestBase extends com.feilong.lib.org.apache.http.client.methods.HttpRequestBase implements com.feilong.lib.org.apache.http.HttpEntityEnclosingRequest {
  public com.feilong.lib.org.apache.http.client.methods.HttpEntityEnclosingRequestBase();
  public com.feilong.lib.org.apache.http.HttpEntity getEntity();
  public void setEntity(com.feilong.lib.org.apache.http.HttpEntity);
  public boolean expectContinue();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.client.methods.HttpExecutionAware`

```java
public interface com.feilong.lib.org.apache.http.client.methods.HttpExecutionAware {
  public abstract boolean isAborted();
  public abstract void setCancellable(com.feilong.lib.org.apache.http.concurrent.Cancellable);
}
```

## `com.feilong.lib.org.apache.http.client.methods.HttpGet`

```java
public class com.feilong.lib.org.apache.http.client.methods.HttpGet extends com.feilong.lib.org.apache.http.client.methods.HttpRequestBase {
  public com.feilong.lib.org.apache.http.client.methods.HttpGet();
  public com.feilong.lib.org.apache.http.client.methods.HttpGet(java.net.URI);
  public com.feilong.lib.org.apache.http.client.methods.HttpGet(java.lang.String);
  public java.lang.String getMethod();
}
```

## `com.feilong.lib.org.apache.http.client.methods.HttpHead`

```java
public class com.feilong.lib.org.apache.http.client.methods.HttpHead extends com.feilong.lib.org.apache.http.client.methods.HttpRequestBase {
  public com.feilong.lib.org.apache.http.client.methods.HttpHead();
  public com.feilong.lib.org.apache.http.client.methods.HttpHead(java.net.URI);
  public com.feilong.lib.org.apache.http.client.methods.HttpHead(java.lang.String);
  public java.lang.String getMethod();
}
```

## `com.feilong.lib.org.apache.http.client.methods.HttpOptions`

```java
public class com.feilong.lib.org.apache.http.client.methods.HttpOptions extends com.feilong.lib.org.apache.http.client.methods.HttpRequestBase {
  public com.feilong.lib.org.apache.http.client.methods.HttpOptions();
  public com.feilong.lib.org.apache.http.client.methods.HttpOptions(java.net.URI);
  public com.feilong.lib.org.apache.http.client.methods.HttpOptions(java.lang.String);
  public java.lang.String getMethod();
  public java.util.Set<java.lang.String> getAllowedMethods(com.feilong.lib.org.apache.http.HttpResponse);
}
```

## `com.feilong.lib.org.apache.http.client.methods.HttpPatch`

```java
public class com.feilong.lib.org.apache.http.client.methods.HttpPatch extends com.feilong.lib.org.apache.http.client.methods.HttpEntityEnclosingRequestBase {
  public com.feilong.lib.org.apache.http.client.methods.HttpPatch();
  public com.feilong.lib.org.apache.http.client.methods.HttpPatch(java.net.URI);
  public com.feilong.lib.org.apache.http.client.methods.HttpPatch(java.lang.String);
  public java.lang.String getMethod();
}
```

## `com.feilong.lib.org.apache.http.client.methods.HttpPost`

```java
public class com.feilong.lib.org.apache.http.client.methods.HttpPost extends com.feilong.lib.org.apache.http.client.methods.HttpEntityEnclosingRequestBase {
  public com.feilong.lib.org.apache.http.client.methods.HttpPost();
  public com.feilong.lib.org.apache.http.client.methods.HttpPost(java.net.URI);
  public com.feilong.lib.org.apache.http.client.methods.HttpPost(java.lang.String);
  public java.lang.String getMethod();
}
```

## `com.feilong.lib.org.apache.http.client.methods.HttpPut`

```java
public class com.feilong.lib.org.apache.http.client.methods.HttpPut extends com.feilong.lib.org.apache.http.client.methods.HttpEntityEnclosingRequestBase {
  public com.feilong.lib.org.apache.http.client.methods.HttpPut();
  public com.feilong.lib.org.apache.http.client.methods.HttpPut(java.net.URI);
  public com.feilong.lib.org.apache.http.client.methods.HttpPut(java.lang.String);
  public java.lang.String getMethod();
}
```

## `com.feilong.lib.org.apache.http.client.methods.HttpRequestBase`

```java
public abstract class com.feilong.lib.org.apache.http.client.methods.HttpRequestBase extends com.feilong.lib.org.apache.http.client.methods.AbstractExecutionAwareRequest implements com.feilong.lib.org.apache.http.client.methods.HttpUriRequest,com.feilong.lib.org.apache.http.client.methods.Configurable {
  public com.feilong.lib.org.apache.http.client.methods.HttpRequestBase();
  public abstract java.lang.String getMethod();
  public void setProtocolVersion(com.feilong.lib.org.apache.http.ProtocolVersion);
  public com.feilong.lib.org.apache.http.ProtocolVersion getProtocolVersion();
  public java.net.URI getURI();
  public com.feilong.lib.org.apache.http.RequestLine getRequestLine();
  public com.feilong.lib.org.apache.http.client.config.RequestConfig getConfig();
  public void setConfig(com.feilong.lib.org.apache.http.client.config.RequestConfig);
  public void setURI(java.net.URI);
  public void started();
  public void releaseConnection();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.client.methods.HttpRequestWrapper`

```java
public class com.feilong.lib.org.apache.http.client.methods.HttpRequestWrapper extends com.feilong.lib.org.apache.http.message.AbstractHttpMessage implements com.feilong.lib.org.apache.http.client.methods.HttpUriRequest {
  public com.feilong.lib.org.apache.http.ProtocolVersion getProtocolVersion();
  public void setProtocolVersion(com.feilong.lib.org.apache.http.ProtocolVersion);
  public java.net.URI getURI();
  public void setURI(java.net.URI);
  public java.lang.String getMethod();
  public void abort() throws java.lang.UnsupportedOperationException;
  public boolean isAborted();
  public com.feilong.lib.org.apache.http.RequestLine getRequestLine();
  public com.feilong.lib.org.apache.http.HttpRequest getOriginal();
  public com.feilong.lib.org.apache.http.HttpHost getTarget();
  public java.lang.String toString();
  public static com.feilong.lib.org.apache.http.client.methods.HttpRequestWrapper wrap(com.feilong.lib.org.apache.http.HttpRequest);
  public static com.feilong.lib.org.apache.http.client.methods.HttpRequestWrapper wrap(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.HttpHost);
}
```

## `com.feilong.lib.org.apache.http.client.methods.HttpTrace`

```java
public class com.feilong.lib.org.apache.http.client.methods.HttpTrace extends com.feilong.lib.org.apache.http.client.methods.HttpRequestBase {
  public com.feilong.lib.org.apache.http.client.methods.HttpTrace();
  public com.feilong.lib.org.apache.http.client.methods.HttpTrace(java.net.URI);
  public com.feilong.lib.org.apache.http.client.methods.HttpTrace(java.lang.String);
  public java.lang.String getMethod();
}
```

## `com.feilong.lib.org.apache.http.client.methods.HttpUriRequest`

```java
public interface com.feilong.lib.org.apache.http.client.methods.HttpUriRequest extends com.feilong.lib.org.apache.http.HttpRequest {
  public abstract java.lang.String getMethod();
  public abstract java.net.URI getURI();
  public abstract void abort() throws java.lang.UnsupportedOperationException;
  public abstract boolean isAborted();
}
```

## `com.feilong.lib.org.apache.http.client.methods.RequestBuilder`

```java
public class com.feilong.lib.org.apache.http.client.methods.RequestBuilder {
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder create(java.lang.String);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder get();
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder get(java.net.URI);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder get(java.lang.String);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder head();
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder head(java.net.URI);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder head(java.lang.String);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder patch();
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder patch(java.net.URI);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder patch(java.lang.String);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder post();
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder post(java.net.URI);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder post(java.lang.String);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder put();
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder put(java.net.URI);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder put(java.lang.String);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder delete();
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder delete(java.net.URI);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder delete(java.lang.String);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder trace();
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder trace(java.net.URI);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder trace(java.lang.String);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder options();
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder options(java.net.URI);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder options(java.lang.String);
  public static com.feilong.lib.org.apache.http.client.methods.RequestBuilder copy(com.feilong.lib.org.apache.http.HttpRequest);
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder setCharset(java.nio.charset.Charset);
  public java.nio.charset.Charset getCharset();
  public java.lang.String getMethod();
  public com.feilong.lib.org.apache.http.ProtocolVersion getVersion();
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder setVersion(com.feilong.lib.org.apache.http.ProtocolVersion);
  public java.net.URI getUri();
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder setUri(java.net.URI);
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder setUri(java.lang.String);
  public com.feilong.lib.org.apache.http.Header getFirstHeader(java.lang.String);
  public com.feilong.lib.org.apache.http.Header getLastHeader(java.lang.String);
  public com.feilong.lib.org.apache.http.Header[] getHeaders(java.lang.String);
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder addHeader(com.feilong.lib.org.apache.http.Header);
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder addHeader(java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder removeHeader(com.feilong.lib.org.apache.http.Header);
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder removeHeaders(java.lang.String);
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder setHeader(com.feilong.lib.org.apache.http.Header);
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder setHeader(java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.HttpEntity getEntity();
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder setEntity(com.feilong.lib.org.apache.http.HttpEntity);
  public java.util.List<com.feilong.lib.org.apache.http.NameValuePair> getParameters();
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder addParameter(com.feilong.lib.org.apache.http.NameValuePair);
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder addParameter(java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder addParameters(com.feilong.lib.org.apache.http.NameValuePair...);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig getConfig();
  public com.feilong.lib.org.apache.http.client.methods.RequestBuilder setConfig(com.feilong.lib.org.apache.http.client.config.RequestConfig);
  public com.feilong.lib.org.apache.http.client.methods.HttpUriRequest build();
  public java.lang.String toString();
}
```
