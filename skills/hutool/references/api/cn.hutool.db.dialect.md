# cn.hutool.db.dialect

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.db.dialect.Dialect`

```java
public interface cn.hutool.db.dialect.Dialect extends java.io.Serializable {
  public abstract cn.hutool.db.sql.Wrapper getWrapper();
  public abstract void setWrapper(cn.hutool.db.sql.Wrapper);
  public abstract java.sql.PreparedStatement psForInsert(java.sql.Connection, cn.hutool.db.Entity) throws java.sql.SQLException;
  public abstract java.sql.PreparedStatement psForInsertBatch(java.sql.Connection, cn.hutool.db.Entity...) throws java.sql.SQLException;
  public abstract java.sql.PreparedStatement psForDelete(java.sql.Connection, cn.hutool.db.sql.Query) throws java.sql.SQLException;
  public abstract java.sql.PreparedStatement psForUpdate(java.sql.Connection, cn.hutool.db.Entity, cn.hutool.db.sql.Query) throws java.sql.SQLException;
  public abstract java.sql.PreparedStatement psForFind(java.sql.Connection, cn.hutool.db.sql.Query) throws java.sql.SQLException;
  public abstract java.sql.PreparedStatement psForPage(java.sql.Connection, cn.hutool.db.sql.Query) throws java.sql.SQLException;
  public abstract java.sql.PreparedStatement psForPage(java.sql.Connection, cn.hutool.db.sql.SqlBuilder, cn.hutool.db.Page) throws java.sql.SQLException;
  public default java.sql.PreparedStatement psForCount(java.sql.Connection, cn.hutool.db.sql.Query) throws java.sql.SQLException;
  public default java.sql.PreparedStatement psForCount(java.sql.Connection, cn.hutool.db.sql.SqlBuilder) throws java.sql.SQLException;
  public default java.sql.PreparedStatement psForUpsert(java.sql.Connection, cn.hutool.db.Entity, java.lang.String...) throws java.sql.SQLException;
  public abstract java.lang.String dialectName();
}
```

## `cn.hutool.db.dialect.DialectFactory`

```java
public class cn.hutool.db.dialect.DialectFactory implements cn.hutool.db.dialect.DriverNamePool {
  public static cn.hutool.db.dialect.Dialect newDialect(java.lang.String);
  public static java.lang.String identifyDriver(java.lang.String);
  public static java.lang.String identifyDriver(java.lang.String, java.lang.ClassLoader);
  public static cn.hutool.db.dialect.Dialect getDialect(javax.sql.DataSource);
  public static cn.hutool.db.dialect.Dialect newDialect(javax.sql.DataSource);
  public static cn.hutool.db.dialect.Dialect newDialect(java.sql.Connection);
}
```

## `cn.hutool.db.dialect.DialectName`

```java
public final class cn.hutool.db.dialect.DialectName extends java.lang.Enum<cn.hutool.db.dialect.DialectName> {
  public static cn.hutool.db.dialect.DialectName[] values();
  public static cn.hutool.db.dialect.DialectName valueOf(java.lang.String);
  public boolean match(java.lang.String);
}
```

## `cn.hutool.db.dialect.DriverUtil`

```java
public class cn.hutool.db.dialect.DriverUtil {
  public cn.hutool.db.dialect.DriverUtil();
  public static java.lang.String identifyDriver(java.lang.String);
  public static java.lang.String identifyDriver(javax.sql.DataSource);
  public static java.lang.String identifyDriver(java.sql.Connection) throws cn.hutool.db.DbRuntimeException;
}
```
