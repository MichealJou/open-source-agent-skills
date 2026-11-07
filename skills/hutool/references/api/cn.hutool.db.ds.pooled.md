# cn.hutool.db.ds.pooled

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.db.ds.pooled.ConnectionWraper`

```java
public abstract class cn.hutool.db.ds.pooled.ConnectionWraper implements java.sql.Connection {
  public cn.hutool.db.ds.pooled.ConnectionWraper();
  public <T> T unwrap(java.lang.Class<T>) throws java.sql.SQLException;
  public boolean isWrapperFor(java.lang.Class<?>) throws java.sql.SQLException;
  public java.sql.Statement createStatement() throws java.sql.SQLException;
  public java.sql.PreparedStatement prepareStatement(java.lang.String) throws java.sql.SQLException;
  public java.sql.CallableStatement prepareCall(java.lang.String) throws java.sql.SQLException;
  public java.lang.String nativeSQL(java.lang.String) throws java.sql.SQLException;
  public void setAutoCommit(boolean) throws java.sql.SQLException;
  public boolean getAutoCommit() throws java.sql.SQLException;
  public void commit() throws java.sql.SQLException;
  public void rollback() throws java.sql.SQLException;
  public java.sql.DatabaseMetaData getMetaData() throws java.sql.SQLException;
  public void setReadOnly(boolean) throws java.sql.SQLException;
  public boolean isReadOnly() throws java.sql.SQLException;
  public void setCatalog(java.lang.String) throws java.sql.SQLException;
  public java.lang.String getCatalog() throws java.sql.SQLException;
  public void setTransactionIsolation(int) throws java.sql.SQLException;
  public int getTransactionIsolation() throws java.sql.SQLException;
  public java.sql.SQLWarning getWarnings() throws java.sql.SQLException;
  public void clearWarnings() throws java.sql.SQLException;
  public java.sql.Statement createStatement(int, int) throws java.sql.SQLException;
  public java.sql.PreparedStatement prepareStatement(java.lang.String, int, int) throws java.sql.SQLException;
  public java.sql.CallableStatement prepareCall(java.lang.String, int, int) throws java.sql.SQLException;
  public java.util.Map<java.lang.String, java.lang.Class<?>> getTypeMap() throws java.sql.SQLException;
  public void setTypeMap(java.util.Map<java.lang.String, java.lang.Class<?>>) throws java.sql.SQLException;
  public void setHoldability(int) throws java.sql.SQLException;
  public int getHoldability() throws java.sql.SQLException;
  public java.sql.Savepoint setSavepoint() throws java.sql.SQLException;
  public java.sql.Savepoint setSavepoint(java.lang.String) throws java.sql.SQLException;
  public void rollback(java.sql.Savepoint) throws java.sql.SQLException;
  public void releaseSavepoint(java.sql.Savepoint) throws java.sql.SQLException;
  public java.sql.Statement createStatement(int, int, int) throws java.sql.SQLException;
  public java.sql.PreparedStatement prepareStatement(java.lang.String, int, int, int) throws java.sql.SQLException;
  public java.sql.CallableStatement prepareCall(java.lang.String, int, int, int) throws java.sql.SQLException;
  public java.sql.PreparedStatement prepareStatement(java.lang.String, int) throws java.sql.SQLException;
  public java.sql.PreparedStatement prepareStatement(java.lang.String, int[]) throws java.sql.SQLException;
  public java.sql.PreparedStatement prepareStatement(java.lang.String, java.lang.String[]) throws java.sql.SQLException;
  public java.sql.Clob createClob() throws java.sql.SQLException;
  public java.sql.Blob createBlob() throws java.sql.SQLException;
  public java.sql.NClob createNClob() throws java.sql.SQLException;
  public java.sql.SQLXML createSQLXML() throws java.sql.SQLException;
  public boolean isValid(int) throws java.sql.SQLException;
  public void setClientInfo(java.lang.String, java.lang.String) throws java.sql.SQLClientInfoException;
  public void setClientInfo(java.util.Properties) throws java.sql.SQLClientInfoException;
  public java.lang.String getClientInfo(java.lang.String) throws java.sql.SQLException;
  public java.util.Properties getClientInfo() throws java.sql.SQLException;
  public java.sql.Array createArrayOf(java.lang.String, java.lang.Object[]) throws java.sql.SQLException;
  public java.sql.Struct createStruct(java.lang.String, java.lang.Object[]) throws java.sql.SQLException;
  public void setSchema(java.lang.String) throws java.sql.SQLException;
  public java.lang.String getSchema() throws java.sql.SQLException;
  public void abort(java.util.concurrent.Executor) throws java.sql.SQLException;
  public void setNetworkTimeout(java.util.concurrent.Executor, int) throws java.sql.SQLException;
  public int getNetworkTimeout() throws java.sql.SQLException;
  public java.sql.Connection getRaw();
}
```

## `cn.hutool.db.ds.pooled.DbConfig`

```java
public class cn.hutool.db.ds.pooled.DbConfig {
  public cn.hutool.db.ds.pooled.DbConfig();
  public cn.hutool.db.ds.pooled.DbConfig(java.lang.String, java.lang.String, java.lang.String);
  public void init(java.lang.String, java.lang.String, java.lang.String);
  public java.lang.String getDriver();
  public void setDriver(java.lang.String);
  public java.lang.String getUrl();
  public void setUrl(java.lang.String);
  public java.lang.String getUser();
  public void setUser(java.lang.String);
  public java.lang.String getPass();
  public void setPass(java.lang.String);
  public int getInitialSize();
  public void setInitialSize(int);
  public int getMinIdle();
  public void setMinIdle(int);
  public int getMaxActive();
  public void setMaxActive(int);
  public long getMaxWait();
  public void setMaxWait(long);
  public java.util.Properties getConnProps();
  public void setConnProps(java.util.Properties);
  public void addConnProps(java.lang.String, java.lang.String);
}
```

## `cn.hutool.db.ds.pooled.DbSetting`

```java
public class cn.hutool.db.ds.pooled.DbSetting {
  public cn.hutool.db.ds.pooled.DbSetting();
  public cn.hutool.db.ds.pooled.DbSetting(cn.hutool.setting.Setting);
  public cn.hutool.db.ds.pooled.DbConfig getDbConfig(java.lang.String);
}
```

## `cn.hutool.db.ds.pooled.PooledConnection`

```java
public class cn.hutool.db.ds.pooled.PooledConnection extends cn.hutool.db.ds.pooled.ConnectionWraper {
  public cn.hutool.db.ds.pooled.PooledConnection(cn.hutool.db.ds.pooled.PooledDataSource) throws java.sql.SQLException;
  public cn.hutool.db.ds.pooled.PooledConnection(cn.hutool.db.ds.pooled.PooledDataSource, java.sql.Connection);
  public void close();
  public boolean isClosed() throws java.sql.SQLException;
}
```

## `cn.hutool.db.ds.pooled.PooledDSFactory`

```java
public class cn.hutool.db.ds.pooled.PooledDSFactory extends cn.hutool.db.ds.AbstractDSFactory {
  public cn.hutool.db.ds.pooled.PooledDSFactory();
  public cn.hutool.db.ds.pooled.PooledDSFactory(cn.hutool.setting.Setting);
}
```

## `cn.hutool.db.ds.pooled.PooledDataSource`

```java
public class cn.hutool.db.ds.pooled.PooledDataSource extends cn.hutool.db.ds.simple.AbstractDataSource {
  public static synchronized cn.hutool.db.ds.pooled.PooledDataSource getDataSource(java.lang.String);
  public static synchronized cn.hutool.db.ds.pooled.PooledDataSource getDataSource();
  public cn.hutool.db.ds.pooled.PooledDataSource();
  public cn.hutool.db.ds.pooled.PooledDataSource(java.lang.String);
  public cn.hutool.db.ds.pooled.PooledDataSource(cn.hutool.db.ds.pooled.DbSetting, java.lang.String);
  public cn.hutool.db.ds.pooled.PooledDataSource(cn.hutool.db.ds.pooled.DbConfig);
  public synchronized java.sql.Connection getConnection() throws java.sql.SQLException;
  public java.sql.Connection getConnection(java.lang.String, java.lang.String) throws java.sql.SQLException;
  public cn.hutool.db.ds.pooled.PooledConnection newConnection() throws java.sql.SQLException;
  public cn.hutool.db.ds.pooled.DbConfig getConfig();
  public cn.hutool.db.ds.pooled.PooledConnection getConnection(long) throws java.sql.SQLException;
  public synchronized void close();
}
```
