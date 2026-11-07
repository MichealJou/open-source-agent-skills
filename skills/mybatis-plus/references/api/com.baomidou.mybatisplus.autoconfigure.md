# com.baomidou.mybatisplus.autoconfigure

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.autoconfigure.ConfigurationCustomizer`

```java
public interface com.baomidou.mybatisplus.autoconfigure.ConfigurationCustomizer {
  public abstract void customize(com.baomidou.mybatisplus.core.MybatisConfiguration);
}
```

## `com.baomidou.mybatisplus.autoconfigure.DdlApplicationRunner`

```java
public class com.baomidou.mybatisplus.autoconfigure.DdlApplicationRunner implements org.springframework.boot.ApplicationRunner {
  public com.baomidou.mybatisplus.autoconfigure.DdlApplicationRunner(java.util.List<com.baomidou.mybatisplus.extension.ddl.IDdl>);
  public void run(org.springframework.boot.ApplicationArguments);
  public void setAutoCommit(boolean);
  public void setDdlScriptErrorHandler(com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler);
  public void setScriptRunnerConsumer(java.util.function.Consumer<org.apache.ibatis.jdbc.ScriptRunner>);
  public void setThrowException(boolean);
}
```

## `com.baomidou.mybatisplus.autoconfigure.DdlAutoConfiguration`

```java
public class com.baomidou.mybatisplus.autoconfigure.DdlAutoConfiguration {
  public com.baomidou.mybatisplus.autoconfigure.DdlAutoConfiguration();
  public com.baomidou.mybatisplus.autoconfigure.DdlApplicationRunner ddlApplicationRunner(java.util.List<com.baomidou.mybatisplus.extension.ddl.IDdl>);
}
```

## `com.baomidou.mybatisplus.autoconfigure.IdentifierGeneratorAutoConfiguration`

```java
public class com.baomidou.mybatisplus.autoconfigure.IdentifierGeneratorAutoConfiguration {
  public com.baomidou.mybatisplus.autoconfigure.IdentifierGeneratorAutoConfiguration();
  public com.baomidou.mybatisplus.core.incrementer.IdentifierGenerator identifierGenerator(org.springframework.cloud.commons.util.InetUtils);
}
```

## `com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration`

```java
public class com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration implements org.springframework.beans.factory.InitializingBean {
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration(com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties, org.springframework.beans.factory.ObjectProvider<org.apache.ibatis.plugin.Interceptor[]>, org.springframework.beans.factory.ObjectProvider<org.apache.ibatis.type.TypeHandler[]>, org.springframework.beans.factory.ObjectProvider<org.apache.ibatis.scripting.LanguageDriver[]>, org.springframework.core.io.ResourceLoader, org.springframework.beans.factory.ObjectProvider<org.apache.ibatis.mapping.DatabaseIdProvider>, org.springframework.beans.factory.ObjectProvider<java.util.List<com.baomidou.mybatisplus.autoconfigure.ConfigurationCustomizer>>, org.springframework.beans.factory.ObjectProvider<java.util.List<com.baomidou.mybatisplus.autoconfigure.SqlSessionFactoryBeanCustomizer>>, org.springframework.beans.factory.ObjectProvider<java.util.List<com.baomidou.mybatisplus.autoconfigure.MybatisPlusPropertiesCustomizer>>, org.springframework.context.ApplicationContext);
  public void afterPropertiesSet();
  public org.apache.ibatis.session.SqlSessionFactory sqlSessionFactory(javax.sql.DataSource) throws java.lang.Exception;
  public org.mybatis.spring.SqlSessionTemplate sqlSessionTemplate(org.apache.ibatis.session.SqlSessionFactory);
  public com.baomidou.mybatisplus.extension.spring.MybatisPlusApplicationContextAware mybatisPlusSpringApplicationContextAware();
}
```

## `com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration$AutoConfiguredMapperScannerRegistrar`

```java
public class com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration$AutoConfiguredMapperScannerRegistrar implements org.springframework.beans.factory.BeanFactoryAware,org.springframework.context.EnvironmentAware,org.springframework.context.annotation.ImportBeanDefinitionRegistrar {
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration$AutoConfiguredMapperScannerRegistrar();
  public void registerBeanDefinitions(org.springframework.core.type.AnnotationMetadata, org.springframework.beans.factory.support.BeanDefinitionRegistry);
  public void setBeanFactory(org.springframework.beans.factory.BeanFactory);
  public void setEnvironment(org.springframework.core.env.Environment);
}
```

## `com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration$MapperScannerRegistrarNotFoundConfiguration`

```java
public class com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration$MapperScannerRegistrarNotFoundConfiguration implements org.springframework.beans.factory.InitializingBean {
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusAutoConfiguration$MapperScannerRegistrarNotFoundConfiguration();
  public void afterPropertiesSet();
}
```

## `com.baomidou.mybatisplus.autoconfigure.MybatisPlusInnerInterceptorAutoConfiguration`

```java
public class com.baomidou.mybatisplus.autoconfigure.MybatisPlusInnerInterceptorAutoConfiguration {
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusInnerInterceptorAutoConfiguration();
  public com.baomidou.mybatisplus.extension.plugins.MybatisPlusInterceptor defaultMybatisPlusInterceptor(java.util.List<com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor>);
}
```

## `com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration`

```java
public class com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration {
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration();
}
```

## `com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$FreeMarkerConfiguration`

```java
public class com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$FreeMarkerConfiguration {
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$FreeMarkerConfiguration();
  public org.mybatis.scripting.freemarker.FreeMarkerLanguageDriverConfig freeMarkerLanguageDriverConfig();
}
```

## `com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$LegacyFreeMarkerConfiguration`

```java
public class com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$LegacyFreeMarkerConfiguration {
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$LegacyFreeMarkerConfiguration();
}
```

## `com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$LegacyVelocityConfiguration`

```java
public class com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$LegacyVelocityConfiguration {
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$LegacyVelocityConfiguration();
}
```

## `com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$ThymeleafConfiguration`

```java
public class com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$ThymeleafConfiguration {
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$ThymeleafConfiguration();
  public org.mybatis.scripting.thymeleaf.ThymeleafLanguageDriverConfig thymeleafLanguageDriverConfig();
}
```

## `com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$VelocityConfiguration`

```java
public class com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$VelocityConfiguration {
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusLanguageDriverAutoConfiguration$VelocityConfiguration();
  public org.mybatis.scripting.velocity.VelocityLanguageDriverConfig velocityLanguageDriverConfig();
}
```

## `com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties`

```java
public class com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties {
  public org.springframework.core.io.Resource[] resolveMapperLocations();
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties();
  public java.lang.String getConfigLocation();
  public java.lang.String[] getMapperLocations();
  public java.lang.String getTypeAliasesPackage();
  public java.lang.Class<?> getTypeAliasesSuperType();
  public java.lang.String getTypeHandlersPackage();
  public boolean isCheckConfigLocation();
  public org.apache.ibatis.session.ExecutorType getExecutorType();
  public java.lang.Class<? extends org.apache.ibatis.scripting.LanguageDriver> getDefaultScriptingLanguageDriver();
  public java.util.Properties getConfigurationProperties();
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration getConfiguration();
  public com.baomidou.mybatisplus.core.config.GlobalConfig getGlobalConfig();
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties setConfigLocation(java.lang.String);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties setMapperLocations(java.lang.String[]);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties setTypeAliasesPackage(java.lang.String);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties setTypeAliasesSuperType(java.lang.Class<?>);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties setTypeHandlersPackage(java.lang.String);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties setCheckConfigLocation(boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties setExecutorType(org.apache.ibatis.session.ExecutorType);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties setDefaultScriptingLanguageDriver(java.lang.Class<? extends org.apache.ibatis.scripting.LanguageDriver>);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties setConfigurationProperties(java.util.Properties);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties setConfiguration(com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties setGlobalConfig(com.baomidou.mybatisplus.core.config.GlobalConfig);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration`

```java
public class com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration {
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration();
  public void applyTo(com.baomidou.mybatisplus.core.MybatisConfiguration);
  public java.lang.Boolean getSafeRowBoundsEnabled();
  public java.lang.Boolean getSafeResultHandlerEnabled();
  public java.lang.Boolean getMapUnderscoreToCamelCase();
  public java.lang.Boolean getAggressiveLazyLoading();
  public java.lang.Boolean getMultipleResultSetsEnabled();
  public java.lang.Boolean getUseGeneratedKeys();
  public java.lang.Boolean getUseColumnLabel();
  public java.lang.Boolean getCacheEnabled();
  public java.lang.Boolean getCallSettersOnNulls();
  public java.lang.Boolean getUseActualParamName();
  public java.lang.Boolean getReturnInstanceForEmptyRow();
  public java.lang.Boolean getShrinkWhitespacesInSql();
  public java.lang.Boolean getNullableOnForEach();
  public java.lang.Boolean getArgNameBasedConstructorAutoMapping();
  public java.lang.Boolean getLazyLoadingEnabled();
  public java.lang.Integer getDefaultStatementTimeout();
  public java.lang.Integer getDefaultFetchSize();
  public org.apache.ibatis.session.LocalCacheScope getLocalCacheScope();
  public org.apache.ibatis.type.JdbcType getJdbcTypeForNull();
  public org.apache.ibatis.mapping.ResultSetType getDefaultResultSetType();
  public org.apache.ibatis.session.ExecutorType getDefaultExecutorType();
  public org.apache.ibatis.session.AutoMappingBehavior getAutoMappingBehavior();
  public org.apache.ibatis.session.AutoMappingUnknownColumnBehavior getAutoMappingUnknownColumnBehavior();
  public java.lang.String getLogPrefix();
  public java.util.Set<java.lang.String> getLazyLoadTriggerMethods();
  public java.lang.Class<? extends org.apache.ibatis.logging.Log> getLogImpl();
  public java.lang.Class<? extends org.apache.ibatis.io.VFS> getVfsImpl();
  public java.lang.Class<?> getDefaultSqlProviderType();
  public java.lang.Class<? extends org.apache.ibatis.type.TypeHandler> getDefaultEnumTypeHandler();
  public java.lang.Class<?> getConfigurationFactory();
  public java.util.Properties getVariables();
  public java.lang.String getDatabaseId();
  public java.lang.Class<? extends org.apache.ibatis.scripting.LanguageDriver> getDefaultScriptingLanguageDriver();
  public java.lang.Boolean getUseGeneratedShortKey();
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setSafeRowBoundsEnabled(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setSafeResultHandlerEnabled(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setMapUnderscoreToCamelCase(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setAggressiveLazyLoading(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setMultipleResultSetsEnabled(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setUseGeneratedKeys(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setUseColumnLabel(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setCacheEnabled(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setCallSettersOnNulls(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setUseActualParamName(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setReturnInstanceForEmptyRow(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setShrinkWhitespacesInSql(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setNullableOnForEach(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setArgNameBasedConstructorAutoMapping(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setLazyLoadingEnabled(java.lang.Boolean);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setDefaultStatementTimeout(java.lang.Integer);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setDefaultFetchSize(java.lang.Integer);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setLocalCacheScope(org.apache.ibatis.session.LocalCacheScope);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setJdbcTypeForNull(org.apache.ibatis.type.JdbcType);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setDefaultResultSetType(org.apache.ibatis.mapping.ResultSetType);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setDefaultExecutorType(org.apache.ibatis.session.ExecutorType);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setAutoMappingBehavior(org.apache.ibatis.session.AutoMappingBehavior);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setAutoMappingUnknownColumnBehavior(org.apache.ibatis.session.AutoMappingUnknownColumnBehavior);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setLogPrefix(java.lang.String);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setLazyLoadTriggerMethods(java.util.Set<java.lang.String>);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setLogImpl(java.lang.Class<? extends org.apache.ibatis.logging.Log>);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setVfsImpl(java.lang.Class<? extends org.apache.ibatis.io.VFS>);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setDefaultSqlProviderType(java.lang.Class<?>);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setDefaultEnumTypeHandler(java.lang.Class<? extends org.apache.ibatis.type.TypeHandler>);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setConfigurationFactory(java.lang.Class<?>);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setVariables(java.util.Properties);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setDatabaseId(java.lang.String);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setDefaultScriptingLanguageDriver(java.lang.Class<? extends org.apache.ibatis.scripting.LanguageDriver>);
  public com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties$CoreConfiguration setUseGeneratedShortKey(java.lang.Boolean);
}
```

## `com.baomidou.mybatisplus.autoconfigure.MybatisPlusPropertiesCustomizer`

```java
public interface com.baomidou.mybatisplus.autoconfigure.MybatisPlusPropertiesCustomizer {
  public abstract void customize(com.baomidou.mybatisplus.autoconfigure.MybatisPlusProperties);
}
```

## `com.baomidou.mybatisplus.autoconfigure.SafetyEncryptProcessor`

```java
public class com.baomidou.mybatisplus.autoconfigure.SafetyEncryptProcessor implements org.springframework.boot.env.EnvironmentPostProcessor {
  public com.baomidou.mybatisplus.autoconfigure.SafetyEncryptProcessor();
  public void postProcessEnvironment(org.springframework.core.env.ConfigurableEnvironment, org.springframework.boot.SpringApplication);
}
```

## `com.baomidou.mybatisplus.autoconfigure.SpringBootVFS`

```java
public class com.baomidou.mybatisplus.autoconfigure.SpringBootVFS extends org.apache.ibatis.io.VFS {
  public com.baomidou.mybatisplus.autoconfigure.SpringBootVFS();
  public boolean isValid();
  public static void setUrlDecodingCharset(java.nio.charset.Charset);
  public static void setClassLoaderSupplier(java.util.function.Supplier<java.lang.ClassLoader>);
}
```

## `com.baomidou.mybatisplus.autoconfigure.SqlSessionFactoryBeanCustomizer`

```java
public interface com.baomidou.mybatisplus.autoconfigure.SqlSessionFactoryBeanCustomizer {
  public abstract void customize(com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean);
}
```
