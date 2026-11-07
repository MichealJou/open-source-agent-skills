# com.google.common.cache

版本：33.4.8-jre。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.google.common.cache.AbstractCache`

```java
public abstract class com.google.common.cache.AbstractCache<K, V> implements com.google.common.cache.Cache<K, V> {
  public V get(K, java.util.concurrent.Callable<? extends V>) throws java.util.concurrent.ExecutionException;
  public com.google.common.collect.ImmutableMap<K, V> getAllPresent(java.lang.Iterable<? extends java.lang.Object>);
  public void put(K, V);
  public void putAll(java.util.Map<? extends K, ? extends V>);
  public void cleanUp();
  public long size();
  public void invalidate(java.lang.Object);
  public void invalidateAll(java.lang.Iterable<? extends java.lang.Object>);
  public void invalidateAll();
  public com.google.common.cache.CacheStats stats();
  public java.util.concurrent.ConcurrentMap<K, V> asMap();
}
```

## `com.google.common.cache.AbstractCache$SimpleStatsCounter`

```java
public final class com.google.common.cache.AbstractCache$SimpleStatsCounter implements com.google.common.cache.AbstractCache$StatsCounter {
  public com.google.common.cache.AbstractCache$SimpleStatsCounter();
  public void recordHits(int);
  public void recordMisses(int);
  public void recordLoadSuccess(long);
  public void recordLoadException(long);
  public void recordEviction();
  public com.google.common.cache.CacheStats snapshot();
  public void incrementBy(com.google.common.cache.AbstractCache$StatsCounter);
}
```

## `com.google.common.cache.AbstractCache$StatsCounter`

```java
public interface com.google.common.cache.AbstractCache$StatsCounter {
  public abstract void recordHits(int);
  public abstract void recordMisses(int);
  public abstract void recordLoadSuccess(long);
  public abstract void recordLoadException(long);
  public abstract void recordEviction();
  public abstract com.google.common.cache.CacheStats snapshot();
}
```

## `com.google.common.cache.AbstractLoadingCache`

```java
public abstract class com.google.common.cache.AbstractLoadingCache<K, V> extends com.google.common.cache.AbstractCache<K, V> implements com.google.common.cache.LoadingCache<K, V> {
  public V getUnchecked(K);
  public com.google.common.collect.ImmutableMap<K, V> getAll(java.lang.Iterable<? extends K>) throws java.util.concurrent.ExecutionException;
  public final V apply(K);
  public void refresh(K);
}
```

## `com.google.common.cache.Cache`

```java
public interface com.google.common.cache.Cache<K, V> {
  public abstract V getIfPresent(java.lang.Object);
  public abstract V get(K, java.util.concurrent.Callable<? extends V>) throws java.util.concurrent.ExecutionException;
  public abstract com.google.common.collect.ImmutableMap<K, V> getAllPresent(java.lang.Iterable<? extends java.lang.Object>);
  public abstract void put(K, V);
  public abstract void putAll(java.util.Map<? extends K, ? extends V>);
  public abstract void invalidate(java.lang.Object);
  public abstract void invalidateAll(java.lang.Iterable<? extends java.lang.Object>);
  public abstract void invalidateAll();
  public abstract long size();
  public abstract com.google.common.cache.CacheStats stats();
  public abstract java.util.concurrent.ConcurrentMap<K, V> asMap();
  public abstract void cleanUp();
}
```

## `com.google.common.cache.CacheBuilder`

```java
public final class com.google.common.cache.CacheBuilder<K, V> {
  public static com.google.common.cache.CacheBuilder<java.lang.Object, java.lang.Object> newBuilder();
  public static com.google.common.cache.CacheBuilder<java.lang.Object, java.lang.Object> from(com.google.common.cache.CacheBuilderSpec);
  public static com.google.common.cache.CacheBuilder<java.lang.Object, java.lang.Object> from(java.lang.String);
  public com.google.common.cache.CacheBuilder<K, V> initialCapacity(int);
  public com.google.common.cache.CacheBuilder<K, V> concurrencyLevel(int);
  public com.google.common.cache.CacheBuilder<K, V> maximumSize(long);
  public com.google.common.cache.CacheBuilder<K, V> maximumWeight(long);
  public <K1 extends K, V1 extends V> com.google.common.cache.CacheBuilder<K1, V1> weigher(com.google.common.cache.Weigher<? super K1, ? super V1>);
  public com.google.common.cache.CacheBuilder<K, V> weakKeys();
  public com.google.common.cache.CacheBuilder<K, V> weakValues();
  public com.google.common.cache.CacheBuilder<K, V> softValues();
  public com.google.common.cache.CacheBuilder<K, V> expireAfterWrite(java.time.Duration);
  public com.google.common.cache.CacheBuilder<K, V> expireAfterWrite(long, java.util.concurrent.TimeUnit);
  public com.google.common.cache.CacheBuilder<K, V> expireAfterAccess(java.time.Duration);
  public com.google.common.cache.CacheBuilder<K, V> expireAfterAccess(long, java.util.concurrent.TimeUnit);
  public com.google.common.cache.CacheBuilder<K, V> refreshAfterWrite(java.time.Duration);
  public com.google.common.cache.CacheBuilder<K, V> refreshAfterWrite(long, java.util.concurrent.TimeUnit);
  public com.google.common.cache.CacheBuilder<K, V> ticker(com.google.common.base.Ticker);
  public <K1 extends K, V1 extends V> com.google.common.cache.CacheBuilder<K1, V1> removalListener(com.google.common.cache.RemovalListener<? super K1, ? super V1>);
  public com.google.common.cache.CacheBuilder<K, V> recordStats();
  public <K1 extends K, V1 extends V> com.google.common.cache.LoadingCache<K1, V1> build(com.google.common.cache.CacheLoader<? super K1, V1>);
  public <K1 extends K, V1 extends V> com.google.common.cache.Cache<K1, V1> build();
  public java.lang.String toString();
}
```

## `com.google.common.cache.CacheBuilderSpec`

```java
public final class com.google.common.cache.CacheBuilderSpec {
  public static com.google.common.cache.CacheBuilderSpec parse(java.lang.String);
  public static com.google.common.cache.CacheBuilderSpec disableCaching();
  public java.lang.String toParsableString();
  public java.lang.String toString();
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```

## `com.google.common.cache.CacheLoader`

```java
public abstract class com.google.common.cache.CacheLoader<K, V> {
  public abstract V load(K) throws java.lang.Exception;
  public com.google.common.util.concurrent.ListenableFuture<V> reload(K, V) throws java.lang.Exception;
  public java.util.Map<K, V> loadAll(java.lang.Iterable<? extends K>) throws java.lang.Exception;
  public static <K, V> com.google.common.cache.CacheLoader<K, V> from(com.google.common.base.Function<K, V>);
  public static <V> com.google.common.cache.CacheLoader<java.lang.Object, V> from(com.google.common.base.Supplier<V>);
  public static <K, V> com.google.common.cache.CacheLoader<K, V> asyncReloading(com.google.common.cache.CacheLoader<K, V>, java.util.concurrent.Executor);
}
```

## `com.google.common.cache.CacheLoader$InvalidCacheLoadException`

```java
public final class com.google.common.cache.CacheLoader$InvalidCacheLoadException extends java.lang.RuntimeException {
  public com.google.common.cache.CacheLoader$InvalidCacheLoadException(java.lang.String);
}
```

## `com.google.common.cache.CacheStats`

```java
public final class com.google.common.cache.CacheStats {
  public com.google.common.cache.CacheStats(long, long, long, long, long, long);
  public long requestCount();
  public long hitCount();
  public double hitRate();
  public long missCount();
  public double missRate();
  public long loadCount();
  public long loadSuccessCount();
  public long loadExceptionCount();
  public double loadExceptionRate();
  public long totalLoadTime();
  public double averageLoadPenalty();
  public long evictionCount();
  public com.google.common.cache.CacheStats minus(com.google.common.cache.CacheStats);
  public com.google.common.cache.CacheStats plus(com.google.common.cache.CacheStats);
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
}
```

## `com.google.common.cache.ForwardingCache`

```java
public abstract class com.google.common.cache.ForwardingCache<K, V> extends com.google.common.collect.ForwardingObject implements com.google.common.cache.Cache<K, V> {
  public V getIfPresent(java.lang.Object);
  public V get(K, java.util.concurrent.Callable<? extends V>) throws java.util.concurrent.ExecutionException;
  public com.google.common.collect.ImmutableMap<K, V> getAllPresent(java.lang.Iterable<? extends java.lang.Object>);
  public void put(K, V);
  public void putAll(java.util.Map<? extends K, ? extends V>);
  public void invalidate(java.lang.Object);
  public void invalidateAll(java.lang.Iterable<? extends java.lang.Object>);
  public void invalidateAll();
  public long size();
  public com.google.common.cache.CacheStats stats();
  public java.util.concurrent.ConcurrentMap<K, V> asMap();
  public void cleanUp();
}
```

## `com.google.common.cache.ForwardingLoadingCache`

```java
public abstract class com.google.common.cache.ForwardingLoadingCache<K, V> extends com.google.common.cache.ForwardingCache<K, V> implements com.google.common.cache.LoadingCache<K, V> {
  public V get(K) throws java.util.concurrent.ExecutionException;
  public V getUnchecked(K);
  public com.google.common.collect.ImmutableMap<K, V> getAll(java.lang.Iterable<? extends K>) throws java.util.concurrent.ExecutionException;
  public V apply(K);
  public void refresh(K);
}
```

## `com.google.common.cache.LoadingCache`

```java
public interface com.google.common.cache.LoadingCache<K, V> extends com.google.common.cache.Cache<K, V>, com.google.common.base.Function<K, V> {
  public abstract V get(K) throws java.util.concurrent.ExecutionException;
  public abstract V getUnchecked(K);
  public abstract com.google.common.collect.ImmutableMap<K, V> getAll(java.lang.Iterable<? extends K>) throws java.util.concurrent.ExecutionException;
  public abstract V apply(K);
  public abstract void refresh(K);
  public abstract java.util.concurrent.ConcurrentMap<K, V> asMap();
}
```

## `com.google.common.cache.RemovalCause`

```java
public abstract class com.google.common.cache.RemovalCause extends java.lang.Enum<com.google.common.cache.RemovalCause> {
  public static com.google.common.cache.RemovalCause[] values();
  public static com.google.common.cache.RemovalCause valueOf(java.lang.String);
}
```

## `com.google.common.cache.RemovalListener`

```java
public interface com.google.common.cache.RemovalListener<K, V> {
  public abstract void onRemoval(com.google.common.cache.RemovalNotification<K, V>);
}
```

## `com.google.common.cache.RemovalListeners`

```java
public final class com.google.common.cache.RemovalListeners {
  public static <K, V> com.google.common.cache.RemovalListener<K, V> asynchronous(com.google.common.cache.RemovalListener<K, V>, java.util.concurrent.Executor);
}
```

## `com.google.common.cache.RemovalNotification`

```java
public final class com.google.common.cache.RemovalNotification<K, V> extends java.util.AbstractMap$SimpleImmutableEntry<K, V> {
  public static <K, V> com.google.common.cache.RemovalNotification<K, V> create(K, V, com.google.common.cache.RemovalCause);
  public com.google.common.cache.RemovalCause getCause();
  public boolean wasEvicted();
}
```

## `com.google.common.cache.Weigher`

```java
public interface com.google.common.cache.Weigher<K, V> {
  public abstract int weigh(K, V);
}
```
