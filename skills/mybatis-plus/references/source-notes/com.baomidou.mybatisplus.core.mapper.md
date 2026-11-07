# com.baomidou.mybatisplus.core.mapper

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<BatchResult> insert(Collection<T> entityList)` | 插入（批量） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<BatchResult> insert(Collection<T> entityList,int batchSize)` | 插入（批量） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<BatchResult> insertOrUpdate(Collection<T> entityList)` | 批量修改或插入 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<BatchResult> insertOrUpdate(Collection<T> entityList,BiPredicate<BatchSqlSession, T> insertPredicate)` | 批量修改或插入 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<BatchResult> insertOrUpdate(Collection<T> entityList,BiPredicate<BatchSqlSession, T> insertPredicate,int batchSize)` | 批量修改或插入 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<BatchResult> insertOrUpdate(Collection<T> entityList,int batchSize)` | 批量修改或插入 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<BatchResult> updateById(Collection<T> entityList)` | 根据ID 批量更新 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<BatchResult> updateById(Collection<T> entityList,int batchSize)` | 根据ID 批量更新 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<E> selectObjs(@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper)` | 根据 Wrapper 条件，查询全部记录 注意： 只返回第一个字段的值 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<Map<String, Object>> selectMaps(@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper)` | 根据 Wrapper 条件，查询全部记录 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<Map<String, Object>> selectMaps(IPage<? extends Map<String, Object>> page,@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper)` | 根据 Wrapper 条件，查询全部记录（并翻页） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<T> selectBatchIds(@Param(Constants.COLL)
Collection<? extends Serializable> idList)` | 查询（根据ID 批量查询） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<T> selectByIds(@Param(Constants.COLL)
Collection<? extends Serializable> idList)` | 查询（根据ID 批量查询） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<T> selectByMap(Map<String, Object> columnMap)` | 查询（根据 columnMap 条件） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<T> selectList(@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper)` | 根据 entity 条件，查询全部记录 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `List<T> selectList(IPage<T> page,@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper)` | 根据 entity 条件，查询全部记录（并翻页） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `Long selectCount(@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper)` | 根据 Wrapper 条件，查询总记录数 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `P selectMapsPage(P page,@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper)` | 根据 Wrapper 条件，查询全部记录（并翻页） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `P selectPage(P page,@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper)` | 根据 entity 条件，查询全部记录（并翻页） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `T selectById(Serializable id)` | 根据 ID 查询 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `T selectOne(@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper)` | 根据 entity 条件，查询一条记录 查询一条记录，例如 qw.last("limit 1") 限制取一条记录, 注意：多条数据会报异常 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `T selectOne(@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper,boolean throwEx)` | 根据 entity 条件，查询一条记录，现在会根据throwEx参数判断是否抛出异常，如果为false就直接返回一条数据 查询一条记录，例如 qw.last("limit 1") 限制取一条记录, 注意：多条数据会报异常 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `boolean exists(Wrapper<T> queryWrapper)` | 根据 Wrapper 条件，判断是否存在记录 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `boolean insertOrUpdate(T entity)` | 主键存在更新记录，否插入一条记录 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `int delete(@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper)` | 根据 entity 条件，删除记录 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `int deleteBatchIds(@Param(Constants.COLL)
Collection<?> idList)` | 删除（根据ID或实体 批量删除） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `int deleteById(Object obj,boolean useFill)` | 根据 ID 删除 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `int deleteById(Serializable id)` | 根据 ID 删除 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `int deleteById(T entity)` | 根据实体(ID)删除 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `int deleteByIds(@Param(Constants.COLL)
Collection<?> collections,boolean useFill)` | 删除（根据ID或实体 批量删除） 普通删除: DELETE FROM h2user WHERE id IN ( ? , ? ) 逻辑删除: UPDATE h2user SET deleted=1 WHERE id IN ( ? , ? ) AND deleted=0 逻辑删除(填充): UPDATE h2user SET delete_user = 'xxx', deleted=1 WHERE id IN ( ? , ? ) AND deleted=0 注意:无论参数为id还是实体,填充参数只会以方法追加的et参数为准. |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `int deleteByIds(@Param(Constants.COLL)
Collection<?> idList)` | 删除（根据ID或实体 批量删除） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `int deleteByMap(Map<String, Object> columnMap)` | 根据 columnMap 条件，删除记录 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `int insert(T entity)` | 插入一条记录 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `int update(@Param(Constants.ENTITY)
T entity,@Param(Constants.WRAPPER)
Wrapper<T> updateWrapper)` | 根据 whereEntity 条件，更新记录 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `int update(@Param(Constants.WRAPPER)
Wrapper<T> updateWrapper)` | 根据 Wrapper 更新记录 此方法无法进行自动填充,如需自动填充请使用#update(Object, Wrapper) |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `int updateById(@Param(Constants.ENTITY)
T entity)` | 根据 ID 修改 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `void selectBatchIds(@Param(Constants.COLL)
Collection<? extends Serializable> idList,ResultHandler<T> resultHandler)` | @param idList idList 主键ID列表(不能为 null 以及 empty) |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `void selectByIds(@Param(Constants.COLL)
Collection<? extends Serializable> idList,ResultHandler<T> resultHandler)` | 查询（根据ID 批量查询） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `void selectByMap(Map<String, Object> columnMap,ResultHandler<T> resultHandler)` | 查询（根据 columnMap 条件） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `void selectList(@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper,ResultHandler<T> resultHandler)` | 根据 entity 条件，查询全部记录 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `void selectList(IPage<T> page,@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper,ResultHandler<T> resultHandler)` | 根据 entity 条件，查询全部记录（并翻页） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `void selectMaps(@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper,ResultHandler<Map<String, Object>> resultHandler)` | 根据 Wrapper 条件，查询全部记录 |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `void selectMaps(IPage<? extends Map<String, Object>> page,@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper,ResultHandler<Map<String, Object>> resultHandler)` | 根据 Wrapper 条件，查询全部记录（并翻页） |
| `com.baomidou.mybatisplus.core.mapper.BaseMapper` | `void selectObjs(@Param(Constants.WRAPPER)
Wrapper<T> queryWrapper,ResultHandler<E> resultHandler)` | 根据 Wrapper 条件，查询全部记录 注意： 只返回第一个字段的值 |
