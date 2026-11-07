# com.baomidou.mybatisplus.extension.ddl.history

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator`

```java
public interface com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator {
  public default boolean existTable(java.lang.String, java.util.function.Function<java.lang.String, java.lang.Boolean>);
  public default boolean existTable(java.sql.Connection) throws java.sql.SQLException;
  public default java.lang.String getDdlHistory();
  public abstract java.lang.String createDdlHistory();
  public default java.lang.String selectDdlHistory(java.lang.String, java.lang.String);
  public default java.lang.String insertDdlHistory(java.lang.String, java.lang.String, java.lang.String);
}
```

## `com.baomidou.mybatisplus.extension.ddl.history.MysqlDdlGenerator`

```java
public class com.baomidou.mybatisplus.extension.ddl.history.MysqlDdlGenerator implements com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator {
  public com.baomidou.mybatisplus.extension.ddl.history.MysqlDdlGenerator();
  public static com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator newInstance();
  public boolean existTable(java.lang.String, java.util.function.Function<java.lang.String, java.lang.Boolean>);
  public java.lang.String createDdlHistory();
}
```

## `com.baomidou.mybatisplus.extension.ddl.history.OracleDdlGenerator`

```java
public class com.baomidou.mybatisplus.extension.ddl.history.OracleDdlGenerator implements com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator {
  public com.baomidou.mybatisplus.extension.ddl.history.OracleDdlGenerator();
  public com.baomidou.mybatisplus.extension.ddl.history.OracleDdlGenerator(java.lang.String);
  public static com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator newInstance();
  public boolean existTable(java.sql.Connection) throws java.sql.SQLException;
  public boolean existTable(java.lang.String, java.util.function.Function<java.lang.String, java.lang.Boolean>);
  public java.lang.String getDdlHistory();
  public java.lang.String createDdlHistory();
}
```

## `com.baomidou.mybatisplus.extension.ddl.history.PostgreDdlGenerator`

```java
public class com.baomidou.mybatisplus.extension.ddl.history.PostgreDdlGenerator implements com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator {
  public com.baomidou.mybatisplus.extension.ddl.history.PostgreDdlGenerator();
  public com.baomidou.mybatisplus.extension.ddl.history.PostgreDdlGenerator(java.lang.String);
  public static com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator newInstance();
  public static com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator newInstanceWithSchema(java.lang.String);
  public static com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator newInstanceWithAutoSchema();
  public boolean existTable(java.lang.String, java.util.function.Function<java.lang.String, java.lang.Boolean>);
  public boolean existTable(java.sql.Connection) throws java.sql.SQLException;
  public java.lang.String getDdlHistory();
  public java.lang.String createDdlHistory();
  public void setSchema(java.lang.String);
}
```

## `com.baomidou.mybatisplus.extension.ddl.history.SQLiteDdlGenerator`

```java
public class com.baomidou.mybatisplus.extension.ddl.history.SQLiteDdlGenerator implements com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator {
  public com.baomidou.mybatisplus.extension.ddl.history.SQLiteDdlGenerator();
  public static com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator newInstance();
  public boolean existTable(java.lang.String, java.util.function.Function<java.lang.String, java.lang.Boolean>);
  public java.lang.String createDdlHistory();
}
```
