# com.feilong.context

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.context.AbstractDataListTask`

```java
public abstract class com.feilong.context.AbstractDataListTask<T extends com.feilong.context.Data> implements com.feilong.context.Task<java.lang.Void> {
  public com.feilong.context.AbstractDataListTask();
  public java.lang.Void run();
  public void setDataListQuery(com.feilong.context.DataListQuery<T>);
  public java.lang.Object run();
}
```

## `com.feilong.context.BeanLogMessageBuilder`

```java
public final class com.feilong.context.BeanLogMessageBuilder {
  public static java.lang.String buildFieldsMessage(java.lang.Object);
  public static java.lang.String buildFieldsSimpleMessage(java.lang.Object);
}
```

## `com.feilong.context.Condition`

```java
public interface com.feilong.context.Condition {
  public abstract boolean canRun();
}
```

## `com.feilong.context.ConditionableTask`

```java
public class com.feilong.context.ConditionableTask<T> implements com.feilong.context.Task<T>, com.feilong.context.log.UseTimeLogable {
  public com.feilong.context.ConditionableTask();
  public T run();
  public void setCondition(com.feilong.context.Condition);
  public void setTask(com.feilong.context.Task<T>);
}
```

## `com.feilong.context.DataHandler`

```java
public interface com.feilong.context.DataHandler {
  public abstract void handle(java.util.Map<java.lang.String, java.lang.Object>);
}
```

## `com.feilong.context.DataListQuery`

```java
public interface com.feilong.context.DataListQuery<T extends com.feilong.context.Data> {
  public abstract java.util.List<T> query();
}
```

## `com.feilong.context.FileReworker`

```java
public interface com.feilong.context.FileReworker {
  public abstract java.lang.String rework(java.lang.String);
}
```

## `com.feilong.context.MapBuilder`

```java
public interface com.feilong.context.MapBuilder<T> {
  public abstract java.util.Map<java.lang.String, java.lang.Object> build(T);
}
```

## `com.feilong.context.MemberIdBuilder`

```java
public interface com.feilong.context.MemberIdBuilder<T> {
  public abstract T build(javax.servlet.http.HttpServletRequest);
}
```

## `com.feilong.context.ObjectValidator`

```java
public interface com.feilong.context.ObjectValidator<T> {
  public abstract void validate(T);
}
```

## `com.feilong.context.Rebuilder`

```java
public interface com.feilong.context.Rebuilder<T> {
  public abstract T rebuild(T);
}
```

## `com.feilong.context.RequestDataBuilder`

```java
public interface com.feilong.context.RequestDataBuilder {
  public abstract java.util.Map<java.lang.String, java.lang.Object> build(javax.servlet.http.HttpServletRequest);
}
```

## `com.feilong.context.ReturnResult`

```java
public class com.feilong.context.ReturnResult<T> implements java.io.Serializable {
  public com.feilong.context.ReturnResult();
  public com.feilong.context.ReturnResult(boolean, java.lang.String);
  public com.feilong.context.ReturnResult(boolean, T);
  public com.feilong.context.ReturnResult(boolean, java.lang.String, T);
  public java.lang.String getStatusCode();
  public void setStatusCode(java.lang.String);
  public T getReturnData();
  public void setReturnData(T);
  public boolean getIsSuccess();
  public void setIsSuccess(boolean);
}
```

## `com.feilong.context.ReturnResultBuilder`

```java
public final class com.feilong.context.ReturnResultBuilder {
  public static com.feilong.context.ReturnResult<java.lang.Object> buildFailureResult(java.lang.String);
}
```

## `com.feilong.context.SimpleParamNameConfigCondition`

```java
public class com.feilong.context.SimpleParamNameConfigCondition implements com.feilong.context.Condition {
  public com.feilong.context.SimpleParamNameConfigCondition();
  public boolean canRun();
  public void setSimpleParamNameValueLoader(com.feilong.context.SimpleParamNameValueLoader<java.lang.Boolean>);
}
```

## `com.feilong.context.SimpleParamNameValueLoader`

```java
public class com.feilong.context.SimpleParamNameValueLoader<V> implements com.feilong.context.ValueLoader<V> {
  public com.feilong.context.SimpleParamNameValueLoader();
  public V load();
  public void setParamName(java.lang.String);
  public void setTargetTypeClass(java.lang.Class<V>);
  public void setIfNullDefaultValue(V);
  public void setStringValueParamLoader(com.feilong.context.StringValueParamLoader<V>);
}
```

## `com.feilong.context.SimpleValueLoader`

```java
public class com.feilong.context.SimpleValueLoader<V> implements com.feilong.context.ValueLoader<V> {
  public com.feilong.context.SimpleValueLoader();
  public com.feilong.context.SimpleValueLoader(V);
  public V load();
  public void setV(V);
}
```

## `com.feilong.context.Task`

```java
public interface com.feilong.context.Task<T> {
  public abstract T run();
}
```

## `com.feilong.context.ValidatorHandler`

```java
public interface com.feilong.context.ValidatorHandler<T> {
  public abstract com.feilong.context.ValidatorHandlerResult validate(T);
}
```

## `com.feilong.context.ValidatorHandlerResult`

```java
public final class com.feilong.context.ValidatorHandlerResult extends java.lang.Enum<com.feilong.context.ValidatorHandlerResult> {
  public static com.feilong.context.ValidatorHandlerResult[] values();
  public static com.feilong.context.ValidatorHandlerResult valueOf(java.lang.String);
}
```

## `com.feilong.context.ValueLoader`

```java
public interface com.feilong.context.ValueLoader<V> {
  public abstract V load();
}
```

## `com.feilong.context.ValueParamLoader`

```java
public interface com.feilong.context.ValueParamLoader<T, V> {
  public abstract V load(T);
}
```
