# com.feilong.accessor

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.accessor.Accessor` | `T get(String key,HttpServletRequest request)` | 获取. |
| `com.feilong.accessor.Accessor` | `void remove(String key,HttpServletRequest request)` | 删除保存的key. |
| `com.feilong.accessor.AutoKeyAccessor` | `String save(Serializable serializable,HttpServletRequest request)` | 将对象 serializable 保存起来. key自动生成 |
| `com.feilong.accessor.KeyAccessor` | `void save(String key,Serializable serializable,HttpServletRequest request)` | 保存. |
