# com.baomidou.mybatisplus.annotation

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.annotation.DbType`

```java
public final class com.baomidou.mybatisplus.annotation.DbType extends java.lang.Enum<com.baomidou.mybatisplus.annotation.DbType> {
  public static com.baomidou.mybatisplus.annotation.DbType[] values();
  public static com.baomidou.mybatisplus.annotation.DbType valueOf(java.lang.String);
  public static com.baomidou.mybatisplus.annotation.DbType getDbType(java.lang.String);
  public boolean mysqlSameType();
  public boolean oracleSameType();
  public boolean postgresqlSameType();
  public java.lang.String getDb();
  public java.lang.String getDesc();
}
```

## `com.baomidou.mybatisplus.annotation.FieldFill`

```java
public final class com.baomidou.mybatisplus.annotation.FieldFill extends java.lang.Enum<com.baomidou.mybatisplus.annotation.FieldFill> {
  public static com.baomidou.mybatisplus.annotation.FieldFill[] values();
  public static com.baomidou.mybatisplus.annotation.FieldFill valueOf(java.lang.String);
}
```

## `com.baomidou.mybatisplus.annotation.FieldStrategy`

```java
public final class com.baomidou.mybatisplus.annotation.FieldStrategy extends java.lang.Enum<com.baomidou.mybatisplus.annotation.FieldStrategy> {
  public static com.baomidou.mybatisplus.annotation.FieldStrategy[] values();
  public static com.baomidou.mybatisplus.annotation.FieldStrategy valueOf(java.lang.String);
}
```

## `com.baomidou.mybatisplus.annotation.IEnum`

```java
public interface com.baomidou.mybatisplus.annotation.IEnum<T extends java.io.Serializable> {
  public abstract T getValue();
}
```

## `com.baomidou.mybatisplus.annotation.IdType`

```java
public final class com.baomidou.mybatisplus.annotation.IdType extends java.lang.Enum<com.baomidou.mybatisplus.annotation.IdType> {
  public static com.baomidou.mybatisplus.annotation.IdType[] values();
  public static com.baomidou.mybatisplus.annotation.IdType valueOf(java.lang.String);
  public int getKey();
}
```

## `com.baomidou.mybatisplus.annotation.InterceptorIgnore`

```java
public interface com.baomidou.mybatisplus.annotation.InterceptorIgnore extends java.lang.annotation.Annotation {
  public abstract java.lang.String tenantLine();
  public abstract java.lang.String dynamicTableName();
  public abstract java.lang.String blockAttack();
  public abstract java.lang.String illegalSql();
  public abstract java.lang.String dataPermission();
  public abstract java.lang.String[] others();
}
```

## `com.baomidou.mybatisplus.annotation.KeySequence`

```java
public interface com.baomidou.mybatisplus.annotation.KeySequence extends java.lang.annotation.Annotation {
  public abstract java.lang.String value();
  public abstract com.baomidou.mybatisplus.annotation.DbType dbType();
}
```

## `com.baomidou.mybatisplus.annotation.OrderBy`

```java
public interface com.baomidou.mybatisplus.annotation.OrderBy extends java.lang.annotation.Annotation {
  public abstract boolean asc();
  public abstract short sort();
}
```

## `com.baomidou.mybatisplus.annotation.SqlCondition`

```java
public class com.baomidou.mybatisplus.annotation.SqlCondition {
  public com.baomidou.mybatisplus.annotation.SqlCondition();
}
```

## `com.baomidou.mybatisplus.annotation.TableField`

```java
public interface com.baomidou.mybatisplus.annotation.TableField extends java.lang.annotation.Annotation {
  public abstract java.lang.String value();
  public abstract boolean exist();
  public abstract java.lang.String condition();
  public abstract java.lang.String update();
  public abstract com.baomidou.mybatisplus.annotation.FieldStrategy insertStrategy();
  public abstract com.baomidou.mybatisplus.annotation.FieldStrategy updateStrategy();
  public abstract com.baomidou.mybatisplus.annotation.FieldStrategy whereStrategy();
  public abstract com.baomidou.mybatisplus.annotation.FieldFill fill();
  public abstract boolean select();
  public abstract boolean keepGlobalFormat();
  public abstract java.lang.String property();
  public abstract org.apache.ibatis.type.JdbcType jdbcType();
  public abstract java.lang.Class<? extends org.apache.ibatis.type.TypeHandler> typeHandler();
  public abstract boolean javaType();
  public abstract java.lang.String numericScale();
}
```

## `com.baomidou.mybatisplus.annotation.TableId`

```java
public interface com.baomidou.mybatisplus.annotation.TableId extends java.lang.annotation.Annotation {
  public abstract java.lang.String value();
  public abstract com.baomidou.mybatisplus.annotation.IdType type();
}
```

## `com.baomidou.mybatisplus.annotation.TableLogic`

```java
public interface com.baomidou.mybatisplus.annotation.TableLogic extends java.lang.annotation.Annotation {
  public abstract java.lang.String value();
  public abstract java.lang.String delval();
}
```

## `com.baomidou.mybatisplus.annotation.TableName`

```java
public interface com.baomidou.mybatisplus.annotation.TableName extends java.lang.annotation.Annotation {
  public abstract java.lang.String value();
  public abstract java.lang.String schema();
  public abstract boolean keepGlobalPrefix();
  public abstract java.lang.String resultMap();
  public abstract boolean autoResultMap();
  public abstract java.lang.String[] properties();
  public abstract java.lang.String[] excludeProperty();
}
```
