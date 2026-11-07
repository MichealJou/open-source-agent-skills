# com.feilong.net.http.callback

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.net.http.callback.AbstractResultCallback`

```java
public abstract class com.feilong.net.http.callback.AbstractResultCallback<T> implements com.feilong.net.http.callback.ResultCallback<T> {
  public com.feilong.net.http.callback.AbstractResultCallback();
  public T doException(com.feilong.net.http.HttpRequest, com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.net.http.ConnectionConfig, com.feilong.net.UncheckedHttpException, java.util.Date);
}
```

## `com.feilong.net.http.callback.HttpFullInfoResultCallback`

```java
public class com.feilong.net.http.callback.HttpFullInfoResultCallback<T> extends com.feilong.net.http.callback.AbstractResultCallback<com.feilong.net.http.HttpFullInfo<T>> {
  public com.feilong.net.http.callback.HttpFullInfoResultCallback(com.feilong.net.http.callback.ResultBeanConverter<T>);
  public com.feilong.net.http.HttpFullInfo<T> on(com.feilong.net.http.HttpRequest, com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.net.http.ConnectionConfig, java.util.Date);
  public com.feilong.net.http.HttpFullInfo<T> doException(com.feilong.net.http.HttpRequest, com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.net.http.ConnectionConfig, com.feilong.net.UncheckedHttpException, java.util.Date);
  public com.feilong.net.http.callback.ResultBeanConverter<T> getResultBeanConverter();
  public void setResultBeanConverter(com.feilong.net.http.callback.ResultBeanConverter<T>);
  public java.lang.Object doException(com.feilong.net.http.HttpRequest, com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.net.http.ConnectionConfig, com.feilong.net.UncheckedHttpException, java.util.Date);
  public java.lang.Object on(com.feilong.net.http.HttpRequest, com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.net.http.ConnectionConfig, java.util.Date);
}
```

## `com.feilong.net.http.callback.HttpResponseResultCallback`

```java
public class com.feilong.net.http.callback.HttpResponseResultCallback extends com.feilong.net.http.callback.AbstractResultCallback<com.feilong.net.http.HttpResponse> {
  public com.feilong.net.http.callback.HttpResponseResultCallback();
  public com.feilong.net.http.HttpResponse on(com.feilong.net.http.HttpRequest, com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.net.http.ConnectionConfig, java.util.Date);
  public java.lang.Object on(com.feilong.net.http.HttpRequest, com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.net.http.ConnectionConfig, java.util.Date);
}
```

## `com.feilong.net.http.callback.ResponseBodyAsStringResultCallback`

```java
public class com.feilong.net.http.callback.ResponseBodyAsStringResultCallback extends com.feilong.net.http.callback.AbstractResultCallback<java.lang.String> {
  public com.feilong.net.http.callback.ResponseBodyAsStringResultCallback();
  public java.lang.String on(com.feilong.net.http.HttpRequest, com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.net.http.ConnectionConfig, java.util.Date);
  public java.lang.Object on(com.feilong.net.http.HttpRequest, com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.net.http.ConnectionConfig, java.util.Date);
}
```

## `com.feilong.net.http.callback.ResultBeanConverter`

```java
public interface com.feilong.net.http.callback.ResultBeanConverter<T> {
  public abstract T convert(com.feilong.net.http.HttpRequest, com.feilong.net.http.ConnectionConfig, com.feilong.net.http.HttpResponse);
}
```

## `com.feilong.net.http.callback.ResultCallback`

```java
public interface com.feilong.net.http.callback.ResultCallback<T> {
  public abstract T on(com.feilong.net.http.HttpRequest, com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.net.http.ConnectionConfig, java.util.Date);
  public abstract T doException(com.feilong.net.http.HttpRequest, com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.net.http.ConnectionConfig, com.feilong.net.UncheckedHttpException, java.util.Date);
}
```

## `com.feilong.net.http.callback.StatusCodeResultCallback`

```java
public class com.feilong.net.http.callback.StatusCodeResultCallback extends com.feilong.net.http.callback.AbstractResultCallback<java.lang.Integer> {
  public com.feilong.net.http.callback.StatusCodeResultCallback();
  public java.lang.Integer on(com.feilong.net.http.HttpRequest, com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.net.http.ConnectionConfig, java.util.Date);
  public java.lang.Object on(com.feilong.net.http.HttpRequest, com.feilong.lib.org.apache.http.client.methods.HttpUriRequest, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.net.http.ConnectionConfig, java.util.Date);
}
```
