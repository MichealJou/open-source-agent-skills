# com.baomidou.mybatisplus.extension.toolkit

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers`

```java
public final class com.baomidou.mybatisplus.extension.toolkit.ChainWrappers {
  public static <T> com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper<T> queryChain(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>);
  public static <T> com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper<T> queryChain(java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T> lambdaQueryChain(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>);
  public static <T> com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T> lambdaQueryChain(java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T> lambdaQueryChain(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, T);
  public static <T> com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T> lambdaQueryChain(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper<T> ktQueryChain(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper<T> ktQueryChain(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, T);
  public static <T> com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper<T> ktQueryChain(java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper<T> updateChain(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>);
  public static <T> com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper<T> updateChain(java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper<T> lambdaUpdateChain(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>);
  public static <T> com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper<T> lambdaUpdateChain(java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper<T> ktUpdateChain(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper<T> ktUpdateChain(java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper<T> ktUpdateChain(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, T);
}
```

## `com.baomidou.mybatisplus.extension.toolkit.Db`

```java
public class com.baomidou.mybatisplus.extension.toolkit.Db {
  public static <T> boolean save(T);
  public static <T> boolean saveBatch(java.util.Collection<T>);
  public static <T> boolean saveBatch(java.util.Collection<T>, int);
  public static <T> boolean saveOrUpdateBatch(java.util.Collection<T>);
  public static <T> boolean saveOrUpdateBatch(java.util.Collection<T>, int);
  public static <T> boolean removeById(java.io.Serializable, java.lang.Class<T>);
  public static <T> boolean removeById(T);
  public static <T> boolean remove(com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>);
  public static <T> boolean updateById(T);
  public static <T> boolean update(com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>);
  public static <T> boolean update(T, com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>);
  public static <T> boolean updateBatchById(java.util.Collection<T>);
  public static <T> boolean updateBatchById(java.util.Collection<T>, int);
  public static <T> boolean removeByIds(java.util.Collection<? extends java.io.Serializable>, java.lang.Class<T>);
  public static <T> boolean removeByMap(java.util.Map<java.lang.String, java.lang.Object>, java.lang.Class<T>);
  public static <T> boolean saveOrUpdate(T);
  public static <T> T getById(java.io.Serializable, java.lang.Class<T>);
  public static <T> T getOne(com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>);
  public static <T> T getOne(T);
  public static <T> T getOne(T, boolean);
  public static <T> T getOne(com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>, boolean);
  public static <T> java.util.List<T> listByMap(java.util.Map<java.lang.String, java.lang.Object>, java.lang.Class<T>);
  public static <T> java.util.List<T> listByIds(java.util.Collection<? extends java.io.Serializable>, java.lang.Class<T>);
  public static <T> java.util.Map<java.lang.String, java.lang.Object> getMap(com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>);
  public static <T> java.util.Map<java.lang.String, java.lang.Object> getMap(T);
  public static <T> long count(java.lang.Class<T>);
  public static <T> long count(T);
  public static <T> long count(com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>);
  public static <T> java.util.List<T> list(com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>);
  public static <T> java.util.List<T> list(com.baomidou.mybatisplus.core.metadata.IPage<T>, com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>);
  public static <T> java.util.List<T> list(java.lang.Class<T>);
  public static <T> java.util.List<T> list(com.baomidou.mybatisplus.core.metadata.IPage<T>, java.lang.Class<T>);
  public static <T> java.util.List<T> list(T);
  public static <T> java.util.List<T> list(com.baomidou.mybatisplus.core.metadata.IPage<T>, T);
  public static <T> java.util.List<java.util.Map<java.lang.String, java.lang.Object>> listMaps(com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>);
  public static <T> java.util.List<java.util.Map<java.lang.String, java.lang.Object>> listMaps(com.baomidou.mybatisplus.core.metadata.IPage<? extends java.util.Map<java.lang.String, java.lang.Object>>, com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>);
  public static <T> java.util.List<java.util.Map<java.lang.String, java.lang.Object>> listMaps(java.lang.Class<T>);
  public static <T> java.util.List<java.util.Map<java.lang.String, java.lang.Object>> listMaps(com.baomidou.mybatisplus.core.metadata.IPage<? extends java.util.Map<java.lang.String, java.lang.Object>>, java.lang.Class<T>);
  public static <T> java.util.List<java.util.Map<java.lang.String, java.lang.Object>> listMaps(T);
  public static <T> java.util.List<java.util.Map<java.lang.String, java.lang.Object>> listMaps(com.baomidou.mybatisplus.core.metadata.IPage<? extends java.util.Map<java.lang.String, java.lang.Object>>, T);
  public static <T> java.util.List<T> listObjs(java.lang.Class<T>);
  public static <E, T> java.util.List<E> listObjs(com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>);
  public static <T, V> java.util.List<V> listObjs(com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<? super T, V>);
  public static <T, V> java.util.List<V> listObjs(java.lang.Class<T>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<? super T, V>);
  public static <T, E extends com.baomidou.mybatisplus.core.metadata.IPage<java.util.Map<java.lang.String, java.lang.Object>>> E pageMaps(E, java.lang.Class<T>);
  public static <T, E extends com.baomidou.mybatisplus.core.metadata.IPage<java.util.Map<java.lang.String, java.lang.Object>>> E pageMaps(E, com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>);
  public static <T> com.baomidou.mybatisplus.core.metadata.IPage<T> page(com.baomidou.mybatisplus.core.metadata.IPage<T>, java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.core.metadata.IPage<T> page(com.baomidou.mybatisplus.core.metadata.IPage<T>, com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>);
  public static <T> com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper<T> query(java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper<T> ktQuery(java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper<T> lambdaQuery(java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper<T> update(java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper<T> ktUpdate(java.lang.Class<T>);
  public static <T> com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper<T> lambdaUpdate(java.lang.Class<T>);
  public static <T> boolean saveOrUpdate(T, com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>);
  public static <T, V> V getObj(com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, ?, ?>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<? super T, V>);
}
```

## `com.baomidou.mybatisplus.extension.toolkit.JdbcUtils`

```java
public class com.baomidou.mybatisplus.extension.toolkit.JdbcUtils {
  public com.baomidou.mybatisplus.extension.toolkit.JdbcUtils();
  public static com.baomidou.mybatisplus.annotation.DbType getDbType(org.apache.ibatis.executor.Executor);
  public static com.baomidou.mybatisplus.annotation.DbType getDbType(java.lang.String);
  public static boolean regexFind(java.lang.String, java.lang.CharSequence);
}
```

## `com.baomidou.mybatisplus.extension.toolkit.PropertyMapper`

```java
public class com.baomidou.mybatisplus.extension.toolkit.PropertyMapper {
  public static com.baomidou.mybatisplus.extension.toolkit.PropertyMapper newInstance(java.util.Properties);
  public java.util.Set<java.lang.String> keys();
  public com.baomidou.mybatisplus.extension.toolkit.PropertyMapper whenNotBlank(java.lang.String, java.util.function.Consumer<java.lang.String>);
  public <T> com.baomidou.mybatisplus.extension.toolkit.PropertyMapper whenNotBlank(java.lang.String, java.util.function.Function<java.lang.String, T>, java.util.function.Consumer<T>);
  public java.util.Map<java.lang.String, java.util.Properties> group(java.lang.String);
}
```

## `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery`

```java
public class com.baomidou.mybatisplus.extension.toolkit.SimpleQuery {
  public static <E> java.lang.Class<E> getType(com.baomidou.mybatisplus.core.toolkit.support.SFunction<E, ?>);
  public static <E, A> java.util.Map<A, E> keyMap(com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<E>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<E, A>, java.util.function.Consumer<E>...);
  public static <E, A> java.util.Map<A, E> keyMap(com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<E>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<E, A>, boolean, java.util.function.Consumer<E>...);
  public static <E, A, P> java.util.Map<A, P> map(com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<E>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<E, A>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<E, P>, java.util.function.Consumer<E>...);
  public static <E, A, P> java.util.Map<A, P> map(com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<E>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<E, A>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<E, P>, boolean, java.util.function.Consumer<E>...);
  public static <E, A> java.util.Map<A, java.util.List<E>> group(com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<E>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<E, A>, java.util.function.Consumer<E>...);
  public static <T, K> java.util.Map<K, java.util.List<T>> group(com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, K>, boolean, java.util.function.Consumer<T>...);
  public static <T, K, D, A> java.util.Map<K, D> group(com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, K>, java.util.stream.Collector<T, A, D>, java.util.function.Consumer<T>...);
  public static <T, K, D, A> java.util.Map<K, D> group(com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, K>, java.util.stream.Collector<T, A, D>, boolean, java.util.function.Consumer<T>...);
  public static <E, A> java.util.List<A> list(com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<E>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<E, A>, java.util.function.Consumer<E>...);
  public static <E, A> java.util.List<A> list(com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<E>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<E, A>, boolean, java.util.function.Consumer<E>...);
  public static <A, E> java.util.List<A> list2List(java.util.List<E>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<E, A>, java.util.function.Consumer<E>...);
  public static <A, E> java.util.List<A> list2List(java.util.List<E>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<E, A>, boolean, java.util.function.Consumer<E>...);
  public static <K, T> java.util.Map<K, java.util.List<T>> listGroupBy(java.util.List<T>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, K>, java.util.function.Consumer<T>...);
  public static <K, T> java.util.Map<K, java.util.List<T>> listGroupBy(java.util.List<T>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, K>, boolean, java.util.function.Consumer<T>...);
  public static <T, K, D, A> java.util.Map<K, D> listGroupBy(java.util.List<T>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, K>, java.util.stream.Collector<T, A, D>, java.util.function.Consumer<T>...);
  public static <T, K, D, A> java.util.Map<K, D> listGroupBy(java.util.List<T>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, K>, java.util.stream.Collector<T, A, D>, boolean, java.util.function.Consumer<T>...);
  public static <E, A, P> java.util.Map<A, P> list2Map(java.util.List<E>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<E, A>, java.util.function.Function<E, P>, java.util.function.Consumer<E>...);
  public static <E, A, P> java.util.Map<A, P> list2Map(java.util.List<E>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<E, A>, java.util.function.Function<E, P>, boolean, java.util.function.Consumer<E>...);
  public static <E> java.util.stream.Stream<E> peekStream(java.util.List<E>, boolean, java.util.function.Consumer<E>...);
}
```

## `com.baomidou.mybatisplus.extension.toolkit.SqlHelper`

```java
public final class com.baomidou.mybatisplus.extension.toolkit.SqlHelper {
  public com.baomidou.mybatisplus.extension.toolkit.SqlHelper();
  public static org.apache.ibatis.session.SqlSession sqlSessionBatch(java.lang.Class<?>);
  public static org.apache.ibatis.session.SqlSessionFactory sqlSessionFactory(java.lang.Class<?>);
  public static org.apache.ibatis.session.SqlSession sqlSession(java.lang.Class<?>);
  public static com.baomidou.mybatisplus.core.metadata.TableInfo table(java.lang.Class<?>);
  public static boolean retBool(java.lang.Integer);
  public static boolean retBool(java.lang.Long);
  public static boolean retBool(java.util.List<org.apache.ibatis.executor.BatchResult>);
  public static long retCount(java.lang.Long);
  public static <E> E getObject(org.apache.ibatis.logging.Log, java.util.List<E>);
  public static <E> E getObject(java.util.function.Supplier<org.apache.ibatis.logging.Log>, java.util.List<E>);
  public static boolean executeBatch(java.lang.Class<?>, org.apache.ibatis.logging.Log, java.util.function.Consumer<org.apache.ibatis.session.SqlSession>);
  public static boolean executeBatch(org.apache.ibatis.session.SqlSessionFactory, org.apache.ibatis.logging.Log, java.util.function.Consumer<org.apache.ibatis.session.SqlSession>);
  public static <E> boolean executeBatch(java.lang.Class<?>, org.apache.ibatis.logging.Log, java.util.Collection<E>, int, java.util.function.BiConsumer<org.apache.ibatis.session.SqlSession, E>);
  public static <E> boolean executeBatch(org.apache.ibatis.session.SqlSessionFactory, org.apache.ibatis.logging.Log, java.util.Collection<E>, int, java.util.function.BiConsumer<org.apache.ibatis.session.SqlSession, E>);
  public static <E> boolean saveOrUpdateBatch(java.lang.Class<?>, java.lang.Class<?>, org.apache.ibatis.logging.Log, java.util.Collection<E>, int, java.util.function.BiPredicate<org.apache.ibatis.session.SqlSession, E>, java.util.function.BiConsumer<org.apache.ibatis.session.SqlSession, E>);
  public static <E> boolean saveOrUpdateBatch(org.apache.ibatis.session.SqlSessionFactory, java.lang.Class<?>, org.apache.ibatis.logging.Log, java.util.Collection<E>, int, java.util.function.BiPredicate<org.apache.ibatis.session.SqlSession, E>, java.util.function.BiConsumer<org.apache.ibatis.session.SqlSession, E>);
  public static java.lang.String getSqlStatement(java.lang.Class<?>, com.baomidou.mybatisplus.core.enums.SqlMethod);
  public static <T, M extends com.baomidou.mybatisplus.core.mapper.BaseMapper<T>> M getMapper(java.lang.Class<T>, org.apache.ibatis.session.SqlSession);
  public static <T, R, M extends com.baomidou.mybatisplus.core.mapper.BaseMapper<T>> R execute(java.lang.Class<T>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<M, R>);
}
```

## `com.baomidou.mybatisplus.extension.toolkit.SqlParserUtils`

```java
public class com.baomidou.mybatisplus.extension.toolkit.SqlParserUtils {
  public com.baomidou.mybatisplus.extension.toolkit.SqlParserUtils();
  public static java.lang.String getOriginalCountSql(java.lang.String);
  public static java.lang.String removeWrapperSymbol(java.lang.String);
}
```

## `com.baomidou.mybatisplus.extension.toolkit.SqlRunner`

```java
public class com.baomidou.mybatisplus.extension.toolkit.SqlRunner extends com.baomidou.mybatisplus.core.assist.AbstractSqlRunner {
  public com.baomidou.mybatisplus.extension.toolkit.SqlRunner();
  public com.baomidou.mybatisplus.extension.toolkit.SqlRunner(java.lang.Class<?>);
  public static com.baomidou.mybatisplus.extension.toolkit.SqlRunner db();
  public static com.baomidou.mybatisplus.extension.toolkit.SqlRunner db(java.lang.Class<?>);
  public boolean insert(java.lang.String, java.lang.Object...);
  public boolean delete(java.lang.String, java.lang.Object...);
  public boolean update(java.lang.String, java.lang.Object...);
  public java.util.List<java.util.Map<java.lang.String, java.lang.Object>> selectList(java.lang.String, java.lang.Object...);
  public java.util.List<java.lang.Object> selectObjs(java.lang.String, java.lang.Object...);
  public java.lang.Object selectObj(java.lang.String, java.lang.Object...);
  public long selectCount(java.lang.String, java.lang.Object...);
  public java.util.Map<java.lang.String, java.lang.Object> selectOne(java.lang.String, java.lang.Object...);
  public <E extends com.baomidou.mybatisplus.core.metadata.IPage<java.util.Map<java.lang.String, java.lang.Object>>> E selectPage(E, java.lang.String, java.lang.Object...);
  public void close();
}
```
