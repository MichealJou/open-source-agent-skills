# com.baomidou.mybatisplus.extension.plugins.inner

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.plugins.inner.BaseMultiTableInnerInterceptor`

```java
public abstract class com.baomidou.mybatisplus.extension.plugins.inner.BaseMultiTableInnerInterceptor extends com.baomidou.mybatisplus.extension.parser.JsqlParserSupport implements com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor {
  public abstract net.sf.jsqlparser.expression.Expression buildTableExpression(net.sf.jsqlparser.schema.Table, net.sf.jsqlparser.expression.Expression, java.lang.String);
  public com.baomidou.mybatisplus.jsqlparser.enums.ExpressionAppendMode getExpressionAppendMode();
  public void setExpressionAppendMode(com.baomidou.mybatisplus.jsqlparser.enums.ExpressionAppendMode);
  public com.baomidou.mybatisplus.extension.plugins.inner.BaseMultiTableInnerInterceptor();
  public java.lang.String toString();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.BlockAttackInnerInterceptor`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.BlockAttackInnerInterceptor extends com.baomidou.mybatisplus.extension.parser.JsqlParserSupport implements com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor {
  public com.baomidou.mybatisplus.extension.plugins.inner.BlockAttackInnerInterceptor();
  public void beforePrepare(org.apache.ibatis.executor.statement.StatementHandler, java.sql.Connection, java.lang.Integer);
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor implements com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor {
  public com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor();
  public void beforePrepare(org.apache.ibatis.executor.statement.StatementHandler, java.sql.Connection, java.lang.Integer);
  public com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$OperationResult processInsert(net.sf.jsqlparser.statement.insert.Insert, org.apache.ibatis.mapping.BoundSql);
  public com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$OperationResult processUpdate(net.sf.jsqlparser.statement.update.Update, org.apache.ibatis.mapping.MappedStatement, org.apache.ibatis.mapping.BoundSql, java.sql.Connection);
  public com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$OperationResult processDelete(net.sf.jsqlparser.statement.delete.Delete, org.apache.ibatis.mapping.MappedStatement, org.apache.ibatis.mapping.BoundSql, java.sql.Connection);
  public com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor setBatchUpdateLimit(int);
  public com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor openBatchUpdateLimitation();
  public com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor configTableLimitation(java.lang.String, int);
  public void setProperties(java.util.Properties);
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$Columns2SelectItemsResult`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$Columns2SelectItemsResult {
  public static com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$Columns2SelectItemsResult build(java.util.List<net.sf.jsqlparser.statement.select.SelectItem<?>>, int);
  public com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$Columns2SelectItemsResult();
  public net.sf.jsqlparser.schema.Column getPk();
  public java.util.List<net.sf.jsqlparser.statement.select.SelectItem<?>> getSelectItems();
  public int getAdditionalItemCount();
  public void setPk(net.sf.jsqlparser.schema.Column);
  public void setSelectItems(java.util.List<net.sf.jsqlparser.statement.select.SelectItem<?>>);
  public void setAdditionalItemCount(int);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataChangedRecord`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataChangedRecord {
  public boolean hasUpdate(java.util.Map<java.lang.String, java.lang.Object>, java.util.Set<java.lang.String>, java.util.Set<java.lang.String>);
  public java.lang.String generateUpdatedDataStr();
  public java.lang.String convertDoubleQuotes(java.lang.Object);
  public com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataChangedRecord();
  public java.lang.String getPkColumnName();
  public java.lang.Object getPkColumnVal();
  public java.util.List<com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult> getOriginalColumnDatas();
  public java.util.List<com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult> getUpdatedColumns();
  public void setPkColumnName(java.lang.String);
  public void setPkColumnVal(java.lang.Object);
  public void setOriginalColumnDatas(java.util.List<com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult>);
  public void setUpdatedColumns(java.util.List<com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult>);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult {
  public boolean isDataChanged(java.lang.Object);
  public static java.lang.String convertClob(java.sql.Clob);
  public static com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult constrcutByUpdateVal(java.lang.String, java.lang.Object);
  public static com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult constrcutByOriginalVal(java.lang.String, java.lang.Object);
  public java.lang.String generateDataStr();
  public java.lang.String convertDoubleQuotes(java.lang.Object);
  public com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult();
  public java.lang.String getColumnName();
  public java.lang.Object getOriginalValue();
  public java.lang.Object getUpdateValue();
  public void setColumnName(java.lang.String);
  public void setOriginalValue(java.lang.Object);
  public void setUpdateValue(java.lang.Object);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataUpdateLimitationException`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataUpdateLimitationException extends com.baomidou.mybatisplus.core.exceptions.MybatisPlusException {
  public com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataUpdateLimitationException(java.lang.String);
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$OperationResult`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$OperationResult {
  public void buildDataStr(java.util.List<com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataChangedRecord>);
  public java.lang.String toString();
  public com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$OperationResult();
  public java.lang.String getOperation();
  public boolean isRecordStatus();
  public java.lang.String getTableName();
  public java.lang.String getChangedData();
  public long getCost();
  public void setOperation(java.lang.String);
  public void setRecordStatus(boolean);
  public void setTableName(java.lang.String);
  public void setChangedData(java.lang.String);
  public void setCost(long);
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$OriginalDataObj`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$OriginalDataObj {
  public boolean isEmpty();
  public com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$OriginalDataObj();
  public java.util.List<com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataChangedRecord> getOriginalDataObj();
  public void setOriginalDataObj(java.util.List<com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataChangedRecord>);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.DataPermissionInterceptor`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.DataPermissionInterceptor extends com.baomidou.mybatisplus.extension.plugins.inner.BaseMultiTableInnerInterceptor implements com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor {
  public void beforeQuery(org.apache.ibatis.executor.Executor, org.apache.ibatis.mapping.MappedStatement, java.lang.Object, org.apache.ibatis.session.RowBounds, org.apache.ibatis.session.ResultHandler, org.apache.ibatis.mapping.BoundSql) throws java.sql.SQLException;
  public void beforePrepare(org.apache.ibatis.executor.statement.StatementHandler, java.sql.Connection, java.lang.Integer);
  public net.sf.jsqlparser.expression.Expression buildTableExpression(net.sf.jsqlparser.schema.Table, net.sf.jsqlparser.expression.Expression, java.lang.String);
  public com.baomidou.mybatisplus.extension.plugins.handler.DataPermissionHandler getDataPermissionHandler();
  public void setDataPermissionHandler(com.baomidou.mybatisplus.extension.plugins.handler.DataPermissionHandler);
  public com.baomidou.mybatisplus.extension.plugins.inner.DataPermissionInterceptor();
  public com.baomidou.mybatisplus.extension.plugins.inner.DataPermissionInterceptor(com.baomidou.mybatisplus.extension.plugins.handler.DataPermissionHandler);
  public java.lang.String toString();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.DynamicTableNameInnerInterceptor`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.DynamicTableNameInnerInterceptor implements com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor {
  public com.baomidou.mybatisplus.extension.plugins.inner.DynamicTableNameInnerInterceptor();
  public com.baomidou.mybatisplus.extension.plugins.inner.DynamicTableNameInnerInterceptor(com.baomidou.mybatisplus.extension.plugins.handler.TableNameHandler);
  public void beforeQuery(org.apache.ibatis.executor.Executor, org.apache.ibatis.mapping.MappedStatement, java.lang.Object, org.apache.ibatis.session.RowBounds, org.apache.ibatis.session.ResultHandler, org.apache.ibatis.mapping.BoundSql) throws java.sql.SQLException;
  public void beforePrepare(org.apache.ibatis.executor.statement.StatementHandler, java.sql.Connection, java.lang.Integer);
  public java.lang.String changeTable(java.lang.String);
  public java.lang.Runnable getHook();
  public com.baomidou.mybatisplus.extension.plugins.handler.TableNameHandler getTableNameHandler();
  public void setHook(java.lang.Runnable);
  public void setTableNameHandler(com.baomidou.mybatisplus.extension.plugins.handler.TableNameHandler);
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.DynamicTableNameJsqlParserInnerInterceptor`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.DynamicTableNameJsqlParserInnerInterceptor extends com.baomidou.mybatisplus.extension.plugins.inner.DynamicTableNameInnerInterceptor {
  public com.baomidou.mybatisplus.extension.plugins.inner.DynamicTableNameJsqlParserInnerInterceptor();
  public com.baomidou.mybatisplus.extension.plugins.inner.DynamicTableNameJsqlParserInnerInterceptor(com.baomidou.mybatisplus.extension.plugins.handler.TableNameHandler);
  public void setIgnoreException(boolean);
  public void setShouldFallback(boolean);
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.IllegalSQLInnerInterceptor`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.IllegalSQLInnerInterceptor extends com.baomidou.mybatisplus.extension.parser.JsqlParserSupport implements com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor {
  public com.baomidou.mybatisplus.extension.plugins.inner.IllegalSQLInnerInterceptor();
  public void beforePrepare(org.apache.ibatis.executor.statement.StatementHandler, java.sql.Connection, java.lang.Integer);
  public java.util.List<com.baomidou.mybatisplus.extension.plugins.inner.IllegalSQLInnerInterceptor$IndexInfo> getIndexInfos(java.lang.String, java.lang.String, java.sql.Connection);
  public java.util.List<com.baomidou.mybatisplus.extension.plugins.inner.IllegalSQLInnerInterceptor$IndexInfo> getIndexInfos(java.lang.String, java.lang.String, java.lang.String, java.sql.Connection);
  public java.util.List<com.baomidou.mybatisplus.extension.plugins.inner.IllegalSQLInnerInterceptor$IndexInfo> getIndexInfos(java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.sql.Connection);
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor`

```java
public interface com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor {
  public default boolean willDoQuery(org.apache.ibatis.executor.Executor, org.apache.ibatis.mapping.MappedStatement, java.lang.Object, org.apache.ibatis.session.RowBounds, org.apache.ibatis.session.ResultHandler, org.apache.ibatis.mapping.BoundSql) throws java.sql.SQLException;
  public default void beforeQuery(org.apache.ibatis.executor.Executor, org.apache.ibatis.mapping.MappedStatement, java.lang.Object, org.apache.ibatis.session.RowBounds, org.apache.ibatis.session.ResultHandler, org.apache.ibatis.mapping.BoundSql) throws java.sql.SQLException;
  public default boolean willDoUpdate(org.apache.ibatis.executor.Executor, org.apache.ibatis.mapping.MappedStatement, java.lang.Object) throws java.sql.SQLException;
  public default void beforeUpdate(org.apache.ibatis.executor.Executor, org.apache.ibatis.mapping.MappedStatement, java.lang.Object) throws java.sql.SQLException;
  public default void beforePrepare(org.apache.ibatis.executor.statement.StatementHandler, java.sql.Connection, java.lang.Integer);
  public default void beforeGetBoundSql(org.apache.ibatis.executor.statement.StatementHandler);
  public default void setProperties(java.util.Properties);
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.OptimisticLockerInnerInterceptor`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.OptimisticLockerInnerInterceptor implements com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor {
  public com.baomidou.mybatisplus.extension.plugins.inner.OptimisticLockerInnerInterceptor();
  public com.baomidou.mybatisplus.extension.plugins.inner.OptimisticLockerInnerInterceptor(boolean);
  public void beforeUpdate(org.apache.ibatis.executor.Executor, org.apache.ibatis.mapping.MappedStatement, java.lang.Object);
  public void setException(java.lang.RuntimeException);
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.PaginationInnerInterceptor`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.PaginationInnerInterceptor implements com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor {
  public com.baomidou.mybatisplus.extension.plugins.inner.PaginationInnerInterceptor(com.baomidou.mybatisplus.annotation.DbType);
  public com.baomidou.mybatisplus.extension.plugins.inner.PaginationInnerInterceptor(com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect);
  public boolean willDoQuery(org.apache.ibatis.executor.Executor, org.apache.ibatis.mapping.MappedStatement, java.lang.Object, org.apache.ibatis.session.RowBounds, org.apache.ibatis.session.ResultHandler, org.apache.ibatis.mapping.BoundSql) throws java.sql.SQLException;
  public void beforeQuery(org.apache.ibatis.executor.Executor, org.apache.ibatis.mapping.MappedStatement, java.lang.Object, org.apache.ibatis.session.RowBounds, org.apache.ibatis.session.ResultHandler, org.apache.ibatis.mapping.BoundSql);
  public java.lang.String autoCountSql(com.baomidou.mybatisplus.core.metadata.IPage<?>, java.lang.String);
  public java.lang.String concatOrderBy(java.lang.String, java.util.List<com.baomidou.mybatisplus.core.metadata.OrderItem>);
  public void setProperties(java.util.Properties);
  public org.apache.ibatis.logging.Log getLogger();
  public boolean isOverflow();
  public java.lang.Long getMaxLimit();
  public com.baomidou.mybatisplus.annotation.DbType getDbType();
  public com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect getDialect();
  public boolean isOptimizeJoin();
  public void setOverflow(boolean);
  public void setMaxLimit(java.lang.Long);
  public void setDbType(com.baomidou.mybatisplus.annotation.DbType);
  public void setDialect(com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect);
  public void setOptimizeJoin(boolean);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public com.baomidou.mybatisplus.extension.plugins.inner.PaginationInnerInterceptor();
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.ReplacePlaceholderInnerInterceptor`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.ReplacePlaceholderInnerInterceptor implements com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor {
  public com.baomidou.mybatisplus.extension.plugins.inner.ReplacePlaceholderInnerInterceptor();
  public com.baomidou.mybatisplus.extension.plugins.inner.ReplacePlaceholderInnerInterceptor(java.lang.String);
  public void beforeQuery(org.apache.ibatis.executor.Executor, org.apache.ibatis.mapping.MappedStatement, java.lang.Object, org.apache.ibatis.session.RowBounds, org.apache.ibatis.session.ResultHandler, org.apache.ibatis.mapping.BoundSql) throws java.sql.SQLException;
}
```

## `com.baomidou.mybatisplus.extension.plugins.inner.TenantLineInnerInterceptor`

```java
public class com.baomidou.mybatisplus.extension.plugins.inner.TenantLineInnerInterceptor extends com.baomidou.mybatisplus.extension.plugins.inner.BaseMultiTableInnerInterceptor implements com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor {
  public void beforeQuery(org.apache.ibatis.executor.Executor, org.apache.ibatis.mapping.MappedStatement, java.lang.Object, org.apache.ibatis.session.RowBounds, org.apache.ibatis.session.ResultHandler, org.apache.ibatis.mapping.BoundSql);
  public void beforePrepare(org.apache.ibatis.executor.statement.StatementHandler, java.sql.Connection, java.lang.Integer);
  public void setProperties(java.util.Properties);
  public net.sf.jsqlparser.expression.Expression buildTableExpression(net.sf.jsqlparser.schema.Table, net.sf.jsqlparser.expression.Expression, java.lang.String);
  public com.baomidou.mybatisplus.extension.plugins.handler.TenantLineHandler getTenantLineHandler();
  public void setTenantLineHandler(com.baomidou.mybatisplus.extension.plugins.handler.TenantLineHandler);
  public com.baomidou.mybatisplus.extension.plugins.inner.TenantLineInnerInterceptor();
  public com.baomidou.mybatisplus.extension.plugins.inner.TenantLineInnerInterceptor(com.baomidou.mybatisplus.extension.plugins.handler.TenantLineHandler);
  public java.lang.String toString();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```
