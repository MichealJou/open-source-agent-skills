# com.feilong.core.lang.thread

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.core.lang.thread.AbstractPartitionThreadExecutor`

```java
public abstract class com.feilong.core.lang.thread.AbstractPartitionThreadExecutor implements com.feilong.core.lang.thread.PartitionThreadExecutor {
  public com.feilong.core.lang.thread.AbstractPartitionThreadExecutor();
  public <T> void execute(java.util.List<T>, int, com.feilong.core.lang.thread.PartitionRunnableBuilder<T>);
  public <T> void execute(java.util.List<T>, int, java.util.Map<java.lang.String, ?>, com.feilong.core.lang.thread.PartitionRunnableBuilder<T>);
}
```

## `com.feilong.core.lang.thread.DefaultPartitionPerHandler`

```java
public class com.feilong.core.lang.thread.DefaultPartitionPerHandler<T> implements com.feilong.core.lang.thread.PartitionPerHandler<T> {
  public com.feilong.core.lang.thread.DefaultPartitionPerHandler(com.feilong.core.lang.thread.PartitionPerElementHandler<T>);
  public void handle(java.util.List<T>, com.feilong.core.lang.thread.PartitionThreadEntity, java.util.Map<java.lang.String, ?>);
}
```

## `com.feilong.core.lang.thread.DefaultPartitionRunnableBuilder`

```java
public class com.feilong.core.lang.thread.DefaultPartitionRunnableBuilder<T> implements com.feilong.core.lang.thread.PartitionRunnableBuilder<T> {
  public com.feilong.core.lang.thread.DefaultPartitionRunnableBuilder(com.feilong.core.lang.thread.PartitionPerHandler<T>);
  public java.lang.Runnable build(java.util.List<T>, com.feilong.core.lang.thread.PartitionThreadEntity, java.util.Map<java.lang.String, ?>);
}
```

## `com.feilong.core.lang.thread.DefaultPartitionThreadExecutor`

```java
public class com.feilong.core.lang.thread.DefaultPartitionThreadExecutor extends com.feilong.core.lang.thread.AbstractPartitionThreadExecutor {
  public com.feilong.core.lang.thread.DefaultPartitionThreadExecutor();
}
```

## `com.feilong.core.lang.thread.PartitionEachSizeBuilder`

```java
public interface com.feilong.core.lang.thread.PartitionEachSizeBuilder {
  public abstract int build(int);
}
```

## `com.feilong.core.lang.thread.PartitionEachSizeThreadConfigBuilder`

```java
public class com.feilong.core.lang.thread.PartitionEachSizeThreadConfigBuilder implements com.feilong.core.lang.thread.PartitionEachSizeBuilder {
  public com.feilong.core.lang.thread.PartitionEachSizeThreadConfigBuilder();
  public com.feilong.core.lang.thread.PartitionEachSizeThreadConfigBuilder(com.feilong.core.lang.thread.PartitionThreadConfig);
  public int build(int);
  public void setPartitionThreadConfig(com.feilong.core.lang.thread.PartitionThreadConfig);
}
```

## `com.feilong.core.lang.thread.PartitionPerElementHandler`

```java
public interface com.feilong.core.lang.thread.PartitionPerElementHandler<T> {
  public abstract void handle(T, com.feilong.core.lang.thread.PartitionThreadEntity, java.util.Map<java.lang.String, ?>);
}
```

## `com.feilong.core.lang.thread.PartitionPerHandler`

```java
public interface com.feilong.core.lang.thread.PartitionPerHandler<T> {
  public abstract void handle(java.util.List<T>, com.feilong.core.lang.thread.PartitionThreadEntity, java.util.Map<java.lang.String, ?>);
}
```

## `com.feilong.core.lang.thread.PartitionRunnableBuilder`

```java
public interface com.feilong.core.lang.thread.PartitionRunnableBuilder<T> {
  public abstract java.lang.Runnable build(java.util.List<T>, com.feilong.core.lang.thread.PartitionThreadEntity, java.util.Map<java.lang.String, ?>);
}
```

## `com.feilong.core.lang.thread.PartitionThreadConfig`

```java
public class com.feilong.core.lang.thread.PartitionThreadConfig {
  public com.feilong.core.lang.thread.PartitionThreadConfig();
  public com.feilong.core.lang.thread.PartitionThreadConfig(int);
  public com.feilong.core.lang.thread.PartitionThreadConfig(int, int);
  public int getMaxThreadCount();
  public void setMaxThreadCount(int);
  public int getMinPerThreadHandlerCount();
  public void setMinPerThreadHandlerCount(int);
  public java.lang.String toString();
}
```

## `com.feilong.core.lang.thread.PartitionThreadEntity`

```java
public class com.feilong.core.lang.thread.PartitionThreadEntity implements java.io.Serializable {
  public com.feilong.core.lang.thread.PartitionThreadEntity(java.lang.String, int, int, int, int);
  public java.lang.String getName();
  public int getTotalListCount();
  public int getBatchNumber();
  public int getCurrentListSize();
  public int getEachSize();
  public java.lang.String toString();
}
```

## `com.feilong.core.lang.thread.PartitionThreadExecutor`

```java
public interface com.feilong.core.lang.thread.PartitionThreadExecutor {
  public abstract <T> void execute(java.util.List<T>, int, com.feilong.core.lang.thread.PartitionRunnableBuilder<T>);
  public abstract <T> void execute(java.util.List<T>, int, java.util.Map<java.lang.String, ?>, com.feilong.core.lang.thread.PartitionRunnableBuilder<T>);
}
```
