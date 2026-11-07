# cn.hutool.cron

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.cron.CronConfig`

```java
public class cn.hutool.cron.CronConfig {
  public cn.hutool.cron.CronConfig();
  public cn.hutool.cron.CronConfig setTimeZone(java.util.TimeZone);
  public java.util.TimeZone getTimeZone();
  public boolean isMatchSecond();
  public cn.hutool.cron.CronConfig setMatchSecond(boolean);
}
```

## `cn.hutool.cron.CronException`

```java
public class cn.hutool.cron.CronException extends java.lang.RuntimeException {
  public cn.hutool.cron.CronException(java.lang.Throwable);
  public cn.hutool.cron.CronException(java.lang.String);
  public cn.hutool.cron.CronException(java.lang.String, java.lang.Object...);
  public cn.hutool.cron.CronException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.cron.CronException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.cron.CronTimer`

```java
public class cn.hutool.cron.CronTimer extends java.lang.Thread implements java.io.Serializable {
  public cn.hutool.cron.CronTimer(cn.hutool.cron.Scheduler);
  public void run();
  public synchronized void stopTimer();
}
```

## `cn.hutool.cron.CronUtil`

```java
public class cn.hutool.cron.CronUtil {
  public cn.hutool.cron.CronUtil();
  public static void setCronSetting(cn.hutool.setting.Setting);
  public static void setCronSetting(java.lang.String);
  public static void setMatchSecond(boolean);
  public static java.lang.String schedule(java.lang.String, cn.hutool.cron.task.Task);
  public static java.lang.String schedule(java.lang.String, java.lang.String, cn.hutool.cron.task.Task);
  public static java.lang.String schedule(java.lang.String, java.lang.Runnable);
  public static void schedule(cn.hutool.setting.Setting);
  public static boolean remove(java.lang.String);
  public static void updatePattern(java.lang.String, cn.hutool.cron.pattern.CronPattern);
  public static cn.hutool.cron.Scheduler getScheduler();
  public static void start();
  public static synchronized void start(boolean);
  public static void restart();
  public static void stop();
}
```

## `cn.hutool.cron.Scheduler`

```java
public class cn.hutool.cron.Scheduler implements java.io.Serializable {
  public cn.hutool.cron.Scheduler();
  public cn.hutool.cron.Scheduler setTimeZone(java.util.TimeZone);
  public java.util.TimeZone getTimeZone();
  public cn.hutool.cron.Scheduler setDaemon(boolean) throws cn.hutool.cron.CronException;
  public cn.hutool.cron.Scheduler setThreadExecutor(java.util.concurrent.ExecutorService) throws cn.hutool.cron.CronException;
  public boolean isDaemon();
  public boolean isMatchSecond();
  public cn.hutool.cron.Scheduler setMatchSecond(boolean);
  public cn.hutool.cron.Scheduler addListener(cn.hutool.cron.listener.TaskListener);
  public cn.hutool.cron.Scheduler removeListener(cn.hutool.cron.listener.TaskListener);
  public cn.hutool.cron.Scheduler schedule(cn.hutool.setting.Setting);
  public java.lang.String schedule(java.lang.String, java.lang.Runnable);
  public java.lang.String schedule(java.lang.String, cn.hutool.cron.task.Task);
  public cn.hutool.cron.Scheduler schedule(java.lang.String, java.lang.String, java.lang.Runnable);
  public cn.hutool.cron.Scheduler schedule(java.lang.String, java.lang.String, cn.hutool.cron.task.Task);
  public cn.hutool.cron.Scheduler schedule(java.lang.String, cn.hutool.cron.pattern.CronPattern, cn.hutool.cron.task.Task);
  public cn.hutool.cron.Scheduler deschedule(java.lang.String);
  public boolean descheduleWithStatus(java.lang.String);
  public cn.hutool.cron.Scheduler updatePattern(java.lang.String, cn.hutool.cron.pattern.CronPattern);
  public cn.hutool.cron.TaskTable getTaskTable();
  public cn.hutool.cron.pattern.CronPattern getPattern(java.lang.String);
  public cn.hutool.cron.task.Task getTask(java.lang.String);
  public boolean isEmpty();
  public int size();
  public cn.hutool.cron.Scheduler clear();
  public boolean isStarted();
  public cn.hutool.cron.Scheduler start(boolean);
  public cn.hutool.cron.Scheduler start();
  public cn.hutool.cron.Scheduler stop();
  public cn.hutool.cron.Scheduler stop(boolean);
}
```

## `cn.hutool.cron.TaskExecutor`

```java
public class cn.hutool.cron.TaskExecutor implements java.lang.Runnable {
  public cn.hutool.cron.task.Task getTask();
  public cn.hutool.cron.task.CronTask getCronTask();
  public cn.hutool.cron.TaskExecutor(cn.hutool.cron.Scheduler, cn.hutool.cron.task.CronTask);
  public void run();
}
```

## `cn.hutool.cron.TaskExecutorManager`

```java
public class cn.hutool.cron.TaskExecutorManager implements java.io.Serializable {
  public cn.hutool.cron.TaskExecutorManager(cn.hutool.cron.Scheduler);
  public java.util.List<cn.hutool.cron.TaskExecutor> getExecutors();
  public cn.hutool.cron.TaskExecutor spawnExecutor(cn.hutool.cron.task.CronTask);
  public cn.hutool.cron.TaskExecutorManager notifyExecutorCompleted(cn.hutool.cron.TaskExecutor);
}
```

## `cn.hutool.cron.TaskLauncher`

```java
public class cn.hutool.cron.TaskLauncher implements java.lang.Runnable {
  public cn.hutool.cron.TaskLauncher(cn.hutool.cron.Scheduler, long);
  public void run();
}
```

## `cn.hutool.cron.TaskLauncherManager`

```java
public class cn.hutool.cron.TaskLauncherManager implements java.io.Serializable {
  public cn.hutool.cron.TaskLauncherManager(cn.hutool.cron.Scheduler);
}
```

## `cn.hutool.cron.TaskTable`

```java
public class cn.hutool.cron.TaskTable implements java.io.Serializable {
  public cn.hutool.cron.TaskTable();
  public cn.hutool.cron.TaskTable(int);
  public cn.hutool.cron.TaskTable add(java.lang.String, cn.hutool.cron.pattern.CronPattern, cn.hutool.cron.task.Task);
  public java.util.List<java.lang.String> getIds();
  public java.util.List<cn.hutool.cron.pattern.CronPattern> getPatterns();
  public java.util.List<cn.hutool.cron.task.Task> getTasks();
  public boolean remove(java.lang.String);
  public boolean updatePattern(java.lang.String, cn.hutool.cron.pattern.CronPattern);
  public cn.hutool.cron.task.Task getTask(int);
  public cn.hutool.cron.task.Task getTask(java.lang.String);
  public cn.hutool.cron.pattern.CronPattern getPattern(int);
  public int size();
  public boolean isEmpty();
  public cn.hutool.cron.pattern.CronPattern getPattern(java.lang.String);
  public void executeTaskIfMatch(cn.hutool.cron.Scheduler, long);
  public java.lang.String toString();
}
```
