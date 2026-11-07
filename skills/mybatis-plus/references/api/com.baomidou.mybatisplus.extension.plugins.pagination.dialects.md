# com.baomidou.mybatisplus.extension.plugins.pagination.dialects

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.DB2Dialect`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.dialects.DB2Dialect implements com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect {
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.DB2Dialect();
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel buildPaginationSql(java.lang.String, long, long);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.GBase8sDialect`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.dialects.GBase8sDialect implements com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect {
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.GBase8sDialect();
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel buildPaginationSql(java.lang.String, long, long);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.GaussDBDialect`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.dialects.GaussDBDialect implements com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect {
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.GaussDBDialect();
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel buildPaginationSql(java.lang.String, long, long);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.Hive2Dialect`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.dialects.Hive2Dialect implements com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect {
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.Hive2Dialect();
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel buildPaginationSql(java.lang.String, long, long);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect`

```java
public interface com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect {
  public abstract com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel buildPaginationSql(java.lang.String, long, long);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.InformixDialect`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.dialects.InformixDialect implements com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect {
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.InformixDialect();
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel buildPaginationSql(java.lang.String, long, long);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.MySqlDialect`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.dialects.MySqlDialect implements com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect {
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.MySqlDialect();
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel buildPaginationSql(java.lang.String, long, long);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.Oracle12cDialect`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.dialects.Oracle12cDialect implements com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect {
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.Oracle12cDialect();
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel buildPaginationSql(java.lang.String, long, long);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.OracleDialect`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.dialects.OracleDialect implements com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect {
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.OracleDialect();
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel buildPaginationSql(java.lang.String, long, long);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.PostgreDialect`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.dialects.PostgreDialect implements com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect {
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.PostgreDialect();
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel buildPaginationSql(java.lang.String, long, long);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.SQLServer2005Dialect`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.dialects.SQLServer2005Dialect implements com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect {
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.SQLServer2005Dialect();
  public java.lang.String getOrderByPart(java.lang.String);
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel buildPaginationSql(java.lang.String, long, long);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.SQLServerDialect`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.dialects.SQLServerDialect extends com.baomidou.mybatisplus.extension.plugins.pagination.dialects.Oracle12cDialect {
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.SQLServerDialect();
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.SybaseDialect`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.dialects.SybaseDialect implements com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect {
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.SybaseDialect();
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.SybaseDialect(boolean);
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel buildPaginationSql(java.lang.String, long, long);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.TrinoDialect`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.dialects.TrinoDialect implements com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect {
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.TrinoDialect();
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel buildPaginationSql(java.lang.String, long, long);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.dialects.XCloudDialect`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.dialects.XCloudDialect implements com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect {
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.XCloudDialect();
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel buildPaginationSql(java.lang.String, long, long);
}
```
