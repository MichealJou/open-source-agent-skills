# com.baomidou.mybatisplus.core.mapper

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.mapper.BaseMapper`

```java
public interface com.baomidou.mybatisplus.core.mapper.BaseMapper<T> extends com.baomidou.mybatisplus.core.mapper.Mapper<T> {
  public abstract int insert(T);
  public default int deleteById(java.io.Serializable);
  public default int deleteById(java.lang.Object, boolean);
  public abstract int deleteById(T);
  public default int deleteByMap(java.util.Map<java.lang.String, java.lang.Object>);
  public abstract int delete(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default int deleteBatchIds(java.util.Collection<?>);
  public default int deleteByIds(java.util.Collection<?>);
  public default int deleteByIds(java.util.Collection<?>, boolean);
  public abstract int updateById(T);
  public abstract int update(T, com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default int update(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public abstract T selectById(java.io.Serializable);
  public abstract java.util.List<T> selectByIds(java.util.Collection<? extends java.io.Serializable>);
  public default java.util.List<T> selectBatchIds(java.util.Collection<? extends java.io.Serializable>);
  public abstract void selectByIds(java.util.Collection<? extends java.io.Serializable>, org.apache.ibatis.session.ResultHandler<T>);
  public default void selectBatchIds(java.util.Collection<? extends java.io.Serializable>, org.apache.ibatis.session.ResultHandler<T>);
  public default java.util.List<T> selectByMap(java.util.Map<java.lang.String, java.lang.Object>);
  public default void selectByMap(java.util.Map<java.lang.String, java.lang.Object>, org.apache.ibatis.session.ResultHandler<T>);
  public default T selectOne(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default T selectOne(com.baomidou.mybatisplus.core.conditions.Wrapper<T>, boolean);
  public default boolean exists(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public abstract java.lang.Long selectCount(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public abstract java.util.List<T> selectList(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public abstract void selectList(com.baomidou.mybatisplus.core.conditions.Wrapper<T>, org.apache.ibatis.session.ResultHandler<T>);
  public abstract java.util.List<T> selectList(com.baomidou.mybatisplus.core.metadata.IPage<T>, com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public abstract void selectList(com.baomidou.mybatisplus.core.metadata.IPage<T>, com.baomidou.mybatisplus.core.conditions.Wrapper<T>, org.apache.ibatis.session.ResultHandler<T>);
  public abstract java.util.List<java.util.Map<java.lang.String, java.lang.Object>> selectMaps(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public abstract void selectMaps(com.baomidou.mybatisplus.core.conditions.Wrapper<T>, org.apache.ibatis.session.ResultHandler<java.util.Map<java.lang.String, java.lang.Object>>);
  public abstract java.util.List<java.util.Map<java.lang.String, java.lang.Object>> selectMaps(com.baomidou.mybatisplus.core.metadata.IPage<? extends java.util.Map<java.lang.String, java.lang.Object>>, com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public abstract void selectMaps(com.baomidou.mybatisplus.core.metadata.IPage<? extends java.util.Map<java.lang.String, java.lang.Object>>, com.baomidou.mybatisplus.core.conditions.Wrapper<T>, org.apache.ibatis.session.ResultHandler<java.util.Map<java.lang.String, java.lang.Object>>);
  public abstract <E> java.util.List<E> selectObjs(com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public abstract <E> void selectObjs(com.baomidou.mybatisplus.core.conditions.Wrapper<T>, org.apache.ibatis.session.ResultHandler<E>);
  public default <P extends com.baomidou.mybatisplus.core.metadata.IPage<T>> P selectPage(P, com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default <P extends com.baomidou.mybatisplus.core.metadata.IPage<java.util.Map<java.lang.String, java.lang.Object>>> P selectMapsPage(P, com.baomidou.mybatisplus.core.conditions.Wrapper<T>);
  public default boolean insertOrUpdate(T);
  public default java.util.List<org.apache.ibatis.executor.BatchResult> insert(java.util.Collection<T>);
  public default java.util.List<org.apache.ibatis.executor.BatchResult> insert(java.util.Collection<T>, int);
  public default java.util.List<org.apache.ibatis.executor.BatchResult> updateById(java.util.Collection<T>);
  public default java.util.List<org.apache.ibatis.executor.BatchResult> updateById(java.util.Collection<T>, int);
  public default java.util.List<org.apache.ibatis.executor.BatchResult> insertOrUpdate(java.util.Collection<T>);
  public default java.util.List<org.apache.ibatis.executor.BatchResult> insertOrUpdate(java.util.Collection<T>, int);
  public default java.util.List<org.apache.ibatis.executor.BatchResult> insertOrUpdate(java.util.Collection<T>, java.util.function.BiPredicate<com.baomidou.mybatisplus.core.batch.BatchSqlSession, T>);
  public default java.util.List<org.apache.ibatis.executor.BatchResult> insertOrUpdate(java.util.Collection<T>, java.util.function.BiPredicate<com.baomidou.mybatisplus.core.batch.BatchSqlSession, T>, int);
}
```
