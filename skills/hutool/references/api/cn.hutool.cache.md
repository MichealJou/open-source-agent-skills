# cn.hutool.cache

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.cache.Cache`

```java
public interface cn.hutool.cache.Cache<K, V> extends java.lang.Iterable<V>, java.io.Serializable {
  public abstract int capacity();
  public abstract long timeout();
  public abstract void put(K, V);
  public abstract void put(K, V, long);
  public default V get(K);
  public default V get(K, cn.hutool.core.lang.func.Func0<V>);
  public abstract V get(K, boolean, cn.hutool.core.lang.func.Func0<V>);
  public abstract V get(K, boolean, long, cn.hutool.core.lang.func.Func0<V>);
  public abstract V get(K, boolean);
  public abstract java.util.Iterator<cn.hutool.cache.impl.CacheObj<K, V>> cacheObjIterator();
  public abstract int prune();
  public abstract boolean isFull();
  public abstract void remove(K);
  public abstract void clear();
  public abstract int size();
  public abstract boolean isEmpty();
  public abstract boolean containsKey(K);
  public default cn.hutool.cache.Cache<K, V> setListener(cn.hutool.cache.CacheListener<K, V>);
}
```

## `cn.hutool.cache.CacheListener`

```java
public interface cn.hutool.cache.CacheListener<K, V> {
  public abstract void onRemove(K, V);
}
```

## `cn.hutool.cache.CacheUtil`

```java
public class cn.hutool.cache.CacheUtil {
  public cn.hutool.cache.CacheUtil();
  public static <K, V> cn.hutool.cache.impl.FIFOCache<K, V> newFIFOCache(int, long);
  public static <K, V> cn.hutool.cache.impl.FIFOCache<K, V> newFIFOCache(int);
  public static <K, V> cn.hutool.cache.impl.LFUCache<K, V> newLFUCache(int, long);
  public static <K, V> cn.hutool.cache.impl.LFUCache<K, V> newLFUCache(int);
  public static <K, V> cn.hutool.cache.impl.LRUCache<K, V> newLRUCache(int, long);
  public static <K, V> cn.hutool.cache.impl.LRUCache<K, V> newLRUCache(int);
  public static <K, V> cn.hutool.cache.impl.TimedCache<K, V> newTimedCache(long, long);
  public static <K, V> cn.hutool.cache.impl.TimedCache<K, V> newTimedCache(long);
  public static <K, V> cn.hutool.cache.impl.WeakCache<K, V> newWeakCache(long);
  public static <K, V> cn.hutool.cache.impl.NoCache<K, V> newNoCache();
}
```

## `cn.hutool.cache.GlobalPruneTimer`

```java
public final class cn.hutool.cache.GlobalPruneTimer extends java.lang.Enum<cn.hutool.cache.GlobalPruneTimer> {
  public static cn.hutool.cache.GlobalPruneTimer[] values();
  public static cn.hutool.cache.GlobalPruneTimer valueOf(java.lang.String);
  public java.util.concurrent.ScheduledFuture<?> schedule(java.lang.Runnable, long);
  public void create();
  public void shutdown();
  public java.util.List<java.lang.Runnable> shutdownNow();
}
```
