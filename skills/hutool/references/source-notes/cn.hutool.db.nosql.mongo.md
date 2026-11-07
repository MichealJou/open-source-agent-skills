# cn.hutool.db.nosql.mongo

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.db.nosql.mongo.MongoDS` | `MongoClient getMongo()` | @return 获得MongoDB客户端对象 |
| `cn.hutool.db.nosql.mongo.MongoDS` | `MongoCollection<Document> getCollection(String dbName,String collectionName)` | 获得MongoDB中指定集合对象 |
| `cn.hutool.db.nosql.mongo.MongoDS` | `MongoDatabase getDb(String dbName)` | 获得DB |
| `cn.hutool.db.nosql.mongo.MongoDS` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.nosql.mongo.MongoDS` | `void init()` | 初始化，当给定分组数大于一个时使用 |
| `cn.hutool.db.nosql.mongo.MongoDS` | `void initCloud()` | 初始化集群 集群的其它客户端设定参数使用全局设定 集群中每一个实例成员用一个group表示，例如： |
| `cn.hutool.db.nosql.mongo.MongoDS` | `void initSingle()` | 初始化 设定文件中的host和端口有三种形式： |
| `cn.hutool.db.nosql.mongo.MongoDS` | `void setSetting(Setting setting)` | 设定MongoDB配置文件 |
| `cn.hutool.db.nosql.mongo.MongoFactory` | `MongoDS getDS(Collection<String> groups)` | 获取MongoDB数据源 |
| `cn.hutool.db.nosql.mongo.MongoFactory` | `MongoDS getDS(Setting setting,Collection<String> groups)` | 获取MongoDB数据源 |
| `cn.hutool.db.nosql.mongo.MongoFactory` | `MongoDS getDS(Setting setting,String... groups)` | 获取MongoDB数据源 |
| `cn.hutool.db.nosql.mongo.MongoFactory` | `MongoDS getDS(String host,int port)` | 获取MongoDB数据源 |
| `cn.hutool.db.nosql.mongo.MongoFactory` | `MongoDS getDS(String... groups)` | 获取MongoDB数据源 多个分组名对应的连接组成集群 |
| `cn.hutool.db.nosql.mongo.MongoFactory` | `void closeAll()` | 关闭全部连接 |
