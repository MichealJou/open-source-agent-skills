# com.baomidou.mybatisplus.core.batch

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.batch.BatchMethod` | `ParameterConvert<T> getParameterConvert()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.batch.BatchMethod` | `String getStatementId()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.batch.BatchSqlSession` | `List<BatchResult> getResultBatchList()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.batch.BatchSqlSession` | `List<E> selectList(String statement)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.batch.BatchSqlSession` | `List<E> selectList(String statement,Object parameter)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.batch.BatchSqlSession` | `List<E> selectList(String statement,Object parameter,RowBounds rowBounds)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.batch.BatchSqlSession` | `Map<K, V> selectMap(String statement,Object parameter,String mapKey)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.batch.BatchSqlSession` | `Map<K, V> selectMap(String statement,Object parameter,String mapKey,RowBounds rowBounds)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.batch.BatchSqlSession` | `Map<K, V> selectMap(String statement,String mapKey)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.batch.BatchSqlSession` | `T selectOne(String statement)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.batch.BatchSqlSession` | `T selectOne(String statement,Object parameter)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch` | `List<BatchResult> execute(BatchMethod<T> batchMethod)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch` | `List<BatchResult> execute(String statement)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch` | `List<BatchResult> execute(String statement,ParameterConvert<T> parameterConvert)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch` | `List<BatchResult> execute(boolean autoCommit,BatchMethod<T> batchMethod)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch` | `List<BatchResult> execute(boolean autoCommit,String statement)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch` | `List<BatchResult> execute(boolean autoCommit,String statement,ParameterConvert<T> parameterConvert)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch` | `List<BatchResult> saveOrUpdate(BatchMethod<T> insertMethod,BiPredicate<BatchSqlSession, T> insertPredicate,BatchMethod<T> updateMethod)` | 批量保存或更新 这里需要注意一下,如果在insertPredicate里判断调用其他sqlSession(类似mapper.xxx)时,要注意一级缓存问题或数据感知问题(因为当前会话数据还未提交) 举个例子(事务开启状态下): 如果当前批次里面执行两个主键相同的数据,当调用mapper.selectById时,如果数据库未有这条记录,在同个sqlSession下,由于一级缓存的问题,下次再查就还是null,导致插入主键冲突, 但使用 BatchSqlSession时,由于每次select操作都会触发一次flushStatements,就会执行更新操作 |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch` | `List<BatchResult> saveOrUpdate(boolean autoCommit,BatchMethod<T> insertMethod,BiPredicate<BatchSqlSession, T> insertPredicate,BatchMethod<T> updateMethod)` | 批量保存或更新 这里需要注意一下,如果在insertPredicate里判断调用其他sqlSession(类似mapper.xxx)时,要注意一级缓存问题或数据感知问题(因为当前会话数据还未提交) 举个例子(事务开启状态下): 如果当前批次里面执行两个主键相同的数据,当调用mapper.selectById时,如果数据库未有这条记录,在同个sqlSession下,由于一级缓存的问题,下次再查就还是null,导致插入主键冲突, 但使用 BatchSqlSession时,由于每次select操作都会触发一次flushStatements,就会执行更新操作 |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch$Method` | `BatchMethod<E> deleteById(Function<E, T> function)` | 删除方法 com.baomidou.mybatisplus.core.mapper.BaseMapper#deleteById(Object) or com.baomidou.mybatisplus.core.mapper.BaseMapper#deleteById(Serializable) |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch$Method` | `BatchMethod<E> get(String method)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch$Method` | `BatchMethod<E> get(String method,ParameterConvert<E> parameterConvert)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch$Method` | `BatchMethod<E> insert(Function<E, T> function)` | 新增方法 |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch$Method` | `BatchMethod<E> update(Function<E, T> entityFunction,Function<E, Wrapper<T>> wrapperFunction)` | 更新方法 com.baomidou.mybatisplus.core.mapper.BaseMapper#update(java.lang.Object, com.baomidou.mybatisplus.core.conditions.Wrapper) |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch$Method` | `BatchMethod<E> update(Function<E, Wrapper<T>> wrapperFunction)` | 更新方法 com.baomidou.mybatisplus.core.mapper.BaseMapper#update(java.lang.Object, com.baomidou.mybatisplus.core.conditions.Wrapper) |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch$Method` | `BatchMethod<E> updateById(Function<E, T> etFunction)` | 更新方法 com.baomidou.mybatisplus.core.mapper.BaseMapper#updateById(java.lang.Object) |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch$Method` | `BatchMethod<T> deleteById()` | 删除方法 com.baomidou.mybatisplus.core.mapper.BaseMapper#deleteById(Object) or com.baomidou.mybatisplus.core.mapper.BaseMapper#deleteById(Serializable) |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch$Method` | `BatchMethod<T> insert()` | 新增方法 |
| `com.baomidou.mybatisplus.core.batch.MybatisBatch$Method` | `BatchMethod<T> updateById()` | 更新方法 com.baomidou.mybatisplus.core.mapper.BaseMapper#updateById(java.lang.Object) |
| `com.baomidou.mybatisplus.core.batch.ParameterConvert` | `Object convert(T parameter)` | 转换当前实体参数为mapper方法参数 |
