# com.feilong.lib.org.apache.http.protocol

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.protocol.BasicHttpContext`

```java
public class com.feilong.lib.org.apache.http.protocol.BasicHttpContext implements com.feilong.lib.org.apache.http.protocol.HttpContext {
  public com.feilong.lib.org.apache.http.protocol.BasicHttpContext();
  public com.feilong.lib.org.apache.http.protocol.BasicHttpContext(com.feilong.lib.org.apache.http.protocol.HttpContext);
  public java.lang.Object getAttribute(java.lang.String);
  public void setAttribute(java.lang.String, java.lang.Object);
  public java.lang.Object removeAttribute(java.lang.String);
  public void clear();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.protocol.HTTP`

```java
public final class com.feilong.lib.org.apache.http.protocol.HTTP {
  public static boolean isWhitespace(char);
}
```

## `com.feilong.lib.org.apache.http.protocol.HttpContext`

```java
public interface com.feilong.lib.org.apache.http.protocol.HttpContext {
  public abstract java.lang.Object getAttribute(java.lang.String);
  public abstract void setAttribute(java.lang.String, java.lang.Object);
  public abstract java.lang.Object removeAttribute(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.protocol.HttpCoreContext`

```java
public class com.feilong.lib.org.apache.http.protocol.HttpCoreContext implements com.feilong.lib.org.apache.http.protocol.HttpContext {
  public static com.feilong.lib.org.apache.http.protocol.HttpCoreContext create();
  public static com.feilong.lib.org.apache.http.protocol.HttpCoreContext adapt(com.feilong.lib.org.apache.http.protocol.HttpContext);
  public com.feilong.lib.org.apache.http.protocol.HttpCoreContext(com.feilong.lib.org.apache.http.protocol.HttpContext);
  public com.feilong.lib.org.apache.http.protocol.HttpCoreContext();
  public java.lang.Object getAttribute(java.lang.String);
  public void setAttribute(java.lang.String, java.lang.Object);
  public java.lang.Object removeAttribute(java.lang.String);
  public <T> T getAttribute(java.lang.String, java.lang.Class<T>);
  public <T extends com.feilong.lib.org.apache.http.HttpConnection> T getConnection(java.lang.Class<T>);
  public com.feilong.lib.org.apache.http.HttpConnection getConnection();
  public com.feilong.lib.org.apache.http.HttpRequest getRequest();
  public boolean isRequestSent();
  public com.feilong.lib.org.apache.http.HttpResponse getResponse();
  public void setTargetHost(com.feilong.lib.org.apache.http.HttpHost);
  public com.feilong.lib.org.apache.http.HttpHost getTargetHost();
}
```

## `com.feilong.lib.org.apache.http.protocol.HttpDateGenerator`

```java
public class com.feilong.lib.org.apache.http.protocol.HttpDateGenerator {
  public com.feilong.lib.org.apache.http.protocol.HttpDateGenerator();
  public synchronized java.lang.String getCurrentDate();
}
```

## `com.feilong.lib.org.apache.http.protocol.HttpExpectationVerifier`

```java
public interface com.feilong.lib.org.apache.http.protocol.HttpExpectationVerifier {
  public abstract void verify(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder`

```java
public class com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder {
  public static com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder create();
  public com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder addFirst(com.feilong.lib.org.apache.http.HttpRequestInterceptor);
  public com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder addLast(com.feilong.lib.org.apache.http.HttpRequestInterceptor);
  public com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder add(com.feilong.lib.org.apache.http.HttpRequestInterceptor);
  public com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder addAllFirst(com.feilong.lib.org.apache.http.HttpRequestInterceptor...);
  public com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder addAllLast(com.feilong.lib.org.apache.http.HttpRequestInterceptor...);
  public com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder addAll(com.feilong.lib.org.apache.http.HttpRequestInterceptor...);
  public com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder addFirst(com.feilong.lib.org.apache.http.HttpResponseInterceptor);
  public com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder addLast(com.feilong.lib.org.apache.http.HttpResponseInterceptor);
  public com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder add(com.feilong.lib.org.apache.http.HttpResponseInterceptor);
  public com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder addAllFirst(com.feilong.lib.org.apache.http.HttpResponseInterceptor...);
  public com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder addAllLast(com.feilong.lib.org.apache.http.HttpResponseInterceptor...);
  public com.feilong.lib.org.apache.http.protocol.HttpProcessorBuilder addAll(com.feilong.lib.org.apache.http.HttpResponseInterceptor...);
  public com.feilong.lib.org.apache.http.protocol.HttpProcessor build();
}
```

## `com.feilong.lib.org.apache.http.protocol.HttpRequestExecutor`

```java
public class com.feilong.lib.org.apache.http.protocol.HttpRequestExecutor {
  public com.feilong.lib.org.apache.http.protocol.HttpRequestExecutor(int);
  public com.feilong.lib.org.apache.http.protocol.HttpRequestExecutor();
  public com.feilong.lib.org.apache.http.HttpResponse execute(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.HttpClientConnection, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
  public void preProcess(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpProcessor, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
  public void postProcess(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpProcessor, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.protocol.HttpRequestHandler`

```java
public interface com.feilong.lib.org.apache.http.protocol.HttpRequestHandler {
  public abstract void handle(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.protocol.HttpRequestHandlerMapper`

```java
public interface com.feilong.lib.org.apache.http.protocol.HttpRequestHandlerMapper {
  public abstract com.feilong.lib.org.apache.http.protocol.HttpRequestHandler lookup(com.feilong.lib.org.apache.http.HttpRequest);
}
```

## `com.feilong.lib.org.apache.http.protocol.HttpService`

```java
public class com.feilong.lib.org.apache.http.protocol.HttpService {
  public com.feilong.lib.org.apache.http.protocol.HttpService(com.feilong.lib.org.apache.http.protocol.HttpProcessor, com.feilong.lib.org.apache.http.ConnectionReuseStrategy, com.feilong.lib.org.apache.http.HttpResponseFactory, com.feilong.lib.org.apache.http.protocol.HttpRequestHandlerMapper, com.feilong.lib.org.apache.http.protocol.HttpExpectationVerifier);
  public com.feilong.lib.org.apache.http.protocol.HttpService(com.feilong.lib.org.apache.http.protocol.HttpProcessor, com.feilong.lib.org.apache.http.ConnectionReuseStrategy, com.feilong.lib.org.apache.http.HttpResponseFactory, com.feilong.lib.org.apache.http.protocol.HttpRequestHandlerMapper);
  public com.feilong.lib.org.apache.http.protocol.HttpService(com.feilong.lib.org.apache.http.protocol.HttpProcessor, com.feilong.lib.org.apache.http.protocol.HttpRequestHandlerMapper);
  public void handleRequest(com.feilong.lib.org.apache.http.HttpServerConnection, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.protocol.ImmutableHttpProcessor`

```java
public final class com.feilong.lib.org.apache.http.protocol.ImmutableHttpProcessor implements com.feilong.lib.org.apache.http.protocol.HttpProcessor {
  public com.feilong.lib.org.apache.http.protocol.ImmutableHttpProcessor(com.feilong.lib.org.apache.http.HttpRequestInterceptor[], com.feilong.lib.org.apache.http.HttpResponseInterceptor[]);
  public com.feilong.lib.org.apache.http.protocol.ImmutableHttpProcessor(java.util.List<com.feilong.lib.org.apache.http.HttpRequestInterceptor>, java.util.List<com.feilong.lib.org.apache.http.HttpResponseInterceptor>);
  public com.feilong.lib.org.apache.http.protocol.ImmutableHttpProcessor(com.feilong.lib.org.apache.http.HttpRequestInterceptor...);
  public com.feilong.lib.org.apache.http.protocol.ImmutableHttpProcessor(com.feilong.lib.org.apache.http.HttpResponseInterceptor...);
  public void process(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
  public void process(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.protocol.RequestConnControl`

```java
public class com.feilong.lib.org.apache.http.protocol.RequestConnControl implements com.feilong.lib.org.apache.http.HttpRequestInterceptor {
  public com.feilong.lib.org.apache.http.protocol.RequestConnControl();
  public void process(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.protocol.RequestContent`

```java
public class com.feilong.lib.org.apache.http.protocol.RequestContent implements com.feilong.lib.org.apache.http.HttpRequestInterceptor {
  public com.feilong.lib.org.apache.http.protocol.RequestContent();
  public com.feilong.lib.org.apache.http.protocol.RequestContent(boolean);
  public void process(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.protocol.RequestDate`

```java
public class com.feilong.lib.org.apache.http.protocol.RequestDate implements com.feilong.lib.org.apache.http.HttpRequestInterceptor {
  public com.feilong.lib.org.apache.http.protocol.RequestDate();
  public void process(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.protocol.RequestExpectContinue`

```java
public class com.feilong.lib.org.apache.http.protocol.RequestExpectContinue implements com.feilong.lib.org.apache.http.HttpRequestInterceptor {
  public com.feilong.lib.org.apache.http.protocol.RequestExpectContinue(boolean);
  public void process(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.protocol.RequestTargetHost`

```java
public class com.feilong.lib.org.apache.http.protocol.RequestTargetHost implements com.feilong.lib.org.apache.http.HttpRequestInterceptor {
  public com.feilong.lib.org.apache.http.protocol.RequestTargetHost();
  public void process(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.protocol.RequestUserAgent`

```java
public class com.feilong.lib.org.apache.http.protocol.RequestUserAgent implements com.feilong.lib.org.apache.http.HttpRequestInterceptor {
  public com.feilong.lib.org.apache.http.protocol.RequestUserAgent(java.lang.String);
  public com.feilong.lib.org.apache.http.protocol.RequestUserAgent();
  public void process(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.protocol.ResponseConnControl`

```java
public class com.feilong.lib.org.apache.http.protocol.ResponseConnControl implements com.feilong.lib.org.apache.http.HttpResponseInterceptor {
  public com.feilong.lib.org.apache.http.protocol.ResponseConnControl();
  public void process(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.protocol.ResponseContent`

```java
public class com.feilong.lib.org.apache.http.protocol.ResponseContent implements com.feilong.lib.org.apache.http.HttpResponseInterceptor {
  public com.feilong.lib.org.apache.http.protocol.ResponseContent();
  public com.feilong.lib.org.apache.http.protocol.ResponseContent(boolean);
  public void process(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.protocol.ResponseDate`

```java
public class com.feilong.lib.org.apache.http.protocol.ResponseDate implements com.feilong.lib.org.apache.http.HttpResponseInterceptor {
  public com.feilong.lib.org.apache.http.protocol.ResponseDate();
  public void process(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.protocol.ResponseServer`

```java
public class com.feilong.lib.org.apache.http.protocol.ResponseServer implements com.feilong.lib.org.apache.http.HttpResponseInterceptor {
  public com.feilong.lib.org.apache.http.protocol.ResponseServer(java.lang.String);
  public com.feilong.lib.org.apache.http.protocol.ResponseServer();
  public void process(com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.protocol.UriHttpRequestHandlerMapper`

```java
public class com.feilong.lib.org.apache.http.protocol.UriHttpRequestHandlerMapper implements com.feilong.lib.org.apache.http.protocol.HttpRequestHandlerMapper {
  public com.feilong.lib.org.apache.http.protocol.UriHttpRequestHandlerMapper();
  public void register(java.lang.String, com.feilong.lib.org.apache.http.protocol.HttpRequestHandler);
  public void unregister(java.lang.String);
  public com.feilong.lib.org.apache.http.protocol.HttpRequestHandler lookup(com.feilong.lib.org.apache.http.HttpRequest);
}
```

## `com.feilong.lib.org.apache.http.protocol.UriPatternMatcher`

```java
public class com.feilong.lib.org.apache.http.protocol.UriPatternMatcher<T> {
  public com.feilong.lib.org.apache.http.protocol.UriPatternMatcher();
  public synchronized java.util.Set<java.util.Map$Entry<java.lang.String, T>> entrySet();
  public synchronized void register(java.lang.String, T);
  public synchronized void unregister(java.lang.String);
  public synchronized void setHandlers(java.util.Map<java.lang.String, T>);
  public synchronized void setObjects(java.util.Map<java.lang.String, T>);
  public synchronized java.util.Map<java.lang.String, T> getObjects();
  public synchronized T lookup(java.lang.String);
  public java.lang.String toString();
}
```
