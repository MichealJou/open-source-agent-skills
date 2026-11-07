# com.baomidou.mybatisplus.core.config

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.config.GlobalConfig`

```java
public class com.baomidou.mybatisplus.core.config.GlobalConfig implements java.io.Serializable {
  public com.baomidou.mybatisplus.core.config.GlobalConfig();
  public boolean isBanner();
  public boolean isEnableSqlRunner();
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig getDbConfig();
  public com.baomidou.mybatisplus.core.injector.ISqlInjector getSqlInjector();
  public java.lang.Class<?> getSuperMapperClass();
  public org.apache.ibatis.session.SqlSessionFactory getSqlSessionFactory();
  public java.util.Set<java.lang.String> getMapperRegistryCache();
  public com.baomidou.mybatisplus.core.handlers.MetaObjectHandler getMetaObjectHandler();
  public com.baomidou.mybatisplus.core.handlers.AnnotationHandler getAnnotationHandler();
  public com.baomidou.mybatisplus.core.handlers.PostInitTableInfoHandler getPostInitTableInfoHandler();
  public com.baomidou.mybatisplus.core.incrementer.IdentifierGenerator getIdentifierGenerator();
  public com.baomidou.mybatisplus.core.config.GlobalConfig$Sequence getSequence();
  public com.baomidou.mybatisplus.core.config.GlobalConfig setBanner(boolean);
  public com.baomidou.mybatisplus.core.config.GlobalConfig setEnableSqlRunner(boolean);
  public com.baomidou.mybatisplus.core.config.GlobalConfig setDbConfig(com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig);
  public com.baomidou.mybatisplus.core.config.GlobalConfig setSqlInjector(com.baomidou.mybatisplus.core.injector.ISqlInjector);
  public com.baomidou.mybatisplus.core.config.GlobalConfig setSuperMapperClass(java.lang.Class<?>);
  public com.baomidou.mybatisplus.core.config.GlobalConfig setSqlSessionFactory(org.apache.ibatis.session.SqlSessionFactory);
  public com.baomidou.mybatisplus.core.config.GlobalConfig setMapperRegistryCache(java.util.Set<java.lang.String>);
  public com.baomidou.mybatisplus.core.config.GlobalConfig setMetaObjectHandler(com.baomidou.mybatisplus.core.handlers.MetaObjectHandler);
  public com.baomidou.mybatisplus.core.config.GlobalConfig setAnnotationHandler(com.baomidou.mybatisplus.core.handlers.AnnotationHandler);
  public com.baomidou.mybatisplus.core.config.GlobalConfig setPostInitTableInfoHandler(com.baomidou.mybatisplus.core.handlers.PostInitTableInfoHandler);
  public com.baomidou.mybatisplus.core.config.GlobalConfig setIdentifierGenerator(com.baomidou.mybatisplus.core.incrementer.IdentifierGenerator);
  public com.baomidou.mybatisplus.core.config.GlobalConfig setSequence(com.baomidou.mybatisplus.core.config.GlobalConfig$Sequence);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig`

```java
public class com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig {
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig();
  public com.baomidou.mybatisplus.annotation.IdType getIdType();
  public java.lang.String getTablePrefix();
  public java.lang.String getSchema();
  public java.lang.String getColumnFormat();
  public java.lang.String getTableFormat();
  public java.lang.String getPropertyFormat();
  public boolean isReplacePlaceholder();
  public java.lang.String getEscapeSymbol();
  public boolean isTableUnderline();
  public boolean isCapitalMode();
  public java.util.List<com.baomidou.mybatisplus.core.incrementer.IKeyGenerator> getKeyGenerators();
  public java.lang.String getLogicDeleteField();
  public java.lang.String getLogicDeleteValue();
  public java.lang.String getLogicNotDeleteValue();
  public com.baomidou.mybatisplus.annotation.FieldStrategy getInsertStrategy();
  public com.baomidou.mybatisplus.annotation.FieldStrategy getUpdateStrategy();
  public com.baomidou.mybatisplus.annotation.FieldStrategy getWhereStrategy();
  public boolean isInsertIgnoreAutoIncrementColumn();
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setIdType(com.baomidou.mybatisplus.annotation.IdType);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setTablePrefix(java.lang.String);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setSchema(java.lang.String);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setColumnFormat(java.lang.String);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setTableFormat(java.lang.String);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setPropertyFormat(java.lang.String);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setReplacePlaceholder(boolean);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setEscapeSymbol(java.lang.String);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setTableUnderline(boolean);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setCapitalMode(boolean);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setKeyGenerators(java.util.List<com.baomidou.mybatisplus.core.incrementer.IKeyGenerator>);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setLogicDeleteField(java.lang.String);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setLogicDeleteValue(java.lang.String);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setLogicNotDeleteValue(java.lang.String);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setInsertStrategy(com.baomidou.mybatisplus.annotation.FieldStrategy);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setUpdateStrategy(com.baomidou.mybatisplus.annotation.FieldStrategy);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setWhereStrategy(com.baomidou.mybatisplus.annotation.FieldStrategy);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$DbConfig setInsertIgnoreAutoIncrementColumn(boolean);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.baomidou.mybatisplus.core.config.GlobalConfig$Sequence`

```java
public class com.baomidou.mybatisplus.core.config.GlobalConfig$Sequence {
  public com.baomidou.mybatisplus.core.config.GlobalConfig$Sequence();
  public java.lang.Long getWorkerId();
  public java.lang.Long getDatacenterId();
  public java.util.List<java.lang.String> getPreferredNetworks();
  public java.util.List<java.lang.String> getIgnoredInterfaces();
  public com.baomidou.mybatisplus.core.config.GlobalConfig$Sequence setWorkerId(java.lang.Long);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$Sequence setDatacenterId(java.lang.Long);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$Sequence setPreferredNetworks(java.util.List<java.lang.String>);
  public com.baomidou.mybatisplus.core.config.GlobalConfig$Sequence setIgnoredInterfaces(java.util.List<java.lang.String>);
}
```
