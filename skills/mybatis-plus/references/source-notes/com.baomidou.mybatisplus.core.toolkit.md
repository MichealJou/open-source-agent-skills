# com.baomidou.mybatisplus.core.toolkit

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.toolkit.AES` | `String decrypt(String data,String key)` | 解密 |
| `com.baomidou.mybatisplus.core.toolkit.AES` | `String encrypt(String data,String key)` | 加密 |
| `com.baomidou.mybatisplus.core.toolkit.AES` | `String generateRandomKey()` | 生成一个随机字符串密钥 |
| `com.baomidou.mybatisplus.core.toolkit.AES` | `byte[] decrypt(byte[] data,byte[] key)` | 解密 |
| `com.baomidou.mybatisplus.core.toolkit.AES` | `byte[] encrypt(byte[] data,byte[] key)` | 加密 |
| `com.baomidou.mybatisplus.core.toolkit.AnnotationUtils` | `T findFirstAnnotation(Class<T> annotationClazz,Class<?> clz)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.AnnotationUtils` | `T findFirstAnnotation(Class<T> annotationClazz,Field field)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.AnnotationUtils` | `T findFirstAnnotation(Class<T> annotationClazz,Method method)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.AopUtils` | `T getTargetObject(T proxy)` | 获取源目标对象 |
| `com.baomidou.mybatisplus.core.toolkit.AopUtils` | `boolean isLoadSpringAop()` | 是否加载Spring-Aop模块 |
| `com.baomidou.mybatisplus.core.toolkit.ArrayUtils` | `boolean isArray(Object obj)` | 判断是否为数组 |
| `com.baomidou.mybatisplus.core.toolkit.ArrayUtils` | `boolean isEmpty(Object[] array)` | 判断数据是否为空 |
| `com.baomidou.mybatisplus.core.toolkit.ArrayUtils` | `boolean isNotEmpty(Object[] array)` | 判断数组是否不为空 |
| `com.baomidou.mybatisplus.core.toolkit.Assert` | `void isEmpty(Map<?, ?> map,String message,Object... params)` | 断言这个 map 为 empty 为 empty 则抛异常 |
| `com.baomidou.mybatisplus.core.toolkit.Assert` | `void isFalse(boolean expression,String message,Object... params)` | 断言这个 boolean 为 false 为 true 则抛出异常 |
| `com.baomidou.mybatisplus.core.toolkit.Assert` | `void isNull(Object object,String message,Object... params)` | 断言这个 object 为 null 不为 null 则抛异常 |
| `com.baomidou.mybatisplus.core.toolkit.Assert` | `void isTrue(boolean expression,String message,Object... params)` | 断言这个 boolean 为 true 为 false 则抛出异常 |
| `com.baomidou.mybatisplus.core.toolkit.Assert` | `void notEmpty(Collection<?> collection,String message,Object... params)` | 断言这个 collection 不为 empty 为 empty 则抛异常 |
| `com.baomidou.mybatisplus.core.toolkit.Assert` | `void notEmpty(Map<?, ?> map,String message,Object... params)` | 断言这个 map 不为 empty 为 empty 则抛异常 |
| `com.baomidou.mybatisplus.core.toolkit.Assert` | `void notEmpty(Object[] array,String message,Object... params)` | 断言这个 数组 不为 empty 为 empty 则抛异常 |
| `com.baomidou.mybatisplus.core.toolkit.Assert` | `void notEmpty(String value,String message,Object... params)` | 断言这个 value 不为 empty 为 empty 则抛异常 |
| `com.baomidou.mybatisplus.core.toolkit.Assert` | `void notNull(Object object,String message,Object... params)` | 断言这个 object 不为 null 为 null 则抛异常 |
| `com.baomidou.mybatisplus.core.toolkit.BeanUtils` | `List<Map<String, Object>> beansToMaps(List<T> beans)` | List<T> 转换为 List<Map<String, Object>> |
| `com.baomidou.mybatisplus.core.toolkit.BeanUtils` | `List<T> mapsToBeans(List<? extends Map<String, ?>> maps,Class<T> clazz)` | List<Map<String, Object>> 转换为 List<T> |
| `com.baomidou.mybatisplus.core.toolkit.BeanUtils` | `Map<String, Object> beanToMap(Object bean)` | 将对象装换为 map,对象转成 map，key肯定是字符串 |
| `com.baomidou.mybatisplus.core.toolkit.BeanUtils` | `T mapToBean(Map<String, ?> map,Class<T> clazz)` | map 转换为 java bean 对象 |
| `com.baomidou.mybatisplus.core.toolkit.ClassUtils` | `Class<?> getUserClass(Class<?> clazz)` | 获取当前对象的 class |
| `com.baomidou.mybatisplus.core.toolkit.ClassUtils` | `Class<?> getUserClass(Object object)` | 获取当前对象的class |
| `com.baomidou.mybatisplus.core.toolkit.ClassUtils` | `Class<?> toClassConfident(String name)` | 请仅在确定类存在的情况下调用该方法 |
| `com.baomidou.mybatisplus.core.toolkit.ClassUtils` | `Class<?> toClassConfident(String name,ClassLoader classLoader)` | @param name 全类名 |
| `com.baomidou.mybatisplus.core.toolkit.ClassUtils` | `ClassLoader getDefaultClassLoader()` | 【原文待译】Return the default ClassLoader to use: typically the thread context ClassLoader, if available; the ClassLoader that loaded the ClassUtils class will be used as fallback. Call this method if you intend to use the thread context ClassLoader in a scenario where you clearly prefer a non-null ClassLoader… |
| `com.baomidou.mybatisplus.core.toolkit.ClassUtils` | `String getPackageName(Class<?> clazz)` | 【原文待译】Determine the name of the package of the given class, e.g. "java.lang" for the java.lang.String class. |
| `com.baomidou.mybatisplus.core.toolkit.ClassUtils` | `String getPackageName(String fqClassName)` | 【原文待译】Determine the name of the package of the given fully-qualified class name, e.g. "java.lang" for the java.lang.String class name. |
| `com.baomidou.mybatisplus.core.toolkit.ClassUtils` | `T newInstance(Class<T> clazz)` | 根据指定的 class ， 实例化一个对象，根据构造参数来实例化 在 java9 及其之后的版本 Class.newInstance() 方法已被废弃 |
| `com.baomidou.mybatisplus.core.toolkit.ClassUtils` | `T newInstance(String clazzName)` | 实例化对象. |
| `com.baomidou.mybatisplus.core.toolkit.ClassUtils` | `boolean isBoolean(Class<?> type)` | 判断传入的类型是否是布尔类型 |
| `com.baomidou.mybatisplus.core.toolkit.ClassUtils` | `boolean isProxy(Class<?> clazz)` | 判断是否为代理对象 |
| `com.baomidou.mybatisplus.core.toolkit.CollectionUtils` | `HashMap<K, V> newHashMap()` | 创建默认HashMap |
| `com.baomidou.mybatisplus.core.toolkit.CollectionUtils` | `HashMap<K, V> newHashMapWithExpectedSize(int expectedSize)` | 根据预期大小创建HashMap. |
| `com.baomidou.mybatisplus.core.toolkit.CollectionUtils` | `List<List<T>> split(Collection<T> entityList,int batchSize)` | 切割集合为多个集合 |
| `com.baomidou.mybatisplus.core.toolkit.CollectionUtils` | `List<T> toList(T... t)` | 构建List |
| `com.baomidou.mybatisplus.core.toolkit.CollectionUtils` | `List<V> getCollection(Map<K, V> map,Iterable<K> keys)` | 批量取出Map中的值 |
| `com.baomidou.mybatisplus.core.toolkit.CollectionUtils` | `List<V> getCollection(Map<K, V> map,Iterable<K> keys,Comparator<V> comparator)` | 批量取出Map中的值 |
| `com.baomidou.mybatisplus.core.toolkit.CollectionUtils` | `V computeIfAbsent(Map<K, V> concurrentHashMap,K key,Function<? super K, ? extends V> mappingFunction)` | 用来过渡下Jdk1.8下ConcurrentHashMap的性能bug JDK-8161372 A temporary workaround for Java 8 ConcurrentHashMap#computeIfAbsent specific performance issue: JDK-8161372. |
| `com.baomidou.mybatisplus.core.toolkit.CollectionUtils` | `boolean isEmpty(Collection<?> coll)` | 校验集合是否为空 |
| `com.baomidou.mybatisplus.core.toolkit.CollectionUtils` | `boolean isEmpty(Map<?, ?> map)` | 判断Map是否为空 |
| `com.baomidou.mybatisplus.core.toolkit.CollectionUtils` | `boolean isNotEmpty(Collection<?> coll)` | 校验集合是否不为空 |
| `com.baomidou.mybatisplus.core.toolkit.CollectionUtils` | `boolean isNotEmpty(Map<?, ?> map)` | 判断Map是否不为空 |
| `com.baomidou.mybatisplus.core.toolkit.EncryptUtils` | `String md5Base64(String str)` | MD5 Base64 加密 |
| `com.baomidou.mybatisplus.core.toolkit.ExceptionUtils` | `MybatisPlusException mpe(String msg,Object... params)` | 重载的方法 |
| `com.baomidou.mybatisplus.core.toolkit.ExceptionUtils` | `MybatisPlusException mpe(String msg,Throwable t,Object... params)` | 返回一个新的异常，统一构建，方便统一处理 |
| `com.baomidou.mybatisplus.core.toolkit.ExceptionUtils` | `MybatisPlusException mpe(Throwable t)` | 重载的方法 |
| `com.baomidou.mybatisplus.core.toolkit.ExceptionUtils` | `void throwMpe(boolean condition,String msg,Object... params)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils` | `Class<?> getSuperMapperClass(Configuration configuration)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils` | `GlobalConfig defaults()` | 获取默认 MybatisGlobalConfig |
| `com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils` | `GlobalConfig getGlobalConfig(Configuration configuration)` | 获取MybatisGlobalConfig (统一所有入口) |
| `com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils` | `GlobalConfig.DbConfig getDbConfig(Configuration configuration)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils` | `ISqlInjector getSqlInjector(Configuration configuration)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils` | `IdType getIdType(Configuration configuration)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils` | `List<IKeyGenerator> getKeyGenerators(Configuration configuration)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils` | `Optional<AnnotationHandler> getAnnotationHandler(Configuration configuration)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils` | `Optional<MetaObjectHandler> getMetaObjectHandler(Configuration configuration)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils` | `Set<String> getMapperRegistryCache(Configuration configuration)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils` | `SqlSessionFactory currentSessionFactory(Class<?> clazz)` | 获取当前的SqlSessionFactory |
| `com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils` | `boolean isSupperMapperChildren(Configuration configuration,Class<?> mapperClass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.GlobalConfigUtils` | `void setGlobalConfig(Configuration configuration,GlobalConfig globalConfig)` | 设置全局设置(以configuration地址值作为Key) |
| `com.baomidou.mybatisplus.core.toolkit.IdWorker` | `String get32UUID()` | 使用ThreadLocalRandom获取UUID获取更优的效果 去掉"-" |
| `com.baomidou.mybatisplus.core.toolkit.IdWorker` | `String getIdStr()` | 获取唯一ID |
| `com.baomidou.mybatisplus.core.toolkit.IdWorker` | `String getIdStr(Object entity)` | 获取唯一ID |
| `com.baomidou.mybatisplus.core.toolkit.IdWorker` | `String getMillisecond()` | 格式化的毫秒时间 |
| `com.baomidou.mybatisplus.core.toolkit.IdWorker` | `String getTimeId()` | 时间 ID = Time + ID 例如：可用于商品订单 ID |
| `com.baomidou.mybatisplus.core.toolkit.IdWorker` | `long getId()` | 获取唯一ID |
| `com.baomidou.mybatisplus.core.toolkit.IdWorker` | `long getId(Object entity)` | 获取唯一ID |
| `com.baomidou.mybatisplus.core.toolkit.IdWorker` | `void initSequence(long workerId,long dataCenterId)` | 有参构造器 |
| `com.baomidou.mybatisplus.core.toolkit.IdWorker` | `void setIdentifierGenerator(IdentifierGenerator identifierGenerator)` | 自定义id 生成方式 |
| `com.baomidou.mybatisplus.core.toolkit.LambdaUtils` | `LambdaMeta extract(SFunction<T, ?> func)` | 该缓存可能会在任意不定的时间被清除 |
| `com.baomidou.mybatisplus.core.toolkit.LambdaUtils` | `Map<String, ColumnCache> getColumnMap(Class<?> clazz)` | 获取实体对应字段 MAP |
| `com.baomidou.mybatisplus.core.toolkit.LambdaUtils` | `String formatKey(String key)` | 格式化 key 将传入的 key 变更为大写格式 为了支持首字母是大写的字段 |
| `com.baomidou.mybatisplus.core.toolkit.LambdaUtils` | `void installCache(TableInfo tableInfo)` | 将传入的表信息加入缓存 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> execute(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,BatchMethod<T> batchMethod)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> execute(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,BatchMethod<T> batchMethod,int batchSize)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> execute(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,String statement)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> execute(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,String statement,ParameterConvert<T> parameterConvert)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> execute(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,String statement,ParameterConvert<T> parameterConvert,int batchSize)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> execute(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,String statement,int batchSize)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> execute(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,boolean autoCommit,BatchMethod<T> batchMethod)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> execute(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,boolean autoCommit,BatchMethod<T> batchMethod,int batchSize)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> execute(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,boolean autoCommit,String statement)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> execute(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,boolean autoCommit,String statement,ParameterConvert<T> parameterConvert)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> execute(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,boolean autoCommit,String statement,ParameterConvert<T> parameterConvert,int batchSize)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> execute(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,boolean autoCommit,String statement,int batchSize)` | 执行批量操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> saveOrUpdate(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,BatchMethod<T> insertMethod,BiPredicate<BatchSqlSession, T> insertPredicate,BatchMethod<T> updateMethod)` | 批量保存或更新 这里需要注意一下,如果在insertPredicate里判断调用其他sqlSession(类似mapper.xxx)时,要注意一级缓存问题或数据感知问题(因为当前会话数据还未提交) 举个例子(事务开启状态下): 如果当前批次里面执行两个主键相同的数据,当调用mapper.selectById时,如果数据库未有这条记录,在同个sqlSession下,由于一级缓存的问题,下次再查就还是null,导致插入主键冲突, 但使用 BatchSqlSession时,由于每次select操作都会触发一次flushStatements,就会执行更新操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> saveOrUpdate(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,BatchMethod<T> insertMethod,BiPredicate<BatchSqlSession, T> insertPredicate,BatchMethod<T> updateMethod,int batchSize)` | 批量保存或更新 这里需要注意一下,如果在insertPredicate里判断调用其他sqlSession(类似mapper.xxx)时,要注意一级缓存问题或数据感知问题(因为当前会话数据还未提交) 举个例子(事务开启状态下): 如果当前批次里面执行两个主键相同的数据,当调用mapper.selectById时,如果数据库未有这条记录,在同个sqlSession下,由于一级缓存的问题,下次再查就还是null,导致插入主键冲突, 但使用 BatchSqlSession时,由于每次select操作都会触发一次flushStatements,就会执行更新操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> saveOrUpdate(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,boolean autoCommit,BatchMethod<T> insertMethod,BiPredicate<BatchSqlSession, T> insertPredicate,BatchMethod<T> updateMethod)` | 批量保存或更新 这里需要注意一下,如果在insertPredicate里判断调用其他sqlSession(类似mapper.xxx)时,要注意一级缓存问题或数据感知问题(因为当前会话数据还未提交) 举个例子(事务开启状态下): 如果当前批次里面执行两个主键相同的数据,当调用mapper.selectById时,如果数据库未有这条记录,在同个sqlSession下,由于一级缓存的问题,下次再查就还是null,导致插入主键冲突, 但使用 BatchSqlSession时,由于每次select操作都会触发一次flushStatements,就会执行更新操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisBatchUtils` | `List<BatchResult> saveOrUpdate(SqlSessionFactory sqlSessionFactory,Collection<T> dataList,boolean autoCommit,BatchMethod<T> insertMethod,BiPredicate<BatchSqlSession, T> insertPredicate,BatchMethod<T> updateMethod,int batchSize)` | 批量保存或更新 这里需要注意一下,如果在insertPredicate里判断调用其他sqlSession(类似mapper.xxx)时,要注意一级缓存问题或数据感知问题(因为当前会话数据还未提交) 举个例子(事务开启状态下): 如果当前批次里面执行两个主键相同的数据,当调用mapper.selectById时,如果数据库未有这条记录,在同个sqlSession下,由于一级缓存的问题,下次再查就还是null,导致插入主键冲突, 但使用 BatchSqlSession时,由于每次select操作都会触发一次flushStatements,就会执行更新操作 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisUtils` | `MapperProxyMetadata getMapperProxy(Object mapper)` | 获取MapperProxy元数据信息 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisUtils` | `MybatisMapperProxy<?> getMybatisMapperProxy(Object mapper)` | 获取代理实现 |
| `com.baomidou.mybatisplus.core.toolkit.MybatisUtils` | `Object extractMapperProxy(Object mapper)` | 提取MapperProxy |
| `com.baomidou.mybatisplus.core.toolkit.MybatisUtils` | `SqlSessionFactory getSqlSessionFactory(MybatisMapperProxy<?> mybatisMapperProxy)` | 获取SqlSessionFactory 当自定义实现SqlSession时,请实现对SqlSessionFactory的访问 (spring的方式) 当无法获得SqlSessionFactory时,需要将SqlSessionFactory绑定至上下文对象中(原生mybatis访问方式) |
| `com.baomidou.mybatisplus.core.toolkit.MybatisUtils` | `SqlSessionFactory getSqlSessionFactory(SqlSession sqlSession)` | 获取sqlSession中的SqlSessionFactory |
| `com.baomidou.mybatisplus.core.toolkit.MybatisUtils` | `TypeHandler<?> newJsonTypeHandler(Class<? extends TypeHandler<?>> typeHandler,Class<?> javaTypeClass,Field field)` | 实例化Json类型处理器 1.子类需要包含构造(Class,Field) 2.如果无上述构造或者无属性字段,则使用默认构造(Class)进行实例化 |
| `com.baomidou.mybatisplus.core.toolkit.NetUtils` | `InetAddress findFirstNonLoopbackAddress()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.ObjectUtils` | `boolean isEmpty(Object obj)` | 对象空判断 |
| `com.baomidou.mybatisplus.core.toolkit.ObjectUtils` | `boolean isNotEmpty(Object obj)` | 对象非空判断 |
| `com.baomidou.mybatisplus.core.toolkit.ObjectUtils` | `boolean isNotNull(Object... obj)` | 判断object是否不为空,集合会校验size |
| `com.baomidou.mybatisplus.core.toolkit.ObjectUtils` | `boolean isNull(Object... objs)` | 判断object是否为空,集合会校验size |
| `com.baomidou.mybatisplus.core.toolkit.ParameterUtils` | `Optional<IPage> findPage(Object parameterObject)` | 查找分页参数 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils` | `MPBoundSql mpBoundSql(BoundSql boundSql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils` | `MPStatementHandler mpStatementHandler(StatementHandler statementHandler)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils` | `MetaObject getMetaObject(Object object)` | 获取对象元数据信息 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils` | `T realTarget(Object target)` | 获得真正的处理对象,可能多层代理. |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils` | `void setAdditionalParameter(BoundSql boundSql,Map<String, Object> additionalParameters)` | 给 BoundSql 设置 additionalParameters |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPBoundSql` | `List<ParameterMapping> parameterMappings()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPBoundSql` | `Map<String, Object> additionalParameters()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPBoundSql` | `Object parameterObject()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPBoundSql` | `String sql()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPBoundSql` | `void parameterMappings(List<ParameterMapping> parameterMappings)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPBoundSql` | `void sql(String sql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPStatementHandler` | `BoundSql boundSql()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPStatementHandler` | `Configuration configuration()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPStatementHandler` | `Executor executor()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPStatementHandler` | `MPBoundSql mPBoundSql()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPStatementHandler` | `MappedStatement mappedStatement()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.PluginUtils$MPStatementHandler` | `ParameterHandler parameterHandler()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.ReflectionKit` | `Class<?> getSuperClassGenericType(final Class<?> clazz,final Class<?> genericIfc,final int index)` | 反射对象获取泛型 |
| `com.baomidou.mybatisplus.core.toolkit.ReflectionKit` | `Class<?> resolvePrimitiveIfNecessary(Class<?> clazz)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.ReflectionKit` | `List<Field> getFieldList(Class<?> clazz)` | 获取该类的所有属性列表 |
| `com.baomidou.mybatisplus.core.toolkit.ReflectionKit` | `Map<String, Field> excludeOverrideSuperField(Field[] fields,List<Field> superFieldList)` | 排序重置父类属性 |
| `com.baomidou.mybatisplus.core.toolkit.ReflectionKit` | `Map<String, Field> getFieldMap(Class<?> clazz)` | 获取该类的所有属性列表 |
| `com.baomidou.mybatisplus.core.toolkit.ReflectionKit` | `Object getFieldValue(Object entity,String fieldName)` | 获取字段值 |
| `com.baomidou.mybatisplus.core.toolkit.ReflectionKit` | `T setAccessible(T object)` | 设置可访问对象的可访问权限为 true |
| `com.baomidou.mybatisplus.core.toolkit.ReflectionKit` | `boolean isPrimitiveOrWrapper(Class<?> clazz)` | 判断是否为基本类型或基本包装类型 |
| `com.baomidou.mybatisplus.core.toolkit.Sequence` | `long nextId()` | 获取下一个 ID |
| `com.baomidou.mybatisplus.core.toolkit.Sequence` | `long parseIdTimestamp(long id)` | 反解id的时间戳部分 |
| `com.baomidou.mybatisplus.core.toolkit.SerializationUtils` | `Object deserialize(byte[] bytes)` | 【原文待译】Deserialize the byte array into an object. |
| `com.baomidou.mybatisplus.core.toolkit.SerializationUtils` | `T clone(final T object)` | 【原文待译】Deep clone an Object using serialization. This is many times slower than writing clone methods by hand on all objects in your object graph. However, for complex object graphs, or for those that don't support deep cloning this can be a simple alternative implementation. Of course all the objects must… |
| `com.baomidou.mybatisplus.core.toolkit.SerializationUtils` | `byte[] serialize(Object object)` | 【原文待译】Serialize the given object to a byte array. |
| `com.baomidou.mybatisplus.core.toolkit.SetAccessibleAction` | `T run()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String camelToHyphen(String input)` | 驼峰转连字符 StringUtils.camelToHyphen( "managerAdminUserService" ) = manager-admin-user-service |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String camelToUnderline(String param)` | 字符串驼峰转下划线格式 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String concatCapitalize(String concatStr,final String str)` | 拼接字符串第二个字符串第一个字母大写 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String firstToLowerCase(String param)` | 首字母转换小写 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String getTargetColumn(String column)` | 获取真正的字段名 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String prefixToLower(String rawString,int index)` | 前n个首字母小写,之后字符大小写的不变 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String quotaMark(Object obj)` | 使用单引号包含字符串 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String quotaMarkList(Collection<?> coll)` | 使用单引号包含字符串 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String removePrefixAfterPrefixToLower(String rawString,int index)` | 删除字符前缀之后,首字母小写,之后字符大小写的不变 StringUtils.removePrefixAfterPrefixToLower( "isUser", 2 ) = user StringUtils.removePrefixAfterPrefixToLower( "isUserInfo", 2 ) = userInfo |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String replaceAllBlank(String str)` | 字符串去除空白内容： \n 回车 \t 水平制表符 \s 空格 \r 换行 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String sqlArgsFill(String content,Object... args)` | 替换 SQL 语句中的占位符，例如输入 SELECT * FROM test WHERE id = {0} AND name = {1} 会被替换为 SELECT * FROM test WHERE id = 1 AND name = 'MP' 当数组中参数不足时，该方法会抛出错误：数组下标越界ArrayIndexOutOfBoundsException |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String sqlInjectionReplaceBlank(String str)` | SQL 注入字符串去除空白内容： \n 回车 \t 水平制表符 \s 空格 \r 换行 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String sqlParam(Object obj)` | 获取SQL PARAMS字符串 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String toStringTrim(Object o)` | 对象转为字符串去除左右空格 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `String underlineToCamel(String param)` | 字符串下划线转驼峰格式 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `StringBuilder replace(CharSequence src,Pattern ptn,BiIntFunction<Matcher, CharSequence> replacer)` | 根据指定的表达式替换字符串中指定格式的部分 BiIntFunction 中的 第二个 参数将传递 参数在字符串中的索引 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean checkValNotNull(Object object)` | 判断对象是否不为空 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean checkValNull(Object object)` | 判断对象是否为空 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean containsUpperCase(String word)` | 包含大写字母 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean endsWith(String str,String suffix)` | 判断是否以某个字符串结尾（区分大小写） Check if a String ends with a specified suffix. null s are handled without exceptions. Two null references are considered to be equal. The comparison is case sensitive. |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean equals(final CharSequence cs1,final CharSequence cs2)` | 比较两个字符串，相同则返回true。字符串可为null 对字符串大小写敏感 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean isBlank(CharSequence cs)` | 判断字符串中是否全是空白字符 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean isCamel(String str)` | 判断字符串是不是驼峰命名 包含 '_' 不算 首字母大写的不算 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean isCapitalMode(String word)` | 是否为大写命名 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean isCharSequence(Class<?> clazz)` | 是否为CharSequence类型 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean isEmpty(CharSequence cs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean isMixedMode(String word)` | 是否为驼峰下划线混合命名 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean isNotBlank(CharSequence cs)` | 【原文待译】@see #isBlank(CharSequence) |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean isNotColumnName(String str)` | 判断字符串是否符合数据库字段的命名 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean isNotEmpty(CharSequence cs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.StringUtils` | `boolean matches(String regex,String input)` | 正则表达式匹配 |
| `com.baomidou.mybatisplus.core.toolkit.SystemClock` | `String nowDate()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.SystemClock` | `long now()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.TableNameParser` | `Collection<String> tables()` | 【原文待译】parser tables |
| `com.baomidou.mybatisplus.core.toolkit.TableNameParser` | `void accept(TableNameVisitor visitor)` | 接受一个新的访问者，并访问当前 SQL 的表名称 现在我们改成了访问者模式，不在对以前的 SQL 做改动 同时，你可以方便的获得表名位置的索引 |
| `com.baomidou.mybatisplus.core.toolkit.TableNameParser$SqlToken` | `String getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.TableNameParser$SqlToken` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.TableNameParser$SqlToken` | `int compareTo(SqlToken o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.TableNameParser$SqlToken` | `int getEnd()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.TableNameParser$SqlToken` | `int getStart()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.TableNameParser$TableNameVisitor` | `void visit(SqlToken name)` | @param name 表示表名称的 token |
| `com.baomidou.mybatisplus.core.toolkit.Wrappers` | `LambdaQueryWrapper<T> lambdaQuery()` | 获取 LambdaQueryWrapper<T> |
| `com.baomidou.mybatisplus.core.toolkit.Wrappers` | `LambdaQueryWrapper<T> lambdaQuery(Class<T> entityClass)` | 获取 LambdaQueryWrapper<T> |
| `com.baomidou.mybatisplus.core.toolkit.Wrappers` | `LambdaQueryWrapper<T> lambdaQuery(T entity)` | 获取 LambdaQueryWrapper<T> |
| `com.baomidou.mybatisplus.core.toolkit.Wrappers` | `LambdaUpdateWrapper<T> lambdaUpdate()` | 获取 LambdaUpdateWrapper<T> |
| `com.baomidou.mybatisplus.core.toolkit.Wrappers` | `LambdaUpdateWrapper<T> lambdaUpdate(Class<T> entityClass)` | 获取 LambdaUpdateWrapper<T> |
| `com.baomidou.mybatisplus.core.toolkit.Wrappers` | `LambdaUpdateWrapper<T> lambdaUpdate(T entity)` | 获取 LambdaUpdateWrapper<T> |
| `com.baomidou.mybatisplus.core.toolkit.Wrappers` | `QueryWrapper<T> emptyWrapper()` | 获取 EmptyWrapper<T> |
| `com.baomidou.mybatisplus.core.toolkit.Wrappers` | `QueryWrapper<T> query()` | 获取 QueryWrapper<T> |
| `com.baomidou.mybatisplus.core.toolkit.Wrappers` | `QueryWrapper<T> query(Class<T> entityClass)` | 获取 QueryWrapper<T> |
| `com.baomidou.mybatisplus.core.toolkit.Wrappers` | `QueryWrapper<T> query(T entity)` | 获取 QueryWrapper<T> |
| `com.baomidou.mybatisplus.core.toolkit.Wrappers` | `UpdateWrapper<T> update()` | 获取 UpdateWrapper<T> |
| `com.baomidou.mybatisplus.core.toolkit.Wrappers` | `UpdateWrapper<T> update(T entity)` | 获取 UpdateWrapper<T> |
