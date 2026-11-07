# com.baomidou.mybatisplus.extension.toolkit

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `KtQueryChainWrapper<T> ktQueryChain(BaseMapper<T> mapper,Class<T> entityClass)` | 链式查询 lambda 式 仅支持 Kotlin |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `KtQueryChainWrapper<T> ktQueryChain(BaseMapper<T> mapper,T entity)` | 链式查询 lambda 式 仅支持 Kotlin |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `KtQueryChainWrapper<T> ktQueryChain(Class<T> entityClass)` | 链式查询 lambda 式 仅支持 Kotlin 仅传 entityClass 实体类 |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `KtUpdateChainWrapper<T> ktUpdateChain(BaseMapper<T> mapper,Class<T> entityClass)` | 链式更改 lambda 式 仅支持 Kotlin |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `KtUpdateChainWrapper<T> ktUpdateChain(BaseMapper<T> mapper,T entity)` | 链式更改 lambda 式 仅支持 Kotlin |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `KtUpdateChainWrapper<T> ktUpdateChain(Class<T> entityClass)` | 链式更改 lambda 式 仅支持 Kotlin 仅传 entityClass 实体类 |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `LambdaQueryChainWrapper<T> lambdaQueryChain(BaseMapper<T> mapper)` | 链式查询 lambda 式 注意：不支持 Kotlin |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `LambdaQueryChainWrapper<T> lambdaQueryChain(BaseMapper<T> mapper,Class<T> entityClass)` | 链式查询 lambda 式 注意：不支持 Kotlin |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `LambdaQueryChainWrapper<T> lambdaQueryChain(BaseMapper<T> mapper,T entity)` | 链式查询 lambda 式 注意：不支持 Kotlin |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `LambdaQueryChainWrapper<T> lambdaQueryChain(Class<T> entityClass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `LambdaUpdateChainWrapper<T> lambdaUpdateChain(BaseMapper<T> mapper)` | 链式更改 lambda 式 注意：不支持 Kotlin |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `LambdaUpdateChainWrapper<T> lambdaUpdateChain(Class<T> entityClass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `QueryChainWrapper<T> queryChain(BaseMapper<T> mapper)` | 链式查询 普通 |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `QueryChainWrapper<T> queryChain(Class<T> entityClass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `UpdateChainWrapper<T> updateChain(BaseMapper<T> mapper)` | 链式更改 普通 |
| `com.baomidou.mybatisplus.extension.toolkit.ChainWrappers` | `UpdateChainWrapper<T> updateChain(Class<T> entityClass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `E pageMaps(E page,AbstractWrapper<T, ?, ?> queryWrapper)` | 翻页查询 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `E pageMaps(E page,Class<T> entityClass)` | 无条件翻页查询 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `IPage<T> page(IPage<T> page,AbstractWrapper<T, ?, ?> queryWrapper)` | 翻页查询 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `IPage<T> page(IPage<T> page,Class<T> entityClass)` | 无条件翻页查询 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `KtQueryChainWrapper<T> ktQuery(Class<T> entityClass)` | kt链式查询 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `KtUpdateChainWrapper<T> ktUpdate(Class<T> entityClass)` | kt链式更改 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `LambdaQueryChainWrapper<T> lambdaQuery(Class<T> entityClass)` | 链式查询 lambda 式 注意：不支持 Kotlin |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `LambdaUpdateChainWrapper<T> lambdaUpdate(Class<T> entityClass)` | 链式更改 lambda 式 注意：不支持 Kotlin |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<E> listObjs(AbstractWrapper<T, ?, ?> queryWrapper)` | 根据 Wrapper 条件，查询全部记录 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<Map<String, Object>> listMaps(AbstractWrapper<T, ?, ?> queryWrapper)` | 查询列表 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<Map<String, Object>> listMaps(Class<T> entityClass)` | 查询所有列表 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<Map<String, Object>> listMaps(IPage<? extends Map<String, Object>> page,AbstractWrapper<T, ?, ?> queryWrapper)` | 【原文待译】@since 3.5.3.2 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<Map<String, Object>> listMaps(IPage<? extends Map<String, Object>> page,Class<T> entityClass)` | 分页查询列表 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<Map<String, Object>> listMaps(IPage<? extends Map<String, Object>> page,T entity)` | 根据entity不为空的条件查询列表 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<Map<String, Object>> listMaps(T entity)` | 根据entity不为空的条件查询列表 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<T> list(AbstractWrapper<T, ?, ?> queryWrapper)` | 查询列表 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<T> list(Class<T> entityClass)` | 查询所有 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<T> list(IPage<T> page,AbstractWrapper<T, ?, ?> queryWrapper)` | @param page 分页条件 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<T> list(IPage<T> page,Class<T> entityClass)` | @param page 分页条件 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<T> list(IPage<T> page,T entity)` | 根据entity中不为空的字段进行查询 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<T> list(T entity)` | 根据entity中不为空的字段进行查询 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<T> listByIds(Collection<? extends Serializable> idList,Class<T> entityClass)` | 查询（根据ID 批量查询） |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<T> listByMap(Map<String, Object> columnMap,Class<T> entityClass)` | 查询（根据 columnMap 条件） |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<T> listObjs(Class<T> entityClass)` | 查询全部记录 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<V> listObjs(AbstractWrapper<T, ?, ?> queryWrapper,SFunction<? super T, V> mapper)` | 根据 Wrapper 条件，查询全部记录 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `List<V> listObjs(Class<T> entityClass,SFunction<? super T, V> mapper)` | 查询全部记录 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `Map<String, Object> getMap(AbstractWrapper<T, ?, ?> queryWrapper)` | 根据 Wrapper，查询一条记录 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `Map<String, Object> getMap(T entity)` | 根据 entity不为空条件，查询一条记录 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `QueryChainWrapper<T> query(Class<T> entityClass)` | 链式查询 普通 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `T getById(Serializable id,Class<T> entityClass)` | 根据 ID 查询 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `T getOne(AbstractWrapper<T, ?, ?> queryWrapper)` | 根据 Wrapper，查询一条记录 结果集，如果是多个会抛出异常，随机取一条加上限制条件 wrapper.last("LIMIT 1") |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `T getOne(AbstractWrapper<T, ?, ?> queryWrapper,boolean throwEx)` | 根据 Wrapper，查询一条记录 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `T getOne(T entity)` | 根据 entity里不为空的字段，查询一条记录 结果集，如果是多个会抛出异常，随机取一条加上限制条件 wrapper.last("LIMIT 1") |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `T getOne(T entity,boolean throwEx)` | 根据 entity里不为空的字段，查询一条记录 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `UpdateChainWrapper<T> update(Class<T> entityClass)` | 链式更改 普通 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `V getObj(AbstractWrapper<T, ?, ?> queryWrapper,SFunction<? super T, V> mapper)` | 根据 Wrapper，查询一条记录 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean remove(AbstractWrapper<T, ?, ?> queryWrapper)` | 根据 entity 条件，删除记录 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean removeById(Serializable id,Class<T> entityClass)` | 根据 ID 删除 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean removeById(T entity)` | 根据实体(ID)删除 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean removeByIds(Collection<? extends Serializable> list,Class<T> entityClass)` | 删除（根据ID 批量删除） |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean removeByMap(Map<String, Object> columnMap,Class<T> entityClass)` | 根据 columnMap 条件，删除记录 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean save(T entity)` | 插入一条记录（选择字段，策略插入） |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean saveBatch(Collection<T> entityList)` | 插入（批量） |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean saveBatch(Collection<T> entityList,int batchSize)` | 插入（批量） |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean saveOrUpdate(T entity)` | TableId 注解存在更新记录，否插入一条记录 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean saveOrUpdate(T entity,AbstractWrapper<T, ?, ?> updateWrapper)` | 根据updateWrapper尝试更新，否继续执行saveOrUpdate(T)方法 此次修改主要是减少了此项业务代码的代码量（存在性验证之后的saveOrUpdate操作） |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean saveOrUpdateBatch(Collection<T> entityList)` | 批量修改插入 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean saveOrUpdateBatch(Collection<T> entityList,int batchSize)` | 批量修改插入 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean update(AbstractWrapper<T, ?, ?> updateWrapper)` | 根据 UpdateWrapper 条件，更新记录 需要设置sqlset |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean update(T entity,AbstractWrapper<T, ?, ?> updateWrapper)` | 根据 whereEntity 条件，更新记录 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean updateBatchById(Collection<T> entityList)` | 根据ID 批量更新 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean updateBatchById(Collection<T> entityList,int batchSize)` | 根据ID 批量更新 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `boolean updateById(T entity)` | 根据 ID 选择修改 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `long count(AbstractWrapper<T, ?, ?> queryWrapper)` | 根据 Wrapper 条件，查询总记录数 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `long count(Class<T> entityClass)` | 查询总记录数 |
| `com.baomidou.mybatisplus.extension.toolkit.Db` | `long count(T entity)` | 根据entity中不为空的数据查询记录数 |
| `com.baomidou.mybatisplus.extension.toolkit.JdbcUtils` | `DbType getDbType(Executor executor)` | 不关闭 Connection,因为是从事务里获取的,sqlSession会负责关闭 |
| `com.baomidou.mybatisplus.extension.toolkit.JdbcUtils` | `DbType getDbType(String jdbcUrl)` | 根据连接地址判断数据库类型 |
| `com.baomidou.mybatisplus.extension.toolkit.JdbcUtils` | `boolean regexFind(String regex,CharSequence input)` | 正则匹配 |
| `com.baomidou.mybatisplus.extension.toolkit.PropertyMapper` | `Map<String, Properties> group(String group)` | mp 内部规则分组 |
| `com.baomidou.mybatisplus.extension.toolkit.PropertyMapper` | `PropertyMapper newInstance(Properties properties)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.toolkit.PropertyMapper` | `PropertyMapper whenNotBlank(String key,Consumer<String> consumer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.toolkit.PropertyMapper` | `PropertyMapper whenNotBlank(String key,Function<String, T> function,Consumer<T> consumer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.toolkit.PropertyMapper` | `Set<String> keys()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Class<E> getType(SFunction<E, ?> sFunction)` | 通过lambda获取Class |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `List<A> list(LambdaQueryWrapper<E> wrapper,SFunction<E, A> sFunction,Consumer<E>... peeks)` | 【原文待译】ignore |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `List<A> list(LambdaQueryWrapper<E> wrapper,SFunction<E, A> sFunction,boolean isParallel,Consumer<E>... peeks)` | 传入wrappers和需要的某一列，从数据中根据条件查询出对应的列，转换成list |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `List<A> list2List(List<E> list,SFunction<E, A> sFunction,Consumer<E>... peeks)` | 【原文待译】ignore |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `List<A> list2List(List<E> list,SFunction<E, A> sFunction,boolean isParallel,Consumer<E>... peeks)` | 对list进行map、peek操作 |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Map<A, E> keyMap(LambdaQueryWrapper<E> wrapper,SFunction<E, A> sFunction,Consumer<E>... peeks)` | 【原文待译】ignore |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Map<A, E> keyMap(LambdaQueryWrapper<E> wrapper,SFunction<E, A> sFunction,boolean isParallel,Consumer<E>... peeks)` | 传入Wrappers和key，从数据库中根据条件查询出对应的列表，封装成Map |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Map<A, List<E>> group(LambdaQueryWrapper<E> wrapper,SFunction<E, A> sFunction,Consumer<E>... peeks)` | 【原文待译】ignore |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Map<A, P> list2Map(List<E> list,SFunction<E, A> keyFunc,Function<E, P> valueFunc,Consumer<E>... peeks)` | 【原文待译】ignore |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Map<A, P> list2Map(List<E> list,SFunction<E, A> keyFunc,Function<E, P> valueFunc,boolean isParallel,Consumer<E>... peeks)` | list转换为map |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Map<A, P> map(LambdaQueryWrapper<E> wrapper,SFunction<E, A> keyFunc,SFunction<E, P> valueFunc,Consumer<E>... peeks)` | 【原文待译】ignore |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Map<A, P> map(LambdaQueryWrapper<E> wrapper,SFunction<E, A> keyFunc,SFunction<E, P> valueFunc,boolean isParallel,Consumer<E>... peeks)` | 传入Wrappers和key，从数据库中根据条件查询出对应的列表，封装成Map |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Map<K, D> group(LambdaQueryWrapper<T> wrapper,SFunction<T, K> sFunction,Collector<T, A, D> downstream,Consumer<T>... peeks)` | 【原文待译】ignore |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Map<K, D> group(LambdaQueryWrapper<T> wrapper,SFunction<T, K> sFunction,Collector<T, A, D> downstream,boolean isParallel,Consumer<T>... peeks)` | 传入Wrappers和key，从数据库中根据条件查询出对应的列表，封装成Map |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Map<K, D> listGroupBy(List<T> list,SFunction<T, K> sFunction,Collector<T, A, D> downstream,Consumer<T>... peeks)` | 【原文待译】ignore |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Map<K, D> listGroupBy(List<T> list,SFunction<T, K> sFunction,Collector<T, A, D> downstream,boolean isParallel,Consumer<T>... peeks)` | 对list进行groupBy操作 |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Map<K, List<T>> group(LambdaQueryWrapper<T> wrapper,SFunction<T, K> sFunction,boolean isParallel,Consumer<T>... peeks)` | 【原文待译】ignore |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Map<K, List<T>> listGroupBy(List<T> list,SFunction<T, K> sFunction,Consumer<T>... peeks)` | 【原文待译】ignore |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Map<K, List<T>> listGroupBy(List<T> list,SFunction<T, K> sFunction,boolean isParallel,Consumer<T>... peeks)` | 【原文待译】ignore |
| `com.baomidou.mybatisplus.extension.toolkit.SimpleQuery` | `Stream<E> peekStream(List<E> list,boolean isParallel,Consumer<E>... peeks)` | 将list转为Stream流，然后再叠加peek操作 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `E getObject(Log log,List<E> list)` | 从list中取第一条数据返回对应List中泛型的单个结果 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `E getObject(Supplier<Log> supplier,List<E> list)` | 【原文待译】@since 3.4.3 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `M getMapper(Class<T> entityClass,SqlSession sqlSession)` | 通过entityClass获取Mapper，记得要释放连接 例： SqlSession sqlSession = SqlHelper.sqlSession(entityClass); try { BaseMapper userMapper = getMapper(User.class, sqlSession); finally { sqlSession.close(); } } |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `R execute(Class<T> entityClass,SFunction<M, R> sFunction)` | 通过entityClass获取BaseMapper，再传入lambda使用该mapper，本方法自动释放链接 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `SqlSession sqlSession(Class<?> clazz)` | 获取Session |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `SqlSession sqlSessionBatch(Class<?> clazz)` | 批量操作 SqlSession |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `SqlSessionFactory sqlSessionFactory(Class<?> clazz)` | 获取SqlSessionFactory |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `String getSqlStatement(Class<?> mapper,SqlMethod sqlMethod)` | 获取mapperStatementId |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `TableInfo table(Class<?> clazz)` | 获取TableInfo |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `boolean executeBatch(Class<?> entityClass,Log log,Collection<E> list,int batchSize,BiConsumer<SqlSession, E> consumer)` | 执行批量操作 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `boolean executeBatch(Class<?> entityClass,Log log,Consumer<SqlSession> consumer)` | 执行批量操作 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `boolean executeBatch(SqlSessionFactory sqlSessionFactory,Log log,Collection<E> list,int batchSize,BiConsumer<SqlSession, E> consumer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `boolean executeBatch(SqlSessionFactory sqlSessionFactory,Log log,Consumer<SqlSession> consumer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `boolean retBool(Integer result)` | 判断数据库操作是否成功 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `boolean retBool(List<BatchResult> result)` | 批量操作是否成功 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `boolean retBool(Long result)` | 判断数据库操作是否成功 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `boolean saveOrUpdateBatch(Class<?> entityClass,Class<?> mapper,Log log,Collection<E> list,int batchSize,BiPredicate<SqlSession, E> predicate,BiConsumer<SqlSession, E> consumer)` | 批量更新或保存 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `boolean saveOrUpdateBatch(SqlSessionFactory sqlSessionFactory,Class<?> mapper,Log log,Collection<E> list,int batchSize,BiPredicate<SqlSession, E> predicate,BiConsumer<SqlSession, E> consumer)` | 批量更新或保存 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlHelper` | `long retCount(Long result)` | 返回SelectCount执行结果 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlParserUtils` | `String getOriginalCountSql(String originalSql)` | 获取 COUNT 原生 SQL 包装 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlParserUtils` | `String removeWrapperSymbol(String tableOrColumn)` | 去除表或字段包裹符号 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlRunner` | `E selectPage(E page,String sql,Object... args)` | 分页查询 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlRunner` | `List<Map<String, Object>> selectList(String sql,Object... args)` | 根据sql查询Map结果集 SqlRunner.db().selectList("select * from tbl_user where name={0}", "Caratacus") |
| `com.baomidou.mybatisplus.extension.toolkit.SqlRunner` | `List<Object> selectObjs(String sql,Object... args)` | 根据sql查询一个字段值的结果集 注意：该方法只会返回一个字段的值， 如果需要多字段，请参考#selectList(String, Object...) |
| `com.baomidou.mybatisplus.extension.toolkit.SqlRunner` | `Map<String, Object> selectOne(String sql,Object... args)` | 获取单条记录 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlRunner` | `Object selectObj(String sql,Object... args)` | 根据sql查询一个字段值的一条结果 注意：该方法只会返回一个字段的值， 如果需要多字段，请参考#selectOne(String, Object...) |
| `com.baomidou.mybatisplus.extension.toolkit.SqlRunner` | `SqlRunner db()` | 获取默认的SqlQuery(适用于单库) |
| `com.baomidou.mybatisplus.extension.toolkit.SqlRunner` | `SqlRunner db(Class<?> clazz)` | 根据当前class对象获取SqlQuery(适用于多库) |
| `com.baomidou.mybatisplus.extension.toolkit.SqlRunner` | `boolean delete(String sql,Object... args)` | 执行删除语句 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlRunner` | `boolean insert(String sql,Object... args)` | 执行插入语句 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlRunner` | `boolean update(String sql,Object... args)` | 执行更新语句 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlRunner` | `long selectCount(String sql,Object... args)` | 查询总数 |
| `com.baomidou.mybatisplus.extension.toolkit.SqlRunner` | `void close()` | 【原文待译】@deprecated 3.5.3.2 |
