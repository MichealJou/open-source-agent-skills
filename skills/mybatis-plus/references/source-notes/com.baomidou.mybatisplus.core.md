# com.baomidou.mybatisplus.core

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.InjectorResolver` | `void resolve()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `Cache getCache(String id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `Collection<Cache> getCaches()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `Collection<KeyGenerator> getKeyGenerators()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `Collection<MappedStatement> getMappedStatements()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `Collection<ParameterMap> getParameterMaps()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `Collection<ResultMap> getResultMaps()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `Collection<String> getCacheNames()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `Collection<String> getKeyGeneratorNames()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `Collection<String> getMappedStatementNames()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `Collection<String> getParameterMapNames()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `Collection<String> getResultMapNames()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `Executor newExecutor(Transaction transaction,ExecutorType executorType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `KeyGenerator getKeyGenerator(String id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `Map<String, XNode> getSqlFragments()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `MappedStatement getMappedStatement(String id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `MappedStatement getMappedStatement(String id,boolean validateIncompleteStatements)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `MapperRegistry getMapperRegistry()` | 使用自己的 MybatisMapperRegistry |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `ParameterMap getParameterMap(String id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `ResultMap getResultMap(String id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `T getMapper(Class<T> type,SqlSession sqlSession)` | 使用自己的 MybatisMapperRegistry |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `boolean hasCache(String id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `boolean hasKeyGenerator(String id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `boolean hasMapper(Class<?> type)` | 使用自己的 MybatisMapperRegistry |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `boolean hasParameterMap(String id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `boolean hasResultMap(String id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `boolean hasStatement(String statementName,boolean validateIncompleteStatements)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `void addCache(Cache cache)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `void addKeyGenerator(String id,KeyGenerator keyGenerator)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `void addMappedStatement(MappedStatement ms)` | MybatisPlus 加载 SQL 顺序： 1、加载 XML中的 SQL 2、加载 SqlProvider 中的 SQL 3、XmlSql 与 SqlProvider不能包含相同的 SQL 调整后的 SQL优先级：XmlSql > sqlProvider > CurdSql |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `void addMapper(Class<T> type)` | 使用自己的 MybatisMapperRegistry |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `void addMappers(String packageName)` | 使用自己的 MybatisMapperRegistry |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `void addMappers(String packageName,Class<?> superType)` | 使用自己的 MybatisMapperRegistry |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `void addNewMapper(Class<T> type)` | 新增注入新的 Mapper 信息，新增前会清理之前的缓存信息 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `void addParameterMap(ParameterMap pm)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `void addResultMap(ResultMap rm)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `void checkGloballyForDiscriminatedNestedResultMaps(ResultMap rm)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `void removeMapper(Class<T> type)` | 移除 Mapper 相关缓存，支持 GroovyClassLoader 动态注入 Mapper |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `void setDefaultEnumTypeHandler(Class<? extends TypeHandler> typeHandler)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisConfiguration` | `void setDefaultScriptingLanguage(Class<? extends LanguageDriver> driver)` | 指定动态SQL生成的默认语言 |
| `com.baomidou.mybatisplus.core.MybatisMapperAnnotationBuilder` | `Class<?> getMethodReturnType(String mapperFqn,String localStatementId)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisMapperAnnotationBuilder` | `void parse()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisMapperBuilderAssistant` | `ResultMapping buildResultMapping(Class<?> resultType,String property,String column,Class<?> javaType,JdbcType jdbcType,String nestedSelect,String nestedResultMap,String notNullColumn,String columnPrefix,Class<? extends TypeHandler<?>> typeHandler,List<ResultFlag> flags,String resultSet,String foreignColumn,boolean lazy)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisMapperRegistry` | `Collection<Class<?>> getMappers()` | 使用自己的 knownMappers |
| `com.baomidou.mybatisplus.core.MybatisMapperRegistry` | `T getMapper(Class<T> type,SqlSession sqlSession)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisMapperRegistry` | `boolean hasMapper(Class<T> type)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisMapperRegistry` | `void addMapper(Class<T> type)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisMethodResolver` | `void resolve()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisParameterHandler` | `void processParameter(Object parameter)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisPlusVersion` | `String getVersion()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisSqlSessionFactoryBuilder` | `SqlSessionFactory build(Configuration configuration)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisSqlSessionFactoryBuilder` | `SqlSessionFactory build(InputStream inputStream,String environment,Properties properties)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisSqlSessionFactoryBuilder` | `SqlSessionFactory build(Reader reader,String environment,Properties properties)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisXMLConfigBuilder` | `Configuration parse()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisXMLLanguageDriver` | `ParameterHandler createParameterHandler(MappedStatement mappedStatement,Object parameterObject,BoundSql boundSql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisXMLLanguageDriver` | `SqlSource createSqlSource(Configuration configuration,String script,Class<?> parameterType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisXMLLanguageDriver` | `SqlSource createSqlSource(Configuration configuration,XNode script,Class<?> parameterType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisXMLMapperBuilder` | `XNode getSqlFragment(String refid)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisXMLMapperBuilder` | `void parse()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisXMLScriptBuilder` | `SqlSource parseScriptNode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.MybatisXMLScriptBuilder` | `String replaceLeadingAndTrailingWhitespace(String str)` | 将前后空白符替换成空格 |
