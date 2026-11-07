# com.baomidou.mybatisplus.core.incrementer

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.incrementer.DefaultIdentifierGenerator`

```java
public class com.baomidou.mybatisplus.core.incrementer.DefaultIdentifierGenerator implements com.baomidou.mybatisplus.core.incrementer.IdentifierGenerator {
  public com.baomidou.mybatisplus.core.incrementer.DefaultIdentifierGenerator();
  public com.baomidou.mybatisplus.core.incrementer.DefaultIdentifierGenerator(java.net.InetAddress);
  public com.baomidou.mybatisplus.core.incrementer.DefaultIdentifierGenerator(long, long);
  public com.baomidou.mybatisplus.core.incrementer.DefaultIdentifierGenerator(com.baomidou.mybatisplus.core.toolkit.Sequence);
  public static com.baomidou.mybatisplus.core.incrementer.IdentifierGenerator getFixedIdentifierGenerator(org.apache.ibatis.logging.Log);
  public java.lang.Long nextId(java.lang.Object);
  public static com.baomidou.mybatisplus.core.incrementer.DefaultIdentifierGenerator getInstance();
  public java.lang.Number nextId(java.lang.Object);
}
```

## `com.baomidou.mybatisplus.core.incrementer.IKeyGenerator`

```java
public interface com.baomidou.mybatisplus.core.incrementer.IKeyGenerator {
  public abstract java.lang.String executeSql(java.lang.String);
  public abstract com.baomidou.mybatisplus.annotation.DbType dbType();
}
```

## `com.baomidou.mybatisplus.core.incrementer.IdentifierGenerator`

```java
public interface com.baomidou.mybatisplus.core.incrementer.IdentifierGenerator {
  public default boolean assignId(java.lang.Object);
  public abstract java.lang.Number nextId(java.lang.Object);
  public default java.lang.String nextUUID(java.lang.Object);
}
```

## `com.baomidou.mybatisplus.core.incrementer.ImadcnIdentifierGenerator`

```java
public class com.baomidou.mybatisplus.core.incrementer.ImadcnIdentifierGenerator implements com.baomidou.mybatisplus.core.incrementer.IdentifierGenerator,java.io.Closeable {
  public com.baomidou.mybatisplus.core.incrementer.ImadcnIdentifierGenerator(java.lang.String);
  public com.baomidou.mybatisplus.core.incrementer.ImadcnIdentifierGenerator(com.imadcn.framework.idworker.config.ZookeeperConfiguration);
  public com.baomidou.mybatisplus.core.incrementer.ImadcnIdentifierGenerator(com.imadcn.framework.idworker.config.ZookeeperConfiguration, com.imadcn.framework.idworker.config.ApplicationConfiguration);
  public java.lang.Number nextId(java.lang.Object);
  public java.lang.String nextUUID(java.lang.Object);
  public void close() throws java.io.IOException;
}
```
