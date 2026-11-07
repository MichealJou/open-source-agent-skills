# cn.hutool.cache.impl

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.cache.impl.AbstractCache` | `AbstractCache<K, V> setListener(CacheListener<K, V> listener)` | 设置监听 |
| `cn.hutool.cache.impl.AbstractCache` | `Iterator<V> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.AbstractCache` | `Set<K> keySet()` | 返回所有键 |
| `cn.hutool.cache.impl.AbstractCache` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.AbstractCache` | `V get(K key,boolean isUpdateLastAccess,Func0<V> supplier)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.AbstractCache` | `V get(K key,boolean isUpdateLastAccess,long timeout,Func0<V> supplier)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.AbstractCache` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.AbstractCache` | `boolean isFull()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.AbstractCache` | `int capacity()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.AbstractCache` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.AbstractCache` | `long getHitCount()` | @return 命中数 |
| `cn.hutool.cache.impl.AbstractCache` | `long getMissCount()` | @return 丢失数 |
| `cn.hutool.cache.impl.AbstractCache` | `long timeout()` | @return 默认缓存失效时长。 每个对象可以单独设置失效时长 |
| `cn.hutool.cache.impl.AbstractCache` | `void put(K key,V object)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.CacheObj` | `Date getExpiredTime()` | 获取过期时间，返回null表示永不过期 |
| `cn.hutool.cache.impl.CacheObj` | `K getKey()` | 获取键 |
| `cn.hutool.cache.impl.CacheObj` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.CacheObj` | `V getValue()` | 获取值 |
| `cn.hutool.cache.impl.CacheObj` | `long getLastAccess()` | 获取上次访问时间 |
| `cn.hutool.cache.impl.CacheObj` | `long getTtl()` | 获取对象存活时长，即超时总时长，0表示无限 |
| `cn.hutool.cache.impl.CacheObjIterator` | `CacheObj<K, V> next()` | @return 下一个值 |
| `cn.hutool.cache.impl.CacheObjIterator` | `boolean hasNext()` | @return 是否有下一个值 |
| `cn.hutool.cache.impl.CacheObjIterator` | `void remove()` | 从缓存中移除没有过期的当前值，此方法不支持 |
| `cn.hutool.cache.impl.CacheValuesIterator` | `V next()` | @return 下一个值 |
| `cn.hutool.cache.impl.CacheValuesIterator` | `boolean hasNext()` | @return 是否有下一个值 |
| `cn.hutool.cache.impl.CacheValuesIterator` | `void remove()` | 从缓存中移除没有过期的当前值，不支持此方法 |
| `cn.hutool.cache.impl.NoCache` | `Iterator<CacheObj<K, V>> cacheObjIterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `Iterator<V> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `V get(K key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `V get(K key,Func0<V> supplier)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `V get(K key,boolean isUpdateLastAccess)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `V get(K key,boolean isUpdateLastAccess,Func0<V> supplier)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `V get(K key,boolean isUpdateLastAccess,long timeout,Func0<V> supplier)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `boolean containsKey(K key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `boolean isFull()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `int capacity()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `int prune()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `long timeout()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `void put(K key,V object)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `void put(K key,V object,long timeout)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.NoCache` | `void remove(K key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.ReentrantCache` | `Iterator<CacheObj<K, V>> cacheObjIterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.ReentrantCache` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.ReentrantCache` | `V get(K key,boolean isUpdateLastAccess)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.ReentrantCache` | `V get(final K key,final boolean isUpdateLastAccess,final long timeout,final Func0<V> valueFactory)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.ReentrantCache` | `boolean containsKey(K key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.ReentrantCache` | `int prune()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.ReentrantCache` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.ReentrantCache` | `void put(K key,V object,long timeout)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.ReentrantCache` | `void remove(K key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.StampedCache` | `Iterator<CacheObj<K, V>> cacheObjIterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.StampedCache` | `V get(K key,boolean isUpdateLastAccess)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.StampedCache` | `boolean containsKey(K key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.StampedCache` | `int prune()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.StampedCache` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.StampedCache` | `void put(K key,V object,long timeout)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.StampedCache` | `void remove(K key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cache.impl.TimedCache` | `void cancelPruneSchedule()` | 取消定时清理 |
| `cn.hutool.cache.impl.TimedCache` | `void schedulePrune(long delay)` | 定时清理 |
| `cn.hutool.cache.impl.WeakCache` | `WeakCache<K, V> setListener(CacheListener<K, V> listener)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
