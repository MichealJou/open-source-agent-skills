# com.feilong.context.invoker.http

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.context.invoker.http.ConnectionConfigBuilder`

```java
public interface com.feilong.context.invoker.http.ConnectionConfigBuilder<T> {
  public abstract com.feilong.net.http.ConnectionConfig build(T);
}
```

## `com.feilong.context.invoker.http.DefaultHttpRequestBuilder`

```java
public class com.feilong.context.invoker.http.DefaultHttpRequestBuilder<T> implements com.feilong.context.invoker.http.HttpRequestBuilder<T> {
  public com.feilong.context.invoker.http.DefaultHttpRequestBuilder();
  public com.feilong.net.http.HttpRequest build(T);
  public void setHttpTypeBeanProperty(com.feilong.context.beanproperty.HttpTypeBeanProperty);
  public void setRequestParamsBuilder(com.feilong.context.invoker.RequestParamsBuilder<T>);
  public void setRequestHeaderBuilder(com.feilong.context.invoker.http.RequestHeaderBuilder<T>);
  public void setRequestBodyBuilder(com.feilong.context.invoker.http.RequestBodyBuilder<T>);
  public void setHttpRequestRebuilder(com.feilong.context.Rebuilder<com.feilong.net.http.HttpRequest>);
}
```

## `com.feilong.context.invoker.http.HttpRequestBuilder`

```java
public interface com.feilong.context.invoker.http.HttpRequestBuilder<T> {
  public abstract com.feilong.net.http.HttpRequest build(T);
}
```

## `com.feilong.context.invoker.http.HttpResponseStringBuilder`

```java
public class com.feilong.context.invoker.http.HttpResponseStringBuilder<T> extends com.feilong.context.invoker.AbstractResponseStringBuilder<T> {
  public com.feilong.context.invoker.http.HttpResponseStringBuilder();
  public void setHttpRequestBuilder(com.feilong.context.invoker.http.HttpRequestBuilder<T>);
  public void setConnectionConfigBuilder(com.feilong.context.invoker.http.ConnectionConfigBuilder<T>);
}
```

## `com.feilong.context.invoker.http.RequestBodyBuilder`

```java
public interface com.feilong.context.invoker.http.RequestBodyBuilder<T> {
  public abstract java.lang.String build(T);
}
```

## `com.feilong.context.invoker.http.RequestHeaderBuilder`

```java
public interface com.feilong.context.invoker.http.RequestHeaderBuilder<T> {
  public abstract java.util.Map<java.lang.String, java.lang.String> build(T);
}
```

## `com.feilong.context.invoker.http.SimpleJsonRequestBodyBuilder`

```java
public class com.feilong.context.invoker.http.SimpleJsonRequestBodyBuilder<T> implements com.feilong.context.invoker.http.RequestBodyBuilder<T> {
  public com.feilong.context.invoker.http.SimpleJsonRequestBodyBuilder();
  public java.lang.String build(T);
  public com.feilong.json.JavaToJsonConfig getJavaToJsonConfig();
  public void setJavaToJsonConfig(com.feilong.json.JavaToJsonConfig);
}
```

## `com.feilong.context.invoker.http.SimpleMapRequestHeaderBuilder`

```java
public class com.feilong.context.invoker.http.SimpleMapRequestHeaderBuilder<T> implements com.feilong.context.invoker.http.RequestHeaderBuilder<T> {
  public com.feilong.context.invoker.http.SimpleMapRequestHeaderBuilder();
  public com.feilong.context.invoker.http.SimpleMapRequestHeaderBuilder(java.util.Map<java.lang.String, java.lang.String>);
  public java.util.Map<java.lang.String, java.lang.String> build(T);
  public java.util.Map<java.lang.String, java.lang.String> getHeaderMap();
  public void setHeaderMap(java.util.Map<java.lang.String, java.lang.String>);
}
```
