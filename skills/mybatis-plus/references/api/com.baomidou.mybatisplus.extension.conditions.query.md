# com.baomidou.mybatisplus.extension.conditions.query

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.conditions.query.ChainQuery`

```java
public interface com.baomidou.mybatisplus.extension.conditions.query.ChainQuery<T> extends com.baomidou.mybatisplus.extension.conditions.ChainWrapper<T> {
  public default java.util.List<T> list();
  public default java.util.List<T> list(com.baomidou.mybatisplus.core.metadata.IPage<T>);
  public default T one();
  public default java.util.Optional<T> oneOpt();
  public default java.lang.Long count();
  public default boolean exists();
  public default <E extends com.baomidou.mybatisplus.core.metadata.IPage<T>> E page(E);
}
```

## `com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper`

```java
public class com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T> extends com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper<T, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T>, com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T>> implements com.baomidou.mybatisplus.extension.conditions.query.ChainQuery<T>, com.baomidou.mybatisplus.core.conditions.query.Query<com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T>, T, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>> {
  public com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>);
  public com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper(java.lang.Class<T>);
  public com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, T);
  public com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, java.lang.Class<T>);
  public com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T>);
  public com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T> select(boolean, java.util.List<com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>>);
  public final com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T> select(com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>...);
  public final com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T> select(boolean, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>...);
  public com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T> select(java.lang.Class<T>, java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public java.lang.String getSqlSelect();
  public com.baomidou.mybatisplus.core.mapper.BaseMapper<T> getBaseMapper();
  public java.lang.Class<T> getEntityClass();
  public com.baomidou.mybatisplus.core.conditions.Wrapper getWrapper();
  public java.lang.Object select(java.lang.Class, java.util.function.Predicate);
  public java.lang.Object select(boolean, java.util.List);
  public java.lang.Object select(boolean, java.lang.Object[]);
  public java.lang.Object select(java.lang.Object[]);
}
```

## `com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper`

```java
public class com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper<T> extends com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper<T, java.lang.String, com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper<T>, com.baomidou.mybatisplus.core.conditions.query.QueryWrapper<T>> implements com.baomidou.mybatisplus.extension.conditions.query.ChainQuery<T>, com.baomidou.mybatisplus.core.conditions.query.Query<com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper<T>, T, java.lang.String> {
  public com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>);
  public com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper(java.lang.Class<T>);
  public com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper<T> select(boolean, java.util.List<java.lang.String>);
  public com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper<T> select(java.lang.Class<T>, java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public java.lang.String getSqlSelect();
  public com.baomidou.mybatisplus.core.mapper.BaseMapper<T> getBaseMapper();
  public java.lang.Class<T> getEntityClass();
  public com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T> lambda();
  public com.baomidou.mybatisplus.core.conditions.Wrapper getWrapper();
  public java.lang.Object select(java.lang.Class, java.util.function.Predicate);
  public java.lang.Object select(boolean, java.util.List);
}
```
