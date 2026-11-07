# com.baomidou.mybatisplus.core.handlers

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.handlers.AnnotationHandler`

```java
public interface com.baomidou.mybatisplus.core.handlers.AnnotationHandler {
  public default <T extends java.lang.annotation.Annotation> T getAnnotation(java.lang.Class<?>, java.lang.Class<T>);
  public default <T extends java.lang.annotation.Annotation> boolean isAnnotationPresent(java.lang.Class<?>, java.lang.Class<T>);
  public default <T extends java.lang.annotation.Annotation> T getAnnotation(java.lang.reflect.Field, java.lang.Class<T>);
  public default <T extends java.lang.annotation.Annotation> boolean isAnnotationPresent(java.lang.reflect.Field, java.lang.Class<T>);
  public default <T extends java.lang.annotation.Annotation> T getAnnotation(java.lang.reflect.Method, java.lang.Class<T>);
  public default <T extends java.lang.annotation.Annotation> boolean isAnnotationPresent(java.lang.reflect.Method, java.lang.Class<T>);
}
```

## `com.baomidou.mybatisplus.core.handlers.CompositeEnumTypeHandler`

```java
public class com.baomidou.mybatisplus.core.handlers.CompositeEnumTypeHandler<E extends java.lang.Enum<E>> implements org.apache.ibatis.type.TypeHandler<E> {
  public com.baomidou.mybatisplus.core.handlers.CompositeEnumTypeHandler(java.lang.Class<E>);
  public static void setDefaultEnumTypeHandler(java.lang.Class<? extends org.apache.ibatis.type.TypeHandler>);
  public void setParameter(java.sql.PreparedStatement, int, E, org.apache.ibatis.type.JdbcType) throws java.sql.SQLException;
  public E getResult(java.sql.ResultSet, java.lang.String) throws java.sql.SQLException;
  public E getResult(java.sql.ResultSet, int) throws java.sql.SQLException;
  public E getResult(java.sql.CallableStatement, int) throws java.sql.SQLException;
  public <T> org.apache.ibatis.type.TypeHandler<T> getInstance(java.lang.Class<?>, java.lang.Class<?>);
  public java.lang.Object getResult(java.sql.CallableStatement, int) throws java.sql.SQLException;
  public java.lang.Object getResult(java.sql.ResultSet, int) throws java.sql.SQLException;
  public java.lang.Object getResult(java.sql.ResultSet, java.lang.String) throws java.sql.SQLException;
  public void setParameter(java.sql.PreparedStatement, int, java.lang.Object, org.apache.ibatis.type.JdbcType) throws java.sql.SQLException;
}
```

## `com.baomidou.mybatisplus.core.handlers.IJsonTypeHandler`

```java
public interface com.baomidou.mybatisplus.core.handlers.IJsonTypeHandler<T> {
  public abstract T parse(java.lang.String);
  public abstract java.lang.String toJson(T);
}
```

## `com.baomidou.mybatisplus.core.handlers.MetaObjectHandler`

```java
public interface com.baomidou.mybatisplus.core.handlers.MetaObjectHandler {
  public default boolean openInsertFill();
  public default boolean openInsertFill(org.apache.ibatis.mapping.MappedStatement);
  public default boolean openUpdateFill();
  public default boolean openUpdateFill(org.apache.ibatis.mapping.MappedStatement);
  public abstract void insertFill(org.apache.ibatis.reflection.MetaObject);
  public abstract void updateFill(org.apache.ibatis.reflection.MetaObject);
  public default com.baomidou.mybatisplus.core.handlers.MetaObjectHandler setFieldValByName(java.lang.String, java.lang.Object, org.apache.ibatis.reflection.MetaObject);
  public default java.lang.Object getFieldValByName(java.lang.String, org.apache.ibatis.reflection.MetaObject);
  public default com.baomidou.mybatisplus.core.metadata.TableInfo findTableInfo(org.apache.ibatis.reflection.MetaObject);
  public default <T, E extends T> com.baomidou.mybatisplus.core.handlers.MetaObjectHandler strictInsertFill(org.apache.ibatis.reflection.MetaObject, java.lang.String, java.lang.Class<T>, E);
  public default <T, E extends T> com.baomidou.mybatisplus.core.handlers.MetaObjectHandler strictInsertFill(org.apache.ibatis.reflection.MetaObject, java.lang.String, java.util.function.Supplier<E>, java.lang.Class<T>);
  public default com.baomidou.mybatisplus.core.handlers.MetaObjectHandler strictInsertFill(com.baomidou.mybatisplus.core.metadata.TableInfo, org.apache.ibatis.reflection.MetaObject, java.util.List<com.baomidou.mybatisplus.core.handlers.StrictFill<?, ?>>);
  public default <T, E extends T> com.baomidou.mybatisplus.core.handlers.MetaObjectHandler strictUpdateFill(org.apache.ibatis.reflection.MetaObject, java.lang.String, java.util.function.Supplier<E>, java.lang.Class<T>);
  public default <T, E extends T> com.baomidou.mybatisplus.core.handlers.MetaObjectHandler strictUpdateFill(org.apache.ibatis.reflection.MetaObject, java.lang.String, java.lang.Class<T>, E);
  public default com.baomidou.mybatisplus.core.handlers.MetaObjectHandler strictUpdateFill(com.baomidou.mybatisplus.core.metadata.TableInfo, org.apache.ibatis.reflection.MetaObject, java.util.List<com.baomidou.mybatisplus.core.handlers.StrictFill<?, ?>>);
  public default com.baomidou.mybatisplus.core.handlers.MetaObjectHandler strictFill(boolean, com.baomidou.mybatisplus.core.metadata.TableInfo, org.apache.ibatis.reflection.MetaObject, java.util.List<com.baomidou.mybatisplus.core.handlers.StrictFill<?, ?>>);
  public default com.baomidou.mybatisplus.core.handlers.MetaObjectHandler fillStrategy(org.apache.ibatis.reflection.MetaObject, java.lang.String, java.lang.Object);
  public default com.baomidou.mybatisplus.core.handlers.MetaObjectHandler strictFillStrategy(org.apache.ibatis.reflection.MetaObject, java.lang.String, java.util.function.Supplier<?>);
}
```

## `com.baomidou.mybatisplus.core.handlers.MybatisEnumTypeHandler`

```java
public final class com.baomidou.mybatisplus.core.handlers.MybatisEnumTypeHandler<E extends java.lang.Enum<E>> extends org.apache.ibatis.type.BaseTypeHandler<E> {
  public com.baomidou.mybatisplus.core.handlers.MybatisEnumTypeHandler(java.lang.Class<E>);
  public static java.util.Optional<java.lang.String> findEnumValueFieldName(java.lang.Class<?>);
  public static boolean isMpEnums(java.lang.Class<?>);
  public void setNonNullParameter(java.sql.PreparedStatement, int, E, org.apache.ibatis.type.JdbcType) throws java.sql.SQLException;
  public E getNullableResult(java.sql.ResultSet, java.lang.String) throws java.sql.SQLException;
  public E getNullableResult(java.sql.ResultSet, int) throws java.sql.SQLException;
  public E getNullableResult(java.sql.CallableStatement, int) throws java.sql.SQLException;
  public java.lang.Object getNullableResult(java.sql.CallableStatement, int) throws java.sql.SQLException;
  public java.lang.Object getNullableResult(java.sql.ResultSet, int) throws java.sql.SQLException;
  public java.lang.Object getNullableResult(java.sql.ResultSet, java.lang.String) throws java.sql.SQLException;
  public void setNonNullParameter(java.sql.PreparedStatement, int, java.lang.Object, org.apache.ibatis.type.JdbcType) throws java.sql.SQLException;
}
```

## `com.baomidou.mybatisplus.core.handlers.PostInitTableInfoHandler`

```java
public interface com.baomidou.mybatisplus.core.handlers.PostInitTableInfoHandler {
  public default com.baomidou.mybatisplus.core.metadata.TableInfo creteTableInfo(org.apache.ibatis.session.Configuration, java.lang.Class<?>);
  public default void postTableInfo(com.baomidou.mybatisplus.core.metadata.TableInfo, org.apache.ibatis.session.Configuration);
  public default void postFieldInfo(com.baomidou.mybatisplus.core.metadata.TableFieldInfo, org.apache.ibatis.session.Configuration);
}
```

## `com.baomidou.mybatisplus.core.handlers.StrictFill`

```java
public class com.baomidou.mybatisplus.core.handlers.StrictFill<T, E extends T> {
  public static <T, E extends T> com.baomidou.mybatisplus.core.handlers.StrictFill<T, E> of(java.lang.String, java.lang.Class<T>, E);
  public static <T, E extends T> com.baomidou.mybatisplus.core.handlers.StrictFill<T, E> of(java.lang.String, java.util.function.Supplier<E>, java.lang.Class<T>);
  public java.lang.String getFieldName();
  public java.lang.Class<T> getFieldType();
  public java.util.function.Supplier<E> getFieldVal();
  public void setFieldName(java.lang.String);
  public void setFieldType(java.lang.Class<T>);
  public void setFieldVal(java.util.function.Supplier<E>);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public com.baomidou.mybatisplus.core.handlers.StrictFill(java.lang.String, java.lang.Class<T>, java.util.function.Supplier<E>);
}
```
