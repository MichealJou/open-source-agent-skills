# com.baomidou.mybatisplus.extension.repository

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.repository.AbstractRepository` | `Class<M> getMapperClass()` | @return baseMapper 真实类型 |
| `com.baomidou.mybatisplus.extension.repository.AbstractRepository` | `Class<T> getEntityClass()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.repository.AbstractRepository` | `Map<String, Object> getMap(Wrapper<T> queryWrapper)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.repository.AbstractRepository` | `Optional<T> getOneOpt(Wrapper<T> queryWrapper,boolean throwEx)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.repository.AbstractRepository` | `T getOne(Wrapper<T> queryWrapper,boolean throwEx)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.repository.AbstractRepository` | `V getObj(Wrapper<T> queryWrapper,Function<? super Object, V> mapper)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.repository.AbstractRepository` | `boolean removeById(Serializable id,boolean useFill)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.repository.AbstractRepository` | `boolean saveOrUpdate(T entity)` | TableId 注解存在更新记录，否插入一条记录 |
| `com.baomidou.mybatisplus.extension.repository.CrudRepository` | `M getBaseMapper()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.repository.CrudRepository` | `boolean saveBatch(Collection<T> entityList,int batchSize)` | 批量插入 |
| `com.baomidou.mybatisplus.extension.repository.CrudRepository` | `boolean saveOrUpdateBatch(Collection<T> entityList,int batchSize)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.repository.CrudRepository` | `boolean updateBatchById(Collection<T> entityList,int batchSize)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `BaseMapper<T> getBaseMapper()` | 获取对应 entity 的 BaseMapper |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `Class<T> getEntityClass()` | 获取 entity 的 class |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `E page(E page)` | 无条件翻页查询 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `E page(E page,Wrapper<T> queryWrapper)` | 翻页查询 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `E pageMaps(E page)` | 无条件翻页查询 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `E pageMaps(E page,Wrapper<T> queryWrapper)` | 翻页查询 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `KtQueryChainWrapper<T> ktQuery()` | 链式查询 lambda 式 kotlin 使用 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `KtUpdateChainWrapper<T> ktUpdate()` | 链式查询 lambda 式 kotlin 使用 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `LambdaQueryChainWrapper<T> lambdaQuery()` | 链式查询 lambda 式 注意：不支持 Kotlin |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `LambdaQueryChainWrapper<T> lambdaQuery(T entity)` | 链式查询 lambda 式 注意：不支持 Kotlin |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `LambdaUpdateChainWrapper<T> lambdaUpdate()` | 链式更改 lambda 式 注意：不支持 Kotlin |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `List<E> listObjs()` | 查询全部记录 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `List<E> listObjs(Wrapper<T> queryWrapper)` | 根据 Wrapper 条件，查询全部记录 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `List<Map<String, Object>> listMaps()` | 查询所有列表 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `List<Map<String, Object>> listMaps(IPage<? extends Map<String, Object>> page)` | 查询列表 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `List<Map<String, Object>> listMaps(IPage<? extends Map<String, Object>> page,Wrapper<T> queryWrapper)` | 查询列表 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `List<Map<String, Object>> listMaps(Wrapper<T> queryWrapper)` | 查询列表 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `List<T> list()` | 查询所有 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `List<T> list(IPage<T> page)` | 分页查询单表数据 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `List<T> list(IPage<T> page,Wrapper<T> queryWrapper)` | 查询列表 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `List<T> list(Wrapper<T> queryWrapper)` | 查询列表 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `List<T> listByIds(Collection<? extends Serializable> idList)` | 查询（根据ID 批量查询） |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `List<T> listByMap(Map<String, Object> columnMap)` | 查询（根据 columnMap 条件） |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `List<V> listObjs(Function<? super Object, V> mapper)` | 查询全部记录 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `List<V> listObjs(Wrapper<T> queryWrapper,Function<? super Object, V> mapper)` | 根据 Wrapper 条件，查询全部记录 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `Map<String, Object> getMap(Wrapper<T> queryWrapper)` | 根据 Wrapper，查询一条记录 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `Optional<T> getOneOpt(Wrapper<T> queryWrapper)` | 根据 Wrapper，查询一条记录 结果集，如果是多个会抛出异常，随机取一条加上限制条件 wrapper.last("LIMIT 1") |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `Optional<T> getOneOpt(Wrapper<T> queryWrapper,boolean throwEx)` | 根据 Wrapper，查询一条记录 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `Optional<T> getOptById(Serializable id)` | 根据 ID 查询，返回一个Option对象 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `QueryChainWrapper<T> query()` | 链式查询 普通 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `T getById(Serializable id)` | 根据 ID 查询 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `T getOne(Wrapper<T> queryWrapper)` | 根据 Wrapper，查询一条记录 结果集，如果是多个会抛出异常，随机取一条加上限制条件 wrapper.last("LIMIT 1") |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `T getOne(Wrapper<T> queryWrapper,boolean throwEx)` | 根据 Wrapper，查询一条记录 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `UpdateChainWrapper<T> update()` | 链式更改 普通 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `V getObj(Wrapper<T> queryWrapper,Function<? super Object, V> mapper)` | 根据 Wrapper，查询一条记录 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean exists(Wrapper<T> queryWrapper)` | 查询指定条件是否存在数据 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean remove(Wrapper<T> queryWrapper)` | 根据 entity 条件，删除记录 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean removeById(Serializable id)` | 根据 ID 删除 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean removeById(Serializable id,boolean useFill)` | 根据 ID 删除 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean removeById(T entity)` | 根据实体(ID)删除 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean removeByIds(Collection<?> list)` | 删除（根据ID 批量删除） |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean removeByIds(Collection<?> list,boolean useFill)` | 批量删除 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean removeByMap(Map<String, Object> columnMap)` | 根据 columnMap 条件，删除记录 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean save(T entity)` | 插入一条记录（选择字段，策略插入） |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean saveBatch(Collection<T> entityList,int batchSize)` | 插入（批量） |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean saveOrUpdate(T entity)` | TableId 注解存在更新记录，否插入一条记录 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean saveOrUpdateBatch(Collection<T> entityList,int batchSize)` | 批量修改插入 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean update(T entity,Wrapper<T> updateWrapper)` | 根据 whereEntity 条件，更新记录 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean update(Wrapper<T> updateWrapper)` | 根据 UpdateWrapper 条件，更新记录 需要设置sqlset 此方法无法进行自动填充,如需自动填充请使用#update(Object, Wrapper) |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean updateBatchById(Collection<T> entityList,int batchSize)` | 根据ID 批量更新 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `boolean updateById(T entity)` | 根据 ID 选择修改 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `long count()` | 查询总记录数 |
| `com.baomidou.mybatisplus.extension.repository.IRepository` | `long count(Wrapper<T> queryWrapper)` | 根据 Wrapper 条件，查询总记录数 |
