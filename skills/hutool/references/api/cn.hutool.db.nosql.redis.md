# cn.hutool.db.nosql.redis

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.db.nosql.redis.RedisDS`

```java
public class cn.hutool.db.nosql.redis.RedisDS implements java.io.Closeable,java.io.Serializable {
  public static cn.hutool.db.nosql.redis.RedisDS create();
  public static cn.hutool.db.nosql.redis.RedisDS create(java.lang.String);
  public static cn.hutool.db.nosql.redis.RedisDS create(cn.hutool.setting.Setting, java.lang.String);
  public cn.hutool.db.nosql.redis.RedisDS();
  public cn.hutool.db.nosql.redis.RedisDS(java.lang.String);
  public cn.hutool.db.nosql.redis.RedisDS(cn.hutool.setting.Setting, java.lang.String);
  public cn.hutool.db.nosql.redis.RedisDS init(java.lang.String);
  public redis.clients.jedis.JedisPool getPool();
  public cn.hutool.setting.Setting getSetting();
  public java.lang.String getGroup();
  public redis.clients.jedis.Jedis getJedis();
  public java.lang.String getStr(java.lang.String);
  public java.lang.String setStr(java.lang.String, java.lang.String);
  public java.lang.Long del(java.lang.String...);
  public void close();
}
```
