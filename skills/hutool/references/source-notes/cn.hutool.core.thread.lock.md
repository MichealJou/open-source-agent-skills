# cn.hutool.core.thread.lock

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.thread.lock.LockUtil` | `Lock getLazySegmentLock(int segments,Object key)` | 根据 key 获取弱引用分段锁，懒加载 |
| `cn.hutool.core.thread.lock.LockUtil` | `Lock getSegmentLock(int segments,Object key)` | 根据 key 获取分段锁（强引用） |
| `cn.hutool.core.thread.lock.LockUtil` | `Lock getSegmentReadLock(int segments,Object key)` | 根据 key 获取分段读锁（强引用） |
| `cn.hutool.core.thread.lock.LockUtil` | `Lock getSegmentWriteLock(int segments,Object key)` | 根据 key 获取分段写锁（强引用） |
| `cn.hutool.core.thread.lock.LockUtil` | `NoLock getNoLock()` | 获取单例的无锁对象 |
| `cn.hutool.core.thread.lock.LockUtil` | `ReentrantReadWriteLock createReadWriteLock(boolean fair)` | 创建ReentrantReadWriteLock锁 |
| `cn.hutool.core.thread.lock.LockUtil` | `SegmentLock<Lock> createLazySegmentLock(int segments)` | 创建弱引用分段锁，使用 ReentrantLock，懒加载 |
| `cn.hutool.core.thread.lock.LockUtil` | `SegmentLock<Lock> createSegmentLock(int segments)` | 创建分段锁（强引用），使用 ReentrantLock |
| `cn.hutool.core.thread.lock.LockUtil` | `SegmentLock<ReadWriteLock> createSegmentReadWriteLock(int segments)` | 创建分段读写锁（强引用），使用 ReentrantReadWriteLock |
| `cn.hutool.core.thread.lock.LockUtil` | `SegmentLock<Semaphore> createSegmentSemaphore(int segments,int permits)` | 创建分段信号量（强引用） |
| `cn.hutool.core.thread.lock.LockUtil` | `Semaphore getSegmentSemaphore(int segments,int permits,Object key)` | 根据 key 获取分段信号量（强引用） |
| `cn.hutool.core.thread.lock.LockUtil` | `StampedLock createStampLock()` | 创建StampedLock锁 |
| `cn.hutool.core.thread.lock.NoLock` | `Condition newCondition()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.lock.NoLock` | `boolean tryLock()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.lock.NoLock` | `boolean tryLock(long time,TimeUnit unit)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.lock.NoLock` | `void lock()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.lock.NoLock` | `void lockInterruptibly()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.lock.NoLock` | `void unlock()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.lock.NoReadWriteLock` | `Lock readLock()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.lock.NoReadWriteLock` | `Lock writeLock()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.lock.SegmentLock` | `Iterable<L> bulkGet(Iterable<?> keys)` | 批量获取多个 key 对应的锁段列表，按索引升序排列，避免死锁。 |
| `cn.hutool.core.thread.lock.SegmentLock` | `L get(Object key)` | 根据 key 获取对应的锁段，保证相同 key 返回相同对象。 |
| `cn.hutool.core.thread.lock.SegmentLock` | `L getAt(int index)` | 根据索引获取锁段，索引范围为 [0, size())。 |
| `cn.hutool.core.thread.lock.SegmentLock` | `SegmentLock<L> custom(int stripes,Supplier<L> supplier)` | 创建强引用的分段锁，所有段在创建时初始化。 |
| `cn.hutool.core.thread.lock.SegmentLock` | `SegmentLock<Lock> lazyWeakLock(int stripes)` | 创建弱引用的可重入锁分段实例，懒加载。 |
| `cn.hutool.core.thread.lock.SegmentLock` | `SegmentLock<Lock> lock(int stripes)` | 创建强引用的可重入锁分段实例。 |
| `cn.hutool.core.thread.lock.SegmentLock` | `SegmentLock<ReadWriteLock> lazyWeakReadWriteLock(int stripes)` | 创建弱引用的读写锁分段实例，懒加载。 |
| `cn.hutool.core.thread.lock.SegmentLock` | `SegmentLock<ReadWriteLock> readWriteLock(int stripes)` | 创建强引用的读写锁分段实例。 |
| `cn.hutool.core.thread.lock.SegmentLock` | `SegmentLock<Semaphore> lazyWeakSemaphore(int stripes,int permits)` | 创建弱引用的信号量分段实例，懒加载。 |
| `cn.hutool.core.thread.lock.SegmentLock` | `SegmentLock<Semaphore> semaphore(int stripes,int permits)` | 创建强引用的信号量分段实例。 |
| `cn.hutool.core.thread.lock.SegmentLock` | `int size()` | 获取总段数。 |
