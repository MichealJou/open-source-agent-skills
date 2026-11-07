# com.baomidou.mybatisplus.extension.handlers

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.handlers.AbstractJsonTypeHandler`

```java
public abstract class com.baomidou.mybatisplus.extension.handlers.AbstractJsonTypeHandler<T> extends org.apache.ibatis.type.BaseTypeHandler<T> implements com.baomidou.mybatisplus.core.handlers.IJsonTypeHandler<T> {
  public com.baomidou.mybatisplus.extension.handlers.AbstractJsonTypeHandler(java.lang.Class<?>);
  public com.baomidou.mybatisplus.extension.handlers.AbstractJsonTypeHandler(java.lang.Class<?>, java.lang.reflect.Field);
  public void setNonNullParameter(java.sql.PreparedStatement, int, T, org.apache.ibatis.type.JdbcType) throws java.sql.SQLException;
  public T getNullableResult(java.sql.ResultSet, java.lang.String) throws java.sql.SQLException;
  public T getNullableResult(java.sql.ResultSet, int) throws java.sql.SQLException;
  public T getNullableResult(java.sql.CallableStatement, int) throws java.sql.SQLException;
  public java.lang.reflect.Type getFieldType();
}
```

## `com.baomidou.mybatisplus.extension.handlers.Fastjson2TypeHandler`

```java
public class com.baomidou.mybatisplus.extension.handlers.Fastjson2TypeHandler extends com.baomidou.mybatisplus.extension.handlers.AbstractJsonTypeHandler<java.lang.Object> {
  public com.baomidou.mybatisplus.extension.handlers.Fastjson2TypeHandler(java.lang.Class<?>);
  public com.baomidou.mybatisplus.extension.handlers.Fastjson2TypeHandler(java.lang.Class<?>, java.lang.reflect.Field);
  public java.lang.Object parse(java.lang.String);
  public java.lang.String toJson(java.lang.Object);
}
```

## `com.baomidou.mybatisplus.extension.handlers.FastjsonTypeHandler`

```java
public class com.baomidou.mybatisplus.extension.handlers.FastjsonTypeHandler extends com.baomidou.mybatisplus.extension.handlers.AbstractJsonTypeHandler<java.lang.Object> {
  public com.baomidou.mybatisplus.extension.handlers.FastjsonTypeHandler(java.lang.Class<?>);
  public com.baomidou.mybatisplus.extension.handlers.FastjsonTypeHandler(java.lang.Class<?>, java.lang.reflect.Field);
  public java.lang.Object parse(java.lang.String);
  public java.lang.String toJson(java.lang.Object);
}
```

## `com.baomidou.mybatisplus.extension.handlers.GsonTypeHandler`

```java
public class com.baomidou.mybatisplus.extension.handlers.GsonTypeHandler extends com.baomidou.mybatisplus.extension.handlers.AbstractJsonTypeHandler<java.lang.Object> {
  public com.baomidou.mybatisplus.extension.handlers.GsonTypeHandler(java.lang.Class<?>);
  public com.baomidou.mybatisplus.extension.handlers.GsonTypeHandler(java.lang.Class<?>, java.lang.reflect.Field);
  public java.lang.Object parse(java.lang.String);
  public java.lang.String toJson(java.lang.Object);
  public static com.google.gson.Gson getGson();
  public static void setGson(com.google.gson.Gson);
}
```

## `com.baomidou.mybatisplus.extension.handlers.Jackson3TypeHandler`

```java
public class com.baomidou.mybatisplus.extension.handlers.Jackson3TypeHandler extends com.baomidou.mybatisplus.extension.handlers.AbstractJsonTypeHandler<java.lang.Object> {
  public com.baomidou.mybatisplus.extension.handlers.Jackson3TypeHandler(java.lang.Class<?>);
  public com.baomidou.mybatisplus.extension.handlers.Jackson3TypeHandler(java.lang.Class<?>, java.lang.reflect.Field);
  public java.lang.Object parse(java.lang.String);
  public java.lang.String toJson(java.lang.Object);
  public static tools.jackson.databind.ObjectMapper getObjectMapper();
  public static void setObjectMapper(tools.jackson.databind.ObjectMapper);
}
```

## `com.baomidou.mybatisplus.extension.handlers.JacksonTypeHandler`

```java
public class com.baomidou.mybatisplus.extension.handlers.JacksonTypeHandler extends com.baomidou.mybatisplus.extension.handlers.AbstractJsonTypeHandler<java.lang.Object> {
  public com.baomidou.mybatisplus.extension.handlers.JacksonTypeHandler(java.lang.Class<?>);
  public com.baomidou.mybatisplus.extension.handlers.JacksonTypeHandler(java.lang.Class<?>, java.lang.reflect.Field);
  public java.lang.Object parse(java.lang.String);
  public java.lang.String toJson(java.lang.Object);
  public static com.fasterxml.jackson.databind.ObjectMapper getObjectMapper();
  public static void setObjectMapper(com.fasterxml.jackson.databind.ObjectMapper);
}
```

## `com.baomidou.mybatisplus.extension.handlers.MybatisMapWrapper`

```java
public class com.baomidou.mybatisplus.extension.handlers.MybatisMapWrapper extends org.apache.ibatis.reflection.wrapper.MapWrapper {
  public com.baomidou.mybatisplus.extension.handlers.MybatisMapWrapper(org.apache.ibatis.reflection.MetaObject, java.util.Map<java.lang.String, java.lang.Object>);
  public java.lang.String findProperty(java.lang.String, boolean);
}
```
