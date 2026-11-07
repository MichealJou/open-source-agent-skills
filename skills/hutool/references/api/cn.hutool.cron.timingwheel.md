# cn.hutool.cron.timingwheel

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.cron.timingwheel.SystemTimer`

```java
public class cn.hutool.cron.timingwheel.SystemTimer {
  public cn.hutool.cron.timingwheel.SystemTimer();
  public cn.hutool.cron.timingwheel.SystemTimer setDelayQueueTimeout(long);
  public cn.hutool.cron.timingwheel.SystemTimer start();
  public void stop();
  public void addTask(cn.hutool.cron.timingwheel.TimerTask);
}
```

## `cn.hutool.cron.timingwheel.TimerTask`

```java
public class cn.hutool.cron.timingwheel.TimerTask {
  public cn.hutool.cron.timingwheel.TimerTask(java.lang.Runnable, long);
  public java.lang.Runnable getTask();
  public long getDelayMs();
  public java.lang.String toString();
}
```

## `cn.hutool.cron.timingwheel.TimerTaskList`

```java
public class cn.hutool.cron.timingwheel.TimerTaskList implements java.util.concurrent.Delayed {
  public cn.hutool.cron.timingwheel.TimerTaskList();
  public boolean setExpiration(long);
  public long getExpire();
  public void addTask(cn.hutool.cron.timingwheel.TimerTask);
  public void removeTask(cn.hutool.cron.timingwheel.TimerTask);
  public synchronized void flush(java.util.function.Consumer<cn.hutool.cron.timingwheel.TimerTask>);
  public long getDelay(java.util.concurrent.TimeUnit);
  public int compareTo(java.util.concurrent.Delayed);
  public int compareTo(java.lang.Object);
}
```

## `cn.hutool.cron.timingwheel.TimingWheel`

```java
public class cn.hutool.cron.timingwheel.TimingWheel {
  public cn.hutool.cron.timingwheel.TimingWheel(long, int, java.util.function.Consumer<cn.hutool.cron.timingwheel.TimerTaskList>);
  public cn.hutool.cron.timingwheel.TimingWheel(long, int, long, java.util.function.Consumer<cn.hutool.cron.timingwheel.TimerTaskList>);
  public boolean addTask(cn.hutool.cron.timingwheel.TimerTask);
  public void advanceClock(long);
}
```
