# cn.hutool.cron.task

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.cron.task.CronTask`

```java
public class cn.hutool.cron.task.CronTask implements cn.hutool.cron.task.Task {
  public cn.hutool.cron.task.CronTask(java.lang.String, cn.hutool.cron.pattern.CronPattern, cn.hutool.cron.task.Task);
  public void execute();
  public java.lang.String getId();
  public cn.hutool.cron.pattern.CronPattern getPattern();
  public cn.hutool.cron.task.CronTask setPattern(cn.hutool.cron.pattern.CronPattern);
  public cn.hutool.cron.task.Task getRaw();
}
```

## `cn.hutool.cron.task.InvokeTask`

```java
public class cn.hutool.cron.task.InvokeTask implements cn.hutool.cron.task.Task {
  public cn.hutool.cron.task.InvokeTask(java.lang.String);
  public void execute();
}
```

## `cn.hutool.cron.task.RunnableTask`

```java
public class cn.hutool.cron.task.RunnableTask implements cn.hutool.cron.task.Task {
  public cn.hutool.cron.task.RunnableTask(java.lang.Runnable);
  public void execute();
}
```

## `cn.hutool.cron.task.Task`

```java
public interface cn.hutool.cron.task.Task {
  public abstract void execute();
}
```
