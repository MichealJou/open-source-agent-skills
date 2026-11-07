# cn.hutool.core.lang.generator

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.lang.generator.Generator`

```java
public interface cn.hutool.core.lang.generator.Generator<T> {
  public abstract T next();
}
```

## `cn.hutool.core.lang.generator.ObjectGenerator`

```java
public class cn.hutool.core.lang.generator.ObjectGenerator<T> implements cn.hutool.core.lang.generator.Generator<T> {
  public cn.hutool.core.lang.generator.ObjectGenerator(java.lang.Class<T>);
  public T next();
}
```

## `cn.hutool.core.lang.generator.ObjectIdGenerator`

```java
public class cn.hutool.core.lang.generator.ObjectIdGenerator implements cn.hutool.core.lang.generator.Generator<java.lang.String> {
  public cn.hutool.core.lang.generator.ObjectIdGenerator();
  public java.lang.String next();
  public java.lang.Object next();
}
```

## `cn.hutool.core.lang.generator.SnowflakeGenerator`

```java
public class cn.hutool.core.lang.generator.SnowflakeGenerator implements cn.hutool.core.lang.generator.Generator<java.lang.Long> {
  public cn.hutool.core.lang.generator.SnowflakeGenerator();
  public cn.hutool.core.lang.generator.SnowflakeGenerator(long, long);
  public java.lang.Long next();
  public java.lang.Object next();
}
```

## `cn.hutool.core.lang.generator.UUIDGenerator`

```java
public class cn.hutool.core.lang.generator.UUIDGenerator implements cn.hutool.core.lang.generator.Generator<java.lang.String> {
  public cn.hutool.core.lang.generator.UUIDGenerator();
  public java.lang.String next();
  public java.lang.Object next();
}
```
