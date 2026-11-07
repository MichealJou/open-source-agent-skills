# com.baomidou.mybatisplus.extension.spring

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.spring.MybatisPlusApplicationContextAware`

```java
public class com.baomidou.mybatisplus.extension.spring.MybatisPlusApplicationContextAware implements org.springframework.context.ApplicationContextAware {
  public com.baomidou.mybatisplus.extension.spring.MybatisPlusApplicationContextAware();
  public void setApplicationContext(org.springframework.context.ApplicationContext) throws org.springframework.beans.BeansException;
  public static boolean hasApplicationContext();
  public static org.springframework.context.ApplicationContext getApplicationContext();
}
```

## `com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean`

```java
public class com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean implements org.springframework.beans.factory.FactoryBean<org.apache.ibatis.session.SqlSessionFactory>, org.springframework.beans.factory.InitializingBean, org.springframework.context.ApplicationListener<org.springframework.context.event.ContextRefreshedEvent>, org.springframework.context.ApplicationContextAware {
  public com.baomidou.mybatisplus.extension.spring.MybatisSqlSessionFactoryBean();
  public void setObjectFactory(org.apache.ibatis.reflection.factory.ObjectFactory);
  public void setObjectWrapperFactory(org.apache.ibatis.reflection.wrapper.ObjectWrapperFactory);
  public org.apache.ibatis.mapping.DatabaseIdProvider getDatabaseIdProvider();
  public void setDatabaseIdProvider(org.apache.ibatis.mapping.DatabaseIdProvider);
  public java.lang.Class<? extends org.apache.ibatis.io.VFS> getVfs();
  public void setVfs(java.lang.Class<? extends org.apache.ibatis.io.VFS>);
  public org.apache.ibatis.cache.Cache getCache();
  public void setCache(org.apache.ibatis.cache.Cache);
  public void setPlugins(org.apache.ibatis.plugin.Interceptor...);
  public void setTypeAliasesPackage(java.lang.String);
  public void setTypeAliasesSuperType(java.lang.Class<?>);
  public void setTypeHandlersPackage(java.lang.String);
  public void setTypeHandlers(org.apache.ibatis.type.TypeHandler<?>...);
  public void setDefaultEnumTypeHandler(java.lang.Class<? extends org.apache.ibatis.type.TypeHandler>);
  public void setTypeAliases(java.lang.Class<?>...);
  public void setFailFast(boolean);
  public void setConfigLocation(org.springframework.core.io.Resource);
  public void setConfiguration(com.baomidou.mybatisplus.core.MybatisConfiguration);
  public com.baomidou.mybatisplus.core.MybatisConfiguration getConfiguration();
  public void setMapperLocations(org.springframework.core.io.Resource...);
  public void setConfigurationProperties(java.util.Properties);
  public void setDataSource(javax.sql.DataSource);
  public void setSqlSessionFactoryBuilder(org.apache.ibatis.session.SqlSessionFactoryBuilder);
  public void setTransactionFactory(org.apache.ibatis.transaction.TransactionFactory);
  public void setEnvironment(java.lang.String);
  public void setScriptingLanguageDrivers(org.apache.ibatis.scripting.LanguageDriver...);
  public void setDefaultScriptingLanguageDriver(java.lang.Class<? extends org.apache.ibatis.scripting.LanguageDriver>);
  public void addMapperLocations(org.springframework.core.io.Resource...);
  public void addTypeHandlers(org.apache.ibatis.type.TypeHandler<?>...);
  public void addScriptingLanguageDrivers(org.apache.ibatis.scripting.LanguageDriver...);
  public void addPlugins(org.apache.ibatis.plugin.Interceptor...);
  public void addTypeAliases(java.lang.Class<?>...);
  public void setApplicationContext(org.springframework.context.ApplicationContext);
  public void afterPropertiesSet() throws java.lang.Exception;
  public org.apache.ibatis.session.SqlSessionFactory getObject() throws java.lang.Exception;
  public java.lang.Class<? extends org.apache.ibatis.session.SqlSessionFactory> getObjectType();
  public boolean isSingleton();
  public void onApplicationEvent(org.springframework.context.event.ContextRefreshedEvent);
  public org.springframework.context.ApplicationContext getApplicationContext();
  public void setGlobalConfig(com.baomidou.mybatisplus.core.config.GlobalConfig);
  public java.lang.Object getObject() throws java.lang.Exception;
  public void onApplicationEvent(org.springframework.context.ApplicationEvent);
}
```
