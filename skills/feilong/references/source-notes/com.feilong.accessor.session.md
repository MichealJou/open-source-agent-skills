# com.feilong.accessor.session

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.accessor.session.AbstractSessionKeyAccessor` | `T get(String key,HttpServletRequest request)` | 获得. |
| `com.feilong.accessor.session.AbstractSessionKeyAccessor` | `void remove(String key,HttpServletRequest request)` | 删除. |
| `com.feilong.accessor.session.SessionAccessor` | `String getKey()` | 获得 key. |
| `com.feilong.accessor.session.SessionAccessor` | `T get(HttpServletRequest request)` | 获得. |
| `com.feilong.accessor.session.SessionAccessor` | `void remove(HttpServletRequest request)` | 删除. |
| `com.feilong.accessor.session.SessionAccessor` | `void save(Serializable serializable,HttpServletRequest request)` | 【原文待译】Save. |
| `com.feilong.accessor.session.SessionAccessor` | `void setKey(String key)` | 设置 key. |
| `com.feilong.accessor.session.SessionAutoKeyAccessor` | `String save(Serializable serializable,HttpServletRequest request)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.accessor.session.SessionAutoKeyAccessor` | `void setKeyGenerator(KeyGenerator keyGenerator)` | 设置 key generator. |
| `com.feilong.accessor.session.SessionKeyAccessor` | `void save(String key,Serializable serializable,HttpServletRequest request)` | 【原文待译】Save. |
