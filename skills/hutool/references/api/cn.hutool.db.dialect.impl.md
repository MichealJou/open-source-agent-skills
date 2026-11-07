# cn.hutool.db.dialect.impl

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.db.dialect.impl.AnsiSqlDialect`

```java
public class cn.hutool.db.dialect.impl.AnsiSqlDialect implements cn.hutool.db.dialect.Dialect {
  public cn.hutool.db.dialect.impl.AnsiSqlDialect();
  public cn.hutool.db.sql.Wrapper getWrapper();
  public void setWrapper(cn.hutool.db.sql.Wrapper);
  public java.sql.PreparedStatement psForInsert(java.sql.Connection, cn.hutool.db.Entity) throws java.sql.SQLException;
  public java.sql.PreparedStatement psForInsertBatch(java.sql.Connection, cn.hutool.db.Entity...) throws java.sql.SQLException;
  public java.sql.PreparedStatement psForDelete(java.sql.Connection, cn.hutool.db.sql.Query) throws java.sql.SQLException;
  public java.sql.PreparedStatement psForUpdate(java.sql.Connection, cn.hutool.db.Entity, cn.hutool.db.sql.Query) throws java.sql.SQLException;
  public java.sql.PreparedStatement psForFind(java.sql.Connection, cn.hutool.db.sql.Query) throws java.sql.SQLException;
  public java.sql.PreparedStatement psForPage(java.sql.Connection, cn.hutool.db.sql.Query) throws java.sql.SQLException;
  public java.sql.PreparedStatement psForPage(java.sql.Connection, cn.hutool.db.sql.SqlBuilder, cn.hutool.db.Page) throws java.sql.SQLException;
  public java.lang.String dialectName();
}
```

## `cn.hutool.db.dialect.impl.DmDialect`

```java
public class cn.hutool.db.dialect.impl.DmDialect extends cn.hutool.db.dialect.impl.AnsiSqlDialect {
  public cn.hutool.db.dialect.impl.DmDialect();
  public java.lang.String dialectName();
  public java.sql.PreparedStatement psForUpsert(java.sql.Connection, cn.hutool.db.Entity, java.lang.String...) throws java.sql.SQLException;
}
```

## `cn.hutool.db.dialect.impl.H2Dialect`

```java
public class cn.hutool.db.dialect.impl.H2Dialect extends cn.hutool.db.dialect.impl.AnsiSqlDialect {
  public cn.hutool.db.dialect.impl.H2Dialect();
  public java.lang.String dialectName();
  public java.sql.PreparedStatement psForUpsert(java.sql.Connection, cn.hutool.db.Entity, java.lang.String...) throws java.sql.SQLException;
}
```

## `cn.hutool.db.dialect.impl.HanaDialect`

```java
public class cn.hutool.db.dialect.impl.HanaDialect extends cn.hutool.db.dialect.impl.AnsiSqlDialect {
  public cn.hutool.db.dialect.impl.HanaDialect();
  public java.lang.String dialectName();
  public java.sql.PreparedStatement psForUpsert(java.sql.Connection, cn.hutool.db.Entity, java.lang.String...) throws java.sql.SQLException;
}
```

## `cn.hutool.db.dialect.impl.MysqlDialect`

```java
public class cn.hutool.db.dialect.impl.MysqlDialect extends cn.hutool.db.dialect.impl.AnsiSqlDialect {
  public cn.hutool.db.dialect.impl.MysqlDialect();
  public java.lang.String dialectName();
  public java.sql.PreparedStatement psForUpsert(java.sql.Connection, cn.hutool.db.Entity, java.lang.String...) throws java.sql.SQLException;
}
```

## `cn.hutool.db.dialect.impl.OracleDialect`

```java
public class cn.hutool.db.dialect.impl.OracleDialect extends cn.hutool.db.dialect.impl.AnsiSqlDialect {
  public static boolean isNextVal(java.lang.Object);
  public cn.hutool.db.dialect.impl.OracleDialect();
  public java.lang.String dialectName();
}
```

## `cn.hutool.db.dialect.impl.PhoenixDialect`

```java
public class cn.hutool.db.dialect.impl.PhoenixDialect extends cn.hutool.db.dialect.impl.AnsiSqlDialect {
  public cn.hutool.db.dialect.impl.PhoenixDialect();
  public java.sql.PreparedStatement psForUpdate(java.sql.Connection, cn.hutool.db.Entity, cn.hutool.db.sql.Query) throws java.sql.SQLException;
  public java.lang.String dialectName();
  public java.sql.PreparedStatement psForUpsert(java.sql.Connection, cn.hutool.db.Entity, java.lang.String...) throws java.sql.SQLException;
}
```

## `cn.hutool.db.dialect.impl.PostgresqlDialect`

```java
public class cn.hutool.db.dialect.impl.PostgresqlDialect extends cn.hutool.db.dialect.impl.AnsiSqlDialect {
  public cn.hutool.db.dialect.impl.PostgresqlDialect();
  public java.lang.String dialectName();
  public java.sql.PreparedStatement psForUpsert(java.sql.Connection, cn.hutool.db.Entity, java.lang.String...) throws java.sql.SQLException;
}
```

## `cn.hutool.db.dialect.impl.SqlServer2012Dialect`

```java
public class cn.hutool.db.dialect.impl.SqlServer2012Dialect extends cn.hutool.db.dialect.impl.AnsiSqlDialect {
  public cn.hutool.db.dialect.impl.SqlServer2012Dialect();
  public java.lang.String dialectName();
}
```

## `cn.hutool.db.dialect.impl.Sqlite3Dialect`

```java
public class cn.hutool.db.dialect.impl.Sqlite3Dialect extends cn.hutool.db.dialect.impl.AnsiSqlDialect {
  public cn.hutool.db.dialect.impl.Sqlite3Dialect();
  public java.lang.String dialectName();
}
```
