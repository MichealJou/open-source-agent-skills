# com.baomidou.mybatisplus.core.toolkit.sql

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.toolkit.sql.SqlInjectionUtils`

```java
public class com.baomidou.mybatisplus.core.toolkit.sql.SqlInjectionUtils {
  public com.baomidou.mybatisplus.core.toolkit.sql.SqlInjectionUtils();
  public static boolean check(java.lang.String);
  public static java.lang.String removeEscapeCharacter(java.lang.String);
}
```

## `com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils`

```java
public abstract class com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils implements com.baomidou.mybatisplus.core.toolkit.Constants {
  public com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils();
  public static java.lang.String convertIf(java.lang.String, java.lang.String, boolean);
  public static java.lang.String convertTrim(java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String convertChoose(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String convertForeach(java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String convertWhere(java.lang.String);
  public static java.lang.String convertSet(java.lang.String);
  public static java.lang.String safeParam(java.lang.String);
  public static java.lang.String safeParam(java.lang.String, java.lang.String);
  public static java.lang.String unSafeParam(java.lang.String);
  public static java.lang.String mappingTypeHandler(java.lang.Class<? extends org.apache.ibatis.type.TypeHandler<?>>);
  public static java.lang.String mappingJdbcType(org.apache.ibatis.type.JdbcType);
  public static java.lang.String mappingNumericScale(java.lang.Integer);
  public static java.lang.String convertParamMapping(java.lang.Class<? extends org.apache.ibatis.type.TypeHandler<?>>, org.apache.ibatis.type.JdbcType, java.lang.Integer);
}
```

## `com.baomidou.mybatisplus.core.toolkit.sql.SqlUtils`

```java
public abstract class com.baomidou.mybatisplus.core.toolkit.sql.SqlUtils implements com.baomidou.mybatisplus.core.toolkit.Constants {
  public com.baomidou.mybatisplus.core.toolkit.sql.SqlUtils();
  public static java.lang.String concatLike(java.lang.Object, com.baomidou.mybatisplus.core.enums.SqlLike);
  public static java.util.List<java.lang.String> findPlaceholder(java.lang.String);
  public static java.lang.String replaceSqlPlaceholder(java.lang.String, java.util.List<java.lang.String>, java.lang.String);
  public static java.lang.String getSelectBody(java.lang.String, java.lang.String);
  public static java.lang.String getSelectBody(java.lang.String, java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String getNewSelectBody(java.lang.String, java.lang.String, java.lang.String, java.lang.String);
}
```

## `com.baomidou.mybatisplus.core.toolkit.sql.StringEscape`

```java
public class com.baomidou.mybatisplus.core.toolkit.sql.StringEscape {
  public com.baomidou.mybatisplus.core.toolkit.sql.StringEscape();
  public static java.lang.String escapeRawString(java.lang.String);
  public static java.lang.String escapeString(java.lang.String);
}
```
