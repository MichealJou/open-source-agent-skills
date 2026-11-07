# cn.hutool.cache.impl

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.cache.impl.AbstractCache`

```java
public abstract class cn.hutool.cache.impl.AbstractCache<K, V> implements cn.hutool.cache.Cache<K, V> {
  public cn.hutool.cache.impl.AbstractCache();
  public void put(K, V);
  public long getHitCount();
  public long getMissCount();
  public V get(K, boolean, cn.hutool.core.lang.func.Func0<V>);
  public V get(K, boolean, long, cn.hutool.core.lang.func.Func0<V>);
  public java.util.Iterator<V> iterator();
  public int capacity();
  public long timeout();
  public boolean isFull();
  public int size();
  public boolean isEmpty();
  public java.lang.String toString();
  public cn.hutool.cache.impl.AbstractCache<K, V> setListener(cn.hutool.cache.CacheListener<K, V>);
  public java.util.Set<K> keySet();
  public cn.hutool.cache.Cache setListener(cn.hutool.cache.CacheListener);
}
```

## `cn.hutool.cache.impl.CacheObj`

```java
public class cn.hutool.cache.impl.CacheObj<K, V> implements java.io.Serializable {
  public K getKey();
  public V getValue();
  public long getTtl();
  public java.util.Date getExpiredTime();
  public long getLastAccess();
  public java.lang.String toString();
}
```

## `cn.hutool.cache.impl.CacheObjIterator`

```java
public class cn.hutool.cache.impl.CacheObjIterator<K, V> implements java.util.Iterator<cn.hutool.cache.impl.CacheObj<K, V>>, java.io.Serializable {
  public boolean hasNext();
  public cn.hutool.cache.impl.CacheObj<K, V> next();
  public void remove();
  public java.lang.Object next();
}
```

## `cn.hutool.cache.impl.CacheValuesIterator`

```java
public class cn.hutool.cache.impl.CacheValuesIterator<V> implements java.util.Iterator<V>, java.io.Serializable {
  public boolean hasNext();
  public V next();
  public void remove();
}
```

## `cn.hutool.cache.impl.FIFOCache`

```java
public class cn.hutool.cache.impl.FIFOCache<K, V> extends cn.hutool.cache.impl.ReentrantCache<K, V> {
  public cn.hutool.cache.impl.FIFOCache(int);
  public cn.hutool.cache.impl.FIFOCache(int, long);
}
```

## `cn.hutool.cache.impl.LFUCache`

```java
public class cn.hutool.cache.impl.LFUCache<K, V> extends cn.hutool.cache.impl.ReentrantCache<K, V> {
  public cn.hutool.cache.impl.LFUCache(int);
  public cn.hutool.cache.impl.LFUCache(int, long);
}
```

## `cn.hutool.cache.impl.LRUCache`

```java
public class cn.hutool.cache.impl.LRUCache<K, V> extends cn.hutool.cache.impl.ReentrantCache<K, V> {
  public cn.hutool.cache.impl.LRUCache(int);
  public cn.hutool.cache.impl.LRUCache(int, long);
}
```

## `cn.hutool.cache.impl.NoCache`

```java
public class cn.hutool.cache.impl.NoCache<K, V> implements cn.hutool.cache.Cache<K, V> {
  public cn.hutool.cache.impl.NoCache();
  public int capacity();
  public long timeout();
  public void put(K, V);
  public void put(K, V, long);
  public boolean containsKey(K);
  public V get(K);
  public V get(K, boolean);
  public V get(K, cn.hutool.core.lang.func.Func0<V>);
  public V get(K, boolean, cn.hutool.core.lang.func.Func0<V>);
  public V get(K, boolean, long, cn.hutool.core.lang.func.Func0<V>);
  public java.util.Iterator<V> iterator();
  public java.util.Iterator<cn.hutool.cache.impl.CacheObj<K, V>> cacheObjIterator();
  public int prune();
  public boolean isFull();
  public void remove(K);
  public void clear();
  public int size();
  public boolean isEmpty();
}
```

## `cn.hutool.cache.impl.ReentrantCache`

```java
public abstract class cn.hutool.cache.impl.ReentrantCache<K, V> extends cn.hutool.cache.impl.AbstractCache<K, V> {
  public cn.hutool.cache.impl.ReentrantCache();
  public void put(K, V, long);
  public boolean containsKey(K);
  public V get(K, boolean);
  public V get(K, boolean, long, cn.hutool.core.lang.func.Func0<V>);
  public java.util.Iterator<cn.hutool.cache.impl.CacheObj<K, V>> cacheObjIterator();
  public final int prune();
  public void remove(K);
  public void clear();
  public java.lang.String toString();
}
```

## `cn.hutool.cache.impl.StampedCache`

```java
public abstract class cn.hutool.cache.impl.StampedCache<K, V> extends cn.hutool.cache.impl.AbstractCache<K, V> {
  public cn.hutool.cache.impl.StampedCache();
  public void put(K, V, long);
  public boolean containsKey(K);
  public V get(K, boolean);
  public java.util.Iterator<cn.hutool.cache.impl.CacheObj<K, V>> cacheObjIterator();
  public final int prune();
  public void remove(K);
  public void clear();
}
```

## `cn.hutool.cache.impl.TimedCache`

```java
public class cn.hutool.cache.impl.TimedCache<K, V> extends cn.hutool.cache.impl.ReentrantCache<K, V> {
  public cn.hutool.cache.impl.TimedCache(long);
  public cn.hutool.cache.impl.TimedCache(long, java.util.Map<cn.hutool.core.lang.mutable.Mutable<K>, cn.hutool.cache.impl.CacheObj<K, V>>);
  public void schedulePrune(long);
  public void cancelPruneSchedule();
}
```

## `cn.hutool.cache.impl.WeakCache`

```java
public class cn.hutool.cache.impl.WeakCache<K, V> extends cn.hutool.cache.impl.TimedCache<K, V> {
  public cn.hutool.cache.impl.WeakCache(long);
  public cn.hutool.cache.impl.WeakCache<K, V> setListener(cn.hutool.cache.CacheListener<K, V>);
  public cn.hutool.cache.impl.AbstractCache setListener(cn.hutool.cache.CacheListener);
  public cn.hutool.cache.Cache setListener(cn.hutool.cache.CacheListener);
}
```
