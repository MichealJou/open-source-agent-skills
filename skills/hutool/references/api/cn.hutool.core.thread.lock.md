# cn.hutool.core.thread.lock

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.thread.lock.LockUtil`

```java
public class cn.hutool.core.thread.lock.LockUtil {
  public cn.hutool.core.thread.lock.LockUtil();
  public static java.util.concurrent.locks.StampedLock createStampLock();
  public static java.util.concurrent.locks.ReentrantReadWriteLock createReadWriteLock(boolean);
  public static cn.hutool.core.thread.lock.NoLock getNoLock();
  public static cn.hutool.core.thread.lock.SegmentLock<java.util.concurrent.locks.Lock> createSegmentLock(int);
  public static cn.hutool.core.thread.lock.SegmentLock<java.util.concurrent.locks.ReadWriteLock> createSegmentReadWriteLock(int);
  public static cn.hutool.core.thread.lock.SegmentLock<java.util.concurrent.Semaphore> createSegmentSemaphore(int, int);
  public static cn.hutool.core.thread.lock.SegmentLock<java.util.concurrent.locks.Lock> createLazySegmentLock(int);
  public static java.util.concurrent.locks.Lock getSegmentLock(int, java.lang.Object);
  public static java.util.concurrent.locks.Lock getSegmentReadLock(int, java.lang.Object);
  public static java.util.concurrent.locks.Lock getSegmentWriteLock(int, java.lang.Object);
  public static java.util.concurrent.Semaphore getSegmentSemaphore(int, int, java.lang.Object);
  public static java.util.concurrent.locks.Lock getLazySegmentLock(int, java.lang.Object);
}
```

## `cn.hutool.core.thread.lock.NoLock`

```java
public class cn.hutool.core.thread.lock.NoLock implements java.util.concurrent.locks.Lock {
  public cn.hutool.core.thread.lock.NoLock();
  public void lock();
  public void lockInterruptibly();
  public boolean tryLock();
  public boolean tryLock(long, java.util.concurrent.TimeUnit);
  public void unlock();
  public java.util.concurrent.locks.Condition newCondition();
}
```

## `cn.hutool.core.thread.lock.NoReadWriteLock`

```java
public class cn.hutool.core.thread.lock.NoReadWriteLock implements java.util.concurrent.locks.ReadWriteLock {
  public cn.hutool.core.thread.lock.NoReadWriteLock();
  public java.util.concurrent.locks.Lock readLock();
  public java.util.concurrent.locks.Lock writeLock();
}
```

## `cn.hutool.core.thread.lock.SegmentLock`

```java
public abstract class cn.hutool.core.thread.lock.SegmentLock<L> {
  public abstract L get(java.lang.Object);
  public abstract L getAt(int);
  public abstract int size();
  public java.lang.Iterable<L> bulkGet(java.lang.Iterable<?>);
  public static <L> cn.hutool.core.thread.lock.SegmentLock<L> custom(int, java.util.function.Supplier<L>);
  public static cn.hutool.core.thread.lock.SegmentLock<java.util.concurrent.locks.Lock> lock(int);
  public static cn.hutool.core.thread.lock.SegmentLock<java.util.concurrent.locks.Lock> lazyWeakLock(int);
  public static cn.hutool.core.thread.lock.SegmentLock<java.util.concurrent.Semaphore> semaphore(int, int);
  public static cn.hutool.core.thread.lock.SegmentLock<java.util.concurrent.Semaphore> lazyWeakSemaphore(int, int);
  public static cn.hutool.core.thread.lock.SegmentLock<java.util.concurrent.locks.ReadWriteLock> readWriteLock(int);
  public static cn.hutool.core.thread.lock.SegmentLock<java.util.concurrent.locks.ReadWriteLock> lazyWeakReadWriteLock(int);
}
```
