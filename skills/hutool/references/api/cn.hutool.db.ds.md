# cn.hutool.db.ds

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.db.ds.AbstractDSFactory`

```java
public abstract class cn.hutool.db.ds.AbstractDSFactory extends cn.hutool.db.ds.DSFactory {
  public cn.hutool.db.ds.AbstractDSFactory(java.lang.String, java.lang.Class<? extends javax.sql.DataSource>, cn.hutool.setting.Setting);
  public cn.hutool.setting.Setting getSetting();
  public synchronized javax.sql.DataSource getDataSource(java.lang.String);
  public void close(java.lang.String);
  public void destroy();
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```

## `cn.hutool.db.ds.DSFactory`

```java
public abstract class cn.hutool.db.ds.DSFactory implements java.io.Closeable,java.io.Serializable {
  public cn.hutool.db.ds.DSFactory(java.lang.String);
  public javax.sql.DataSource getDataSource();
  public abstract javax.sql.DataSource getDataSource(java.lang.String);
  public void close();
  public abstract void close(java.lang.String);
  public abstract void destroy();
  public static javax.sql.DataSource get();
  public static javax.sql.DataSource get(java.lang.String);
  public static cn.hutool.db.ds.DSFactory setCurrentDSFactory(cn.hutool.db.ds.DSFactory);
  public static cn.hutool.db.ds.DSFactory create(cn.hutool.setting.Setting);
}
```

## `cn.hutool.db.ds.DataSourceWrapper`

```java
public class cn.hutool.db.ds.DataSourceWrapper implements javax.sql.DataSource,java.io.Closeable,java.lang.Cloneable {
  public static cn.hutool.db.ds.DataSourceWrapper wrap(javax.sql.DataSource, java.lang.String);
  public cn.hutool.db.ds.DataSourceWrapper(javax.sql.DataSource, java.lang.String);
  public java.lang.String getDriver();
  public javax.sql.DataSource getRaw();
  public java.io.PrintWriter getLogWriter() throws java.sql.SQLException;
  public void setLogWriter(java.io.PrintWriter) throws java.sql.SQLException;
  public void setLoginTimeout(int) throws java.sql.SQLException;
  public int getLoginTimeout() throws java.sql.SQLException;
  public java.util.logging.Logger getParentLogger() throws java.sql.SQLFeatureNotSupportedException;
  public <T> T unwrap(java.lang.Class<T>) throws java.sql.SQLException;
  public boolean isWrapperFor(java.lang.Class<?>) throws java.sql.SQLException;
  public java.sql.Connection getConnection() throws java.sql.SQLException;
  public java.sql.Connection getConnection(java.lang.String, java.lang.String) throws java.sql.SQLException;
  public void close();
  public cn.hutool.db.ds.DataSourceWrapper clone();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `cn.hutool.db.ds.GlobalDSFactory`

```java
public class cn.hutool.db.ds.GlobalDSFactory {
  public cn.hutool.db.ds.GlobalDSFactory();
  public static cn.hutool.db.ds.DSFactory get();
  public static cn.hutool.db.ds.DSFactory set(cn.hutool.db.ds.DSFactory);
}
```
