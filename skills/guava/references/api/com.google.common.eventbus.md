# com.google.common.eventbus

版本：33.4.8-jre。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.google.common.eventbus.AsyncEventBus`

```java
public class com.google.common.eventbus.AsyncEventBus extends com.google.common.eventbus.EventBus {
  public com.google.common.eventbus.AsyncEventBus(java.lang.String, java.util.concurrent.Executor);
  public com.google.common.eventbus.AsyncEventBus(java.util.concurrent.Executor, com.google.common.eventbus.SubscriberExceptionHandler);
  public com.google.common.eventbus.AsyncEventBus(java.util.concurrent.Executor);
}
```

## `com.google.common.eventbus.DeadEvent`

```java
public class com.google.common.eventbus.DeadEvent {
  public com.google.common.eventbus.DeadEvent(java.lang.Object, java.lang.Object);
  public java.lang.Object getSource();
  public java.lang.Object getEvent();
  public java.lang.String toString();
}
```

## `com.google.common.eventbus.EventBus`

```java
public class com.google.common.eventbus.EventBus {
  public com.google.common.eventbus.EventBus();
  public com.google.common.eventbus.EventBus(java.lang.String);
  public com.google.common.eventbus.EventBus(com.google.common.eventbus.SubscriberExceptionHandler);
  public final java.lang.String identifier();
  public void register(java.lang.Object);
  public void unregister(java.lang.Object);
  public void post(java.lang.Object);
  public java.lang.String toString();
}
```

## `com.google.common.eventbus.SubscriberExceptionContext`

```java
public class com.google.common.eventbus.SubscriberExceptionContext {
  public com.google.common.eventbus.EventBus getEventBus();
  public java.lang.Object getEvent();
  public java.lang.Object getSubscriber();
  public java.lang.reflect.Method getSubscriberMethod();
}
```

## `com.google.common.eventbus.SubscriberExceptionHandler`

```java
public interface com.google.common.eventbus.SubscriberExceptionHandler {
  public abstract void handleException(java.lang.Throwable, com.google.common.eventbus.SubscriberExceptionContext);
}
```
