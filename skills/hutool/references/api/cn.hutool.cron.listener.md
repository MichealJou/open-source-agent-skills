# cn.hutool.cron.listener

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.cron.listener.SimpleTaskListener`

```java
public class cn.hutool.cron.listener.SimpleTaskListener implements cn.hutool.cron.listener.TaskListener {
  public cn.hutool.cron.listener.SimpleTaskListener();
  public void onStart(cn.hutool.cron.TaskExecutor);
  public void onSucceeded(cn.hutool.cron.TaskExecutor);
  public void onFailed(cn.hutool.cron.TaskExecutor, java.lang.Throwable);
}
```

## `cn.hutool.cron.listener.TaskListener`

```java
public interface cn.hutool.cron.listener.TaskListener {
  public abstract void onStart(cn.hutool.cron.TaskExecutor);
  public abstract void onSucceeded(cn.hutool.cron.TaskExecutor);
  public abstract void onFailed(cn.hutool.cron.TaskExecutor, java.lang.Throwable);
}
```

## `cn.hutool.cron.listener.TaskListenerManager`

```java
public class cn.hutool.cron.listener.TaskListenerManager implements java.io.Serializable {
  public cn.hutool.cron.listener.TaskListenerManager();
  public cn.hutool.cron.listener.TaskListenerManager addListener(cn.hutool.cron.listener.TaskListener);
  public cn.hutool.cron.listener.TaskListenerManager removeListener(cn.hutool.cron.listener.TaskListener);
  public void notifyTaskStart(cn.hutool.cron.TaskExecutor);
  public void notifyTaskSucceeded(cn.hutool.cron.TaskExecutor);
  public void notifyTaskFailed(cn.hutool.cron.TaskExecutor, java.lang.Throwable);
}
```
