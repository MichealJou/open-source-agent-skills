# cn.hutool.db.sql

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.db.sql.Condition`

```java
public class cn.hutool.db.sql.Condition extends cn.hutool.core.clone.CloneSupport<cn.hutool.db.sql.Condition> {
  public static cn.hutool.db.sql.Condition parse(java.lang.String, java.lang.Object);
  public cn.hutool.db.sql.Condition();
  public cn.hutool.db.sql.Condition(boolean);
  public cn.hutool.db.sql.Condition(java.lang.String, java.lang.Object);
  public cn.hutool.db.sql.Condition(java.lang.String, java.lang.String, java.lang.Object);
  public cn.hutool.db.sql.Condition(java.lang.String, java.lang.String, cn.hutool.db.sql.Condition$LikeType);
  public cn.hutool.db.sql.Condition(java.lang.String, java.lang.Object, java.lang.Object);
  public java.lang.String getField();
  public void setField(java.lang.String);
  public java.lang.String getOperator();
  public void setOperator(java.lang.String);
  public java.lang.Object getValue();
  public void setValue(java.lang.Object);
  public void setValue(java.lang.Object, boolean);
  public boolean isPlaceHolder();
  public void setPlaceHolder(boolean);
  public boolean isOperatorBetween();
  public boolean isOperatorIn();
  public boolean isOperatorIs();
  public boolean isOperatorIsNot();
  public boolean isOperatorLike();
  public cn.hutool.db.sql.Condition checkValueNull();
  public java.lang.Object getSecondValue();
  public void setSecondValue(java.lang.Object);
  public cn.hutool.db.sql.LogicalOperator getLinkOperator();
  public void setLinkOperator(cn.hutool.db.sql.LogicalOperator);
  public java.lang.String toString();
  public java.lang.String toString(java.util.List<java.lang.Object>);
}
```

## `cn.hutool.db.sql.Condition$LikeType`

```java
public final class cn.hutool.db.sql.Condition$LikeType extends java.lang.Enum<cn.hutool.db.sql.Condition$LikeType> {
  public static cn.hutool.db.sql.Condition$LikeType[] values();
  public static cn.hutool.db.sql.Condition$LikeType valueOf(java.lang.String);
}
```

## `cn.hutool.db.sql.ConditionBuilder`

```java
public class cn.hutool.db.sql.ConditionBuilder implements cn.hutool.core.builder.Builder<java.lang.String> {
  public static cn.hutool.db.sql.ConditionBuilder of(cn.hutool.db.sql.Condition...);
  public cn.hutool.db.sql.ConditionBuilder(cn.hutool.db.sql.Condition...);
  public java.util.List<java.lang.Object> getParamValues();
  public java.lang.String build();
  public java.lang.String build(java.util.List<java.lang.Object>);
  public java.lang.String toString();
  public java.lang.Object build();
}
```

## `cn.hutool.db.sql.ConditionGroup`

```java
public class cn.hutool.db.sql.ConditionGroup extends cn.hutool.db.sql.Condition {
  public cn.hutool.db.sql.ConditionGroup();
  public void addConditions(cn.hutool.db.sql.Condition...);
  public java.lang.String toString(java.util.List<java.lang.Object>);
}
```

## `cn.hutool.db.sql.Direction`

```java
public final class cn.hutool.db.sql.Direction extends java.lang.Enum<cn.hutool.db.sql.Direction> {
  public static cn.hutool.db.sql.Direction[] values();
  public static cn.hutool.db.sql.Direction valueOf(java.lang.String);
  public static cn.hutool.db.sql.Direction fromString(java.lang.String) throws java.lang.IllegalArgumentException;
}
```

## `cn.hutool.db.sql.LogicalOperator`

```java
public final class cn.hutool.db.sql.LogicalOperator extends java.lang.Enum<cn.hutool.db.sql.LogicalOperator> {
  public static cn.hutool.db.sql.LogicalOperator[] values();
  public static cn.hutool.db.sql.LogicalOperator valueOf(java.lang.String);
  public boolean isSame(java.lang.String);
}
```

## `cn.hutool.db.sql.NamedSql`

```java
public class cn.hutool.db.sql.NamedSql {
  public cn.hutool.db.sql.NamedSql(java.lang.String, java.util.Map<java.lang.String, java.lang.Object>);
  public java.lang.String getSql();
  public java.lang.Object[] getParams();
  public java.util.List<java.lang.Object> getParamList();
}
```

## `cn.hutool.db.sql.Order`

```java
public class cn.hutool.db.sql.Order implements java.io.Serializable {
  public cn.hutool.db.sql.Order();
  public cn.hutool.db.sql.Order(java.lang.String);
  public cn.hutool.db.sql.Order(java.lang.String, cn.hutool.db.sql.Direction);
  public java.lang.String getField();
  public void setField(java.lang.String);
  public cn.hutool.db.sql.Direction getDirection();
  public void setDirection(cn.hutool.db.sql.Direction);
  public java.lang.String toString();
}
```

## `cn.hutool.db.sql.Query`

```java
public class cn.hutool.db.sql.Query {
  public static cn.hutool.db.sql.Query of(cn.hutool.db.Entity);
  public cn.hutool.db.sql.Query(java.lang.String...);
  public cn.hutool.db.sql.Query(cn.hutool.db.sql.Condition[], java.lang.String...);
  public cn.hutool.db.sql.Query(cn.hutool.db.sql.Condition[], cn.hutool.db.Page, java.lang.String...);
  public cn.hutool.db.sql.Query(java.util.Collection<java.lang.String>, java.lang.String[], cn.hutool.db.sql.Condition[], cn.hutool.db.Page);
  public java.util.Collection<java.lang.String> getFields();
  public cn.hutool.db.sql.Query setFields(java.util.Collection<java.lang.String>);
  public cn.hutool.db.sql.Query setFields(java.lang.String...);
  public java.lang.String[] getTableNames();
  public cn.hutool.db.sql.Query setTableNames(java.lang.String...);
  public cn.hutool.db.sql.Condition[] getWhere();
  public cn.hutool.db.sql.Query setWhere(cn.hutool.db.sql.Condition...);
  public cn.hutool.db.Page getPage();
  public cn.hutool.db.sql.Query setPage(cn.hutool.db.Page);
  public java.lang.String getFirstTableName() throws cn.hutool.db.DbRuntimeException;
}
```

## `cn.hutool.db.sql.SqlBuilder`

```java
public class cn.hutool.db.sql.SqlBuilder implements cn.hutool.core.builder.Builder<java.lang.String> {
  public static cn.hutool.db.sql.SqlBuilder create();
  public static cn.hutool.db.sql.SqlBuilder create(cn.hutool.db.sql.Wrapper);
  public static cn.hutool.db.sql.SqlBuilder of(java.lang.CharSequence);
  public static void validateEntity(cn.hutool.db.Entity) throws cn.hutool.db.DbRuntimeException;
  public cn.hutool.db.sql.SqlBuilder();
  public cn.hutool.db.sql.SqlBuilder(cn.hutool.db.sql.Wrapper);
  public cn.hutool.db.sql.SqlBuilder insert(cn.hutool.db.Entity);
  public cn.hutool.db.sql.SqlBuilder insert(cn.hutool.db.Entity, cn.hutool.db.dialect.DialectName);
  public cn.hutool.db.sql.SqlBuilder insert(cn.hutool.db.Entity, java.lang.String);
  public cn.hutool.db.sql.SqlBuilder delete(java.lang.String);
  public cn.hutool.db.sql.SqlBuilder update(cn.hutool.db.Entity);
  public cn.hutool.db.sql.SqlBuilder select(boolean, java.lang.String...);
  public cn.hutool.db.sql.SqlBuilder select(boolean, java.util.Collection<java.lang.String>);
  public cn.hutool.db.sql.SqlBuilder select(java.lang.String...);
  public cn.hutool.db.sql.SqlBuilder select(java.util.Collection<java.lang.String>);
  public cn.hutool.db.sql.SqlBuilder from(java.lang.String...);
  public cn.hutool.db.sql.SqlBuilder where(cn.hutool.db.sql.Condition...);
  public cn.hutool.db.sql.SqlBuilder where(java.lang.String);
  public <T> cn.hutool.db.sql.SqlBuilder in(java.lang.String, T...);
  public cn.hutool.db.sql.SqlBuilder groupBy(java.lang.String...);
  public cn.hutool.db.sql.SqlBuilder having(cn.hutool.db.sql.Condition...);
  public cn.hutool.db.sql.SqlBuilder having(java.lang.String);
  public cn.hutool.db.sql.SqlBuilder orderBy(cn.hutool.db.sql.Order...);
  public cn.hutool.db.sql.SqlBuilder join(java.lang.String, cn.hutool.db.sql.SqlBuilder$Join);
  public cn.hutool.db.sql.SqlBuilder on(cn.hutool.db.sql.Condition...);
  public cn.hutool.db.sql.SqlBuilder on(java.lang.String);
  public cn.hutool.db.sql.SqlBuilder insertPreFragment(java.lang.Object);
  public cn.hutool.db.sql.SqlBuilder append(java.lang.Object);
  public cn.hutool.db.sql.SqlBuilder addParams(java.lang.Object...);
  public cn.hutool.db.sql.SqlBuilder query(cn.hutool.db.sql.Query);
  public java.util.List<java.lang.Object> getParamValues();
  public java.lang.Object[] getParamValueArray();
  public java.lang.String build();
  public java.lang.String toString();
  public cn.hutool.db.sql.SqlBuilder format();
  public java.lang.Object build();
}
```

## `cn.hutool.db.sql.SqlBuilder$Join`

```java
public final class cn.hutool.db.sql.SqlBuilder$Join extends java.lang.Enum<cn.hutool.db.sql.SqlBuilder$Join> {
  public static cn.hutool.db.sql.SqlBuilder$Join[] values();
  public static cn.hutool.db.sql.SqlBuilder$Join valueOf(java.lang.String);
}
```

## `cn.hutool.db.sql.SqlExecutor`

```java
public class cn.hutool.db.sql.SqlExecutor {
  public cn.hutool.db.sql.SqlExecutor();
  public static int execute(java.sql.Connection, java.lang.String, java.util.Map<java.lang.String, java.lang.Object>) throws java.sql.SQLException;
  public static int execute(java.sql.Connection, java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public static boolean call(java.sql.Connection, java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public static java.sql.ResultSet callQuery(java.sql.Connection, java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public static java.lang.Long executeForGeneratedKey(java.sql.Connection, java.lang.String, java.util.Map<java.lang.String, java.lang.Object>) throws java.sql.SQLException;
  public static java.lang.Long executeForGeneratedKey(java.sql.Connection, java.lang.String, java.lang.Object...) throws java.sql.SQLException;
  public static int[] executeBatch(java.sql.Connection, java.lang.String, java.lang.Object[]...) throws java.sql.SQLException;
  public static int[] executeBatch(java.sql.Connection, java.lang.String, java.lang.Iterable<java.lang.Object[]>) throws java.sql.SQLException;
  public static int[] executeBatch(java.sql.Connection, java.lang.String...) throws java.sql.SQLException;
  public static int[] executeBatch(java.sql.Connection, java.lang.Iterable<java.lang.String>) throws java.sql.SQLException;
  public static <T> T query(java.sql.Connection, java.lang.String, cn.hutool.db.handler.RsHandler<T>, java.util.Map<java.lang.String, java.lang.Object>) throws java.sql.SQLException;
  public static <T> T query(java.sql.Connection, cn.hutool.db.sql.SqlBuilder, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public static <T> T query(java.sql.Connection, java.lang.String, cn.hutool.db.handler.RsHandler<T>, java.lang.Object...) throws java.sql.SQLException;
  public static <T> T query(java.sql.Connection, cn.hutool.core.lang.func.Func1<java.sql.Connection, java.sql.PreparedStatement>, cn.hutool.db.handler.RsHandler<T>) throws java.sql.SQLException;
  public static int executeUpdate(java.sql.PreparedStatement, java.lang.Object...) throws java.sql.SQLException;
  public static boolean execute(java.sql.PreparedStatement, java.lang.Object...) throws java.sql.SQLException;
  public static <T> T query(java.sql.PreparedStatement, cn.hutool.db.handler.RsHandler<T>, java.lang.Object...) throws java.sql.SQLException;
  public static <T> T queryAndClosePs(java.sql.PreparedStatement, cn.hutool.db.handler.RsHandler<T>, java.lang.Object...) throws java.sql.SQLException;
}
```

## `cn.hutool.db.sql.SqlFormatter`

```java
public class cn.hutool.db.sql.SqlFormatter {
  public cn.hutool.db.sql.SqlFormatter();
  public static java.lang.String format(java.lang.String);
}
```

## `cn.hutool.db.sql.SqlLog`

```java
public final class cn.hutool.db.sql.SqlLog extends java.lang.Enum<cn.hutool.db.sql.SqlLog> {
  public static cn.hutool.db.sql.SqlLog[] values();
  public static cn.hutool.db.sql.SqlLog valueOf(java.lang.String);
  public void init(boolean, boolean, boolean, cn.hutool.log.level.Level);
  public void log(java.lang.String);
  public void logForBatch(java.lang.String);
  public void log(java.lang.String, java.lang.Object);
}
```

## `cn.hutool.db.sql.SqlUtil`

```java
public class cn.hutool.db.sql.SqlUtil {
  public cn.hutool.db.sql.SqlUtil();
  public static java.lang.String buildEqualsWhere(cn.hutool.db.Entity, java.util.List<java.lang.Object>);
  public static cn.hutool.db.sql.Condition[] buildConditions(cn.hutool.db.Entity);
  public static java.lang.String buildLikeValue(java.lang.String, cn.hutool.db.sql.Condition$LikeType, boolean);
  public static java.lang.String formatSql(java.lang.String);
  public static java.lang.String rowIdToString(java.sql.RowId);
  public static java.lang.String clobToStr(java.sql.Clob);
  public static java.lang.String blobToStr(java.sql.Blob, java.nio.charset.Charset);
  public static java.sql.Blob createBlob(java.sql.Connection, java.io.InputStream, boolean);
  public static java.sql.Blob createBlob(java.sql.Connection, byte[]);
  public static java.sql.Date toSqlDate(java.util.Date);
  public static java.sql.Timestamp toSqlTimestamp(java.util.Date);
  public static java.lang.String removeOuterOrderBy(java.lang.String);
  public static boolean isInClause(java.lang.CharSequence);
}
```

## `cn.hutool.db.sql.StatementWrapper`

```java
public class cn.hutool.db.sql.StatementWrapper implements java.sql.PreparedStatement {
  public cn.hutool.db.sql.StatementWrapper(java.sql.PreparedStatement);
  public java.sql.ResultSet executeQuery(java.lang.String) throws java.sql.SQLException;
  public int executeUpdate(java.lang.String) throws java.sql.SQLException;
  public void close() throws java.sql.SQLException;
  public int getMaxFieldSize() throws java.sql.SQLException;
  public void setMaxFieldSize(int) throws java.sql.SQLException;
  public int getMaxRows() throws java.sql.SQLException;
  public void setMaxRows(int) throws java.sql.SQLException;
  public void setEscapeProcessing(boolean) throws java.sql.SQLException;
  public int getQueryTimeout() throws java.sql.SQLException;
  public void setQueryTimeout(int) throws java.sql.SQLException;
  public void cancel() throws java.sql.SQLException;
  public java.sql.SQLWarning getWarnings() throws java.sql.SQLException;
  public void clearWarnings() throws java.sql.SQLException;
  public void setCursorName(java.lang.String) throws java.sql.SQLException;
  public boolean execute(java.lang.String) throws java.sql.SQLException;
  public java.sql.ResultSet getResultSet() throws java.sql.SQLException;
  public int getUpdateCount() throws java.sql.SQLException;
  public boolean getMoreResults() throws java.sql.SQLException;
  public void setFetchDirection(int) throws java.sql.SQLException;
  public int getFetchDirection() throws java.sql.SQLException;
  public void setFetchSize(int) throws java.sql.SQLException;
  public int getFetchSize() throws java.sql.SQLException;
  public int getResultSetConcurrency() throws java.sql.SQLException;
  public int getResultSetType() throws java.sql.SQLException;
  public void addBatch(java.lang.String) throws java.sql.SQLException;
  public void clearBatch() throws java.sql.SQLException;
  public int[] executeBatch() throws java.sql.SQLException;
  public java.sql.Connection getConnection() throws java.sql.SQLException;
  public boolean getMoreResults(int) throws java.sql.SQLException;
  public java.sql.ResultSet getGeneratedKeys() throws java.sql.SQLException;
  public int executeUpdate(java.lang.String, int) throws java.sql.SQLException;
  public int executeUpdate(java.lang.String, int[]) throws java.sql.SQLException;
  public int executeUpdate(java.lang.String, java.lang.String[]) throws java.sql.SQLException;
  public boolean execute(java.lang.String, int) throws java.sql.SQLException;
  public boolean execute(java.lang.String, int[]) throws java.sql.SQLException;
  public boolean execute(java.lang.String, java.lang.String[]) throws java.sql.SQLException;
  public int getResultSetHoldability() throws java.sql.SQLException;
  public boolean isClosed() throws java.sql.SQLException;
  public void setPoolable(boolean) throws java.sql.SQLException;
  public boolean isPoolable() throws java.sql.SQLException;
  public void closeOnCompletion() throws java.sql.SQLException;
  public boolean isCloseOnCompletion() throws java.sql.SQLException;
  public <T> T unwrap(java.lang.Class<T>) throws java.sql.SQLException;
  public boolean isWrapperFor(java.lang.Class<?>) throws java.sql.SQLException;
  public java.sql.ResultSet executeQuery() throws java.sql.SQLException;
  public int executeUpdate() throws java.sql.SQLException;
  public void setNull(int, int) throws java.sql.SQLException;
  public void setBoolean(int, boolean) throws java.sql.SQLException;
  public void setByte(int, byte) throws java.sql.SQLException;
  public void setShort(int, short) throws java.sql.SQLException;
  public void setInt(int, int) throws java.sql.SQLException;
  public void setLong(int, long) throws java.sql.SQLException;
  public void setFloat(int, float) throws java.sql.SQLException;
  public void setDouble(int, double) throws java.sql.SQLException;
  public void setBigDecimal(int, java.math.BigDecimal) throws java.sql.SQLException;
  public void setString(int, java.lang.String) throws java.sql.SQLException;
  public void setBytes(int, byte[]) throws java.sql.SQLException;
  public void setDate(int, java.sql.Date) throws java.sql.SQLException;
  public void setTime(int, java.sql.Time) throws java.sql.SQLException;
  public void setTimestamp(int, java.sql.Timestamp) throws java.sql.SQLException;
  public void setAsciiStream(int, java.io.InputStream, int) throws java.sql.SQLException;
  public void setUnicodeStream(int, java.io.InputStream, int) throws java.sql.SQLException;
  public void setBinaryStream(int, java.io.InputStream, int) throws java.sql.SQLException;
  public void clearParameters() throws java.sql.SQLException;
  public void setObject(int, java.lang.Object, int) throws java.sql.SQLException;
  public void setObject(int, java.lang.Object) throws java.sql.SQLException;
  public boolean execute() throws java.sql.SQLException;
  public void addBatch() throws java.sql.SQLException;
  public void setCharacterStream(int, java.io.Reader, int) throws java.sql.SQLException;
  public void setRef(int, java.sql.Ref) throws java.sql.SQLException;
  public void setBlob(int, java.sql.Blob) throws java.sql.SQLException;
  public void setClob(int, java.sql.Clob) throws java.sql.SQLException;
  public void setArray(int, java.sql.Array) throws java.sql.SQLException;
  public java.sql.ResultSetMetaData getMetaData() throws java.sql.SQLException;
  public void setDate(int, java.sql.Date, java.util.Calendar) throws java.sql.SQLException;
  public void setTime(int, java.sql.Time, java.util.Calendar) throws java.sql.SQLException;
  public void setTimestamp(int, java.sql.Timestamp, java.util.Calendar) throws java.sql.SQLException;
  public void setNull(int, int, java.lang.String) throws java.sql.SQLException;
  public void setURL(int, java.net.URL) throws java.sql.SQLException;
  public java.sql.ParameterMetaData getParameterMetaData() throws java.sql.SQLException;
  public void setRowId(int, java.sql.RowId) throws java.sql.SQLException;
  public void setNString(int, java.lang.String) throws java.sql.SQLException;
  public void setNCharacterStream(int, java.io.Reader, long) throws java.sql.SQLException;
  public void setNClob(int, java.sql.NClob) throws java.sql.SQLException;
  public void setClob(int, java.io.Reader, long) throws java.sql.SQLException;
  public void setBlob(int, java.io.InputStream, long) throws java.sql.SQLException;
  public void setNClob(int, java.io.Reader, long) throws java.sql.SQLException;
  public void setSQLXML(int, java.sql.SQLXML) throws java.sql.SQLException;
  public void setObject(int, java.lang.Object, int, int) throws java.sql.SQLException;
  public void setAsciiStream(int, java.io.InputStream, long) throws java.sql.SQLException;
  public void setBinaryStream(int, java.io.InputStream, long) throws java.sql.SQLException;
  public void setCharacterStream(int, java.io.Reader, long) throws java.sql.SQLException;
  public void setAsciiStream(int, java.io.InputStream) throws java.sql.SQLException;
  public void setBinaryStream(int, java.io.InputStream) throws java.sql.SQLException;
  public void setCharacterStream(int, java.io.Reader) throws java.sql.SQLException;
  public void setNCharacterStream(int, java.io.Reader) throws java.sql.SQLException;
  public void setClob(int, java.io.Reader) throws java.sql.SQLException;
  public void setBlob(int, java.io.InputStream) throws java.sql.SQLException;
  public void setNClob(int, java.io.Reader) throws java.sql.SQLException;
}
```

## `cn.hutool.db.sql.Wrapper`

```java
public class cn.hutool.db.sql.Wrapper implements java.io.Serializable {
  public cn.hutool.db.sql.Wrapper();
  public cn.hutool.db.sql.Wrapper(java.lang.Character);
  public cn.hutool.db.sql.Wrapper(java.lang.Character, java.lang.Character);
  public char getPreWrapQuote();
  public void setPreWrapQuote(java.lang.Character);
  public char getSufWrapQuote();
  public void setSufWrapQuote(java.lang.Character);
  public java.lang.String wrap(java.lang.String);
  public java.lang.String unWrap(java.lang.String);
  public java.lang.String[] wrap(java.lang.String...);
  public java.util.Collection<java.lang.String> wrap(java.util.Collection<java.lang.String>);
  public cn.hutool.db.Entity wrap(cn.hutool.db.Entity);
  public cn.hutool.db.sql.Condition[] wrap(cn.hutool.db.sql.Condition...);
}
```
