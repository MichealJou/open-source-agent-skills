# com.baomidou.mybatisplus.core.metadata

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.metadata.IPage`

```java
public interface com.baomidou.mybatisplus.core.metadata.IPage<T> extends java.io.Serializable {
  public abstract java.util.List<com.baomidou.mybatisplus.core.metadata.OrderItem> orders();
  public default boolean optimizeCountSql();
  public default boolean optimizeJoinOfCountSql();
  public default boolean searchCount();
  public default long offset();
  public default java.lang.Long maxLimit();
  public default long getPages();
  public default com.baomidou.mybatisplus.core.metadata.IPage<T> setPages(long);
  public abstract java.util.List<T> getRecords();
  public abstract com.baomidou.mybatisplus.core.metadata.IPage<T> setRecords(java.util.List<T>);
  public abstract long getTotal();
  public abstract com.baomidou.mybatisplus.core.metadata.IPage<T> setTotal(long);
  public abstract long getSize();
  public abstract com.baomidou.mybatisplus.core.metadata.IPage<T> setSize(long);
  public abstract long getCurrent();
  public abstract com.baomidou.mybatisplus.core.metadata.IPage<T> setCurrent(long);
  public default <R> com.baomidou.mybatisplus.core.metadata.IPage<R> convert(java.util.function.Function<? super T, ? extends R>);
  public default java.lang.String countId();
}
```

## `com.baomidou.mybatisplus.core.metadata.MapperProxyMetadata`

```java
public class com.baomidou.mybatisplus.core.metadata.MapperProxyMetadata {
  public com.baomidou.mybatisplus.core.metadata.MapperProxyMetadata(org.apache.ibatis.reflection.MetaObject);
  public java.lang.Class<?> getMapperInterface();
  public org.apache.ibatis.session.SqlSession getSqlSession();
  public java.lang.String toString();
}
```

## `com.baomidou.mybatisplus.core.metadata.OrderFieldInfo`

```java
public class com.baomidou.mybatisplus.core.metadata.OrderFieldInfo {
  public com.baomidou.mybatisplus.core.metadata.OrderFieldInfo(java.lang.String, boolean, short);
  public java.lang.String getColumn();
  public java.lang.String getType();
  public short getSort();
  public void setColumn(java.lang.String);
  public void setType(java.lang.String);
  public void setSort(short);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.baomidou.mybatisplus.core.metadata.OrderItem`

```java
public class com.baomidou.mybatisplus.core.metadata.OrderItem implements java.io.Serializable {
  public com.baomidou.mybatisplus.core.metadata.OrderItem();
  public static com.baomidou.mybatisplus.core.metadata.OrderItem asc(java.lang.String);
  public static com.baomidou.mybatisplus.core.metadata.OrderItem desc(java.lang.String);
  public static com.baomidou.mybatisplus.core.metadata.OrderItem withExpression(java.lang.String);
  public static com.baomidou.mybatisplus.core.metadata.OrderItem withExpression(java.lang.String, boolean);
  public static java.util.List<com.baomidou.mybatisplus.core.metadata.OrderItem> ascs(java.lang.String...);
  public static java.util.List<com.baomidou.mybatisplus.core.metadata.OrderItem> descs(java.lang.String...);
  public com.baomidou.mybatisplus.core.metadata.OrderItem setColumn(java.lang.String);
  public com.baomidou.mybatisplus.core.metadata.OrderItem setAsc(boolean);
  public java.lang.String toString();
  public java.lang.String getColumn();
  public boolean isAsc();
}
```

## `com.baomidou.mybatisplus.core.metadata.TableFieldInfo`

```java
public class com.baomidou.mybatisplus.core.metadata.TableFieldInfo implements com.baomidou.mybatisplus.core.toolkit.Constants {
  public com.baomidou.mybatisplus.core.metadata.TableFieldInfo(com.baomidou.mybatisplus.core.config.GlobalConfig, com.baomidou.mybatisplus.core.metadata.TableInfo, java.lang.reflect.Field, com.baomidou.mybatisplus.annotation.TableField, org.apache.ibatis.reflection.Reflector, boolean, boolean);
  public com.baomidou.mybatisplus.core.metadata.TableFieldInfo(com.baomidou.mybatisplus.core.config.GlobalConfig, com.baomidou.mybatisplus.core.metadata.TableInfo, java.lang.reflect.Field, com.baomidou.mybatisplus.annotation.TableField, org.apache.ibatis.reflection.Reflector, boolean);
  public com.baomidou.mybatisplus.core.metadata.TableFieldInfo(com.baomidou.mybatisplus.core.config.GlobalConfig, com.baomidou.mybatisplus.core.metadata.TableInfo, java.lang.reflect.Field, org.apache.ibatis.reflection.Reflector, boolean, boolean);
  public com.baomidou.mybatisplus.core.metadata.TableFieldInfo(com.baomidou.mybatisplus.core.config.GlobalConfig, com.baomidou.mybatisplus.core.metadata.TableInfo, java.lang.reflect.Field, org.apache.ibatis.reflection.Reflector, boolean);
  public java.lang.String getInsertSqlProperty(java.lang.String);
  public java.lang.String getInsertSqlPropertyMaybeIf(java.lang.String);
  public java.lang.String getInsertSqlColumn();
  public java.lang.String getInsertSqlColumnMaybeIf(java.lang.String);
  public java.lang.String getSqlSet(java.lang.String);
  public java.lang.String getSqlSet(boolean, java.lang.String);
  public java.lang.String getSqlWhere(java.lang.String);
  public java.lang.String getVersionOli(java.lang.String, java.lang.String);
  public java.lang.reflect.Field getField();
  public java.lang.String getColumn();
  public java.lang.String getProperty();
  public java.lang.String getEl();
  public java.lang.String getMapping();
  public java.lang.Class<?> getPropertyType();
  public boolean isPrimitive();
  public boolean isCharSequence();
  public com.baomidou.mybatisplus.annotation.FieldStrategy getInsertStrategy();
  public com.baomidou.mybatisplus.annotation.FieldStrategy getUpdateStrategy();
  public com.baomidou.mybatisplus.annotation.FieldStrategy getWhereStrategy();
  public boolean isVersion();
  public boolean isSelect();
  public java.lang.String getLogicDeleteValue();
  public java.lang.String getLogicNotDeleteValue();
  public java.lang.String getUpdate();
  public java.lang.String getCondition();
  public com.baomidou.mybatisplus.annotation.FieldFill getFieldFill();
  public boolean isWithInsertFill();
  public boolean isWithUpdateFill();
  public java.lang.String getSqlSelect();
  public org.apache.ibatis.type.JdbcType getJdbcType();
  public java.lang.Class<? extends org.apache.ibatis.type.TypeHandler<?>> getTypeHandler();
  public boolean isOrderBy();
  public java.lang.String getOrderByType();
  public short getOrderBySort();
  public java.lang.String toString();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public boolean isLogicDelete();
}
```

## `com.baomidou.mybatisplus.core.metadata.TableInfo`

```java
public class com.baomidou.mybatisplus.core.metadata.TableInfo implements com.baomidou.mybatisplus.core.toolkit.Constants {
  public com.baomidou.mybatisplus.core.metadata.TableInfo(org.apache.ibatis.session.Configuration, java.lang.Class<?>);
  public java.lang.String getSqlStatement(java.lang.String);
  public boolean havePK();
  public java.lang.String getKeySqlSelect();
  public java.lang.String getAllSqlSelect();
  public java.lang.String chooseSelect(java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public java.lang.String chooseSelect(java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>, java.util.List<java.lang.String>);
  public java.lang.String getKeyInsertSqlProperty(boolean, java.lang.String, boolean);
  public java.lang.String getKeyInsertSqlColumn(boolean, java.lang.String, boolean);
  public java.lang.String getAllInsertSqlPropertyMaybeIf(java.lang.String);
  public java.lang.String getAllInsertSqlPropertyMaybeIf(java.lang.String, boolean);
  public java.lang.String getAllInsertSqlColumnMaybeIf(java.lang.String);
  public java.lang.String getAllInsertSqlColumnMaybeIf(java.lang.String, boolean);
  public java.lang.String getAllSqlWhere(boolean, boolean, boolean, java.lang.String);
  public java.lang.String getAllSqlSet(boolean, java.lang.String);
  public java.lang.String getLogicDeleteSql(boolean, boolean);
  public java.util.List<com.baomidou.mybatisplus.core.metadata.TableFieldInfo> getFieldList();
  public java.util.List<com.baomidou.mybatisplus.core.metadata.OrderFieldInfo> getOrderByFields();
  public boolean isLogicDelete();
  public java.lang.Object getPropertyValue(java.lang.Object, java.lang.String);
  public void setPropertyValue(java.lang.Object, java.lang.String, java.lang.Object...);
  public <T> T newInstance();
  public java.lang.Class<?> getEntityType();
  public com.baomidou.mybatisplus.annotation.IdType getIdType();
  public java.lang.String getTableName();
  public java.lang.String getResultMap();
  public boolean isAutoInitResultMap();
  public boolean isKeyRelated();
  public java.lang.String getKeyColumn();
  public java.lang.String getKeyProperty();
  public java.lang.Class<?> getKeyType();
  public com.baomidou.mybatisplus.annotation.KeySequence getKeySequence();
  public java.lang.String getCurrentNamespace();
  public boolean isUnderCamel();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public org.apache.ibatis.session.Configuration getConfiguration();
  public boolean isWithInsertFill();
  public boolean isWithUpdateFill();
  public boolean isWithLogicDelete();
  public com.baomidou.mybatisplus.core.metadata.TableFieldInfo getLogicDeleteFieldInfo();
  public boolean isWithVersion();
  public com.baomidou.mybatisplus.core.metadata.TableFieldInfo getVersionFieldInfo();
  public com.baomidou.mybatisplus.core.metadata.TableInfo setOrderByFields(java.util.List<com.baomidou.mybatisplus.core.metadata.OrderFieldInfo>);
  public org.apache.ibatis.reflection.Reflector getReflector();
}
```

## `com.baomidou.mybatisplus.core.metadata.TableInfoHelper`

```java
public class com.baomidou.mybatisplus.core.metadata.TableInfoHelper {
  public com.baomidou.mybatisplus.core.metadata.TableInfoHelper();
  public static com.baomidou.mybatisplus.core.metadata.TableInfo getTableInfo(java.lang.Class<?>);
  public static com.baomidou.mybatisplus.core.metadata.TableInfo getTableInfo(java.lang.String);
  public static java.util.List<com.baomidou.mybatisplus.core.metadata.TableInfo> getTableInfos();
  public static void remove(java.lang.Class<?>);
  public static synchronized com.baomidou.mybatisplus.core.metadata.TableInfo initTableInfo(org.apache.ibatis.builder.MapperBuilderAssistant, java.lang.Class<?>);
  public static boolean isExistTableId(java.lang.Class<?>, java.util.List<java.lang.reflect.Field>);
  public static boolean isExistTableId(java.util.List<java.lang.reflect.Field>, com.baomidou.mybatisplus.core.handlers.AnnotationHandler);
  public static boolean isExistTableLogic(java.lang.Class<?>, java.util.List<java.lang.reflect.Field>);
  public static boolean isExistTableLogic(java.util.List<java.lang.reflect.Field>, com.baomidou.mybatisplus.core.handlers.AnnotationHandler);
  public static boolean isExistOrderBy(java.lang.Class<?>, java.util.List<java.lang.reflect.Field>);
  public static boolean isExistOrderBy(java.util.List<java.lang.reflect.Field>, com.baomidou.mybatisplus.core.handlers.AnnotationHandler);
  public static boolean checkRelated(boolean, java.lang.String, java.lang.String);
  public static java.util.List<java.lang.reflect.Field> getAllFields(java.lang.Class<?>);
  public static java.util.List<java.lang.reflect.Field> getAllFields(java.lang.Class<?>, com.baomidou.mybatisplus.core.handlers.AnnotationHandler);
  public static org.apache.ibatis.executor.keygen.KeyGenerator genKeyGenerator(java.lang.String, com.baomidou.mybatisplus.core.metadata.TableInfo, org.apache.ibatis.builder.MapperBuilderAssistant);
}
```
