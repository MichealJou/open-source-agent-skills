# cn.hutool.db.nosql.redis

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.db.nosql.redis.RedisDS` | `Jedis getJedis()` | 从资源池中获取Jedis |
| `cn.hutool.db.nosql.redis.RedisDS` | `JedisPool getPool()` | 获取Jedis连接池 |
| `cn.hutool.db.nosql.redis.RedisDS` | `Long del(String... keys)` | 从Redis中删除多个值 |
| `cn.hutool.db.nosql.redis.RedisDS` | `RedisDS create()` | 创建RedisDS，使用默认配置文件，默认分组 |
| `cn.hutool.db.nosql.redis.RedisDS` | `RedisDS create(Setting setting,String group)` | 创建RedisDS |
| `cn.hutool.db.nosql.redis.RedisDS` | `RedisDS create(String group)` | 创建RedisDS，使用默认配置文件 |
| `cn.hutool.db.nosql.redis.RedisDS` | `RedisDS init(String group)` | 初始化Jedis客户端 |
| `cn.hutool.db.nosql.redis.RedisDS` | `Setting getSetting()` | 获取配置 |
| `cn.hutool.db.nosql.redis.RedisDS` | `String getGroup()` | 获取分组 |
| `cn.hutool.db.nosql.redis.RedisDS` | `String getStr(String key)` | 从Redis中获取值 |
| `cn.hutool.db.nosql.redis.RedisDS` | `String setStr(String key,String value)` | 从Redis中设置值 |
| `cn.hutool.db.nosql.redis.RedisDS` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
