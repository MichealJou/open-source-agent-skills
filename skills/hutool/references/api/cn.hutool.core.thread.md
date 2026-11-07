# cn.hutool.core.thread

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.thread.AsyncUtil`

```java
public class cn.hutool.core.thread.AsyncUtil {
  public cn.hutool.core.thread.AsyncUtil();
  public static void waitAll(java.util.concurrent.CompletableFuture<?>...);
  public static <T> T waitAny(java.util.concurrent.CompletableFuture<?>...);
  public static <T> T get(java.util.concurrent.CompletableFuture<T>);
}
```

## `cn.hutool.core.thread.BlockPolicy`

```java
public class cn.hutool.core.thread.BlockPolicy implements java.util.concurrent.RejectedExecutionHandler {
  public cn.hutool.core.thread.BlockPolicy(java.util.function.Consumer<java.lang.Runnable>);
  public cn.hutool.core.thread.BlockPolicy();
  public void rejectedExecution(java.lang.Runnable, java.util.concurrent.ThreadPoolExecutor);
}
```

## `cn.hutool.core.thread.ConcurrencyTester`

```java
public class cn.hutool.core.thread.ConcurrencyTester implements java.io.Closeable {
  public cn.hutool.core.thread.ConcurrencyTester(int);
  public cn.hutool.core.thread.ConcurrencyTester test(java.lang.Runnable);
  public cn.hutool.core.thread.ConcurrencyTester reset();
  public long getInterval();
  public void close() throws java.io.IOException;
}
```

## `cn.hutool.core.thread.DelegatedExecutorService`

```java
public class cn.hutool.core.thread.DelegatedExecutorService extends java.util.concurrent.AbstractExecutorService {
  public cn.hutool.core.thread.DelegatedExecutorService(java.util.concurrent.ExecutorService);
  public void execute(java.lang.Runnable);
  public void shutdown();
  public java.util.List<java.lang.Runnable> shutdownNow();
  public boolean isShutdown();
  public boolean isTerminated();
  public boolean awaitTermination(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public java.util.concurrent.Future<?> submit(java.lang.Runnable);
  public <T> java.util.concurrent.Future<T> submit(java.util.concurrent.Callable<T>);
  public <T> java.util.concurrent.Future<T> submit(java.lang.Runnable, T);
  public <T> java.util.List<java.util.concurrent.Future<T>> invokeAll(java.util.Collection<? extends java.util.concurrent.Callable<T>>) throws java.lang.InterruptedException;
  public <T> java.util.List<java.util.concurrent.Future<T>> invokeAll(java.util.Collection<? extends java.util.concurrent.Callable<T>>, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public <T> T invokeAny(java.util.Collection<? extends java.util.concurrent.Callable<T>>) throws java.lang.InterruptedException, java.util.concurrent.ExecutionException;
  public <T> T invokeAny(java.util.Collection<? extends java.util.concurrent.Callable<T>>, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException, java.util.concurrent.ExecutionException, java.util.concurrent.TimeoutException;
}
```

## `cn.hutool.core.thread.ExecutorBuilder`

```java
public class cn.hutool.core.thread.ExecutorBuilder implements cn.hutool.core.builder.Builder<java.util.concurrent.ThreadPoolExecutor> {
  public cn.hutool.core.thread.ExecutorBuilder();
  public cn.hutool.core.thread.ExecutorBuilder setCorePoolSize(int);
  public cn.hutool.core.thread.ExecutorBuilder setMaxPoolSize(int);
  public cn.hutool.core.thread.ExecutorBuilder setKeepAliveTime(long, java.util.concurrent.TimeUnit);
  public cn.hutool.core.thread.ExecutorBuilder setKeepAliveTime(long);
  public cn.hutool.core.thread.ExecutorBuilder setWorkQueue(java.util.concurrent.BlockingQueue<java.lang.Runnable>);
  public cn.hutool.core.thread.ExecutorBuilder useArrayBlockingQueue(int);
  public cn.hutool.core.thread.ExecutorBuilder useSynchronousQueue();
  public cn.hutool.core.thread.ExecutorBuilder useSynchronousQueue(boolean);
  public cn.hutool.core.thread.ExecutorBuilder setThreadFactory(java.util.concurrent.ThreadFactory);
  public cn.hutool.core.thread.ExecutorBuilder setHandler(java.util.concurrent.RejectedExecutionHandler);
  public cn.hutool.core.thread.ExecutorBuilder setAllowCoreThreadTimeOut(boolean);
  public static cn.hutool.core.thread.ExecutorBuilder create();
  public java.util.concurrent.ThreadPoolExecutor build();
  public java.util.concurrent.ExecutorService buildFinalizable();
  public java.lang.Object build();
}
```

## `cn.hutool.core.thread.GlobalThreadPool`

```java
public class cn.hutool.core.thread.GlobalThreadPool {
  public static synchronized void init();
  public static synchronized void shutdown(boolean);
  public static java.util.concurrent.ExecutorService getExecutor();
  public static void execute(java.lang.Runnable);
  public static <T> java.util.concurrent.Future<T> submit(java.util.concurrent.Callable<T>);
  public static java.util.concurrent.Future<?> submit(java.lang.Runnable);
}
```

## `cn.hutool.core.thread.NamedThreadFactory`

```java
public class cn.hutool.core.thread.NamedThreadFactory implements java.util.concurrent.ThreadFactory {
  public cn.hutool.core.thread.NamedThreadFactory(java.lang.String, boolean);
  public cn.hutool.core.thread.NamedThreadFactory(java.lang.String, java.lang.ThreadGroup, boolean);
  public cn.hutool.core.thread.NamedThreadFactory(java.lang.String, java.lang.ThreadGroup, boolean, java.lang.Thread$UncaughtExceptionHandler);
  public java.lang.Thread newThread(java.lang.Runnable);
}
```

## `cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor`

```java
public class cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor {
  public cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor(int);
  public cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor(int, java.lang.String);
  public cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor(java.util.concurrent.ExecutorService);
  public void shutdown();
  public java.util.concurrent.ExecutorService getExecutor();
  public <T, R> java.util.List<R> process(java.util.List<T>, int, java.util.function.Function<T, R>);
  public java.util.List<cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor$Warp<?>> processByWarp(cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor$Warp<?>...);
  public java.util.List<cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor$Warp<?>> processByWarp(java.util.List<cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor$Warp<?>>);
}
```

## `cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor$Warp`

```java
public class cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor$Warp<R> {
  public static <R> cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor$Warp<R> of(java.util.function.Supplier<R>);
  public R get();
  public cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor$Warp<R> execute();
}
```

## `cn.hutool.core.thread.RejectPolicy`

```java
public final class cn.hutool.core.thread.RejectPolicy extends java.lang.Enum<cn.hutool.core.thread.RejectPolicy> {
  public static cn.hutool.core.thread.RejectPolicy[] values();
  public static cn.hutool.core.thread.RejectPolicy valueOf(java.lang.String);
  public java.util.concurrent.RejectedExecutionHandler getValue();
}
```

## `cn.hutool.core.thread.SemaphoreRunnable`

```java
public class cn.hutool.core.thread.SemaphoreRunnable implements java.lang.Runnable {
  public cn.hutool.core.thread.SemaphoreRunnable(java.lang.Runnable, java.util.concurrent.Semaphore);
  public java.util.concurrent.Semaphore getSemaphore();
  public void run();
}
```

## `cn.hutool.core.thread.SyncFinisher`

```java
public class cn.hutool.core.thread.SyncFinisher implements java.io.Closeable {
  public cn.hutool.core.thread.SyncFinisher(int);
  public cn.hutool.core.thread.SyncFinisher setExecutorService(java.util.concurrent.ExecutorService);
  public cn.hutool.core.thread.SyncFinisher setBeginAtSameTime(boolean);
  public cn.hutool.core.thread.SyncFinisher setExceptionHandler(java.lang.Thread$UncaughtExceptionHandler);
  public cn.hutool.core.thread.SyncFinisher addRepeatWorker(java.lang.Runnable);
  public cn.hutool.core.thread.SyncFinisher addWorker(java.lang.Runnable);
  public synchronized cn.hutool.core.thread.SyncFinisher addWorker(cn.hutool.core.thread.SyncFinisher$Worker);
  public void start();
  public void start(boolean);
  public void stop();
  public void stopNow();
  public void clearWorker();
  public long count();
  public void close() throws java.io.IOException;
}
```

## `cn.hutool.core.thread.SyncFinisher$Worker`

```java
public abstract class cn.hutool.core.thread.SyncFinisher$Worker implements java.lang.Runnable {
  public cn.hutool.core.thread.SyncFinisher$Worker(cn.hutool.core.thread.SyncFinisher);
  public void run();
  public abstract void work();
}
```

## `cn.hutool.core.thread.ThreadException`

```java
public class cn.hutool.core.thread.ThreadException extends java.lang.RuntimeException {
  public cn.hutool.core.thread.ThreadException(java.lang.Throwable);
  public cn.hutool.core.thread.ThreadException(java.lang.String);
  public cn.hutool.core.thread.ThreadException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.thread.ThreadException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.thread.ThreadException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.core.thread.ThreadException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.core.thread.ThreadFactoryBuilder`

```java
public class cn.hutool.core.thread.ThreadFactoryBuilder implements cn.hutool.core.builder.Builder<java.util.concurrent.ThreadFactory> {
  public cn.hutool.core.thread.ThreadFactoryBuilder();
  public static cn.hutool.core.thread.ThreadFactoryBuilder create();
  public cn.hutool.core.thread.ThreadFactoryBuilder setThreadFactory(java.util.concurrent.ThreadFactory);
  public cn.hutool.core.thread.ThreadFactoryBuilder setNamePrefix(java.lang.String);
  public cn.hutool.core.thread.ThreadFactoryBuilder setDaemon(boolean);
  public cn.hutool.core.thread.ThreadFactoryBuilder setPriority(int);
  public cn.hutool.core.thread.ThreadFactoryBuilder setUncaughtExceptionHandler(java.lang.Thread$UncaughtExceptionHandler);
  public java.util.concurrent.ThreadFactory build();
  public java.lang.Object build();
}
```

## `cn.hutool.core.thread.ThreadUtil`

```java
public class cn.hutool.core.thread.ThreadUtil {
  public cn.hutool.core.thread.ThreadUtil();
  public static java.util.concurrent.ThreadPoolExecutor newExecutor(int);
  public static java.util.concurrent.ThreadPoolExecutor newExecutor();
  public static java.util.concurrent.ExecutorService newSingleExecutor();
  public static java.util.concurrent.ThreadPoolExecutor newExecutor(int, int);
  public static java.util.concurrent.ThreadPoolExecutor newExecutor(int, int, int);
  public static java.util.concurrent.ThreadPoolExecutor newExecutorByBlockingCoefficient(float);
  public static java.util.concurrent.ThreadPoolExecutor newFixedExecutor(int, java.lang.String, boolean);
  public static java.util.concurrent.ThreadPoolExecutor newFixedExecutor(int, int, java.lang.String, boolean);
  public static java.util.concurrent.ThreadPoolExecutor newFixedExecutor(int, int, java.lang.String, java.util.concurrent.RejectedExecutionHandler);
  public static void execute(java.lang.Runnable);
  public static java.lang.Runnable execAsync(java.lang.Runnable, boolean);
  public static <T> java.util.concurrent.Future<T> execAsync(java.util.concurrent.Callable<T>);
  public static java.util.concurrent.Future<?> execAsync(java.lang.Runnable);
  public static <T> java.util.concurrent.CompletionService<T> newCompletionService();
  public static <T> java.util.concurrent.CompletionService<T> newCompletionService(java.util.concurrent.ExecutorService);
  public static java.util.concurrent.CountDownLatch newCountDownLatch(int);
  public static java.lang.Thread newThread(java.lang.Runnable, java.lang.String);
  public static java.lang.Thread newThread(java.lang.Runnable, java.lang.String, boolean);
  public static boolean sleep(java.lang.Number, java.util.concurrent.TimeUnit);
  public static boolean sleep(java.lang.Number);
  public static boolean sleep(long);
  public static boolean safeSleep(java.lang.Number);
  public static boolean safeSleep(long);
  public static java.lang.StackTraceElement[] getStackTrace();
  public static java.lang.StackTraceElement getStackTraceElement(int);
  public static <T> java.lang.ThreadLocal<T> createThreadLocal(boolean);
  public static <T> java.lang.ThreadLocal<T> createThreadLocal(java.util.function.Supplier<? extends T>);
  public static cn.hutool.core.thread.ThreadFactoryBuilder createThreadFactoryBuilder();
  public static java.util.concurrent.ThreadFactory createThreadFactory(java.lang.String);
  public static void interrupt(java.lang.Thread, boolean);
  public static void waitForDie();
  public static void waitForDie(java.lang.Thread);
  public static java.lang.Thread[] getThreads();
  public static java.lang.Thread[] getThreads(java.lang.ThreadGroup);
  public static java.lang.Thread getMainThread();
  public static java.lang.ThreadGroup currentThreadGroup();
  public static java.util.concurrent.ThreadFactory newNamedThreadFactory(java.lang.String, boolean);
  public static java.util.concurrent.ThreadFactory newNamedThreadFactory(java.lang.String, java.lang.ThreadGroup, boolean);
  public static java.util.concurrent.ThreadFactory newNamedThreadFactory(java.lang.String, java.lang.ThreadGroup, boolean, java.lang.Thread$UncaughtExceptionHandler);
  public static void sync(java.lang.Object);
  public static cn.hutool.core.thread.ConcurrencyTester concurrencyTest(int, java.lang.Runnable);
  public static java.util.concurrent.ScheduledThreadPoolExecutor createScheduledExecutor(int);
  public static java.util.concurrent.ScheduledThreadPoolExecutor schedule(java.util.concurrent.ScheduledThreadPoolExecutor, java.lang.Runnable, long, long, boolean);
  public static java.util.concurrent.ScheduledThreadPoolExecutor schedule(java.util.concurrent.ScheduledThreadPoolExecutor, java.lang.Runnable, long, long, java.util.concurrent.TimeUnit, boolean);
}
```
