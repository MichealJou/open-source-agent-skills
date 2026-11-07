# com.feilong.context.log

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.context.log.AbstractFixedContextLogCreator`

```java
public abstract class com.feilong.context.log.AbstractFixedContextLogCreator implements com.feilong.context.log.FixedContextLogCreator {
  public com.feilong.context.log.AbstractFixedContextLogCreator();
}
```

## `com.feilong.context.log.AutoLog`

```java
public class com.feilong.context.log.AutoLog {
  public com.feilong.context.log.AutoLog();
  public static java.lang.String autoLog(java.lang.String, java.lang.Object...);
}
```

## `com.feilong.context.log.ContextLogCreator`

```java
public class com.feilong.context.log.ContextLogCreator {
  public com.feilong.context.log.ContextLogCreator();
  public static java.lang.String getContextLog();
}
```

## `com.feilong.context.log.FixedContextLogCreator`

```java
public interface com.feilong.context.log.FixedContextLogCreator {
  public abstract java.lang.String createContextLog();
}
```

## `com.feilong.context.log.HttpSpringFixedContextLogCreator`

```java
public class com.feilong.context.log.HttpSpringFixedContextLogCreator extends com.feilong.context.log.AbstractFixedContextLogCreator {
  public com.feilong.context.log.HttpSpringFixedContextLogCreator();
  public java.lang.String createContextLog();
}
```

## `com.feilong.context.log.LogContextExecutor`

```java
public class com.feilong.context.log.LogContextExecutor {
  public com.feilong.context.log.LogContextExecutor();
  public static void run(java.lang.String, java.lang.Runnable);
  public static <T> T call(java.lang.String, java.util.concurrent.Callable<T>);
  public static <T> T call(java.lang.String, java.util.concurrent.Callable<T>, com.feilong.context.log.ThrowableCallback);
}
```

## `com.feilong.context.log.LogCounterThreadLocal`

```java
public class com.feilong.context.log.LogCounterThreadLocal {
  public com.feilong.context.log.LogCounterThreadLocal();
  public static void beginCounter();
  public static void setCounter(java.util.concurrent.atomic.AtomicInteger);
  public static java.util.concurrent.atomic.AtomicInteger getCounter();
  public static void removeCounter();
}
```

## `com.feilong.context.log.LogKeyThreadLocal`

```java
public class com.feilong.context.log.LogKeyThreadLocal {
  public com.feilong.context.log.LogKeyThreadLocal();
  public static void setLogKey(java.lang.String);
  public static void appendLogKey(java.lang.String);
  public static java.lang.String getLogKey();
  public static void removeLogKey();
}
```

## `com.feilong.context.log.MqInfo`

```java
public class com.feilong.context.log.MqInfo {
  public com.feilong.context.log.MqInfo();
  public java.lang.String getMqType();
  public void setMqType(java.lang.String);
  public java.lang.String getMqQueueOrConsumer();
  public void setMqQueueOrConsumer(java.lang.String);
  public java.lang.String getMqContent();
  public void setMqContent(java.lang.String);
  public java.lang.String getReceiverApplication();
  public void setReceiverApplication(java.lang.String);
  public java.lang.String toString();
}
```

## `com.feilong.context.log.MqInfoThreadLocal`

```java
public class com.feilong.context.log.MqInfoThreadLocal {
  public com.feilong.context.log.MqInfoThreadLocal();
  public static void setMqInfo(com.feilong.context.log.MqInfo);
  public static com.feilong.context.log.MqInfo getMqInfo();
  public static void removeMqInfo();
}
```

## `com.feilong.context.log.RequestLogHelper`

```java
public final class com.feilong.context.log.RequestLogHelper {
  public com.feilong.context.log.RequestLogHelper();
  public static java.lang.String autoRequestInfo(java.lang.String, java.lang.Object...);
  public static java.lang.String autoRequestInfo(javax.servlet.http.HttpServletRequest, java.lang.String, java.lang.Object...);
}
```

## `com.feilong.context.log.ThrowableCallback`

```java
public interface com.feilong.context.log.ThrowableCallback {
  public abstract void callback(java.lang.Throwable);
}
```
