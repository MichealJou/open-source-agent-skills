# com.baomidou.mybatisplus.extension.repository

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.repository.AbstractRepository`

```java
public abstract class com.baomidou.mybatisplus.extension.repository.AbstractRepository<M extends com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, T> implements com.baomidou.mybatisplus.extension.repository.IRepository<T> {
  public com.baomidou.mybatisplus.extension.repository.AbstractRepository();
  public java.lang.Class<T> getEntityClass();
  public java.lang.Class<M> getMapperClass();
  public boolean saveOrUpdate(T);
  public T getOne(com.baomidou.mybatisplus.core.conditions.Wrapper<T>, boolean);
  public java.util.Optional<T> getOneOpt(com.baomidou.mybatisplus.core.conditions.Wrapper<T>, boolean);
  public java.util.Map<java.lang.String, java.lang.Object> getMap(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public <V> V getObj(com.baomidou.mybatisplus.core.conditions.Wrapper<T>, java.util.function.Function<? super java.lang.Object, V>);
  public boolean removeById(java.io.Serializable, boolean);
}
```

## `com.baomidou.mybatisplus.extension.repository.CrudRepository`

```java
public abstract class com.baomidou.mybatisplus.extension.repository.CrudRepository<M extends com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, T> extends com.baomidou.mybatisplus.extension.repository.AbstractRepository<M, T> {
  public com.baomidou.mybatisplus.extension.repository.CrudRepository();
  public M getBaseMapper();
  public boolean saveBatch(java.util.Collection<T>, int);
  public boolean saveOrUpdateBatch(java.util.Collection<T>, int);
  public boolean updateBatchById(java.util.Collection<T>, int);
}
```

## `com.baomidou.mybatisplus.extension.repository.IRepository`

```java
public interface com.baomidou.mybatisplus.extension.repository.IRepository<T> {
  public default boolean save(T);
  public abstract boolean saveBatch(java.util.Collection<T>, int);
  public abstract boolean saveOrUpdateBatch(java.util.Collection<T>, int);
  public default boolean removeById(java.io.Serializable);
  public default boolean removeById(java.io.Serializable, boolean);
  public default boolean removeById(T);
  public default boolean removeByMap(java.util.Map<java.lang.String, java.lang.Object>);
  public default boolean remove(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default boolean removeByIds(java.util.Collection<?>);
  public default boolean removeByIds(java.util.Collection<?>, boolean);
  public default boolean updateById(T);
  public default boolean update(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default boolean update(T, com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public abstract boolean updateBatchById(java.util.Collection<T>, int);
  public abstract boolean saveOrUpdate(T);
  public default T getById(java.io.Serializable);
  public default java.util.Optional<T> getOptById(java.io.Serializable);
  public default java.util.List<T> listByIds(java.util.Collection<? extends java.io.Serializable>);
  public default java.util.List<T> listByMap(java.util.Map<java.lang.String, java.lang.Object>);
  public default T getOne(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default java.util.Optional<T> getOneOpt(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public abstract T getOne(com.baomidou.mybatisplus.core.conditions.Wrapper<T>, boolean);
  public abstract java.util.Optional<T> getOneOpt(com.baomidou.mybatisplus.core.conditions.Wrapper<T>, boolean);
  public abstract java.util.Map<java.lang.String, java.lang.Object> getMap(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public abstract <V> V getObj(com.baomidou.mybatisplus.core.conditions.Wrapper<T>, java.util.function.Function<? super java.lang.Object, V>);
  public default boolean exists(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default long count();
  public default long count(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default java.util.List<T> list(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default java.util.List<T> list(com.baomidou.mybatisplus.core.metadata.IPage<T>, com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default java.util.List<T> list();
  public default java.util.List<T> list(com.baomidou.mybatisplus.core.metadata.IPage<T>);
  public default <E extends com.baomidou.mybatisplus.core.metadata.IPage<T>> E page(E, com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default <E extends com.baomidou.mybatisplus.core.metadata.IPage<T>> E page(E);
  public default java.util.List<java.util.Map<java.lang.String, java.lang.Object>> listMaps(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default java.util.List<java.util.Map<java.lang.String, java.lang.Object>> listMaps(com.baomidou.mybatisplus.core.metadata.IPage<? extends java.util.Map<java.lang.String, java.lang.Object>>, com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default java.util.List<java.util.Map<java.lang.String, java.lang.Object>> listMaps();
  public default java.util.List<java.util.Map<java.lang.String, java.lang.Object>> listMaps(com.baomidou.mybatisplus.core.metadata.IPage<? extends java.util.Map<java.lang.String, java.lang.Object>>);
  public default <E> java.util.List<E> listObjs();
  public default <V> java.util.List<V> listObjs(java.util.function.Function<? super java.lang.Object, V>);
  public default <E> java.util.List<E> listObjs(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default <V> java.util.List<V> listObjs(com.baomidou.mybatisplus.core.conditions.Wrapper<T>, java.util.function.Function<? super java.lang.Object, V>);
  public default <E extends com.baomidou.mybatisplus.core.metadata.IPage<java.util.Map<java.lang.String, java.lang.Object>>> E pageMaps(E, com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default <E extends com.baomidou.mybatisplus.core.metadata.IPage<java.util.Map<java.lang.String, java.lang.Object>>> E pageMaps(E);
  public abstract com.baomidou.mybatisplus.core.mapper.BaseMapper<T> getBaseMapper();
  public abstract java.lang.Class<T> getEntityClass();
  public default com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper<T> query();
  public default com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T> lambdaQuery();
  public default com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T> lambdaQuery(T);
  public default com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper<T> ktQuery();
  public default com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper<T> ktUpdate();
  public default com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper<T> update();
  public default com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper<T> lambdaUpdate();
}
```
