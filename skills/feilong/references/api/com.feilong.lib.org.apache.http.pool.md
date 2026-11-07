# com.feilong.lib.org.apache.http.pool

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.pool.AbstractConnPool`

```java
public abstract class com.feilong.lib.org.apache.http.pool.AbstractConnPool<T, C, E extends com.feilong.lib.org.apache.http.pool.PoolEntry<T, C>> implements com.feilong.lib.org.apache.http.pool.ConnPool<T, E>, com.feilong.lib.org.apache.http.pool.ConnPoolControl<T> {
  public com.feilong.lib.org.apache.http.pool.AbstractConnPool(com.feilong.lib.org.apache.http.pool.ConnFactory<T, C>, int, int);
  public boolean isShutdown();
  public void shutdown() throws java.io.IOException;
  public java.util.concurrent.Future<E> lease(T, java.lang.Object, com.feilong.lib.org.apache.http.concurrent.FutureCallback<E>);
  public java.util.concurrent.Future<E> lease(T, java.lang.Object);
  public void release(E, boolean);
  public void setMaxTotal(int);
  public int getMaxTotal();
  public void setDefaultMaxPerRoute(int);
  public int getDefaultMaxPerRoute();
  public void setMaxPerRoute(T, int);
  public int getMaxPerRoute(T);
  public com.feilong.lib.org.apache.http.pool.PoolStats getTotalStats();
  public com.feilong.lib.org.apache.http.pool.PoolStats getStats(T);
  public java.util.Set<T> getRoutes();
  public void closeIdle(long, java.util.concurrent.TimeUnit);
  public void closeExpired();
  public int getValidateAfterInactivity();
  public void setValidateAfterInactivity(int);
  public java.lang.String toString();
  public void release(java.lang.Object, boolean);
}
```

## `com.feilong.lib.org.apache.http.pool.ConnFactory`

```java
public interface com.feilong.lib.org.apache.http.pool.ConnFactory<T, C> {
  public abstract C create(T) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.pool.ConnPool`

```java
public interface com.feilong.lib.org.apache.http.pool.ConnPool<T, E> {
  public abstract java.util.concurrent.Future<E> lease(T, java.lang.Object, com.feilong.lib.org.apache.http.concurrent.FutureCallback<E>);
  public abstract void release(E, boolean);
}
```

## `com.feilong.lib.org.apache.http.pool.ConnPoolControl`

```java
public interface com.feilong.lib.org.apache.http.pool.ConnPoolControl<T> {
  public abstract void setMaxTotal(int);
  public abstract int getMaxTotal();
  public abstract void setDefaultMaxPerRoute(int);
  public abstract int getDefaultMaxPerRoute();
  public abstract void setMaxPerRoute(T, int);
  public abstract int getMaxPerRoute(T);
  public abstract com.feilong.lib.org.apache.http.pool.PoolStats getTotalStats();
  public abstract com.feilong.lib.org.apache.http.pool.PoolStats getStats(T);
}
```

## `com.feilong.lib.org.apache.http.pool.PoolEntry`

```java
public abstract class com.feilong.lib.org.apache.http.pool.PoolEntry<T, C> {
  public com.feilong.lib.org.apache.http.pool.PoolEntry(java.lang.String, T, C, long, java.util.concurrent.TimeUnit);
  public com.feilong.lib.org.apache.http.pool.PoolEntry(java.lang.String, T, C);
  public java.lang.String getId();
  public T getRoute();
  public C getConnection();
  public long getCreated();
  public long getValidityDeadline();
  public java.lang.Object getState();
  public void setState(java.lang.Object);
  public synchronized long getUpdated();
  public synchronized long getExpiry();
  public synchronized void updateExpiry(long, java.util.concurrent.TimeUnit);
  public synchronized boolean isExpired(long);
  public abstract void close();
  public abstract boolean isClosed();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.pool.PoolEntryCallback`

```java
public interface com.feilong.lib.org.apache.http.pool.PoolEntryCallback<T, C> {
  public abstract void process(com.feilong.lib.org.apache.http.pool.PoolEntry<T, C>);
}
```

## `com.feilong.lib.org.apache.http.pool.PoolStats`

```java
public class com.feilong.lib.org.apache.http.pool.PoolStats implements java.io.Serializable {
  public com.feilong.lib.org.apache.http.pool.PoolStats(int, int, int, int);
  public int getLeased();
  public int getPending();
  public int getAvailable();
  public int getMax();
  public java.lang.String toString();
}
```
