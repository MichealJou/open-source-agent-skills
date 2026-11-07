# cn.hutool.db.ds.simple

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.db.ds.simple.AbstractDataSource`

```java
public abstract class cn.hutool.db.ds.simple.AbstractDataSource implements javax.sql.DataSource,java.lang.Cloneable,java.io.Closeable {
  public cn.hutool.db.ds.simple.AbstractDataSource();
  public java.io.PrintWriter getLogWriter();
  public void setLogWriter(java.io.PrintWriter);
  public void setLoginTimeout(int);
  public int getLoginTimeout();
  public <T> T unwrap(java.lang.Class<T>) throws java.sql.SQLException;
  public boolean isWrapperFor(java.lang.Class<?>) throws java.sql.SQLException;
  public java.util.logging.Logger getParentLogger() throws java.sql.SQLFeatureNotSupportedException;
}
```

## `cn.hutool.db.ds.simple.SimpleDSFactory`

```java
public class cn.hutool.db.ds.simple.SimpleDSFactory extends cn.hutool.db.ds.AbstractDSFactory {
  public cn.hutool.db.ds.simple.SimpleDSFactory();
  public cn.hutool.db.ds.simple.SimpleDSFactory(cn.hutool.setting.Setting);
}
```

## `cn.hutool.db.ds.simple.SimpleDataSource`

```java
public class cn.hutool.db.ds.simple.SimpleDataSource extends cn.hutool.db.ds.simple.AbstractDataSource {
  public static synchronized cn.hutool.db.ds.simple.SimpleDataSource getDataSource(java.lang.String);
  public static synchronized cn.hutool.db.ds.simple.SimpleDataSource getDataSource();
  public cn.hutool.db.ds.simple.SimpleDataSource();
  public cn.hutool.db.ds.simple.SimpleDataSource(java.lang.String);
  public cn.hutool.db.ds.simple.SimpleDataSource(cn.hutool.setting.Setting, java.lang.String);
  public cn.hutool.db.ds.simple.SimpleDataSource(java.lang.String, java.lang.String, java.lang.String);
  public cn.hutool.db.ds.simple.SimpleDataSource(java.lang.String, java.lang.String, java.lang.String, java.lang.String);
  public void init(java.lang.String, java.lang.String, java.lang.String);
  public void init(java.lang.String, java.lang.String, java.lang.String, java.lang.String);
  public java.lang.String getDriver();
  public void setDriver(java.lang.String);
  public java.lang.String getUrl();
  public void setUrl(java.lang.String);
  public java.lang.String getUser();
  public void setUser(java.lang.String);
  public java.lang.String getPass();
  public void setPass(java.lang.String);
  public java.util.Properties getConnProps();
  public void setConnProps(java.util.Properties);
  public void addConnProps(java.lang.String, java.lang.String);
  public java.sql.Connection getConnection() throws java.sql.SQLException;
  public java.sql.Connection getConnection(java.lang.String, java.lang.String) throws java.sql.SQLException;
  public void close();
}
```
