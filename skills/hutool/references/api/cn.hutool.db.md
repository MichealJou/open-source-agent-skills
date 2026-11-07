# cn.hutool.db

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.db.AbstractDb`

```java
public abstract class cn.hutool.db.AbstractDb implements java.io.Serializable {
  public cn.hutool.db.AbstractDb(javax.sql.DataSource, cn.hutool.db.dialect.Dialect);
  public javax.sql.DataSource getDs();
  public abstract java.sql.Connection getConnection() throws java.sql.SQLException;
  public abstract void closeConnection(java.sql.Connection);
  public java.util.List<cn.hutool.db.Entity> query(java.lang.String, java.util.Map<java.lang.String, java.lang.Object>) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> query(java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public <T> java.util.List<T> query(java.lang.String, java.lang.Class<T>, java.lang.Object...) throws java.sql.SQLException;
  public cn.hutool.db.Entity queryOne(java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public java.lang.Number queryNumber(java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public java.lang.String queryString(java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public <T> T query(java.lang.String, cn.hutool.db.handler.RsHandler<T>, java.lang.Object...) throws java.sql.SQLException;
  public <T> T query(java.lang.String, cn.hutool.db.handler.RsHandler<T>, java.util.Map<java.lang.String, java.lang.Object>) throws java.sql.SQLException;
  public <T> T query(cn.hutool.core.lang.func.Func1<java.sql.Connection, java.sql.PreparedStatement>, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public int execute(java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public java.lang.Long executeForGeneratedKey(java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public int[] executeBatch(java.lang.String, java.lang.Object[]...) throws java.sql.SQLException;
  public int[] executeBatch(java.lang.String, java.lang.Iterable<java.lang.Object[]>) throws java.sql.SQLException;
  public int[] executeBatch(java.lang.String...) throws java.sql.SQLException;
  public int[] executeBatch(java.lang.Iterable<java.lang.String>) throws java.sql.SQLException;
  public int insert(cn.hutool.db.Entity) throws java.sql.SQLException;
  public int insertOrUpdate(cn.hutool.db.Entity, java.lang.String...) throws java.sql.SQLException;
  public int upsert(cn.hutool.db.Entity, java.lang.String...) throws java.sql.SQLException;
  public int[] insert(java.util.Collection<cn.hutool.db.Entity>) throws java.sql.SQLException;
  public java.util.List<java.lang.Object> insertForGeneratedKeys(cn.hutool.db.Entity) throws java.sql.SQLException;
  public java.lang.Long insertForGeneratedKey(cn.hutool.db.Entity) throws java.sql.SQLException;
  public int del(java.lang.String, java.lang.String, java.lang.Object) throws java.sql.SQLException;
  public int del(cn.hutool.db.Entity) throws java.sql.SQLException;
  public int update(cn.hutool.db.Entity, cn.hutool.db.Entity) throws java.sql.SQLException;
  public <T> cn.hutool.db.Entity get(java.lang.String, java.lang.String, T) throws java.sql.SQLException;
  public cn.hutool.db.Entity get(cn.hutool.db.Entity) throws java.sql.SQLException;
  public <T> T find(java.util.Collection<java.lang.String>, cn.hutool.db.Entity, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> find(java.util.Collection<java.lang.String>, cn.hutool.db.Entity) throws java.sql.SQLException;
  public <T> T find(cn.hutool.db.sql.Query, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public <T> T find(cn.hutool.db.Entity, cn.hutool.db.handler.RsHandler<T>, java.lang.String...) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> find(cn.hutool.db.Entity) throws java.sql.SQLException;
  public <T> java.util.List<T> find(cn.hutool.db.Entity, java.lang.Class<T>) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> findAll(cn.hutool.db.Entity) throws java.sql.SQLException;
  public <T> java.util.List<T> findAll(cn.hutool.db.Entity, java.lang.Class<T>) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> findAll(java.lang.String) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> findBy(java.lang.String, java.lang.String, java.lang.Object) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> findBy(java.lang.String, cn.hutool.db.sql.Condition...) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> findLike(java.lang.String, java.lang.String, java.lang.String, cn.hutool.db.sql.Condition$LikeType) throws java.sql.SQLException;
  public long count(cn.hutool.db.Entity) throws java.sql.SQLException;
  public long count(cn.hutool.db.sql.SqlBuilder) throws java.sql.SQLException;
  public long count(java.lang.CharSequence, java.lang.Object...) throws java.sql.SQLException;
  public <T> T page(java.util.Collection<java.lang.String>, cn.hutool.db.Entity, int, int, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public <T> T page(cn.hutool.db.Entity, int, int, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> pageForEntityList(cn.hutool.db.Entity, int, int) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> pageForEntityList(cn.hutool.db.Entity, cn.hutool.db.Page) throws java.sql.SQLException;
  public <T> T page(cn.hutool.db.Entity, cn.hutool.db.Page, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public <T> T page(java.util.Collection<java.lang.String>, cn.hutool.db.Entity, cn.hutool.db.Page, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public <T> T page(java.lang.CharSequence, cn.hutool.db.Page, cn.hutool.db.handler.RsHandler<T>, java.lang.Object...) throws java.sql.SQLException;
  public <T> cn.hutool.db.PageResult<T> page(java.lang.CharSequence, cn.hutool.db.Page, java.lang.Class<T>, java.lang.Object...) throws java.sql.SQLException;
  public <T> T page(cn.hutool.db.sql.SqlBuilder, cn.hutool.db.Page, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public cn.hutool.db.PageResult<cn.hutool.db.Entity> page(java.lang.CharSequence, cn.hutool.db.Page, java.lang.Object...) throws java.sql.SQLException;
  public cn.hutool.db.PageResult<cn.hutool.db.Entity> page(java.util.Collection<java.lang.String>, cn.hutool.db.Entity, int, int) throws java.sql.SQLException;
  public cn.hutool.db.PageResult<cn.hutool.db.Entity> page(java.util.Collection<java.lang.String>, cn.hutool.db.Entity, cn.hutool.db.Page) throws java.sql.SQLException;
  public cn.hutool.db.PageResult<cn.hutool.db.Entity> page(cn.hutool.db.Entity, int, int) throws java.sql.SQLException;
  public cn.hutool.db.PageResult<cn.hutool.db.Entity> page(cn.hutool.db.Entity, cn.hutool.db.Page) throws java.sql.SQLException;
  public void setCaseInsensitive(boolean);
  public cn.hutool.db.SqlConnRunner getRunner();
  public void setRunner(cn.hutool.db.SqlConnRunner);
  public cn.hutool.db.AbstractDb setWrapper(java.lang.Character);
  public cn.hutool.db.AbstractDb setWrapper(cn.hutool.db.sql.Wrapper);
  public cn.hutool.db.AbstractDb disableWrapper();
}
```

## `cn.hutool.db.ActiveEntity`

```java
public class cn.hutool.db.ActiveEntity extends cn.hutool.db.Entity {
  public static cn.hutool.db.ActiveEntity create();
  public static cn.hutool.db.ActiveEntity create(java.lang.String);
  public static <T> cn.hutool.db.ActiveEntity parse(T);
  public static <T> cn.hutool.db.ActiveEntity parse(T, boolean, boolean);
  public static <T> cn.hutool.db.ActiveEntity parseWithUnderlineCase(T);
  public cn.hutool.db.ActiveEntity();
  public cn.hutool.db.ActiveEntity(java.lang.String);
  public cn.hutool.db.ActiveEntity(cn.hutool.db.Entity);
  public cn.hutool.db.ActiveEntity(cn.hutool.db.Db, java.lang.String);
  public cn.hutool.db.ActiveEntity(cn.hutool.db.Db, cn.hutool.db.Entity);
  public cn.hutool.db.ActiveEntity setTableName(java.lang.String);
  public cn.hutool.db.ActiveEntity setFieldNames(java.util.Collection<java.lang.String>);
  public cn.hutool.db.ActiveEntity setFieldNames(java.lang.String...);
  public cn.hutool.db.ActiveEntity setFields(cn.hutool.core.lang.func.Func0<?>...);
  public cn.hutool.db.ActiveEntity addFieldNames(java.lang.String...);
  public <T> cn.hutool.db.ActiveEntity parseBean(T);
  public <T> cn.hutool.db.ActiveEntity parseBean(T, boolean, boolean);
  public cn.hutool.db.ActiveEntity set(java.lang.String, java.lang.Object);
  public cn.hutool.db.ActiveEntity setIgnoreNull(java.lang.String, java.lang.Object);
  public cn.hutool.db.ActiveEntity clone();
  public cn.hutool.db.ActiveEntity add();
  public cn.hutool.db.ActiveEntity load();
  public cn.hutool.db.ActiveEntity del();
  public cn.hutool.db.ActiveEntity update(java.lang.String);
  public cn.hutool.db.Entity clone();
  public cn.hutool.db.Entity setIgnoreNull(java.lang.String, java.lang.Object);
  public cn.hutool.db.Entity set(java.lang.String, java.lang.Object);
  public cn.hutool.db.Entity parseBean(java.lang.Object, boolean, boolean);
  public cn.hutool.db.Entity parseBean(java.lang.Object);
  public cn.hutool.db.Entity addFieldNames(java.lang.String[]);
  public cn.hutool.db.Entity setFields(cn.hutool.core.lang.func.Func0[]);
  public cn.hutool.db.Entity setFieldNames(java.lang.String[]);
  public cn.hutool.db.Entity setFieldNames(java.util.Collection);
  public cn.hutool.db.Entity setTableName(java.lang.String);
  public cn.hutool.core.lang.Dict setFields(cn.hutool.core.lang.func.Func0[]);
  public cn.hutool.core.lang.Dict clone();
  public cn.hutool.core.lang.Dict setIgnoreNull(java.lang.String, java.lang.Object);
  public cn.hutool.core.lang.Dict set(java.lang.String, java.lang.Object);
  public cn.hutool.core.lang.Dict parseBean(java.lang.Object, boolean, boolean);
  public cn.hutool.core.lang.Dict parseBean(java.lang.Object);
  public java.lang.Object clone();
}
```

## `cn.hutool.db.DaoTemplate`

```java
public class cn.hutool.db.DaoTemplate {
  public cn.hutool.db.DaoTemplate(java.lang.String);
  public cn.hutool.db.DaoTemplate(java.lang.String, java.lang.String);
  public cn.hutool.db.DaoTemplate(java.lang.String, javax.sql.DataSource);
  public cn.hutool.db.DaoTemplate(java.lang.String, java.lang.String, javax.sql.DataSource);
  public cn.hutool.db.DaoTemplate(java.lang.String, java.lang.String, cn.hutool.db.Db);
  public int add(cn.hutool.db.Entity) throws java.sql.SQLException;
  public java.util.List<java.lang.Object> addForGeneratedKeys(cn.hutool.db.Entity) throws java.sql.SQLException;
  public java.lang.Long addForGeneratedKey(cn.hutool.db.Entity) throws java.sql.SQLException;
  public <T> int del(T) throws java.sql.SQLException;
  public <T> int del(java.lang.String, T) throws java.sql.SQLException;
  public <T> int del(cn.hutool.db.Entity) throws java.sql.SQLException;
  public int update(cn.hutool.db.Entity, cn.hutool.db.Entity) throws java.sql.SQLException;
  public int update(cn.hutool.db.Entity) throws java.sql.SQLException;
  public int addOrUpdate(cn.hutool.db.Entity) throws java.sql.SQLException;
  public <T> cn.hutool.db.Entity get(T) throws java.sql.SQLException;
  public <T> cn.hutool.db.Entity get(java.lang.String, T) throws java.sql.SQLException;
  public cn.hutool.db.Entity get(cn.hutool.db.Entity) throws java.sql.SQLException;
  public <T> java.util.List<cn.hutool.db.Entity> find(java.lang.String, T) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> findAll() throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> find(cn.hutool.db.Entity) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> findBySql(java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public cn.hutool.db.PageResult<cn.hutool.db.Entity> page(cn.hutool.db.Entity, cn.hutool.db.Page, java.lang.String...) throws java.sql.SQLException;
  public cn.hutool.db.PageResult<cn.hutool.db.Entity> page(cn.hutool.db.Entity, cn.hutool.db.Page) throws java.sql.SQLException;
  public long count(cn.hutool.db.Entity) throws java.sql.SQLException;
  public boolean exist(cn.hutool.db.Entity) throws java.sql.SQLException;
}
```

## `cn.hutool.db.Db`

```java
public class cn.hutool.db.Db extends cn.hutool.db.AbstractDb {
  public static cn.hutool.db.Db use();
  public static cn.hutool.db.Db use(java.lang.String);
  public static cn.hutool.db.Db use(javax.sql.DataSource);
  public static cn.hutool.db.Db use(javax.sql.DataSource, cn.hutool.db.dialect.Dialect);
  public static cn.hutool.db.Db use(javax.sql.DataSource, java.lang.String);
  public cn.hutool.db.Db(javax.sql.DataSource);
  public cn.hutool.db.Db(javax.sql.DataSource, java.lang.String);
  public cn.hutool.db.Db(javax.sql.DataSource, cn.hutool.db.dialect.Dialect);
  public cn.hutool.db.Db setWrapper(java.lang.Character);
  public cn.hutool.db.Db setWrapper(cn.hutool.db.sql.Wrapper);
  public cn.hutool.db.Db disableWrapper();
  public java.sql.Connection getConnection() throws java.sql.SQLException;
  public void closeConnection(java.sql.Connection);
  public cn.hutool.db.Db tx(cn.hutool.core.lang.func.VoidFunc1<cn.hutool.db.Db>) throws java.sql.SQLException;
  public cn.hutool.db.Db tx(cn.hutool.db.transaction.TransactionLevel, cn.hutool.core.lang.func.VoidFunc1<cn.hutool.db.Db>) throws java.sql.SQLException;
  public cn.hutool.db.AbstractDb disableWrapper();
  public cn.hutool.db.AbstractDb setWrapper(cn.hutool.db.sql.Wrapper);
  public cn.hutool.db.AbstractDb setWrapper(java.lang.Character);
}
```

## `cn.hutool.db.DbRuntimeException`

```java
public class cn.hutool.db.DbRuntimeException extends java.lang.RuntimeException {
  public cn.hutool.db.DbRuntimeException(java.lang.Throwable);
  public cn.hutool.db.DbRuntimeException(java.lang.String);
  public cn.hutool.db.DbRuntimeException(java.lang.String, java.lang.Object...);
  public cn.hutool.db.DbRuntimeException(java.lang.String, java.lang.Throwable);
  public cn.hutool.db.DbRuntimeException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.db.DbRuntimeException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.db.DbUtil`

```java
public final class cn.hutool.db.DbUtil {
  public cn.hutool.db.DbUtil();
  public static cn.hutool.db.SqlConnRunner newSqlConnRunner(cn.hutool.db.dialect.Dialect);
  public static cn.hutool.db.SqlConnRunner newSqlConnRunner(javax.sql.DataSource);
  public static cn.hutool.db.SqlConnRunner newSqlConnRunner(java.sql.Connection);
  public static cn.hutool.db.Db use();
  public static cn.hutool.db.Db use(javax.sql.DataSource);
  public static cn.hutool.db.Db use(javax.sql.DataSource, cn.hutool.db.dialect.Dialect);
  public static cn.hutool.db.Session newSession();
  public static cn.hutool.db.Session newSession(javax.sql.DataSource);
  public static void close(java.lang.Object...);
  public static javax.sql.DataSource getDs();
  public static javax.sql.DataSource getDs(java.lang.String);
  public static javax.sql.DataSource getJndiDsWithLog(java.lang.String);
  public static javax.sql.DataSource getJndiDs(java.lang.String);
  public static void removeShowSqlParams(cn.hutool.setting.Setting);
  public static void setShowSqlGlobal(cn.hutool.setting.Setting);
  public static void setShowSqlGlobal(boolean, boolean, boolean, cn.hutool.log.level.Level);
  public static void setCaseInsensitiveGlobal(boolean);
  public static void setReturnGeneratedKeyGlobal(boolean);
  public static void setDbSettingPathGlobal(java.lang.String);
  public static void setStatementFetchSizeGlobal(java.lang.Integer);
}
```

## `cn.hutool.db.DialectRunner`

```java
public class cn.hutool.db.DialectRunner implements java.io.Serializable {
  public cn.hutool.db.DialectRunner(cn.hutool.db.dialect.Dialect);
  public cn.hutool.db.DialectRunner(java.lang.String);
  public int[] insert(java.sql.Connection, cn.hutool.db.Entity...) throws java.sql.SQLException;
  public int upsert(java.sql.Connection, cn.hutool.db.Entity, java.lang.String...) throws java.sql.SQLException;
  public int insertOrUpdate(java.sql.Connection, cn.hutool.db.Entity, java.lang.String...) throws java.sql.SQLException;
  public <T> T insert(java.sql.Connection, cn.hutool.db.Entity, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public int del(java.sql.Connection, cn.hutool.db.Entity) throws java.sql.SQLException;
  public int update(java.sql.Connection, cn.hutool.db.Entity, cn.hutool.db.Entity) throws java.sql.SQLException;
  public <T> T find(java.sql.Connection, cn.hutool.db.sql.Query, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public long count(java.sql.Connection, cn.hutool.db.Entity) throws java.sql.SQLException;
  public long count(java.sql.Connection, cn.hutool.db.sql.SqlBuilder) throws java.sql.SQLException;
  public <T> T page(java.sql.Connection, cn.hutool.db.sql.Query, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public <T> T page(java.sql.Connection, cn.hutool.db.sql.SqlBuilder, cn.hutool.db.Page, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public void setCaseInsensitive(boolean);
  public cn.hutool.db.dialect.Dialect getDialect();
  public void setDialect(cn.hutool.db.dialect.Dialect);
  public void setWrapper(java.lang.Character);
  public void setWrapper(cn.hutool.db.sql.Wrapper);
}
```

## `cn.hutool.db.Entity`

```java
public class cn.hutool.db.Entity extends cn.hutool.core.lang.Dict {
  public static cn.hutool.db.Entity create();
  public static cn.hutool.db.Entity create(java.lang.String);
  public static <T> cn.hutool.db.Entity parse(T);
  public static <T> cn.hutool.db.Entity parse(T, boolean, boolean);
  public static <T> cn.hutool.db.Entity parseWithUnderlineCase(T);
  public cn.hutool.db.Entity();
  public cn.hutool.db.Entity(java.lang.String);
  public cn.hutool.db.Entity(java.lang.String, boolean);
  public java.lang.String getTableName();
  public cn.hutool.db.Entity setTableName(java.lang.String);
  public java.util.Set<java.lang.String> getFieldNames();
  public cn.hutool.db.Entity setFieldNames(java.util.Collection<java.lang.String>);
  public cn.hutool.db.Entity setFieldNames(java.lang.String...);
  public cn.hutool.db.Entity setFields(cn.hutool.core.lang.func.Func0<?>...);
  public cn.hutool.db.Entity addFieldNames(java.lang.String...);
  public <T> cn.hutool.db.Entity parseBean(T);
  public <T> cn.hutool.db.Entity parseBean(T, boolean, boolean);
  public cn.hutool.db.Entity filter(java.lang.String...);
  public cn.hutool.db.Entity removeNew(java.lang.String...);
  public cn.hutool.db.Entity addCondition(cn.hutool.db.sql.Condition);
  public cn.hutool.db.Entity set(java.lang.String, java.lang.Object);
  public cn.hutool.db.Entity setIgnoreNull(java.lang.String, java.lang.Object);
  public java.sql.Clob getClob(java.lang.String);
  public java.sql.Blob getBlob(java.lang.String);
  public java.sql.Time getTime(java.lang.String);
  public java.util.Date getDate(java.lang.String);
  public java.sql.Timestamp getTimestamp(java.lang.String);
  public java.lang.String getStr(java.lang.String);
  public java.lang.String getStr(java.lang.String, java.nio.charset.Charset);
  public java.sql.RowId getRowId();
  public java.sql.RowId getRowId(java.lang.String);
  public cn.hutool.db.Entity clone();
  public java.lang.String toString();
  public cn.hutool.core.lang.Dict setFields(cn.hutool.core.lang.func.Func0[]);
  public cn.hutool.core.lang.Dict clone();
  public cn.hutool.core.lang.Dict setIgnoreNull(java.lang.String, java.lang.Object);
  public cn.hutool.core.lang.Dict set(java.lang.String, java.lang.Object);
  public cn.hutool.core.lang.Dict filter(java.lang.String[]);
  public cn.hutool.core.lang.Dict parseBean(java.lang.Object, boolean, boolean);
  public cn.hutool.core.lang.Dict parseBean(java.lang.Object);
  public java.util.Date getDate(java.lang.Object);
  public java.lang.String getStr(java.lang.Object);
  public java.lang.Object clone();
}
```

## `cn.hutool.db.GlobalDbConfig`

```java
public class cn.hutool.db.GlobalDbConfig {
  public cn.hutool.db.GlobalDbConfig();
  public static void setCaseInsensitive(boolean);
  public static void setReturnGeneratedKey(boolean);
  public static void setDbSettingPath(java.lang.String);
  public static cn.hutool.setting.Setting createDbSetting();
  public static void setShowSql(boolean, boolean, boolean, cn.hutool.log.level.Level);
  public static void setStatementFetchSize(java.lang.Integer);
}
```

## `cn.hutool.db.Page`

```java
public class cn.hutool.db.Page implements cn.hutool.core.lang.Segment<java.lang.Integer>, java.io.Serializable {
  public static cn.hutool.db.Page of(int, int);
  public cn.hutool.db.Page();
  public cn.hutool.db.Page(int, int);
  public cn.hutool.db.Page(int, int, cn.hutool.db.sql.Order);
  public int getPageNumber();
  public void setPageNumber(int);
  public int getPageSize();
  public void setPageSize(int);
  public cn.hutool.db.sql.Order[] getOrders();
  public void setOrder(cn.hutool.db.sql.Order...);
  public void addOrder(cn.hutool.db.sql.Order...);
  public int getStartPosition();
  public java.lang.Integer getStartIndex();
  public int getEndPosition();
  public java.lang.Integer getEndIndex();
  public int[] getStartEnd();
  public java.lang.String toString();
  public java.lang.Number getEndIndex();
  public java.lang.Number getStartIndex();
}
```

## `cn.hutool.db.PageResult`

```java
public class cn.hutool.db.PageResult<T> extends java.util.ArrayList<T> {
  public cn.hutool.db.PageResult();
  public cn.hutool.db.PageResult(int, int);
  public cn.hutool.db.PageResult(int, int, int);
  public int getPage();
  public void setPage(int);
  public int getPageSize();
  public void setPageSize(int);
  public int getTotalPage();
  public void setTotalPage(int);
  public int getTotal();
  public void setTotal(int);
  public boolean isFirst();
  public boolean isLast();
}
```

## `cn.hutool.db.Session`

```java
public class cn.hutool.db.Session extends cn.hutool.db.AbstractDb implements java.io.Closeable {
  public static cn.hutool.db.Session create();
  public static cn.hutool.db.Session create(java.lang.String);
  public static cn.hutool.db.Session create(javax.sql.DataSource);
  public cn.hutool.db.Session(javax.sql.DataSource);
  public cn.hutool.db.Session(javax.sql.DataSource, java.lang.String);
  public cn.hutool.db.Session(javax.sql.DataSource, cn.hutool.db.dialect.Dialect);
  public cn.hutool.db.SqlConnRunner getRunner();
  public void beginTransaction() throws java.sql.SQLException;
  public void commit() throws java.sql.SQLException;
  public void rollback() throws java.sql.SQLException;
  public void quietRollback();
  public void rollback(java.sql.Savepoint) throws java.sql.SQLException;
  public void quietRollback(java.sql.Savepoint);
  public java.sql.Savepoint setSavepoint() throws java.sql.SQLException;
  public java.sql.Savepoint setSavepoint(java.lang.String) throws java.sql.SQLException;
  public void setTransactionIsolation(int) throws java.sql.SQLException;
  public void tx(cn.hutool.core.lang.func.VoidFunc1<cn.hutool.db.Session>) throws java.sql.SQLException;
  public cn.hutool.db.Session setWrapper(java.lang.Character);
  public cn.hutool.db.Session setWrapper(cn.hutool.db.sql.Wrapper);
  public cn.hutool.db.Session disableWrapper();
  public java.sql.Connection getConnection() throws java.sql.SQLException;
  public void closeConnection(java.sql.Connection);
  public void close();
  public cn.hutool.db.AbstractDb disableWrapper();
  public cn.hutool.db.AbstractDb setWrapper(cn.hutool.db.sql.Wrapper);
  public cn.hutool.db.AbstractDb setWrapper(java.lang.Character);
}
```

## `cn.hutool.db.SqlConnRunner`

```java
public class cn.hutool.db.SqlConnRunner extends cn.hutool.db.DialectRunner {
  public static cn.hutool.db.SqlConnRunner create(cn.hutool.db.dialect.Dialect);
  public static cn.hutool.db.SqlConnRunner create(javax.sql.DataSource);
  public static cn.hutool.db.SqlConnRunner create(java.lang.String);
  public cn.hutool.db.SqlConnRunner(cn.hutool.db.dialect.Dialect);
  public cn.hutool.db.SqlConnRunner(java.lang.String);
  public int[] insert(java.sql.Connection, java.util.Collection<cn.hutool.db.Entity>) throws java.sql.SQLException;
  public int insert(java.sql.Connection, cn.hutool.db.Entity) throws java.sql.SQLException;
  public java.util.List<java.lang.Object> insertForGeneratedKeys(java.sql.Connection, cn.hutool.db.Entity) throws java.sql.SQLException;
  public java.lang.Long insertForGeneratedKey(java.sql.Connection, cn.hutool.db.Entity) throws java.sql.SQLException;
  public <T> T find(java.sql.Connection, java.util.Collection<java.lang.String>, cn.hutool.db.Entity, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public <T> T find(java.sql.Connection, cn.hutool.db.Entity, cn.hutool.db.handler.RsHandler<T>, java.lang.String...) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> find(java.sql.Connection, cn.hutool.db.Entity) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> findAll(java.sql.Connection, cn.hutool.db.Entity) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> findAll(java.sql.Connection, java.lang.String) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> findBy(java.sql.Connection, java.lang.String, java.lang.String, java.lang.Object) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> findLike(java.sql.Connection, java.lang.String, java.lang.String, java.lang.String, cn.hutool.db.sql.Condition$LikeType) throws java.sql.SQLException;
  public java.util.List<cn.hutool.db.Entity> findIn(java.sql.Connection, java.lang.String, java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public long count(java.sql.Connection, java.lang.CharSequence, java.lang.Object...) throws java.sql.SQLException;
  public <T> T page(java.sql.Connection, java.util.Collection<java.lang.String>, cn.hutool.db.Entity, int, int, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public cn.hutool.db.PageResult<cn.hutool.db.Entity> page(java.sql.Connection, cn.hutool.db.sql.SqlBuilder, cn.hutool.db.Page) throws java.sql.SQLException;
  public cn.hutool.db.PageResult<cn.hutool.db.Entity> page(java.sql.Connection, java.util.Collection<java.lang.String>, cn.hutool.db.Entity, int, int) throws java.sql.SQLException;
  public cn.hutool.db.PageResult<cn.hutool.db.Entity> page(java.sql.Connection, cn.hutool.db.Entity, cn.hutool.db.Page) throws java.sql.SQLException;
  public cn.hutool.db.PageResult<cn.hutool.db.Entity> page(java.sql.Connection, java.util.Collection<java.lang.String>, cn.hutool.db.Entity, cn.hutool.db.Page) throws java.sql.SQLException;
  public <T> T page(java.sql.Connection, java.util.Collection<java.lang.String>, cn.hutool.db.Entity, cn.hutool.db.Page, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
}
```

## `cn.hutool.db.StatementUtil`

```java
public class cn.hutool.db.StatementUtil {
  public cn.hutool.db.StatementUtil();
  public static java.sql.PreparedStatement fillParams(java.sql.PreparedStatement, java.lang.Object...) throws java.sql.SQLException;
  public static java.sql.PreparedStatement fillParams(java.sql.PreparedStatement, java.lang.Iterable<?>) throws java.sql.SQLException;
  public static java.sql.PreparedStatement fillParams(java.sql.PreparedStatement, java.lang.Iterable<?>, java.util.Map<java.lang.Integer, java.lang.Integer>) throws java.sql.SQLException;
  public static java.sql.PreparedStatement prepareStatement(java.sql.Connection, cn.hutool.db.sql.SqlBuilder) throws java.sql.SQLException;
  public static java.sql.PreparedStatement prepareStatement(java.sql.Connection, java.lang.String, java.util.Collection<java.lang.Object>) throws java.sql.SQLException;
  public static java.sql.PreparedStatement prepareStatement(java.sql.Connection, java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public static java.sql.PreparedStatement prepareStatement(boolean, java.sql.Connection, java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public static java.sql.PreparedStatement prepareStatementForBatch(java.sql.Connection, java.lang.String, java.lang.Object[]...) throws java.sql.SQLException;
  public static java.sql.PreparedStatement prepareStatementForBatch(java.sql.Connection, java.lang.String, java.lang.Iterable<java.lang.Object[]>) throws java.sql.SQLException;
  public static java.sql.PreparedStatement prepareStatementForBatch(java.sql.Connection, java.lang.String, java.lang.Iterable<java.lang.String>, cn.hutool.db.Entity...) throws java.sql.SQLException;
  public static java.sql.CallableStatement prepareCall(java.sql.Connection, java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public static java.lang.Long getGeneratedKeyOfLong(java.sql.Statement) throws java.sql.SQLException;
  public static java.util.List<java.lang.Object> getGeneratedKeys(java.sql.Statement) throws java.sql.SQLException;
  public static <T> T getGeneratedKeys(java.sql.Statement, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public static int getTypeOfNull(java.sql.PreparedStatement, int);
  public static void setParam(java.sql.PreparedStatement, int, java.lang.Object) throws java.sql.SQLException;
}
```

## `cn.hutool.db.ThreadLocalConnection`

```java
public final class cn.hutool.db.ThreadLocalConnection extends java.lang.Enum<cn.hutool.db.ThreadLocalConnection> {
  public static cn.hutool.db.ThreadLocalConnection[] values();
  public static cn.hutool.db.ThreadLocalConnection valueOf(java.lang.String);
  public java.sql.Connection get(javax.sql.DataSource) throws java.sql.SQLException;
  public void close(javax.sql.DataSource);
}
```

## `cn.hutool.db.ThreadLocalConnection$GroupedConnection`

```java
public class cn.hutool.db.ThreadLocalConnection$GroupedConnection {
  public cn.hutool.db.ThreadLocalConnection$GroupedConnection();
  public java.sql.Connection get(javax.sql.DataSource) throws java.sql.SQLException;
  public cn.hutool.db.ThreadLocalConnection$GroupedConnection close(javax.sql.DataSource);
  public boolean isEmpty();
}
```
