# com.feilong.context.invoker

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.context.invoker.AbstractResponseCommandBuilder`

```java
public abstract class com.feilong.context.invoker.AbstractResponseCommandBuilder<R extends com.feilong.context.invoker.InvokerRequest, T> implements com.feilong.context.invoker.ResponseCommandBuilder<R, T> {
  public com.feilong.context.invoker.AbstractResponseCommandBuilder();
  public T build(R);
}
```

## `com.feilong.context.invoker.AbstractResponseStringBuilder`

```java
public abstract class com.feilong.context.invoker.AbstractResponseStringBuilder<T> implements com.feilong.context.invoker.ResponseStringBuilder<T> {
  public com.feilong.context.invoker.AbstractResponseStringBuilder();
  public java.lang.String build(T);
  public void setStringFormatter(com.feilong.context.format.StringFormatter);
  public void setResponseStringRebuilder(com.feilong.context.Rebuilder<java.lang.String>);
  public void setFormat(java.lang.String);
}
```

## `com.feilong.context.invoker.DataAndInvokerResultHandler`

```java
public interface com.feilong.context.invoker.DataAndInvokerResultHandler<D extends com.feilong.context.Data, I extends com.feilong.context.invoker.InvokerResult> {
  public abstract void handle(D, I);
}
```

## `com.feilong.context.invoker.DefaultRequestResultInvoker`

```java
public class com.feilong.context.invoker.DefaultRequestResultInvoker<T extends com.feilong.context.invoker.ResponseCommand, R extends com.feilong.context.invoker.InvokerRequest, N extends com.feilong.context.invoker.InvokerResult> implements com.feilong.context.invoker.RequestResultInvoker<R, N>, com.feilong.context.InputParamsValidateable {
  public com.feilong.context.invoker.DefaultRequestResultInvoker();
  public N invoke(R);
  public N doHandler(R);
  public void setInvokerRequestValidator(com.feilong.context.invoker.InvokerRequestValidator<R>);
  public void setResponseStringBuilder(com.feilong.context.invoker.ResponseStringBuilder<R>);
  public void setStringToBeanConverter(com.feilong.context.converter.StringToBeanConverter<T>);
  public void setInvokerResultConverter(com.feilong.context.invoker.InvokerResultConverter<R, T, N>);
}
```

## `com.feilong.context.invoker.DefaultResponseCommandBuilder`

```java
public class com.feilong.context.invoker.DefaultResponseCommandBuilder<R extends com.feilong.context.invoker.InvokerRequest, T> extends com.feilong.context.invoker.AbstractResponseCommandBuilder<R, T> {
  public com.feilong.context.invoker.DefaultResponseCommandBuilder();
  public void setResponseStringBuilder(com.feilong.context.invoker.ResponseStringBuilder<R>);
  public void setStringToBeanConverter(com.feilong.context.converter.StringToBeanConverter<T>);
}
```

## `com.feilong.context.invoker.DefaultResponseHandler`

```java
public class com.feilong.context.invoker.DefaultResponseHandler<R extends com.feilong.context.invoker.InvokerRequest> implements com.feilong.context.invoker.ResponseHandler<R> {
  public com.feilong.context.invoker.DefaultResponseHandler();
  public void handle(R);
  public void setResponseStringBuilder(com.feilong.context.invoker.ResponseStringBuilder<R>);
  public void setResponseStringHandler(com.feilong.context.invoker.ResponseStringHandler<R>);
}
```

## `com.feilong.context.invoker.InvokerRequestValidator`

```java
public interface com.feilong.context.invoker.InvokerRequestValidator<T extends com.feilong.context.invoker.InvokerRequest> {
  public abstract void validate(T);
}
```

## `com.feilong.context.invoker.InvokerResponseBlankException`

```java
public class com.feilong.context.invoker.InvokerResponseBlankException extends com.feilong.core.DefaultRuntimeException {
  public com.feilong.context.invoker.InvokerResponseBlankException(java.lang.String, java.lang.Object...);
}
```

## `com.feilong.context.invoker.InvokerResultConverter`

```java
public interface com.feilong.context.invoker.InvokerResultConverter<R extends com.feilong.context.invoker.InvokerRequest, T extends com.feilong.context.invoker.ResponseCommand, N extends com.feilong.context.invoker.InvokerResult> {
  public abstract N convert(R, java.lang.String, T);
}
```

## `com.feilong.context.invoker.RequestArrayParamsBuilder`

```java
public interface com.feilong.context.invoker.RequestArrayParamsBuilder<T> {
  public abstract java.lang.Object[] build(T);
}
```

## `com.feilong.context.invoker.RequestParamsBuilder`

```java
public interface com.feilong.context.invoker.RequestParamsBuilder<T> {
  public abstract java.util.Map<java.lang.String, java.lang.String> build(T);
}
```

## `com.feilong.context.invoker.RequestResultInvoker`

```java
public interface com.feilong.context.invoker.RequestResultInvoker<T extends com.feilong.context.invoker.InvokerRequest, K extends com.feilong.context.invoker.InvokerResult> {
  public abstract K invoke(T);
}
```

## `com.feilong.context.invoker.ResponseCommandBuilder`

```java
public interface com.feilong.context.invoker.ResponseCommandBuilder<R extends com.feilong.context.invoker.InvokerRequest, T> {
  public abstract T build(R);
}
```

## `com.feilong.context.invoker.ResponseHandler`

```java
public interface com.feilong.context.invoker.ResponseHandler<R extends com.feilong.context.invoker.InvokerRequest> {
  public abstract void handle(R);
}
```

## `com.feilong.context.invoker.ResponseStringBuilder`

```java
public interface com.feilong.context.invoker.ResponseStringBuilder<T> {
  public abstract java.lang.String build(T);
}
```

## `com.feilong.context.invoker.ResponseStringHandler`

```java
public interface com.feilong.context.invoker.ResponseStringHandler<R extends com.feilong.context.invoker.InvokerRequest> {
  public abstract void handle(java.lang.String, R);
}
```

## `com.feilong.context.invoker.SimpleHttpAndJsonResponseCommandBuilder`

```java
public class com.feilong.context.invoker.SimpleHttpAndJsonResponseCommandBuilder<R extends com.feilong.context.invoker.InvokerRequest, T> extends com.feilong.context.invoker.AbstractResponseCommandBuilder<R, T> {
  public com.feilong.context.invoker.SimpleHttpAndJsonResponseCommandBuilder();
  public com.feilong.context.invoker.SimpleHttpAndJsonResponseCommandBuilder(java.lang.String);
  public com.feilong.context.invoker.SimpleHttpAndJsonResponseCommandBuilder(java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.lang.String>);
  public com.feilong.context.invoker.SimpleHttpAndJsonResponseCommandBuilder(java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.lang.String>, java.lang.Class<T>);
  public void setUri(java.lang.String);
  public void setMethod(java.lang.String);
  public void setHeaderMap(java.util.Map<java.lang.String, java.lang.String>);
  public void setRequestParamsBuilder(com.feilong.context.invoker.RequestParamsBuilder<R>);
  public void setRequestBodyBuilder(com.feilong.context.invoker.http.RequestBodyBuilder<R>);
  public void setResponseCommandRootClass(java.lang.Class<T>);
}
```
