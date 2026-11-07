# com.google.common.util.concurrent

版本：33.4.8-jre。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.google.common.util.concurrent.AbstractExecutionThreadService`

```java
public abstract class com.google.common.util.concurrent.AbstractExecutionThreadService implements com.google.common.util.concurrent.Service {
  public java.lang.String toString();
  public final boolean isRunning();
  public final com.google.common.util.concurrent.Service$State state();
  public final void addListener(com.google.common.util.concurrent.Service$Listener, java.util.concurrent.Executor);
  public final java.lang.Throwable failureCause();
  public final com.google.common.util.concurrent.Service startAsync();
  public final com.google.common.util.concurrent.Service stopAsync();
  public final void awaitRunning();
  public final void awaitRunning(java.time.Duration) throws java.util.concurrent.TimeoutException;
  public final void awaitRunning(long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException;
  public final void awaitTerminated();
  public final void awaitTerminated(java.time.Duration) throws java.util.concurrent.TimeoutException;
  public final void awaitTerminated(long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException;
}
```

## `com.google.common.util.concurrent.AbstractFuture`

```java
public abstract class com.google.common.util.concurrent.AbstractFuture<V> extends com.google.common.util.concurrent.AbstractFutureState<V> {
  public V get(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException, java.util.concurrent.TimeoutException, java.util.concurrent.ExecutionException;
  public V get() throws java.lang.InterruptedException, java.util.concurrent.ExecutionException;
  public boolean isDone();
  public boolean isCancelled();
  public boolean cancel(boolean);
  public void addListener(java.lang.Runnable, java.util.concurrent.Executor);
  public java.lang.String toString();
}
```

## `com.google.common.util.concurrent.AbstractIdleService`

```java
public abstract class com.google.common.util.concurrent.AbstractIdleService implements com.google.common.util.concurrent.Service {
  public java.lang.String toString();
  public final boolean isRunning();
  public final com.google.common.util.concurrent.Service$State state();
  public final void addListener(com.google.common.util.concurrent.Service$Listener, java.util.concurrent.Executor);
  public final java.lang.Throwable failureCause();
  public final com.google.common.util.concurrent.Service startAsync();
  public final com.google.common.util.concurrent.Service stopAsync();
  public final void awaitRunning();
  public final void awaitRunning(java.time.Duration) throws java.util.concurrent.TimeoutException;
  public final void awaitRunning(long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException;
  public final void awaitTerminated();
  public final void awaitTerminated(java.time.Duration) throws java.util.concurrent.TimeoutException;
  public final void awaitTerminated(long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException;
}
```

## `com.google.common.util.concurrent.AbstractListeningExecutorService`

```java
public abstract class com.google.common.util.concurrent.AbstractListeningExecutorService extends java.util.concurrent.AbstractExecutorService implements com.google.common.util.concurrent.ListeningExecutorService {
  public com.google.common.util.concurrent.AbstractListeningExecutorService();
  public com.google.common.util.concurrent.ListenableFuture<?> submit(java.lang.Runnable);
  public <T> com.google.common.util.concurrent.ListenableFuture<T> submit(java.lang.Runnable, T);
  public <T> com.google.common.util.concurrent.ListenableFuture<T> submit(java.util.concurrent.Callable<T>);
  public java.util.concurrent.Future submit(java.util.concurrent.Callable);
  public java.util.concurrent.Future submit(java.lang.Runnable, java.lang.Object);
  public java.util.concurrent.Future submit(java.lang.Runnable);
}
```

## `com.google.common.util.concurrent.AbstractScheduledService`

```java
public abstract class com.google.common.util.concurrent.AbstractScheduledService implements com.google.common.util.concurrent.Service {
  public java.lang.String toString();
  public final boolean isRunning();
  public final com.google.common.util.concurrent.Service$State state();
  public final void addListener(com.google.common.util.concurrent.Service$Listener, java.util.concurrent.Executor);
  public final java.lang.Throwable failureCause();
  public final com.google.common.util.concurrent.Service startAsync();
  public final com.google.common.util.concurrent.Service stopAsync();
  public final void awaitRunning();
  public final void awaitRunning(java.time.Duration) throws java.util.concurrent.TimeoutException;
  public final void awaitRunning(long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException;
  public final void awaitTerminated();
  public final void awaitTerminated(java.time.Duration) throws java.util.concurrent.TimeoutException;
  public final void awaitTerminated(long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException;
}
```

## `com.google.common.util.concurrent.AbstractScheduledService$CustomScheduler`

```java
public abstract class com.google.common.util.concurrent.AbstractScheduledService$CustomScheduler extends com.google.common.util.concurrent.AbstractScheduledService$Scheduler {
  public com.google.common.util.concurrent.AbstractScheduledService$CustomScheduler();
}
```

## `com.google.common.util.concurrent.AbstractScheduledService$CustomScheduler$Schedule`

```java
public final class com.google.common.util.concurrent.AbstractScheduledService$CustomScheduler$Schedule {
  public com.google.common.util.concurrent.AbstractScheduledService$CustomScheduler$Schedule(long, java.util.concurrent.TimeUnit);
  public com.google.common.util.concurrent.AbstractScheduledService$CustomScheduler$Schedule(java.time.Duration);
}
```

## `com.google.common.util.concurrent.AbstractScheduledService$Scheduler`

```java
public abstract class com.google.common.util.concurrent.AbstractScheduledService$Scheduler {
  public static com.google.common.util.concurrent.AbstractScheduledService$Scheduler newFixedDelaySchedule(java.time.Duration, java.time.Duration);
  public static com.google.common.util.concurrent.AbstractScheduledService$Scheduler newFixedDelaySchedule(long, long, java.util.concurrent.TimeUnit);
  public static com.google.common.util.concurrent.AbstractScheduledService$Scheduler newFixedRateSchedule(java.time.Duration, java.time.Duration);
  public static com.google.common.util.concurrent.AbstractScheduledService$Scheduler newFixedRateSchedule(long, long, java.util.concurrent.TimeUnit);
}
```

## `com.google.common.util.concurrent.AbstractService`

```java
public abstract class com.google.common.util.concurrent.AbstractService implements com.google.common.util.concurrent.Service {
  public final com.google.common.util.concurrent.Service startAsync();
  public final com.google.common.util.concurrent.Service stopAsync();
  public final void awaitRunning();
  public final void awaitRunning(java.time.Duration) throws java.util.concurrent.TimeoutException;
  public final void awaitRunning(long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException;
  public final void awaitTerminated();
  public final void awaitTerminated(java.time.Duration) throws java.util.concurrent.TimeoutException;
  public final void awaitTerminated(long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException;
  public final boolean isRunning();
  public final com.google.common.util.concurrent.Service$State state();
  public final java.lang.Throwable failureCause();
  public final void addListener(com.google.common.util.concurrent.Service$Listener, java.util.concurrent.Executor);
  public java.lang.String toString();
}
```

## `com.google.common.util.concurrent.AsyncCallable`

```java
public interface com.google.common.util.concurrent.AsyncCallable<V> {
  public abstract com.google.common.util.concurrent.ListenableFuture<V> call() throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.AsyncFunction`

```java
public interface com.google.common.util.concurrent.AsyncFunction<I, O> {
  public abstract com.google.common.util.concurrent.ListenableFuture<O> apply(I) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.AtomicDouble`

```java
public class com.google.common.util.concurrent.AtomicDouble extends java.lang.Number {
  public com.google.common.util.concurrent.AtomicDouble(double);
  public com.google.common.util.concurrent.AtomicDouble();
  public final double get();
  public final void set(double);
  public final void lazySet(double);
  public final double getAndSet(double);
  public final boolean compareAndSet(double, double);
  public final boolean weakCompareAndSet(double, double);
  public final double getAndAdd(double);
  public final double addAndGet(double);
  public final double getAndAccumulate(double, java.util.function.DoubleBinaryOperator);
  public final double accumulateAndGet(double, java.util.function.DoubleBinaryOperator);
  public final double getAndUpdate(java.util.function.DoubleUnaryOperator);
  public final double updateAndGet(java.util.function.DoubleUnaryOperator);
  public java.lang.String toString();
  public int intValue();
  public long longValue();
  public float floatValue();
  public double doubleValue();
}
```

## `com.google.common.util.concurrent.AtomicDoubleArray`

```java
public class com.google.common.util.concurrent.AtomicDoubleArray implements java.io.Serializable {
  public com.google.common.util.concurrent.AtomicDoubleArray(int);
  public com.google.common.util.concurrent.AtomicDoubleArray(double[]);
  public final int length();
  public final double get(int);
  public final void set(int, double);
  public final void lazySet(int, double);
  public final double getAndSet(int, double);
  public final boolean compareAndSet(int, double, double);
  public final boolean weakCompareAndSet(int, double, double);
  public final double getAndAdd(int, double);
  public double addAndGet(int, double);
  public final double getAndAccumulate(int, double, java.util.function.DoubleBinaryOperator);
  public final double accumulateAndGet(int, double, java.util.function.DoubleBinaryOperator);
  public final double getAndUpdate(int, java.util.function.DoubleUnaryOperator);
  public final double updateAndGet(int, java.util.function.DoubleUnaryOperator);
  public java.lang.String toString();
}
```

## `com.google.common.util.concurrent.AtomicLongMap`

```java
public final class com.google.common.util.concurrent.AtomicLongMap<K> implements java.io.Serializable {
  public static <K> com.google.common.util.concurrent.AtomicLongMap<K> create();
  public static <K> com.google.common.util.concurrent.AtomicLongMap<K> create(java.util.Map<? extends K, ? extends java.lang.Long>);
  public long get(K);
  public long incrementAndGet(K);
  public long decrementAndGet(K);
  public long addAndGet(K, long);
  public long getAndIncrement(K);
  public long getAndDecrement(K);
  public long getAndAdd(K, long);
  public long updateAndGet(K, java.util.function.LongUnaryOperator);
  public long getAndUpdate(K, java.util.function.LongUnaryOperator);
  public long accumulateAndGet(K, long, java.util.function.LongBinaryOperator);
  public long getAndAccumulate(K, long, java.util.function.LongBinaryOperator);
  public long put(K, long);
  public void putAll(java.util.Map<? extends K, ? extends java.lang.Long>);
  public long remove(K);
  public boolean removeIfZero(K);
  public void removeAllZeros();
  public long sum();
  public java.util.Map<K, java.lang.Long> asMap();
  public boolean containsKey(java.lang.Object);
  public int size();
  public boolean isEmpty();
  public void clear();
  public java.lang.String toString();
}
```

## `com.google.common.util.concurrent.Atomics`

```java
public final class com.google.common.util.concurrent.Atomics {
  public static <V> java.util.concurrent.atomic.AtomicReference<V> newReference();
  public static <V> java.util.concurrent.atomic.AtomicReference<V> newReference(V);
  public static <E> java.util.concurrent.atomic.AtomicReferenceArray<E> newReferenceArray(int);
  public static <E> java.util.concurrent.atomic.AtomicReferenceArray<E> newReferenceArray(E[]);
}
```

## `com.google.common.util.concurrent.Callables`

```java
public final class com.google.common.util.concurrent.Callables {
  public static <T> java.util.concurrent.Callable<T> returning(T);
  public static <T> com.google.common.util.concurrent.AsyncCallable<T> asAsyncCallable(java.util.concurrent.Callable<T>, com.google.common.util.concurrent.ListeningExecutorService);
}
```

## `com.google.common.util.concurrent.ClosingFuture`

```java
public final class com.google.common.util.concurrent.ClosingFuture<V> {
  public static <V> com.google.common.util.concurrent.ClosingFuture<V> submit(com.google.common.util.concurrent.ClosingFuture$ClosingCallable<V>, java.util.concurrent.Executor);
  public static <V> com.google.common.util.concurrent.ClosingFuture<V> submitAsync(com.google.common.util.concurrent.ClosingFuture$AsyncClosingCallable<V>, java.util.concurrent.Executor);
  public static <V> com.google.common.util.concurrent.ClosingFuture<V> from(com.google.common.util.concurrent.ListenableFuture<V>);
  public static <C extends java.lang.AutoCloseable> com.google.common.util.concurrent.ClosingFuture<C> eventuallyClosing(com.google.common.util.concurrent.ListenableFuture<C>, java.util.concurrent.Executor);
  public static com.google.common.util.concurrent.ClosingFuture$Combiner whenAllComplete(java.lang.Iterable<? extends com.google.common.util.concurrent.ClosingFuture<?>>);
  public static com.google.common.util.concurrent.ClosingFuture$Combiner whenAllComplete(com.google.common.util.concurrent.ClosingFuture<?>, com.google.common.util.concurrent.ClosingFuture<?>...);
  public static com.google.common.util.concurrent.ClosingFuture$Combiner whenAllSucceed(java.lang.Iterable<? extends com.google.common.util.concurrent.ClosingFuture<?>>);
  public static <V1, V2> com.google.common.util.concurrent.ClosingFuture$Combiner2<V1, V2> whenAllSucceed(com.google.common.util.concurrent.ClosingFuture<V1>, com.google.common.util.concurrent.ClosingFuture<V2>);
  public static <V1, V2, V3> com.google.common.util.concurrent.ClosingFuture$Combiner3<V1, V2, V3> whenAllSucceed(com.google.common.util.concurrent.ClosingFuture<V1>, com.google.common.util.concurrent.ClosingFuture<V2>, com.google.common.util.concurrent.ClosingFuture<V3>);
  public static <V1, V2, V3, V4> com.google.common.util.concurrent.ClosingFuture$Combiner4<V1, V2, V3, V4> whenAllSucceed(com.google.common.util.concurrent.ClosingFuture<V1>, com.google.common.util.concurrent.ClosingFuture<V2>, com.google.common.util.concurrent.ClosingFuture<V3>, com.google.common.util.concurrent.ClosingFuture<V4>);
  public static <V1, V2, V3, V4, V5> com.google.common.util.concurrent.ClosingFuture$Combiner5<V1, V2, V3, V4, V5> whenAllSucceed(com.google.common.util.concurrent.ClosingFuture<V1>, com.google.common.util.concurrent.ClosingFuture<V2>, com.google.common.util.concurrent.ClosingFuture<V3>, com.google.common.util.concurrent.ClosingFuture<V4>, com.google.common.util.concurrent.ClosingFuture<V5>);
  public static com.google.common.util.concurrent.ClosingFuture$Combiner whenAllSucceed(com.google.common.util.concurrent.ClosingFuture<?>, com.google.common.util.concurrent.ClosingFuture<?>, com.google.common.util.concurrent.ClosingFuture<?>, com.google.common.util.concurrent.ClosingFuture<?>, com.google.common.util.concurrent.ClosingFuture<?>, com.google.common.util.concurrent.ClosingFuture<?>, com.google.common.util.concurrent.ClosingFuture<?>...);
  public com.google.common.util.concurrent.ListenableFuture<?> statusFuture();
  public <U> com.google.common.util.concurrent.ClosingFuture<U> transform(com.google.common.util.concurrent.ClosingFuture$ClosingFunction<? super V, U>, java.util.concurrent.Executor);
  public <U> com.google.common.util.concurrent.ClosingFuture<U> transformAsync(com.google.common.util.concurrent.ClosingFuture$AsyncClosingFunction<? super V, U>, java.util.concurrent.Executor);
  public static <V, U> com.google.common.util.concurrent.ClosingFuture$AsyncClosingFunction<V, U> withoutCloser(com.google.common.util.concurrent.AsyncFunction<V, U>);
  public <X extends java.lang.Throwable> com.google.common.util.concurrent.ClosingFuture<V> catching(java.lang.Class<X>, com.google.common.util.concurrent.ClosingFuture$ClosingFunction<? super X, ? extends V>, java.util.concurrent.Executor);
  public <X extends java.lang.Throwable> com.google.common.util.concurrent.ClosingFuture<V> catchingAsync(java.lang.Class<X>, com.google.common.util.concurrent.ClosingFuture$AsyncClosingFunction<? super X, ? extends V>, java.util.concurrent.Executor);
  public com.google.common.util.concurrent.FluentFuture<V> finishToFuture();
  public void finishToValueAndCloser(com.google.common.util.concurrent.ClosingFuture$ValueAndCloserConsumer<? super V>, java.util.concurrent.Executor);
  public boolean cancel(boolean);
  public java.lang.String toString();
}
```

## `com.google.common.util.concurrent.ClosingFuture$AsyncClosingCallable`

```java
public interface com.google.common.util.concurrent.ClosingFuture$AsyncClosingCallable<V> {
  public abstract com.google.common.util.concurrent.ClosingFuture<V> call(com.google.common.util.concurrent.ClosingFuture$DeferredCloser) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.ClosingFuture$AsyncClosingFunction`

```java
public interface com.google.common.util.concurrent.ClosingFuture$AsyncClosingFunction<T, U> {
  public abstract com.google.common.util.concurrent.ClosingFuture<U> apply(com.google.common.util.concurrent.ClosingFuture$DeferredCloser, T) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.ClosingFuture$ClosingCallable`

```java
public interface com.google.common.util.concurrent.ClosingFuture$ClosingCallable<V> {
  public abstract V call(com.google.common.util.concurrent.ClosingFuture$DeferredCloser) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.ClosingFuture$ClosingFunction`

```java
public interface com.google.common.util.concurrent.ClosingFuture$ClosingFunction<T, U> {
  public abstract U apply(com.google.common.util.concurrent.ClosingFuture$DeferredCloser, T) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner`

```java
public class com.google.common.util.concurrent.ClosingFuture$Combiner {
  public <V> com.google.common.util.concurrent.ClosingFuture<V> call(com.google.common.util.concurrent.ClosingFuture$Combiner$CombiningCallable<V>, java.util.concurrent.Executor);
  public <V> com.google.common.util.concurrent.ClosingFuture<V> callAsync(com.google.common.util.concurrent.ClosingFuture$Combiner$AsyncCombiningCallable<V>, java.util.concurrent.Executor);
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner$AsyncCombiningCallable`

```java
public interface com.google.common.util.concurrent.ClosingFuture$Combiner$AsyncCombiningCallable<V> {
  public abstract com.google.common.util.concurrent.ClosingFuture<V> call(com.google.common.util.concurrent.ClosingFuture$DeferredCloser, com.google.common.util.concurrent.ClosingFuture$Peeker) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner$CombiningCallable`

```java
public interface com.google.common.util.concurrent.ClosingFuture$Combiner$CombiningCallable<V> {
  public abstract V call(com.google.common.util.concurrent.ClosingFuture$DeferredCloser, com.google.common.util.concurrent.ClosingFuture$Peeker) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner2`

```java
public final class com.google.common.util.concurrent.ClosingFuture$Combiner2<V1, V2> extends com.google.common.util.concurrent.ClosingFuture$Combiner {
  public <U> com.google.common.util.concurrent.ClosingFuture<U> call(com.google.common.util.concurrent.ClosingFuture$Combiner2$ClosingFunction2<V1, V2, U>, java.util.concurrent.Executor);
  public <U> com.google.common.util.concurrent.ClosingFuture<U> callAsync(com.google.common.util.concurrent.ClosingFuture$Combiner2$AsyncClosingFunction2<V1, V2, U>, java.util.concurrent.Executor);
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner2$AsyncClosingFunction2`

```java
public interface com.google.common.util.concurrent.ClosingFuture$Combiner2$AsyncClosingFunction2<V1, V2, U> {
  public abstract com.google.common.util.concurrent.ClosingFuture<U> apply(com.google.common.util.concurrent.ClosingFuture$DeferredCloser, V1, V2) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner2$ClosingFunction2`

```java
public interface com.google.common.util.concurrent.ClosingFuture$Combiner2$ClosingFunction2<V1, V2, U> {
  public abstract U apply(com.google.common.util.concurrent.ClosingFuture$DeferredCloser, V1, V2) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner3`

```java
public final class com.google.common.util.concurrent.ClosingFuture$Combiner3<V1, V2, V3> extends com.google.common.util.concurrent.ClosingFuture$Combiner {
  public <U> com.google.common.util.concurrent.ClosingFuture<U> call(com.google.common.util.concurrent.ClosingFuture$Combiner3$ClosingFunction3<V1, V2, V3, U>, java.util.concurrent.Executor);
  public <U> com.google.common.util.concurrent.ClosingFuture<U> callAsync(com.google.common.util.concurrent.ClosingFuture$Combiner3$AsyncClosingFunction3<V1, V2, V3, U>, java.util.concurrent.Executor);
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner3$AsyncClosingFunction3`

```java
public interface com.google.common.util.concurrent.ClosingFuture$Combiner3$AsyncClosingFunction3<V1, V2, V3, U> {
  public abstract com.google.common.util.concurrent.ClosingFuture<U> apply(com.google.common.util.concurrent.ClosingFuture$DeferredCloser, V1, V2, V3) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner3$ClosingFunction3`

```java
public interface com.google.common.util.concurrent.ClosingFuture$Combiner3$ClosingFunction3<V1, V2, V3, U> {
  public abstract U apply(com.google.common.util.concurrent.ClosingFuture$DeferredCloser, V1, V2, V3) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner4`

```java
public final class com.google.common.util.concurrent.ClosingFuture$Combiner4<V1, V2, V3, V4> extends com.google.common.util.concurrent.ClosingFuture$Combiner {
  public <U> com.google.common.util.concurrent.ClosingFuture<U> call(com.google.common.util.concurrent.ClosingFuture$Combiner4$ClosingFunction4<V1, V2, V3, V4, U>, java.util.concurrent.Executor);
  public <U> com.google.common.util.concurrent.ClosingFuture<U> callAsync(com.google.common.util.concurrent.ClosingFuture$Combiner4$AsyncClosingFunction4<V1, V2, V3, V4, U>, java.util.concurrent.Executor);
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner4$AsyncClosingFunction4`

```java
public interface com.google.common.util.concurrent.ClosingFuture$Combiner4$AsyncClosingFunction4<V1, V2, V3, V4, U> {
  public abstract com.google.common.util.concurrent.ClosingFuture<U> apply(com.google.common.util.concurrent.ClosingFuture$DeferredCloser, V1, V2, V3, V4) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner4$ClosingFunction4`

```java
public interface com.google.common.util.concurrent.ClosingFuture$Combiner4$ClosingFunction4<V1, V2, V3, V4, U> {
  public abstract U apply(com.google.common.util.concurrent.ClosingFuture$DeferredCloser, V1, V2, V3, V4) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner5`

```java
public final class com.google.common.util.concurrent.ClosingFuture$Combiner5<V1, V2, V3, V4, V5> extends com.google.common.util.concurrent.ClosingFuture$Combiner {
  public <U> com.google.common.util.concurrent.ClosingFuture<U> call(com.google.common.util.concurrent.ClosingFuture$Combiner5$ClosingFunction5<V1, V2, V3, V4, V5, U>, java.util.concurrent.Executor);
  public <U> com.google.common.util.concurrent.ClosingFuture<U> callAsync(com.google.common.util.concurrent.ClosingFuture$Combiner5$AsyncClosingFunction5<V1, V2, V3, V4, V5, U>, java.util.concurrent.Executor);
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner5$AsyncClosingFunction5`

```java
public interface com.google.common.util.concurrent.ClosingFuture$Combiner5$AsyncClosingFunction5<V1, V2, V3, V4, V5, U> {
  public abstract com.google.common.util.concurrent.ClosingFuture<U> apply(com.google.common.util.concurrent.ClosingFuture$DeferredCloser, V1, V2, V3, V4, V5) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.ClosingFuture$Combiner5$ClosingFunction5`

```java
public interface com.google.common.util.concurrent.ClosingFuture$Combiner5$ClosingFunction5<V1, V2, V3, V4, V5, U> {
  public abstract U apply(com.google.common.util.concurrent.ClosingFuture$DeferredCloser, V1, V2, V3, V4, V5) throws java.lang.Exception;
}
```

## `com.google.common.util.concurrent.ClosingFuture$DeferredCloser`

```java
public final class com.google.common.util.concurrent.ClosingFuture$DeferredCloser {
  public <C extends java.lang.AutoCloseable> C eventuallyClose(C, java.util.concurrent.Executor);
}
```

## `com.google.common.util.concurrent.ClosingFuture$Peeker`

```java
public final class com.google.common.util.concurrent.ClosingFuture$Peeker {
  public final <D> D getDone(com.google.common.util.concurrent.ClosingFuture<D>) throws java.util.concurrent.ExecutionException;
}
```

## `com.google.common.util.concurrent.ClosingFuture$ValueAndCloser`

```java
public final class com.google.common.util.concurrent.ClosingFuture$ValueAndCloser<V> {
  public V get() throws java.util.concurrent.ExecutionException;
  public void closeAsync();
}
```

## `com.google.common.util.concurrent.ClosingFuture$ValueAndCloserConsumer`

```java
public interface com.google.common.util.concurrent.ClosingFuture$ValueAndCloserConsumer<V> {
  public abstract void accept(com.google.common.util.concurrent.ClosingFuture$ValueAndCloser<V>);
}
```

## `com.google.common.util.concurrent.CycleDetectingLockFactory`

```java
public class com.google.common.util.concurrent.CycleDetectingLockFactory {
  public static com.google.common.util.concurrent.CycleDetectingLockFactory newInstance(com.google.common.util.concurrent.CycleDetectingLockFactory$Policy);
  public java.util.concurrent.locks.ReentrantLock newReentrantLock(java.lang.String);
  public java.util.concurrent.locks.ReentrantLock newReentrantLock(java.lang.String, boolean);
  public java.util.concurrent.locks.ReentrantReadWriteLock newReentrantReadWriteLock(java.lang.String);
  public java.util.concurrent.locks.ReentrantReadWriteLock newReentrantReadWriteLock(java.lang.String, boolean);
  public static <E extends java.lang.Enum<E>> com.google.common.util.concurrent.CycleDetectingLockFactory$WithExplicitOrdering<E> newInstanceWithExplicitOrdering(java.lang.Class<E>, com.google.common.util.concurrent.CycleDetectingLockFactory$Policy);
}
```

## `com.google.common.util.concurrent.CycleDetectingLockFactory$Policies`

```java
public abstract class com.google.common.util.concurrent.CycleDetectingLockFactory$Policies extends java.lang.Enum<com.google.common.util.concurrent.CycleDetectingLockFactory$Policies> implements com.google.common.util.concurrent.CycleDetectingLockFactory$Policy {
  public static com.google.common.util.concurrent.CycleDetectingLockFactory$Policies[] values();
  public static com.google.common.util.concurrent.CycleDetectingLockFactory$Policies valueOf(java.lang.String);
}
```

## `com.google.common.util.concurrent.CycleDetectingLockFactory$Policy`

```java
public interface com.google.common.util.concurrent.CycleDetectingLockFactory$Policy {
  public abstract void handlePotentialDeadlock(com.google.common.util.concurrent.CycleDetectingLockFactory$PotentialDeadlockException);
}
```

## `com.google.common.util.concurrent.CycleDetectingLockFactory$PotentialDeadlockException`

```java
public final class com.google.common.util.concurrent.CycleDetectingLockFactory$PotentialDeadlockException extends com.google.common.util.concurrent.CycleDetectingLockFactory$ExampleStackTrace {
  public com.google.common.util.concurrent.CycleDetectingLockFactory$ExampleStackTrace getConflictingStackTrace();
  public java.lang.String getMessage();
}
```

## `com.google.common.util.concurrent.CycleDetectingLockFactory$WithExplicitOrdering`

```java
public final class com.google.common.util.concurrent.CycleDetectingLockFactory$WithExplicitOrdering<E extends java.lang.Enum<E>> extends com.google.common.util.concurrent.CycleDetectingLockFactory {
  public java.util.concurrent.locks.ReentrantLock newReentrantLock(E);
  public java.util.concurrent.locks.ReentrantLock newReentrantLock(E, boolean);
  public java.util.concurrent.locks.ReentrantReadWriteLock newReentrantReadWriteLock(E);
  public java.util.concurrent.locks.ReentrantReadWriteLock newReentrantReadWriteLock(E, boolean);
}
```

## `com.google.common.util.concurrent.ExecutionError`

```java
public class com.google.common.util.concurrent.ExecutionError extends java.lang.Error {
  public com.google.common.util.concurrent.ExecutionError(java.lang.String, java.lang.Error);
  public com.google.common.util.concurrent.ExecutionError(java.lang.Error);
}
```

## `com.google.common.util.concurrent.ExecutionList`

```java
public final class com.google.common.util.concurrent.ExecutionList {
  public com.google.common.util.concurrent.ExecutionList();
  public void add(java.lang.Runnable, java.util.concurrent.Executor);
  public void execute();
}
```

## `com.google.common.util.concurrent.ExecutionSequencer`

```java
public final class com.google.common.util.concurrent.ExecutionSequencer {
  public static com.google.common.util.concurrent.ExecutionSequencer create();
  public <T> com.google.common.util.concurrent.ListenableFuture<T> submit(java.util.concurrent.Callable<T>, java.util.concurrent.Executor);
  public <T> com.google.common.util.concurrent.ListenableFuture<T> submitAsync(com.google.common.util.concurrent.AsyncCallable<T>, java.util.concurrent.Executor);
}
```

## `com.google.common.util.concurrent.FakeTimeLimiter`

```java
public final class com.google.common.util.concurrent.FakeTimeLimiter implements com.google.common.util.concurrent.TimeLimiter {
  public com.google.common.util.concurrent.FakeTimeLimiter();
  public <T> T newProxy(T, java.lang.Class<T>, long, java.util.concurrent.TimeUnit);
  public <T> T callWithTimeout(java.util.concurrent.Callable<T>, long, java.util.concurrent.TimeUnit) throws java.util.concurrent.ExecutionException;
  public <T> T callUninterruptiblyWithTimeout(java.util.concurrent.Callable<T>, long, java.util.concurrent.TimeUnit) throws java.util.concurrent.ExecutionException;
  public void runWithTimeout(java.lang.Runnable, long, java.util.concurrent.TimeUnit);
  public void runUninterruptiblyWithTimeout(java.lang.Runnable, long, java.util.concurrent.TimeUnit);
}
```

## `com.google.common.util.concurrent.FluentFuture`

```java
public abstract class com.google.common.util.concurrent.FluentFuture<V> extends com.google.common.util.concurrent.GwtFluentFutureCatchingSpecialization<V> {
  public static <V> com.google.common.util.concurrent.FluentFuture<V> from(com.google.common.util.concurrent.ListenableFuture<V>);
  public static <V> com.google.common.util.concurrent.FluentFuture<V> from(com.google.common.util.concurrent.FluentFuture<V>);
  public final <X extends java.lang.Throwable> com.google.common.util.concurrent.FluentFuture<V> catching(java.lang.Class<X>, com.google.common.base.Function<? super X, ? extends V>, java.util.concurrent.Executor);
  public final <X extends java.lang.Throwable> com.google.common.util.concurrent.FluentFuture<V> catchingAsync(java.lang.Class<X>, com.google.common.util.concurrent.AsyncFunction<? super X, ? extends V>, java.util.concurrent.Executor);
  public final com.google.common.util.concurrent.FluentFuture<V> withTimeout(java.time.Duration, java.util.concurrent.ScheduledExecutorService);
  public final com.google.common.util.concurrent.FluentFuture<V> withTimeout(long, java.util.concurrent.TimeUnit, java.util.concurrent.ScheduledExecutorService);
  public final <T> com.google.common.util.concurrent.FluentFuture<T> transformAsync(com.google.common.util.concurrent.AsyncFunction<? super V, T>, java.util.concurrent.Executor);
  public final <T> com.google.common.util.concurrent.FluentFuture<T> transform(com.google.common.base.Function<? super V, T>, java.util.concurrent.Executor);
  public final void addCallback(com.google.common.util.concurrent.FutureCallback<? super V>, java.util.concurrent.Executor);
}
```

## `com.google.common.util.concurrent.ForwardingBlockingDeque`

```java
public abstract class com.google.common.util.concurrent.ForwardingBlockingDeque<E> extends com.google.common.collect.ForwardingDeque<E> implements java.util.concurrent.BlockingDeque<E> {
  public int remainingCapacity();
  public void putFirst(E) throws java.lang.InterruptedException;
  public void putLast(E) throws java.lang.InterruptedException;
  public boolean offerFirst(E, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public boolean offerLast(E, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public E takeFirst() throws java.lang.InterruptedException;
  public E takeLast() throws java.lang.InterruptedException;
  public E pollFirst(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public E pollLast(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public void put(E) throws java.lang.InterruptedException;
  public boolean offer(E, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public E take() throws java.lang.InterruptedException;
  public E poll(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public int drainTo(java.util.Collection<? super E>);
  public int drainTo(java.util.Collection<? super E>, int);
}
```

## `com.google.common.util.concurrent.ForwardingBlockingQueue`

```java
public abstract class com.google.common.util.concurrent.ForwardingBlockingQueue<E> extends com.google.common.collect.ForwardingQueue<E> implements java.util.concurrent.BlockingQueue<E> {
  public int drainTo(java.util.Collection<? super E>, int);
  public int drainTo(java.util.Collection<? super E>);
  public boolean offer(E, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public E poll(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public void put(E) throws java.lang.InterruptedException;
  public int remainingCapacity();
  public E take() throws java.lang.InterruptedException;
}
```

## `com.google.common.util.concurrent.ForwardingExecutorService`

```java
public abstract class com.google.common.util.concurrent.ForwardingExecutorService extends com.google.common.collect.ForwardingObject implements java.util.concurrent.ExecutorService {
  public boolean awaitTermination(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public <T> java.util.List<java.util.concurrent.Future<T>> invokeAll(java.util.Collection<? extends java.util.concurrent.Callable<T>>) throws java.lang.InterruptedException;
  public <T> java.util.List<java.util.concurrent.Future<T>> invokeAll(java.util.Collection<? extends java.util.concurrent.Callable<T>>, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public <T> T invokeAny(java.util.Collection<? extends java.util.concurrent.Callable<T>>) throws java.lang.InterruptedException, java.util.concurrent.ExecutionException;
  public <T> T invokeAny(java.util.Collection<? extends java.util.concurrent.Callable<T>>, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException, java.util.concurrent.ExecutionException, java.util.concurrent.TimeoutException;
  public boolean isShutdown();
  public boolean isTerminated();
  public void shutdown();
  public java.util.List<java.lang.Runnable> shutdownNow();
  public void execute(java.lang.Runnable);
  public <T> java.util.concurrent.Future<T> submit(java.util.concurrent.Callable<T>);
  public java.util.concurrent.Future<?> submit(java.lang.Runnable);
  public <T> java.util.concurrent.Future<T> submit(java.lang.Runnable, T);
}
```

## `com.google.common.util.concurrent.ForwardingFuture`

```java
public abstract class com.google.common.util.concurrent.ForwardingFuture<V> extends com.google.common.collect.ForwardingObject implements java.util.concurrent.Future<V> {
  public boolean cancel(boolean);
  public boolean isCancelled();
  public boolean isDone();
  public V get() throws java.lang.InterruptedException, java.util.concurrent.ExecutionException;
  public V get(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException, java.util.concurrent.ExecutionException, java.util.concurrent.TimeoutException;
}
```

## `com.google.common.util.concurrent.ForwardingListenableFuture`

```java
public abstract class com.google.common.util.concurrent.ForwardingListenableFuture<V> extends com.google.common.util.concurrent.ForwardingFuture<V> implements com.google.common.util.concurrent.ListenableFuture<V> {
  public void addListener(java.lang.Runnable, java.util.concurrent.Executor);
}
```

## `com.google.common.util.concurrent.ForwardingListeningExecutorService`

```java
public abstract class com.google.common.util.concurrent.ForwardingListeningExecutorService extends com.google.common.util.concurrent.ForwardingExecutorService implements com.google.common.util.concurrent.ListeningExecutorService {
  public <T> com.google.common.util.concurrent.ListenableFuture<T> submit(java.util.concurrent.Callable<T>);
  public com.google.common.util.concurrent.ListenableFuture<?> submit(java.lang.Runnable);
  public <T> com.google.common.util.concurrent.ListenableFuture<T> submit(java.lang.Runnable, T);
  public java.util.concurrent.Future submit(java.lang.Runnable, java.lang.Object);
  public java.util.concurrent.Future submit(java.lang.Runnable);
  public java.util.concurrent.Future submit(java.util.concurrent.Callable);
}
```

## `com.google.common.util.concurrent.FutureCallback`

```java
public interface com.google.common.util.concurrent.FutureCallback<V> {
  public abstract void onSuccess(V);
  public abstract void onFailure(java.lang.Throwable);
}
```

## `com.google.common.util.concurrent.Futures`

```java
public final class com.google.common.util.concurrent.Futures extends com.google.common.util.concurrent.GwtFuturesCatchingSpecialization {
  public static <V> com.google.common.util.concurrent.ListenableFuture<V> immediateFuture(V);
  public static com.google.common.util.concurrent.ListenableFuture<java.lang.Void> immediateVoidFuture();
  public static <V> com.google.common.util.concurrent.ListenableFuture<V> immediateFailedFuture(java.lang.Throwable);
  public static <V> com.google.common.util.concurrent.ListenableFuture<V> immediateCancelledFuture();
  public static <O> com.google.common.util.concurrent.ListenableFuture<O> submit(java.util.concurrent.Callable<O>, java.util.concurrent.Executor);
  public static com.google.common.util.concurrent.ListenableFuture<java.lang.Void> submit(java.lang.Runnable, java.util.concurrent.Executor);
  public static <O> com.google.common.util.concurrent.ListenableFuture<O> submitAsync(com.google.common.util.concurrent.AsyncCallable<O>, java.util.concurrent.Executor);
  public static <O> com.google.common.util.concurrent.ListenableFuture<O> scheduleAsync(com.google.common.util.concurrent.AsyncCallable<O>, java.time.Duration, java.util.concurrent.ScheduledExecutorService);
  public static <O> com.google.common.util.concurrent.ListenableFuture<O> scheduleAsync(com.google.common.util.concurrent.AsyncCallable<O>, long, java.util.concurrent.TimeUnit, java.util.concurrent.ScheduledExecutorService);
  public static <V, X extends java.lang.Throwable> com.google.common.util.concurrent.ListenableFuture<V> catching(com.google.common.util.concurrent.ListenableFuture<? extends V>, java.lang.Class<X>, com.google.common.base.Function<? super X, ? extends V>, java.util.concurrent.Executor);
  public static <V, X extends java.lang.Throwable> com.google.common.util.concurrent.ListenableFuture<V> catchingAsync(com.google.common.util.concurrent.ListenableFuture<? extends V>, java.lang.Class<X>, com.google.common.util.concurrent.AsyncFunction<? super X, ? extends V>, java.util.concurrent.Executor);
  public static <V> com.google.common.util.concurrent.ListenableFuture<V> withTimeout(com.google.common.util.concurrent.ListenableFuture<V>, java.time.Duration, java.util.concurrent.ScheduledExecutorService);
  public static <V> com.google.common.util.concurrent.ListenableFuture<V> withTimeout(com.google.common.util.concurrent.ListenableFuture<V>, long, java.util.concurrent.TimeUnit, java.util.concurrent.ScheduledExecutorService);
  public static <I, O> com.google.common.util.concurrent.ListenableFuture<O> transformAsync(com.google.common.util.concurrent.ListenableFuture<I>, com.google.common.util.concurrent.AsyncFunction<? super I, ? extends O>, java.util.concurrent.Executor);
  public static <I, O> com.google.common.util.concurrent.ListenableFuture<O> transform(com.google.common.util.concurrent.ListenableFuture<I>, com.google.common.base.Function<? super I, ? extends O>, java.util.concurrent.Executor);
  public static <I, O> java.util.concurrent.Future<O> lazyTransform(java.util.concurrent.Future<I>, com.google.common.base.Function<? super I, ? extends O>);
  public static <V> com.google.common.util.concurrent.ListenableFuture<java.util.List<V>> allAsList(com.google.common.util.concurrent.ListenableFuture<? extends V>...);
  public static <V> com.google.common.util.concurrent.ListenableFuture<java.util.List<V>> allAsList(java.lang.Iterable<? extends com.google.common.util.concurrent.ListenableFuture<? extends V>>);
  public static <V> com.google.common.util.concurrent.Futures$FutureCombiner<V> whenAllComplete(com.google.common.util.concurrent.ListenableFuture<? extends V>...);
  public static <V> com.google.common.util.concurrent.Futures$FutureCombiner<V> whenAllComplete(java.lang.Iterable<? extends com.google.common.util.concurrent.ListenableFuture<? extends V>>);
  public static <V> com.google.common.util.concurrent.Futures$FutureCombiner<V> whenAllSucceed(com.google.common.util.concurrent.ListenableFuture<? extends V>...);
  public static <V> com.google.common.util.concurrent.Futures$FutureCombiner<V> whenAllSucceed(java.lang.Iterable<? extends com.google.common.util.concurrent.ListenableFuture<? extends V>>);
  public static <V> com.google.common.util.concurrent.ListenableFuture<V> nonCancellationPropagating(com.google.common.util.concurrent.ListenableFuture<V>);
  public static <V> com.google.common.util.concurrent.ListenableFuture<java.util.List<V>> successfulAsList(com.google.common.util.concurrent.ListenableFuture<? extends V>...);
  public static <V> com.google.common.util.concurrent.ListenableFuture<java.util.List<V>> successfulAsList(java.lang.Iterable<? extends com.google.common.util.concurrent.ListenableFuture<? extends V>>);
  public static <T> com.google.common.collect.ImmutableList<com.google.common.util.concurrent.ListenableFuture<T>> inCompletionOrder(java.lang.Iterable<? extends com.google.common.util.concurrent.ListenableFuture<? extends T>>);
  public static <V> void addCallback(com.google.common.util.concurrent.ListenableFuture<V>, com.google.common.util.concurrent.FutureCallback<? super V>, java.util.concurrent.Executor);
  public static <V> V getDone(java.util.concurrent.Future<V>) throws java.util.concurrent.ExecutionException;
  public static <V, X extends java.lang.Exception> V getChecked(java.util.concurrent.Future<V>, java.lang.Class<X>) throws X;
  public static <V, X extends java.lang.Exception> V getChecked(java.util.concurrent.Future<V>, java.lang.Class<X>, java.time.Duration) throws X;
  public static <V, X extends java.lang.Exception> V getChecked(java.util.concurrent.Future<V>, java.lang.Class<X>, long, java.util.concurrent.TimeUnit) throws X;
  public static <V> V getUnchecked(java.util.concurrent.Future<V>);
}
```

## `com.google.common.util.concurrent.Futures$FutureCombiner`

```java
public final class com.google.common.util.concurrent.Futures$FutureCombiner<V> {
  public <C> com.google.common.util.concurrent.ListenableFuture<C> callAsync(com.google.common.util.concurrent.AsyncCallable<C>, java.util.concurrent.Executor);
  public <C> com.google.common.util.concurrent.ListenableFuture<C> call(java.util.concurrent.Callable<C>, java.util.concurrent.Executor);
  public com.google.common.util.concurrent.ListenableFuture<?> run(java.lang.Runnable, java.util.concurrent.Executor);
}
```

## `com.google.common.util.concurrent.JdkFutureAdapters`

```java
public final class com.google.common.util.concurrent.JdkFutureAdapters {
  public static <V> com.google.common.util.concurrent.ListenableFuture<V> listenInPoolThread(java.util.concurrent.Future<V>);
  public static <V> com.google.common.util.concurrent.ListenableFuture<V> listenInPoolThread(java.util.concurrent.Future<V>, java.util.concurrent.Executor);
}
```

## `com.google.common.util.concurrent.ListenableFuture`

```java
public interface com.google.common.util.concurrent.ListenableFuture<V> extends java.util.concurrent.Future<V> {
  public abstract void addListener(java.lang.Runnable, java.util.concurrent.Executor);
}
```

## `com.google.common.util.concurrent.ListenableFutureTask`

```java
public class com.google.common.util.concurrent.ListenableFutureTask<V> extends java.util.concurrent.FutureTask<V> implements com.google.common.util.concurrent.ListenableFuture<V> {
  public static <V> com.google.common.util.concurrent.ListenableFutureTask<V> create(java.util.concurrent.Callable<V>);
  public static <V> com.google.common.util.concurrent.ListenableFutureTask<V> create(java.lang.Runnable, V);
  public void addListener(java.lang.Runnable, java.util.concurrent.Executor);
  public V get(long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException, java.lang.InterruptedException, java.util.concurrent.ExecutionException;
}
```

## `com.google.common.util.concurrent.ListeningExecutorService`

```java
public interface com.google.common.util.concurrent.ListeningExecutorService extends java.util.concurrent.ExecutorService {
  public abstract <T> com.google.common.util.concurrent.ListenableFuture<T> submit(java.util.concurrent.Callable<T>);
  public abstract com.google.common.util.concurrent.ListenableFuture<?> submit(java.lang.Runnable);
  public abstract <T> com.google.common.util.concurrent.ListenableFuture<T> submit(java.lang.Runnable, T);
  public abstract <T> java.util.List<java.util.concurrent.Future<T>> invokeAll(java.util.Collection<? extends java.util.concurrent.Callable<T>>) throws java.lang.InterruptedException;
  public abstract <T> java.util.List<java.util.concurrent.Future<T>> invokeAll(java.util.Collection<? extends java.util.concurrent.Callable<T>>, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public default <T> java.util.List<java.util.concurrent.Future<T>> invokeAll(java.util.Collection<? extends java.util.concurrent.Callable<T>>, java.time.Duration) throws java.lang.InterruptedException;
  public default <T> T invokeAny(java.util.Collection<? extends java.util.concurrent.Callable<T>>, java.time.Duration) throws java.lang.InterruptedException, java.util.concurrent.ExecutionException, java.util.concurrent.TimeoutException;
  public default boolean awaitTermination(java.time.Duration) throws java.lang.InterruptedException;
  public default java.util.concurrent.Future submit(java.lang.Runnable);
  public default java.util.concurrent.Future submit(java.lang.Runnable, java.lang.Object);
  public default java.util.concurrent.Future submit(java.util.concurrent.Callable);
}
```

## `com.google.common.util.concurrent.ListeningScheduledExecutorService`

```java
public interface com.google.common.util.concurrent.ListeningScheduledExecutorService extends java.util.concurrent.ScheduledExecutorService,com.google.common.util.concurrent.ListeningExecutorService {
  public abstract com.google.common.util.concurrent.ListenableScheduledFuture<?> schedule(java.lang.Runnable, long, java.util.concurrent.TimeUnit);
  public default com.google.common.util.concurrent.ListenableScheduledFuture<?> schedule(java.lang.Runnable, java.time.Duration);
  public abstract <V> com.google.common.util.concurrent.ListenableScheduledFuture<V> schedule(java.util.concurrent.Callable<V>, long, java.util.concurrent.TimeUnit);
  public default <V> com.google.common.util.concurrent.ListenableScheduledFuture<V> schedule(java.util.concurrent.Callable<V>, java.time.Duration);
  public abstract com.google.common.util.concurrent.ListenableScheduledFuture<?> scheduleAtFixedRate(java.lang.Runnable, long, long, java.util.concurrent.TimeUnit);
  public default com.google.common.util.concurrent.ListenableScheduledFuture<?> scheduleAtFixedRate(java.lang.Runnable, java.time.Duration, java.time.Duration);
  public abstract com.google.common.util.concurrent.ListenableScheduledFuture<?> scheduleWithFixedDelay(java.lang.Runnable, long, long, java.util.concurrent.TimeUnit);
  public default com.google.common.util.concurrent.ListenableScheduledFuture<?> scheduleWithFixedDelay(java.lang.Runnable, java.time.Duration, java.time.Duration);
  public default java.util.concurrent.ScheduledFuture scheduleWithFixedDelay(java.lang.Runnable, long, long, java.util.concurrent.TimeUnit);
  public default java.util.concurrent.ScheduledFuture scheduleAtFixedRate(java.lang.Runnable, long, long, java.util.concurrent.TimeUnit);
  public default java.util.concurrent.ScheduledFuture schedule(java.util.concurrent.Callable, long, java.util.concurrent.TimeUnit);
  public default java.util.concurrent.ScheduledFuture schedule(java.lang.Runnable, long, java.util.concurrent.TimeUnit);
}
```

## `com.google.common.util.concurrent.Monitor`

```java
public final class com.google.common.util.concurrent.Monitor {
  public com.google.common.util.concurrent.Monitor();
  public com.google.common.util.concurrent.Monitor(boolean);
  public com.google.common.util.concurrent.Monitor$Guard newGuard(java.util.function.BooleanSupplier);
  public void enter();
  public boolean enter(java.time.Duration);
  public boolean enter(long, java.util.concurrent.TimeUnit);
  public void enterInterruptibly() throws java.lang.InterruptedException;
  public boolean enterInterruptibly(java.time.Duration) throws java.lang.InterruptedException;
  public boolean enterInterruptibly(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public boolean tryEnter();
  public void enterWhen(com.google.common.util.concurrent.Monitor$Guard) throws java.lang.InterruptedException;
  public boolean enterWhen(com.google.common.util.concurrent.Monitor$Guard, java.time.Duration) throws java.lang.InterruptedException;
  public boolean enterWhen(com.google.common.util.concurrent.Monitor$Guard, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public void enterWhenUninterruptibly(com.google.common.util.concurrent.Monitor$Guard);
  public boolean enterWhenUninterruptibly(com.google.common.util.concurrent.Monitor$Guard, java.time.Duration);
  public boolean enterWhenUninterruptibly(com.google.common.util.concurrent.Monitor$Guard, long, java.util.concurrent.TimeUnit);
  public boolean enterIf(com.google.common.util.concurrent.Monitor$Guard);
  public boolean enterIf(com.google.common.util.concurrent.Monitor$Guard, java.time.Duration);
  public boolean enterIf(com.google.common.util.concurrent.Monitor$Guard, long, java.util.concurrent.TimeUnit);
  public boolean enterIfInterruptibly(com.google.common.util.concurrent.Monitor$Guard) throws java.lang.InterruptedException;
  public boolean enterIfInterruptibly(com.google.common.util.concurrent.Monitor$Guard, java.time.Duration) throws java.lang.InterruptedException;
  public boolean enterIfInterruptibly(com.google.common.util.concurrent.Monitor$Guard, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public boolean tryEnterIf(com.google.common.util.concurrent.Monitor$Guard);
  public void waitFor(com.google.common.util.concurrent.Monitor$Guard) throws java.lang.InterruptedException;
  public boolean waitFor(com.google.common.util.concurrent.Monitor$Guard, java.time.Duration) throws java.lang.InterruptedException;
  public boolean waitFor(com.google.common.util.concurrent.Monitor$Guard, long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException;
  public void waitForUninterruptibly(com.google.common.util.concurrent.Monitor$Guard);
  public boolean waitForUninterruptibly(com.google.common.util.concurrent.Monitor$Guard, java.time.Duration);
  public boolean waitForUninterruptibly(com.google.common.util.concurrent.Monitor$Guard, long, java.util.concurrent.TimeUnit);
  public void leave();
  public boolean isFair();
  public boolean isOccupied();
  public boolean isOccupiedByCurrentThread();
  public int getOccupiedDepth();
  public int getQueueLength();
  public boolean hasQueuedThreads();
  public boolean hasQueuedThread(java.lang.Thread);
  public boolean hasWaiters(com.google.common.util.concurrent.Monitor$Guard);
  public int getWaitQueueLength(com.google.common.util.concurrent.Monitor$Guard);
}
```

## `com.google.common.util.concurrent.Monitor$Guard`

```java
public abstract class com.google.common.util.concurrent.Monitor$Guard {
  public abstract boolean isSatisfied();
}
```

## `com.google.common.util.concurrent.MoreExecutors`

```java
public final class com.google.common.util.concurrent.MoreExecutors {
  public static java.util.concurrent.ExecutorService getExitingExecutorService(java.util.concurrent.ThreadPoolExecutor, java.time.Duration);
  public static java.util.concurrent.ExecutorService getExitingExecutorService(java.util.concurrent.ThreadPoolExecutor, long, java.util.concurrent.TimeUnit);
  public static java.util.concurrent.ExecutorService getExitingExecutorService(java.util.concurrent.ThreadPoolExecutor);
  public static java.util.concurrent.ScheduledExecutorService getExitingScheduledExecutorService(java.util.concurrent.ScheduledThreadPoolExecutor, java.time.Duration);
  public static java.util.concurrent.ScheduledExecutorService getExitingScheduledExecutorService(java.util.concurrent.ScheduledThreadPoolExecutor, long, java.util.concurrent.TimeUnit);
  public static java.util.concurrent.ScheduledExecutorService getExitingScheduledExecutorService(java.util.concurrent.ScheduledThreadPoolExecutor);
  public static void addDelayedShutdownHook(java.util.concurrent.ExecutorService, java.time.Duration);
  public static void addDelayedShutdownHook(java.util.concurrent.ExecutorService, long, java.util.concurrent.TimeUnit);
  public static com.google.common.util.concurrent.ListeningExecutorService newDirectExecutorService();
  public static java.util.concurrent.Executor directExecutor();
  public static java.util.concurrent.Executor newSequentialExecutor(java.util.concurrent.Executor);
  public static com.google.common.util.concurrent.ListeningExecutorService listeningDecorator(java.util.concurrent.ExecutorService);
  public static com.google.common.util.concurrent.ListeningScheduledExecutorService listeningDecorator(java.util.concurrent.ScheduledExecutorService);
  public static java.util.concurrent.ThreadFactory platformThreadFactory();
  public static boolean shutdownAndAwaitTermination(java.util.concurrent.ExecutorService, java.time.Duration);
  public static boolean shutdownAndAwaitTermination(java.util.concurrent.ExecutorService, long, java.util.concurrent.TimeUnit);
}
```

## `com.google.common.util.concurrent.RateLimiter`

```java
public abstract class com.google.common.util.concurrent.RateLimiter {
  public static com.google.common.util.concurrent.RateLimiter create(double);
  public static com.google.common.util.concurrent.RateLimiter create(double, java.time.Duration);
  public static com.google.common.util.concurrent.RateLimiter create(double, long, java.util.concurrent.TimeUnit);
  public final void setRate(double);
  public final double getRate();
  public double acquire();
  public double acquire(int);
  public boolean tryAcquire(java.time.Duration);
  public boolean tryAcquire(long, java.util.concurrent.TimeUnit);
  public boolean tryAcquire(int);
  public boolean tryAcquire();
  public boolean tryAcquire(int, java.time.Duration);
  public boolean tryAcquire(int, long, java.util.concurrent.TimeUnit);
  public java.lang.String toString();
}
```

## `com.google.common.util.concurrent.Runnables`

```java
public final class com.google.common.util.concurrent.Runnables {
  public static java.lang.Runnable doNothing();
}
```

## `com.google.common.util.concurrent.Service`

```java
public interface com.google.common.util.concurrent.Service {
  public abstract com.google.common.util.concurrent.Service startAsync();
  public abstract boolean isRunning();
  public abstract com.google.common.util.concurrent.Service$State state();
  public abstract com.google.common.util.concurrent.Service stopAsync();
  public abstract void awaitRunning();
  public default void awaitRunning(java.time.Duration) throws java.util.concurrent.TimeoutException;
  public abstract void awaitRunning(long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException;
  public abstract void awaitTerminated();
  public default void awaitTerminated(java.time.Duration) throws java.util.concurrent.TimeoutException;
  public abstract void awaitTerminated(long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException;
  public abstract java.lang.Throwable failureCause();
  public abstract void addListener(com.google.common.util.concurrent.Service$Listener, java.util.concurrent.Executor);
}
```

## `com.google.common.util.concurrent.Service$Listener`

```java
public abstract class com.google.common.util.concurrent.Service$Listener {
  public com.google.common.util.concurrent.Service$Listener();
  public void starting();
  public void running();
  public void stopping(com.google.common.util.concurrent.Service$State);
  public void terminated(com.google.common.util.concurrent.Service$State);
  public void failed(com.google.common.util.concurrent.Service$State, java.lang.Throwable);
}
```

## `com.google.common.util.concurrent.Service$State`

```java
public final class com.google.common.util.concurrent.Service$State extends java.lang.Enum<com.google.common.util.concurrent.Service$State> {
  public static com.google.common.util.concurrent.Service$State[] values();
  public static com.google.common.util.concurrent.Service$State valueOf(java.lang.String);
}
```

## `com.google.common.util.concurrent.ServiceManager`

```java
public final class com.google.common.util.concurrent.ServiceManager implements com.google.common.util.concurrent.ServiceManagerBridge {
  public com.google.common.util.concurrent.ServiceManager(java.lang.Iterable<? extends com.google.common.util.concurrent.Service>);
  public void addListener(com.google.common.util.concurrent.ServiceManager$Listener, java.util.concurrent.Executor);
  public com.google.common.util.concurrent.ServiceManager startAsync();
  public void awaitHealthy();
  public void awaitHealthy(java.time.Duration) throws java.util.concurrent.TimeoutException;
  public void awaitHealthy(long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException;
  public com.google.common.util.concurrent.ServiceManager stopAsync();
  public void awaitStopped();
  public void awaitStopped(java.time.Duration) throws java.util.concurrent.TimeoutException;
  public void awaitStopped(long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException;
  public boolean isHealthy();
  public com.google.common.collect.ImmutableSetMultimap<com.google.common.util.concurrent.Service$State, com.google.common.util.concurrent.Service> servicesByState();
  public com.google.common.collect.ImmutableMap<com.google.common.util.concurrent.Service, java.lang.Long> startupTimes();
  public com.google.common.collect.ImmutableMap<com.google.common.util.concurrent.Service, java.time.Duration> startupDurations();
  public java.lang.String toString();
  public com.google.common.collect.ImmutableMultimap servicesByState();
}
```

## `com.google.common.util.concurrent.ServiceManager$Listener`

```java
public abstract class com.google.common.util.concurrent.ServiceManager$Listener {
  public com.google.common.util.concurrent.ServiceManager$Listener();
  public void healthy();
  public void stopped();
  public void failure(com.google.common.util.concurrent.Service);
}
```

## `com.google.common.util.concurrent.SettableFuture`

```java
public final class com.google.common.util.concurrent.SettableFuture<V> extends com.google.common.util.concurrent.AbstractFuture$TrustedFuture<V> {
  public static <V> com.google.common.util.concurrent.SettableFuture<V> create();
  public boolean set(V);
  public boolean setException(java.lang.Throwable);
  public boolean setFuture(com.google.common.util.concurrent.ListenableFuture<? extends V>);
}
```

## `com.google.common.util.concurrent.SimpleTimeLimiter`

```java
public final class com.google.common.util.concurrent.SimpleTimeLimiter implements com.google.common.util.concurrent.TimeLimiter {
  public static com.google.common.util.concurrent.SimpleTimeLimiter create(java.util.concurrent.ExecutorService);
  public <T> T newProxy(T, java.lang.Class<T>, long, java.util.concurrent.TimeUnit);
  public <T> T callWithTimeout(java.util.concurrent.Callable<T>, long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException, java.lang.InterruptedException, java.util.concurrent.ExecutionException;
  public <T> T callUninterruptiblyWithTimeout(java.util.concurrent.Callable<T>, long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException, java.util.concurrent.ExecutionException;
  public void runWithTimeout(java.lang.Runnable, long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException, java.lang.InterruptedException;
  public void runUninterruptiblyWithTimeout(java.lang.Runnable, long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException;
}
```

## `com.google.common.util.concurrent.Striped`

```java
public abstract class com.google.common.util.concurrent.Striped<L> {
  public abstract L get(java.lang.Object);
  public abstract L getAt(int);
  public abstract int size();
  public java.lang.Iterable<L> bulkGet(java.lang.Iterable<? extends java.lang.Object>);
  public static com.google.common.util.concurrent.Striped<java.util.concurrent.locks.Lock> lock(int);
  public static com.google.common.util.concurrent.Striped<java.util.concurrent.locks.Lock> lazyWeakLock(int);
  public static com.google.common.util.concurrent.Striped<java.util.concurrent.Semaphore> semaphore(int, int);
  public static com.google.common.util.concurrent.Striped<java.util.concurrent.Semaphore> lazyWeakSemaphore(int, int);
  public static com.google.common.util.concurrent.Striped<java.util.concurrent.locks.ReadWriteLock> readWriteLock(int);
  public static com.google.common.util.concurrent.Striped<java.util.concurrent.locks.ReadWriteLock> lazyWeakReadWriteLock(int);
}
```

## `com.google.common.util.concurrent.ThreadFactoryBuilder`

```java
public final class com.google.common.util.concurrent.ThreadFactoryBuilder {
  public com.google.common.util.concurrent.ThreadFactoryBuilder();
  public com.google.common.util.concurrent.ThreadFactoryBuilder setNameFormat(java.lang.String);
  public com.google.common.util.concurrent.ThreadFactoryBuilder setDaemon(boolean);
  public com.google.common.util.concurrent.ThreadFactoryBuilder setPriority(int);
  public com.google.common.util.concurrent.ThreadFactoryBuilder setUncaughtExceptionHandler(java.lang.Thread$UncaughtExceptionHandler);
  public com.google.common.util.concurrent.ThreadFactoryBuilder setThreadFactory(java.util.concurrent.ThreadFactory);
  public java.util.concurrent.ThreadFactory build();
}
```

## `com.google.common.util.concurrent.TimeLimiter`

```java
public interface com.google.common.util.concurrent.TimeLimiter {
  public abstract <T> T newProxy(T, java.lang.Class<T>, long, java.util.concurrent.TimeUnit);
  public default <T> T newProxy(T, java.lang.Class<T>, java.time.Duration);
  public abstract <T> T callWithTimeout(java.util.concurrent.Callable<T>, long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException, java.lang.InterruptedException, java.util.concurrent.ExecutionException;
  public default <T> T callWithTimeout(java.util.concurrent.Callable<T>, java.time.Duration) throws java.util.concurrent.TimeoutException, java.lang.InterruptedException, java.util.concurrent.ExecutionException;
  public abstract <T> T callUninterruptiblyWithTimeout(java.util.concurrent.Callable<T>, long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException, java.util.concurrent.ExecutionException;
  public default <T> T callUninterruptiblyWithTimeout(java.util.concurrent.Callable<T>, java.time.Duration) throws java.util.concurrent.TimeoutException, java.util.concurrent.ExecutionException;
  public abstract void runWithTimeout(java.lang.Runnable, long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException, java.lang.InterruptedException;
  public default void runWithTimeout(java.lang.Runnable, java.time.Duration) throws java.util.concurrent.TimeoutException, java.lang.InterruptedException;
  public abstract void runUninterruptiblyWithTimeout(java.lang.Runnable, long, java.util.concurrent.TimeUnit) throws java.util.concurrent.TimeoutException;
  public default void runUninterruptiblyWithTimeout(java.lang.Runnable, java.time.Duration) throws java.util.concurrent.TimeoutException;
}
```

## `com.google.common.util.concurrent.UncaughtExceptionHandlers`

```java
public final class com.google.common.util.concurrent.UncaughtExceptionHandlers {
  public static java.lang.Thread$UncaughtExceptionHandler systemExit();
}
```

## `com.google.common.util.concurrent.UncheckedExecutionException`

```java
public class com.google.common.util.concurrent.UncheckedExecutionException extends java.lang.RuntimeException {
  public com.google.common.util.concurrent.UncheckedExecutionException(java.lang.String, java.lang.Throwable);
  public com.google.common.util.concurrent.UncheckedExecutionException(java.lang.Throwable);
}
```

## `com.google.common.util.concurrent.UncheckedTimeoutException`

```java
public class com.google.common.util.concurrent.UncheckedTimeoutException extends java.lang.RuntimeException {
  public com.google.common.util.concurrent.UncheckedTimeoutException();
  public com.google.common.util.concurrent.UncheckedTimeoutException(java.lang.String);
  public com.google.common.util.concurrent.UncheckedTimeoutException(java.lang.Throwable);
  public com.google.common.util.concurrent.UncheckedTimeoutException(java.lang.String, java.lang.Throwable);
}
```

## `com.google.common.util.concurrent.Uninterruptibles`

```java
public final class com.google.common.util.concurrent.Uninterruptibles {
  public static void awaitUninterruptibly(java.util.concurrent.CountDownLatch);
  public static boolean awaitUninterruptibly(java.util.concurrent.CountDownLatch, java.time.Duration);
  public static boolean awaitUninterruptibly(java.util.concurrent.CountDownLatch, long, java.util.concurrent.TimeUnit);
  public static boolean awaitUninterruptibly(java.util.concurrent.locks.Condition, java.time.Duration);
  public static boolean awaitUninterruptibly(java.util.concurrent.locks.Condition, long, java.util.concurrent.TimeUnit);
  public static void joinUninterruptibly(java.lang.Thread);
  public static void joinUninterruptibly(java.lang.Thread, java.time.Duration);
  public static void joinUninterruptibly(java.lang.Thread, long, java.util.concurrent.TimeUnit);
  public static <V> V getUninterruptibly(java.util.concurrent.Future<V>) throws java.util.concurrent.ExecutionException;
  public static <V> V getUninterruptibly(java.util.concurrent.Future<V>, java.time.Duration) throws java.util.concurrent.ExecutionException, java.util.concurrent.TimeoutException;
  public static <V> V getUninterruptibly(java.util.concurrent.Future<V>, long, java.util.concurrent.TimeUnit) throws java.util.concurrent.ExecutionException, java.util.concurrent.TimeoutException;
  public static <E> E takeUninterruptibly(java.util.concurrent.BlockingQueue<E>);
  public static <E> void putUninterruptibly(java.util.concurrent.BlockingQueue<E>, E);
  public static void sleepUninterruptibly(java.time.Duration);
  public static void sleepUninterruptibly(long, java.util.concurrent.TimeUnit);
  public static boolean tryAcquireUninterruptibly(java.util.concurrent.Semaphore, java.time.Duration);
  public static boolean tryAcquireUninterruptibly(java.util.concurrent.Semaphore, long, java.util.concurrent.TimeUnit);
  public static boolean tryAcquireUninterruptibly(java.util.concurrent.Semaphore, int, java.time.Duration);
  public static boolean tryAcquireUninterruptibly(java.util.concurrent.Semaphore, int, long, java.util.concurrent.TimeUnit);
  public static boolean tryLockUninterruptibly(java.util.concurrent.locks.Lock, java.time.Duration);
  public static boolean tryLockUninterruptibly(java.util.concurrent.locks.Lock, long, java.util.concurrent.TimeUnit);
  public static void awaitTerminationUninterruptibly(java.util.concurrent.ExecutorService);
  public static boolean awaitTerminationUninterruptibly(java.util.concurrent.ExecutorService, java.time.Duration);
  public static boolean awaitTerminationUninterruptibly(java.util.concurrent.ExecutorService, long, java.util.concurrent.TimeUnit);
}
```
