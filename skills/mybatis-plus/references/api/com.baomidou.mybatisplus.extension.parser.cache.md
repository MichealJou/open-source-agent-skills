# com.baomidou.mybatisplus.extension.parser.cache

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.parser.cache.AbstractCaffeineJsqlParseCache`

```java
public abstract class com.baomidou.mybatisplus.extension.parser.cache.AbstractCaffeineJsqlParseCache implements com.baomidou.mybatisplus.extension.parser.cache.JsqlParseCache {
  public com.baomidou.mybatisplus.extension.parser.cache.AbstractCaffeineJsqlParseCache(com.github.benmanes.caffeine.cache.Cache<java.lang.String, byte[]>);
  public com.baomidou.mybatisplus.extension.parser.cache.AbstractCaffeineJsqlParseCache(java.util.function.Consumer<com.github.benmanes.caffeine.cache.Caffeine<java.lang.Object, java.lang.Object>>);
  public void putStatement(java.lang.String, net.sf.jsqlparser.statement.Statement);
  public void putStatements(java.lang.String, net.sf.jsqlparser.statement.Statements);
  public net.sf.jsqlparser.statement.Statement getStatement(java.lang.String);
  public net.sf.jsqlparser.statement.Statements getStatements(java.lang.String);
  public abstract byte[] serialize(java.lang.Object);
  public abstract java.lang.Object deserialize(java.lang.String, byte[]);
  public void setAsync(boolean);
  public void setExecutor(java.util.concurrent.Executor);
}
```

## `com.baomidou.mybatisplus.extension.parser.cache.FstFactory`

```java
public class com.baomidou.mybatisplus.extension.parser.cache.FstFactory {
  public static com.baomidou.mybatisplus.extension.parser.cache.FstFactory getDefaultFactory();
  public com.baomidou.mybatisplus.extension.parser.cache.FstFactory();
  public byte[] asByteArray(java.lang.Object);
  public java.lang.Object asObject(byte[]);
}
```

## `com.baomidou.mybatisplus.extension.parser.cache.FstSerialCaffeineJsqlParseCache`

```java
public class com.baomidou.mybatisplus.extension.parser.cache.FstSerialCaffeineJsqlParseCache extends com.baomidou.mybatisplus.extension.parser.cache.AbstractCaffeineJsqlParseCache {
  public com.baomidou.mybatisplus.extension.parser.cache.FstSerialCaffeineJsqlParseCache(com.github.benmanes.caffeine.cache.Cache<java.lang.String, byte[]>);
  public com.baomidou.mybatisplus.extension.parser.cache.FstSerialCaffeineJsqlParseCache(java.util.function.Consumer<com.github.benmanes.caffeine.cache.Caffeine<java.lang.Object, java.lang.Object>>);
  public byte[] serialize(java.lang.Object);
  public java.lang.Object deserialize(java.lang.String, byte[]);
}
```

## `com.baomidou.mybatisplus.extension.parser.cache.FuryFactory`

```java
public final class com.baomidou.mybatisplus.extension.parser.cache.FuryFactory {
  public com.baomidou.mybatisplus.extension.parser.cache.FuryFactory();
  public static com.baomidou.mybatisplus.extension.parser.cache.FuryFactory getFuryFactory();
  public byte[] serialize(java.lang.Object);
  public java.lang.Object deserialize(byte[]);
}
```

## `com.baomidou.mybatisplus.extension.parser.cache.FurySerialCaffeineJsqlParseCache`

```java
public class com.baomidou.mybatisplus.extension.parser.cache.FurySerialCaffeineJsqlParseCache extends com.baomidou.mybatisplus.extension.parser.cache.AbstractCaffeineJsqlParseCache {
  public com.baomidou.mybatisplus.extension.parser.cache.FurySerialCaffeineJsqlParseCache(com.github.benmanes.caffeine.cache.Cache<java.lang.String, byte[]>);
  public com.baomidou.mybatisplus.extension.parser.cache.FurySerialCaffeineJsqlParseCache(java.util.function.Consumer<com.github.benmanes.caffeine.cache.Caffeine<java.lang.Object, java.lang.Object>>);
  public byte[] serialize(java.lang.Object);
  public java.lang.Object deserialize(java.lang.String, byte[]);
}
```

## `com.baomidou.mybatisplus.extension.parser.cache.JdkSerialCaffeineJsqlParseCache`

```java
public class com.baomidou.mybatisplus.extension.parser.cache.JdkSerialCaffeineJsqlParseCache extends com.baomidou.mybatisplus.extension.parser.cache.AbstractCaffeineJsqlParseCache {
  public com.baomidou.mybatisplus.extension.parser.cache.JdkSerialCaffeineJsqlParseCache(com.github.benmanes.caffeine.cache.Cache<java.lang.String, byte[]>);
  public com.baomidou.mybatisplus.extension.parser.cache.JdkSerialCaffeineJsqlParseCache(java.util.function.Consumer<com.github.benmanes.caffeine.cache.Caffeine<java.lang.Object, java.lang.Object>>);
  public byte[] serialize(java.lang.Object);
  public java.lang.Object deserialize(java.lang.String, byte[]);
}
```

## `com.baomidou.mybatisplus.extension.parser.cache.JsqlParseCache`

```java
public interface com.baomidou.mybatisplus.extension.parser.cache.JsqlParseCache {
  public abstract void putStatement(java.lang.String, net.sf.jsqlparser.statement.Statement);
  public abstract void putStatements(java.lang.String, net.sf.jsqlparser.statement.Statements);
  public abstract net.sf.jsqlparser.statement.Statement getStatement(java.lang.String);
  public abstract net.sf.jsqlparser.statement.Statements getStatements(java.lang.String);
}
```
