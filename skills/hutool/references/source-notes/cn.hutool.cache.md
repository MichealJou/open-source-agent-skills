# cn.hutool.cache

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.cache.Cache` | `Cache<K, V> setListener(CacheListener<K, V> listener)` | 设置监听 |
| `cn.hutool.cache.Cache` | `Iterator<CacheObj<K, V>> cacheObjIterator()` | 返回包含键和值得迭代器 |
| `cn.hutool.cache.Cache` | `V get(K key)` | 从缓存中获得对象，当对象不在缓存中或已经过期返回null 调用此方法时，会检查上次调用时间，如果与当前时间差值大于超时时间返回null，否则返回值。 每次调用此方法会刷新最后访问时间，也就是说会重新计算超时时间。 |
| `cn.hutool.cache.Cache` | `V get(K key,Func0<V> supplier)` | 从缓存中获得对象，当对象不在缓存中或已经过期返回Func0回调产生的对象 调用此方法时，会检查上次调用时间，如果与当前时间差值大于超时时间返回返回supplier回调产生的对象，否则返回值。 每次调用此方法会刷新最后访问时间，也就是说会重新计算超时时间。 |
| `cn.hutool.cache.Cache` | `V get(K key,boolean isUpdateLastAccess)` | 从缓存中获得对象，当对象不在缓存中或已经过期返回null 调用此方法时，会检查上次调用时间，如果与当前时间差值大于超时时间返回null，否则返回值。 每次调用此方法会可选是否刷新最后访问时间，true表示会重新计算超时时间。 |
| `cn.hutool.cache.Cache` | `V get(K key,boolean isUpdateLastAccess,Func0<V> supplier)` | 从缓存中获得对象，当对象不在缓存中或已经过期返回Func0回调产生的对象 调用此方法时，会检查上次调用时间，如果与当前时间差值大于超时时间返回supplier回调产生的对象，否则返回值。 每次调用此方法会可选是否刷新最后访问时间，true表示会重新计算超时时间。 |
| `cn.hutool.cache.Cache` | `V get(K key,boolean isUpdateLastAccess,long timeout,Func0<V> supplier)` | 从缓存中获得对象，当对象不在缓存中或已经过期返回Func0回调产生的对象 调用此方法时，会检查上次调用时间，如果与当前时间差值大于超时时间返回supplier回调产生的对象，否则返回值。 每次调用此方法会可选是否刷新最后访问时间，true表示会重新计算超时时间。 |
| `cn.hutool.cache.Cache` | `boolean containsKey(K key)` | 是否包含key |
| `cn.hutool.cache.Cache` | `boolean isEmpty()` | 缓存是否为空 |
| `cn.hutool.cache.Cache` | `boolean isFull()` | 缓存是否已满，仅用于有空间限制的缓存对象 |
| `cn.hutool.cache.Cache` | `int capacity()` | 返回缓存容量，0表示无大小限制 |
| `cn.hutool.cache.Cache` | `int prune()` | 从缓存中清理过期对象，清理策略取决于具体实现 |
| `cn.hutool.cache.Cache` | `int size()` | 缓存的对象数量 |
| `cn.hutool.cache.Cache` | `long timeout()` | 缓存失效时长， 0 表示没有设置，单位毫秒 |
| `cn.hutool.cache.Cache` | `void clear()` | 清空缓存 |
| `cn.hutool.cache.Cache` | `void put(K key,V object)` | 将对象加入到缓存，使用默认失效时长 |
| `cn.hutool.cache.Cache` | `void put(K key,V object,long timeout)` | 将对象加入到缓存，使用指定失效时长 如果缓存空间满了，#prune() 将被调用以获得空间来存放新对象 |
| `cn.hutool.cache.Cache` | `void remove(K key)` | 从缓存中移除对象 |
| `cn.hutool.cache.CacheListener` | `void onRemove(K key,V cachedObject)` | 对象移除回调 |
| `cn.hutool.cache.CacheUtil` | `FIFOCache<K, V> newFIFOCache(int capacity)` | 创建FIFO(first in first out) 先进先出缓存. |
| `cn.hutool.cache.CacheUtil` | `FIFOCache<K, V> newFIFOCache(int capacity,long timeout)` | 创建FIFO(first in first out) 先进先出缓存. |
| `cn.hutool.cache.CacheUtil` | `LFUCache<K, V> newLFUCache(int capacity)` | 创建LFU(least frequently used) 最少使用率缓存. |
| `cn.hutool.cache.CacheUtil` | `LFUCache<K, V> newLFUCache(int capacity,long timeout)` | 创建LFU(least frequently used) 最少使用率缓存. |
| `cn.hutool.cache.CacheUtil` | `LRUCache<K, V> newLRUCache(int capacity)` | 创建LRU (least recently used)最近最久未使用缓存. |
| `cn.hutool.cache.CacheUtil` | `LRUCache<K, V> newLRUCache(int capacity,long timeout)` | 创建LRU (least recently used)最近最久未使用缓存. |
| `cn.hutool.cache.CacheUtil` | `NoCache<K, V> newNoCache()` | 创建无缓存实现. |
| `cn.hutool.cache.CacheUtil` | `TimedCache<K, V> newTimedCache(long timeout)` | 创建定时缓存. |
| `cn.hutool.cache.CacheUtil` | `TimedCache<K, V> newTimedCache(long timeout,long schedulePruneDelay)` | 创建定时缓存，通过定时任务自动清除过期缓存对象 |
| `cn.hutool.cache.CacheUtil` | `WeakCache<K, V> newWeakCache(long timeout)` | 创建弱引用缓存. |
| `cn.hutool.cache.GlobalPruneTimer` | `List<Runnable> shutdownNow()` | 销毁全局定时器 |
| `cn.hutool.cache.GlobalPruneTimer` | `ScheduledFuture<?> schedule(Runnable task,long delay)` | 启动定时任务 |
| `cn.hutool.cache.GlobalPruneTimer` | `void create()` | 创建定时器 |
| `cn.hutool.cache.GlobalPruneTimer` | `void shutdown()` | 销毁全局定时器 |
