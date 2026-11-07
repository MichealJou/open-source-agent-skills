# cn.hutool.db.nosql.mongo

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.db.nosql.mongo.MongoDS`

```java
public class cn.hutool.db.nosql.mongo.MongoDS implements java.io.Closeable {
  public cn.hutool.db.nosql.mongo.MongoDS(java.lang.String, int);
  public cn.hutool.db.nosql.mongo.MongoDS(cn.hutool.setting.Setting, java.lang.String, int);
  public cn.hutool.db.nosql.mongo.MongoDS(java.lang.String...);
  public cn.hutool.db.nosql.mongo.MongoDS(cn.hutool.setting.Setting, java.lang.String...);
  public void init();
  public synchronized void initSingle();
  public synchronized void initCloud();
  public void setSetting(cn.hutool.setting.Setting);
  public com.mongodb.client.MongoClient getMongo();
  public com.mongodb.client.MongoDatabase getDb(java.lang.String);
  public com.mongodb.client.MongoCollection<org.bson.Document> getCollection(java.lang.String, java.lang.String);
  public void close();
}
```

## `cn.hutool.db.nosql.mongo.MongoFactory`

```java
public class cn.hutool.db.nosql.mongo.MongoFactory {
  public cn.hutool.db.nosql.mongo.MongoFactory();
  public static cn.hutool.db.nosql.mongo.MongoDS getDS(java.lang.String, int);
  public static cn.hutool.db.nosql.mongo.MongoDS getDS(java.lang.String...);
  public static cn.hutool.db.nosql.mongo.MongoDS getDS(java.util.Collection<java.lang.String>);
  public static cn.hutool.db.nosql.mongo.MongoDS getDS(cn.hutool.setting.Setting, java.lang.String...);
  public static cn.hutool.db.nosql.mongo.MongoDS getDS(cn.hutool.setting.Setting, java.util.Collection<java.lang.String>);
  public static void closeAll();
}
```
