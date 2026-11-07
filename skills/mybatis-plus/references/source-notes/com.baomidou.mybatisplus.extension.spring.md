# com.baomidou.mybatisplus.extension.spring

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.spring.MybatisPlusApplicationContextAware` | `ApplicationContext getApplicationContext()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.spring.MybatisPlusApplicationContextAware` | `boolean hasApplicationContext()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.spring.MybatisPlusApplicationContextAware` | `void setApplicationContext(@NotNull
ApplicationContext applicationContext)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `Cache getCache()` | 【原文待译】Gets the Cache. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `Class<? extends SqlSessionFactory> getObjectType()` | 【原文待译】{@inheritDoc} |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `Class<? extends VFS> getVfs()` | 【原文待译】Gets the VFS. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `DatabaseIdProvider getDatabaseIdProvider()` | 【原文待译】Gets the DatabaseIdProvider |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `MybatisConfiguration getConfiguration()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `SqlSessionFactory getObject()` | 【原文待译】{@inheritDoc} |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `boolean isSingleton()` | 【原文待译】{@inheritDoc} |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void addMapperLocations(Resource... mapperLocations)` | 【原文待译】Add locations of MyBatis mapper files that are going to be merged into the SqlSessionFactory configuration at runtime. This is an alternative to specifying "<sqlmapper>" entries in an MyBatis config file. This property being based on Spring's resource abstraction also allows for specifying resource … |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void addPlugins(Interceptor... plugins)` | 【原文待译】Add Mybatis plugins. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void addScriptingLanguageDrivers(LanguageDriver... scriptingLanguageDrivers)` | 【原文待译】Add scripting language drivers. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void addTypeAliases(Class<?>... typeAliases)` | 【原文待译】Add type aliases. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void addTypeHandlers(TypeHandler<?>... typeHandlers)` | 【原文待译】Add type handlers. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void afterPropertiesSet()` | 【原文待译】{@inheritDoc} |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void onApplicationEvent(ContextRefreshedEvent event)` | 【原文待译】{@inheritDoc} |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setApplicationContext(ApplicationContext applicationContext)` | 设置上下文对象 注意: 手动构建的bean对象需要手动赋值,通过xml属性初始化的会自动赋值 |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setCache(Cache cache)` | 【原文待译】Sets the Cache. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setConfigLocation(Resource configLocation)` | 【原文待译】Set the location of the MyBatis SqlSessionFactory config file. A typical value is "WEB-INF/mybatis-configuration.xml". |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setConfiguration(MybatisConfiguration configuration)` | 【原文待译】Set a customized MyBatis configuration. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setConfigurationProperties(Properties sqlSessionFactoryProperties)` | 【原文待译】Set optional properties to be passed into the SqlSession configuration, as alternative to a <properties> tag in the configuration xml file. This will be used to resolve placeholders in the config file. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setDataSource(DataSource dataSource)` | 【原文待译】Set the JDBC DataSource that this instance should manage transactions for. The DataSource should match the one used by the SqlSessionFactory: for example, you could specify the same JNDI DataSource for both. A transactional JDBC Connection for this DataSource will be provided to application code acc… |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setDatabaseIdProvider(DatabaseIdProvider databaseIdProvider)` | 【原文待译】Sets the DatabaseIdProvider. As of version 1.2.2 this variable is not initialized by default. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setDefaultEnumTypeHandler(@SuppressWarnings("rawtypes")
Class<? extends TypeHandler> defaultEnumTypeHandler)` | 【原文待译】Set the default type handler class for enum. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setDefaultScriptingLanguageDriver(Class<? extends LanguageDriver> defaultScriptingLanguageDriver)` | 【原文待译】Set a default scripting language driver class. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setEnvironment(String environment)` | 【原文待译】NOTE: This class overrides any Environment you have set in the MyBatis config file. This is used only as a placeholder name. The default value is SqlSessionFactoryBean.class.getSimpleName(). |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setFailFast(boolean failFast)` | 【原文待译】If true, a final check is done on Configuration to assure that all mapped statements are fully loaded and there is no one still pending to resolve includes. Defaults to false. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setMapperLocations(Resource... mapperLocations)` | 【原文待译】Set locations of MyBatis mapper files that are going to be merged into the SqlSessionFactory configuration at runtime. This is an alternative to specifying "<sqlmapper>" entries in an MyBatis config file. This property being based on Spring's resource abstraction also allows for specifying resource … |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setObjectFactory(ObjectFactory objectFactory)` | 【原文待译】Sets the ObjectFactory. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setObjectWrapperFactory(ObjectWrapperFactory objectWrapperFactory)` | 【原文待译】Sets the ObjectWrapperFactory. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setPlugins(Interceptor... plugins)` | 【原文待译】Mybatis plugin list. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setScriptingLanguageDrivers(LanguageDriver... scriptingLanguageDrivers)` | 【原文待译】Set scripting language drivers. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setSqlSessionFactoryBuilder(SqlSessionFactoryBuilder sqlSessionFactoryBuilder)` | 【原文待译】Sets the SqlSessionFactoryBuilder to use when creating the SqlSessionFactory. This is mainly meant for testing so that mock SqlSessionFactory classes can be injected. By default, SqlSessionFactoryBuilder creates DefaultSqlSessionFactory instances. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setTransactionFactory(TransactionFactory transactionFactory)` | 【原文待译】Set the MyBatis TransactionFactory to use. Default is SpringManagedTransactionFactory. The default SpringManagedTransactionFactory should be appropriate for all cases: be it Spring transaction management, EJB CMT or plain JTA. If there is no active transaction, SqlSession operations will execute SQL… |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setTypeAliases(Class<?>... typeAliases)` | 【原文待译】List of type aliases to register. They can be annotated with Alias |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setTypeAliasesPackage(String typeAliasesPackage)` | 【原文待译】Packages to search for type aliases. Since 2.0.1, allow to specify a wildcard such as com.example.*.model. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setTypeAliasesSuperType(Class<?> typeAliasesSuperType)` | 【原文待译】Super class which domain objects have to extend to have a type alias created. No effect if there is no package to scan configured. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setTypeHandlers(TypeHandler<?>... typeHandlers)` | 【原文待译】Set type handlers. They must be annotated with MappedTypes and optionally with MappedJdbcTypes |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setTypeHandlersPackage(String typeHandlersPackage)` | 【原文待译】Packages to search for type handlers. Since 2.0.1, allow to specify a wildcard such as com.example.*.typehandler. |
| `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean` | `void setVfs(Class<? extends VFS> vfs)` | 【原文待译】Sets the VFS. |
