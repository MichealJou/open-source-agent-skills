# com.baomidou.mybatisplus.core.batch

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.batch.BatchMethod`

```java
public class com.baomidou.mybatisplus.core.batch.BatchMethod<T> {
  public com.baomidou.mybatisplus.core.batch.BatchMethod(java.lang.String);
  public com.baomidou.mybatisplus.core.batch.BatchMethod(java.lang.String, com.baomidou.mybatisplus.core.batch.ParameterConvert<T>);
  public java.lang.String getStatementId();
  public com.baomidou.mybatisplus.core.batch.ParameterConvert<T> getParameterConvert();
}
```

## `com.baomidou.mybatisplus.core.batch.BatchSqlSession`

```java
public class com.baomidou.mybatisplus.core.batch.BatchSqlSession {
  public com.baomidou.mybatisplus.core.batch.BatchSqlSession(org.apache.ibatis.session.SqlSession);
  public <T> T selectOne(java.lang.String);
  public <T> T selectOne(java.lang.String, java.lang.Object);
  public <E> java.util.List<E> selectList(java.lang.String);
  public <E> java.util.List<E> selectList(java.lang.String, java.lang.Object);
  public <E> java.util.List<E> selectList(java.lang.String, java.lang.Object, org.apache.ibatis.session.RowBounds);
  public <K, V> java.util.Map<K, V> selectMap(java.lang.String, java.lang.String);
  public <K, V> java.util.Map<K, V> selectMap(java.lang.String, java.lang.Object, java.lang.String);
  public <K, V> java.util.Map<K, V> selectMap(java.lang.String, java.lang.Object, java.lang.String, org.apache.ibatis.session.RowBounds);
  public java.util.List<org.apache.ibatis.executor.BatchResult> getResultBatchList();
}
```

## `com.baomidou.mybatisplus.core.batch.MybatisBatch`

```java
public class com.baomidou.mybatisplus.core.batch.MybatisBatch<T> {
  public com.baomidou.mybatisplus.core.batch.MybatisBatch(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>);
  public com.baomidou.mybatisplus.core.batch.MybatisBatch(org.apache.ibatis.session.SqlSessionFactory, java.util.Collection<T>, int);
  public java.util.List<org.apache.ibatis.executor.BatchResult> execute(java.lang.String);
  public java.util.List<org.apache.ibatis.executor.BatchResult> execute(java.lang.String, com.baomidou.mybatisplus.core.batch.ParameterConvert<T>);
  public java.util.List<org.apache.ibatis.executor.BatchResult> execute(boolean, java.lang.String);
  public java.util.List<org.apache.ibatis.executor.BatchResult> execute(com.baomidou.mybatisplus.core.batch.BatchMethod<T>);
  public java.util.List<org.apache.ibatis.executor.BatchResult> execute(boolean, com.baomidou.mybatisplus.core.batch.BatchMethod<T>);
  public java.util.List<org.apache.ibatis.executor.BatchResult> execute(boolean, java.lang.String, com.baomidou.mybatisplus.core.batch.ParameterConvert<T>);
  public java.util.List<org.apache.ibatis.executor.BatchResult> saveOrUpdate(com.baomidou.mybatisplus.core.batch.BatchMethod<T>, java.util.function.BiPredicate<com.baomidou.mybatisplus.core.batch.BatchSqlSession, T>, com.baomidou.mybatisplus.core.batch.BatchMethod<T>);
  public java.util.List<org.apache.ibatis.executor.BatchResult> saveOrUpdate(boolean, com.baomidou.mybatisplus.core.batch.BatchMethod<T>, java.util.function.BiPredicate<com.baomidou.mybatisplus.core.batch.BatchSqlSession, T>, com.baomidou.mybatisplus.core.batch.BatchMethod<T>);
}
```

## `com.baomidou.mybatisplus.core.batch.MybatisBatch$Method`

```java
public class com.baomidou.mybatisplus.core.batch.MybatisBatch$Method<T> {
  public com.baomidou.mybatisplus.core.batch.MybatisBatch$Method(java.lang.Class<?>);
  public com.baomidou.mybatisplus.core.batch.BatchMethod<T> insert();
  public <E> com.baomidou.mybatisplus.core.batch.BatchMethod<E> insert(java.util.function.Function<E, T>);
  public com.baomidou.mybatisplus.core.batch.BatchMethod<T> updateById();
  public <E> com.baomidou.mybatisplus.core.batch.BatchMethod<E> updateById(java.util.function.Function<E, T>);
  public <E> com.baomidou.mybatisplus.core.batch.BatchMethod<E> update(java.util.function.Function<E, com.baomidou.mybatisplus.core.conditions.Wrapper<T>>);
  public <E> com.baomidou.mybatisplus.core.batch.BatchMethod<E> update(java.util.function.Function<E, T>, java.util.function.Function<E, com.baomidou.mybatisplus.core.conditions.Wrapper<T>>);
  public <E> com.baomidou.mybatisplus.core.batch.BatchMethod<E> deleteById(java.util.function.Function<E, T>);
  public <T> com.baomidou.mybatisplus.core.batch.BatchMethod<T> deleteById();
  public <E> com.baomidou.mybatisplus.core.batch.BatchMethod<E> get(java.lang.String);
  public <E> com.baomidou.mybatisplus.core.batch.BatchMethod<E> get(java.lang.String, com.baomidou.mybatisplus.core.batch.ParameterConvert<E>);
}
```

## `com.baomidou.mybatisplus.core.batch.ParameterConvert`

```java
public interface com.baomidou.mybatisplus.core.batch.ParameterConvert<T> {
  public abstract java.lang.Object convert(T);
}
```
