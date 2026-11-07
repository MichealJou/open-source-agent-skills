# com.baomidou.mybatisplus.extension.conditions.update

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.conditions.update.ChainUpdate`

```java
public interface com.baomidou.mybatisplus.extension.conditions.update.ChainUpdate<T> extends com.baomidou.mybatisplus.extension.conditions.ChainWrapper<T> {
  public default boolean update();
  public default boolean update(T);
  public default boolean remove();
}
```

## `com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper`

```java
public class com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper<T> extends com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper<T, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper<T>, com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper<T>> implements com.baomidou.mybatisplus.extension.conditions.update.ChainUpdate<T>, com.baomidou.mybatisplus.core.conditions.update.Update<com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper<T>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>> {
  public com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>);
  public com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper(java.lang.Class<T>);
  public com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper<T>);
  public com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper<T> set(boolean, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, java.lang.Object, java.lang.String);
  public com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper<T> setSql(boolean, java.lang.String, java.lang.Object...);
  public com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper<T> setIncrBy(boolean, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, java.lang.Number);
  public com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper<T> setDecrBy(boolean, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, java.lang.Number);
  public com.baomidou.mybatisplus.core.mapper.BaseMapper<T> getBaseMapper();
  public java.lang.Class<T> getEntityClass();
  public com.baomidou.mybatisplus.core.conditions.Wrapper getWrapper();
  public java.lang.Object setDecrBy(boolean, java.lang.Object, java.lang.Number);
  public java.lang.Object setIncrBy(boolean, java.lang.Object, java.lang.Number);
  public java.lang.Object setSql(boolean, java.lang.String, java.lang.Object[]);
  public java.lang.Object set(boolean, java.lang.Object, java.lang.Object, java.lang.String);
}
```

## `com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper`

```java
public class com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper<T> extends com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper<T, java.lang.String, com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper<T>, com.baomidou.mybatisplus.core.conditions.update.UpdateWrapper<T>> implements com.baomidou.mybatisplus.extension.conditions.update.ChainUpdate<T>, com.baomidou.mybatisplus.core.conditions.update.Update<com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper<T>, java.lang.String> {
  public com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>);
  public com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper(java.lang.Class<T>);
  public com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper<T> set(boolean, java.lang.String, java.lang.Object, java.lang.String);
  public com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper<T> setSql(boolean, java.lang.String, java.lang.Object...);
  public com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper<T> setIncrBy(boolean, java.lang.String, java.lang.Number);
  public com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper<T> setDecrBy(boolean, java.lang.String, java.lang.Number);
  public java.lang.String getSqlSet();
  public com.baomidou.mybatisplus.core.mapper.BaseMapper<T> getBaseMapper();
  public java.lang.Class<T> getEntityClass();
  public com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper<T> lambda();
  public com.baomidou.mybatisplus.core.conditions.Wrapper getWrapper();
  public java.lang.Object setDecrBy(boolean, java.lang.Object, java.lang.Number);
  public java.lang.Object setIncrBy(boolean, java.lang.Object, java.lang.Number);
  public java.lang.Object setSql(boolean, java.lang.String, java.lang.Object[]);
  public java.lang.Object set(boolean, java.lang.Object, java.lang.Object, java.lang.String);
}
```
