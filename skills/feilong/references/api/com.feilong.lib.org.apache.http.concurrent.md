# com.feilong.lib.org.apache.http.concurrent

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.concurrent.BasicFuture`

```java
public class com.feilong.lib.org.apache.http.concurrent.BasicFuture<T> implements java.util.concurrent.Future<T>, com.feilong.lib.org.apache.http.concurrent.Cancellable {
  public com.feilong.lib.org.apache.http.concurrent.BasicFuture(com.feilong.lib.org.apache.http.concurrent.FutureCallback<T>);
  public boolean isCancelled();
  public boolean isDone();
  public synchronized T get() throws java.lang.InterruptedException, java.util.concurrent.ExecutionException;
  public synchronized T get(long, java.util.concurrent.TimeUnit) throws java.lang.InterruptedException, java.util.concurrent.ExecutionException, java.util.concurrent.TimeoutException;
  public boolean completed(T);
  public boolean failed(java.lang.Exception);
  public boolean cancel(boolean);
  public boolean cancel();
}
```

## `com.feilong.lib.org.apache.http.concurrent.Cancellable`

```java
public interface com.feilong.lib.org.apache.http.concurrent.Cancellable {
  public abstract boolean cancel();
}
```

## `com.feilong.lib.org.apache.http.concurrent.FutureCallback`

```java
public interface com.feilong.lib.org.apache.http.concurrent.FutureCallback<T> {
  public abstract void completed(T);
  public abstract void failed(java.lang.Exception);
  public abstract void cancelled();
}
```
