# com.baomidou.mybatisplus.core

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.InjectorResolver`

```java
public class com.baomidou.mybatisplus.core.InjectorResolver extends org.apache.ibatis.builder.annotation.MethodResolver {
  public com.baomidou.mybatisplus.core.InjectorResolver(com.baomidou.mybatisplus.core.MybatisMapperAnnotationBuilder);
  public void resolve();
}
```

## `com.baomidou.mybatisplus.core.MybatisConfiguration`

```java
public class com.baomidou.mybatisplus.core.MybatisConfiguration extends org.apache.ibatis.session.Configuration {
  public com.baomidou.mybatisplus.core.MybatisConfiguration(org.apache.ibatis.mapping.Environment);
  public com.baomidou.mybatisplus.core.MybatisConfiguration();
  public void addMappedStatement(org.apache.ibatis.mapping.MappedStatement);
  public org.apache.ibatis.binding.MapperRegistry getMapperRegistry();
  public <T> void addMapper(java.lang.Class<T>);
  public <T> void addNewMapper(java.lang.Class<T>);
  public <T> void removeMapper(java.lang.Class<T>);
  public void addMappers(java.lang.String, java.lang.Class<?>);
  public void addMappers(java.lang.String);
  public <T> T getMapper(java.lang.Class<T>, org.apache.ibatis.session.SqlSession);
  public boolean hasMapper(java.lang.Class<?>);
  public void setDefaultScriptingLanguage(java.lang.Class<? extends org.apache.ibatis.scripting.LanguageDriver>);
  public void setDefaultEnumTypeHandler(java.lang.Class<? extends org.apache.ibatis.type.TypeHandler>);
  public void addKeyGenerator(java.lang.String, org.apache.ibatis.executor.keygen.KeyGenerator);
  public java.util.Collection<java.lang.String> getKeyGeneratorNames();
  public java.util.Collection<org.apache.ibatis.executor.keygen.KeyGenerator> getKeyGenerators();
  public org.apache.ibatis.executor.keygen.KeyGenerator getKeyGenerator(java.lang.String);
  public boolean hasKeyGenerator(java.lang.String);
  public void addCache(org.apache.ibatis.cache.Cache);
  public java.util.Collection<java.lang.String> getCacheNames();
  public java.util.Collection<org.apache.ibatis.cache.Cache> getCaches();
  public org.apache.ibatis.cache.Cache getCache(java.lang.String);
  public boolean hasCache(java.lang.String);
  public void addResultMap(org.apache.ibatis.mapping.ResultMap);
  public java.util.Collection<java.lang.String> getResultMapNames();
  public java.util.Collection<org.apache.ibatis.mapping.ResultMap> getResultMaps();
  public org.apache.ibatis.mapping.ResultMap getResultMap(java.lang.String);
  public boolean hasResultMap(java.lang.String);
  public void addParameterMap(org.apache.ibatis.mapping.ParameterMap);
  public java.util.Collection<java.lang.String> getParameterMapNames();
  public java.util.Collection<org.apache.ibatis.mapping.ParameterMap> getParameterMaps();
  public org.apache.ibatis.mapping.ParameterMap getParameterMap(java.lang.String);
  public boolean hasParameterMap(java.lang.String);
  public java.util.Map<java.lang.String, org.apache.ibatis.parsing.XNode> getSqlFragments();
  public java.util.Collection<java.lang.String> getMappedStatementNames();
  public java.util.Collection<org.apache.ibatis.mapping.MappedStatement> getMappedStatements();
  public org.apache.ibatis.mapping.MappedStatement getMappedStatement(java.lang.String);
  public org.apache.ibatis.mapping.MappedStatement getMappedStatement(java.lang.String, boolean);
  public boolean hasStatement(java.lang.String, boolean);
  public org.apache.ibatis.executor.Executor newExecutor(org.apache.ibatis.transaction.Transaction, org.apache.ibatis.session.ExecutorType);
  public void checkGloballyForDiscriminatedNestedResultMaps(org.apache.ibatis.mapping.ResultMap);
  public void setUseGeneratedShortKey(boolean);
  public boolean isUseGeneratedShortKey();
}
```

## `com.baomidou.mybatisplus.core.MybatisConfiguration$StrictMap`

```java
public class com.baomidou.mybatisplus.core.MybatisConfiguration$StrictMap<V> extends java.util.concurrent.ConcurrentHashMap<java.lang.String, V> {
  public com.baomidou.mybatisplus.core.MybatisConfiguration$StrictMap(com.baomidou.mybatisplus.core.MybatisConfiguration, java.lang.String, int, float);
  public com.baomidou.mybatisplus.core.MybatisConfiguration$StrictMap(com.baomidou.mybatisplus.core.MybatisConfiguration, java.lang.String, int);
  public com.baomidou.mybatisplus.core.MybatisConfiguration$StrictMap(com.baomidou.mybatisplus.core.MybatisConfiguration, java.lang.String);
  public com.baomidou.mybatisplus.core.MybatisConfiguration$StrictMap(java.lang.String, java.util.Map<java.lang.String, ? extends V>);
  public com.baomidou.mybatisplus.core.MybatisConfiguration$StrictMap<V> conflictMessageProducer(java.util.function.BiFunction<V, V, java.lang.String>);
  public V put(java.lang.String, V);
  public boolean containsKey(java.lang.Object);
  public V get(java.lang.Object);
  public java.lang.Object put(java.lang.Object, java.lang.Object);
}
```

## `com.baomidou.mybatisplus.core.MybatisMapperAnnotationBuilder`

```java
public class com.baomidou.mybatisplus.core.MybatisMapperAnnotationBuilder extends org.apache.ibatis.builder.annotation.MapperAnnotationBuilder {
  public com.baomidou.mybatisplus.core.MybatisMapperAnnotationBuilder(org.apache.ibatis.session.Configuration, java.lang.Class<?>);
  public void parse();
  public static java.lang.Class<?> getMethodReturnType(java.lang.String, java.lang.String);
}
```

## `com.baomidou.mybatisplus.core.MybatisMapperBuilderAssistant`

```java
public class com.baomidou.mybatisplus.core.MybatisMapperBuilderAssistant extends org.apache.ibatis.builder.MapperBuilderAssistant {
  public com.baomidou.mybatisplus.core.MybatisMapperBuilderAssistant(org.apache.ibatis.session.Configuration, java.lang.String);
  public org.apache.ibatis.mapping.ResultMapping buildResultMapping(java.lang.Class<?>, java.lang.String, java.lang.String, java.lang.Class<?>, org.apache.ibatis.type.JdbcType, java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.Class<? extends org.apache.ibatis.type.TypeHandler<?>>, java.util.List<org.apache.ibatis.mapping.ResultFlag>, java.lang.String, java.lang.String, boolean);
}
```

## `com.baomidou.mybatisplus.core.MybatisMapperRegistry`

```java
public class com.baomidou.mybatisplus.core.MybatisMapperRegistry extends org.apache.ibatis.binding.MapperRegistry {
  public com.baomidou.mybatisplus.core.MybatisMapperRegistry(org.apache.ibatis.session.Configuration);
  public <T> T getMapper(java.lang.Class<T>, org.apache.ibatis.session.SqlSession);
  public <T> boolean hasMapper(java.lang.Class<T>);
  public <T> void addMapper(java.lang.Class<T>);
  public java.util.Collection<java.lang.Class<?>> getMappers();
}
```

## `com.baomidou.mybatisplus.core.MybatisMethodResolver`

```java
public class com.baomidou.mybatisplus.core.MybatisMethodResolver extends org.apache.ibatis.builder.annotation.MethodResolver {
  public com.baomidou.mybatisplus.core.MybatisMethodResolver(com.baomidou.mybatisplus.core.MybatisMapperAnnotationBuilder, java.lang.reflect.Method);
  public void resolve();
}
```

## `com.baomidou.mybatisplus.core.MybatisParameterHandler`

```java
public class com.baomidou.mybatisplus.core.MybatisParameterHandler extends org.apache.ibatis.scripting.defaults.DefaultParameterHandler {
  public com.baomidou.mybatisplus.core.MybatisParameterHandler(org.apache.ibatis.mapping.MappedStatement, java.lang.Object, org.apache.ibatis.mapping.BoundSql);
  public void processParameter(java.lang.Object);
}
```

## `com.baomidou.mybatisplus.core.MybatisPlusVersion`

```java
public class com.baomidou.mybatisplus.core.MybatisPlusVersion {
  public static java.lang.String getVersion();
}
```

## `com.baomidou.mybatisplus.core.MybatisSqlSessionFactoryBuilder`

```java
public class com.baomidou.mybatisplus.core.MybatisSqlSessionFactoryBuilder extends org.apache.ibatis.session.SqlSessionFactoryBuilder {
  public com.baomidou.mybatisplus.core.MybatisSqlSessionFactoryBuilder();
  public org.apache.ibatis.session.SqlSessionFactory build(java.io.Reader, java.lang.String, java.util.Properties);
  public org.apache.ibatis.session.SqlSessionFactory build(java.io.InputStream, java.lang.String, java.util.Properties);
  public org.apache.ibatis.session.SqlSessionFactory build(org.apache.ibatis.session.Configuration);
}
```

## `com.baomidou.mybatisplus.core.MybatisXMLConfigBuilder`

```java
public class com.baomidou.mybatisplus.core.MybatisXMLConfigBuilder extends org.apache.ibatis.builder.BaseBuilder {
  public com.baomidou.mybatisplus.core.MybatisXMLConfigBuilder(java.io.Reader);
  public com.baomidou.mybatisplus.core.MybatisXMLConfigBuilder(java.io.Reader, java.lang.String);
  public com.baomidou.mybatisplus.core.MybatisXMLConfigBuilder(java.io.Reader, java.lang.String, java.util.Properties);
  public com.baomidou.mybatisplus.core.MybatisXMLConfigBuilder(java.lang.Class<? extends org.apache.ibatis.session.Configuration>, java.io.Reader, java.lang.String, java.util.Properties);
  public com.baomidou.mybatisplus.core.MybatisXMLConfigBuilder(java.io.InputStream);
  public com.baomidou.mybatisplus.core.MybatisXMLConfigBuilder(java.io.InputStream, java.lang.String);
  public com.baomidou.mybatisplus.core.MybatisXMLConfigBuilder(java.io.InputStream, java.lang.String, java.util.Properties);
  public com.baomidou.mybatisplus.core.MybatisXMLConfigBuilder(java.lang.Class<? extends org.apache.ibatis.session.Configuration>, java.io.InputStream, java.lang.String, java.util.Properties);
  public org.apache.ibatis.session.Configuration parse();
}
```

## `com.baomidou.mybatisplus.core.MybatisXMLLanguageDriver`

```java
public class com.baomidou.mybatisplus.core.MybatisXMLLanguageDriver extends org.apache.ibatis.scripting.xmltags.XMLLanguageDriver {
  public com.baomidou.mybatisplus.core.MybatisXMLLanguageDriver();
  public org.apache.ibatis.executor.parameter.ParameterHandler createParameterHandler(org.apache.ibatis.mapping.MappedStatement, java.lang.Object, org.apache.ibatis.mapping.BoundSql);
  public org.apache.ibatis.mapping.SqlSource createSqlSource(org.apache.ibatis.session.Configuration, org.apache.ibatis.parsing.XNode, java.lang.Class<?>);
  public org.apache.ibatis.mapping.SqlSource createSqlSource(org.apache.ibatis.session.Configuration, java.lang.String, java.lang.Class<?>);
}
```

## `com.baomidou.mybatisplus.core.MybatisXMLMapperBuilder`

```java
public class com.baomidou.mybatisplus.core.MybatisXMLMapperBuilder extends org.apache.ibatis.builder.BaseBuilder {
  public com.baomidou.mybatisplus.core.MybatisXMLMapperBuilder(java.io.Reader, org.apache.ibatis.session.Configuration, java.lang.String, java.util.Map<java.lang.String, org.apache.ibatis.parsing.XNode>, java.lang.String);
  public com.baomidou.mybatisplus.core.MybatisXMLMapperBuilder(java.io.Reader, org.apache.ibatis.session.Configuration, java.lang.String, java.util.Map<java.lang.String, org.apache.ibatis.parsing.XNode>);
  public com.baomidou.mybatisplus.core.MybatisXMLMapperBuilder(java.io.InputStream, org.apache.ibatis.session.Configuration, java.lang.String, java.util.Map<java.lang.String, org.apache.ibatis.parsing.XNode>, java.lang.String);
  public com.baomidou.mybatisplus.core.MybatisXMLMapperBuilder(java.io.InputStream, org.apache.ibatis.session.Configuration, java.lang.String, java.util.Map<java.lang.String, org.apache.ibatis.parsing.XNode>);
  public void parse();
  public org.apache.ibatis.parsing.XNode getSqlFragment(java.lang.String);
}
```

## `com.baomidou.mybatisplus.core.MybatisXMLScriptBuilder`

```java
public class com.baomidou.mybatisplus.core.MybatisXMLScriptBuilder extends org.apache.ibatis.builder.BaseBuilder {
  public com.baomidou.mybatisplus.core.MybatisXMLScriptBuilder(org.apache.ibatis.session.Configuration, org.apache.ibatis.parsing.XNode);
  public com.baomidou.mybatisplus.core.MybatisXMLScriptBuilder(org.apache.ibatis.session.Configuration, org.apache.ibatis.parsing.XNode, java.lang.Class<?>);
  public org.apache.ibatis.mapping.SqlSource parseScriptNode();
  public static java.lang.String replaceLeadingAndTrailingWhitespace(java.lang.String);
}
```
