# com.baomidou.mybatisplus.extension.plugins.inner

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.plugins.inner.BaseMultiTableInnerInterceptor` | `Expression buildTableExpression(final Table table,final Expression where,final String whereSegment)` | 构建数据库表的查询条件 |
| `com.baomidou.mybatisplus.extension.plugins.inner.BlockAttackInnerInterceptor` | `void beforePrepare(StatementHandler sh,Connection connection,Integer transactionTimeout)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor` | `DataChangeRecorderInnerInterceptor configTableLimitation(String tableName,int limit)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor` | `DataChangeRecorderInnerInterceptor openBatchUpdateLimitation()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor` | `DataChangeRecorderInnerInterceptor setBatchUpdateLimit(int limit)` | 设置批量更新记录条数上限 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor` | `OperationResult processDelete(Delete deleteStmt,MappedStatement mappedStatement,BoundSql boundSql,Connection connection)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor` | `OperationResult processInsert(Insert insertStmt,BoundSql boundSql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor` | `OperationResult processUpdate(Update updateStmt,MappedStatement mappedStatement,BoundSql boundSql,Connection connection)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor` | `void beforePrepare(StatementHandler sh,Connection connection,Integer transactionTimeout)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor` | `void setProperties(Properties properties)` | ignoredColumns = TABLE_NAME1.COLUMN1,COLUMN2; TABLE2.COLUMN1,COLUMN2; TABLE3.*; *.COLUMN1,COLUMN2 多个表用分号分隔 TABLE_NAME1.COLUMN1,COLUMN2 : 表示忽略这个表的这2个字段 TABLE3.*: 表示忽略这张表的INSERT/UPDATE，delete暂时还保留 *.COLUMN1,COLUMN2:表示所有表的这个2个字段名都忽略 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$Columns2SelectItemsResult` | `Columns2SelectItemsResult build(List<SelectItem<?>> selectItems,int additionalItemCount)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataChangedRecord` | `String convertDoubleQuotes(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataChangedRecord` | `String generateUpdatedDataStr()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataChangedRecord` | `boolean hasUpdate(Map<String, Object> columnNameValMap,Set<String> ignoredColumns,Set<String> ignoreAllColumns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult` | `DataColumnChangeResult constrcutByOriginalVal(String columnName,Object originalValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult` | `DataColumnChangeResult constrcutByUpdateVal(String columnName,Object updateValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult` | `String convertClob(Clob clobObj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult` | `String convertDoubleQuotes(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult` | `String generateDataStr()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$DataColumnChangeResult` | `boolean isDataChanged(Object updateValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$OperationResult` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$OperationResult` | `void buildDataStr(List<DataChangedRecord> records)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataChangeRecorderInnerInterceptor$OriginalDataObj` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataPermissionInterceptor` | `Expression buildTableExpression(final Table table,final Expression where,final String whereSegment)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataPermissionInterceptor` | `void beforePrepare(StatementHandler sh,Connection connection,Integer transactionTimeout)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DataPermissionInterceptor` | `void beforeQuery(Executor executor,MappedStatement ms,Object parameter,RowBounds rowBounds,ResultHandler resultHandler,BoundSql boundSql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DynamicTableNameInnerInterceptor` | `String changeTable(String sql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DynamicTableNameInnerInterceptor` | `void beforePrepare(StatementHandler sh,Connection connection,Integer transactionTimeout)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.DynamicTableNameInnerInterceptor` | `void beforeQuery(Executor executor,MappedStatement ms,Object parameter,RowBounds rowBounds,ResultHandler resultHandler,BoundSql boundSql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.IllegalSQLInnerInterceptor` | `List<IndexInfo> getIndexInfos(String dbName,String tableName,Connection conn)` | 得到表的索引信息 |
| `com.baomidou.mybatisplus.extension.plugins.inner.IllegalSQLInnerInterceptor` | `List<IndexInfo> getIndexInfos(String key,String catalogName,String dbName,String tableName,Connection conn)` | 得到表的索引信息 |
| `com.baomidou.mybatisplus.extension.plugins.inner.IllegalSQLInnerInterceptor` | `List<IndexInfo> getIndexInfos(String key,String dbName,String tableName,Connection conn)` | 得到表的索引信息 |
| `com.baomidou.mybatisplus.extension.plugins.inner.IllegalSQLInnerInterceptor` | `void beforePrepare(StatementHandler sh,Connection connection,Integer transactionTimeout)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor` | `boolean willDoQuery(Executor executor,MappedStatement ms,Object parameter,RowBounds rowBounds,ResultHandler resultHandler,BoundSql boundSql)` | 判断是否执行 Executor#query(MappedStatement, Object, RowBounds, ResultHandler, CacheKey, BoundSql) 如果不执行query操作,则返回 Collections#emptyList() |
| `com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor` | `boolean willDoUpdate(Executor executor,MappedStatement ms,Object parameter)` | 判断是否执行 Executor#update(MappedStatement, Object) 如果不执行update操作,则影响行数的值为 -1 |
| `com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor` | `void beforeGetBoundSql(StatementHandler sh)` | StatementHandler#getBoundSql() 操作前置处理 只有 BatchExecutor 和 ReuseExecutor 才会调用到这个方法 |
| `com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor` | `void beforePrepare(StatementHandler sh,Connection connection,Integer transactionTimeout)` | StatementHandler#prepare(Connection, Integer) 操作前置处理 改改sql啥的 |
| `com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor` | `void beforeQuery(Executor executor,MappedStatement ms,Object parameter,RowBounds rowBounds,ResultHandler resultHandler,BoundSql boundSql)` | Executor#query(MappedStatement, Object, RowBounds, ResultHandler, CacheKey, BoundSql) 操作前置处理 改改sql啥的 |
| `com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor` | `void beforeUpdate(Executor executor,MappedStatement ms,Object parameter)` | Executor#update(MappedStatement, Object) 操作前置处理 改改sql啥的 |
| `com.baomidou.mybatisplus.extension.plugins.inner.InnerInterceptor` | `void setProperties(Properties properties)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.OptimisticLockerInnerInterceptor` | `void beforeUpdate(Executor executor,MappedStatement ms,Object parameter)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.PaginationInnerInterceptor` | `String autoCountSql(IPage<?> page,String sql)` | 获取自动优化的 countSql |
| `com.baomidou.mybatisplus.extension.plugins.inner.PaginationInnerInterceptor` | `String concatOrderBy(String originalSql,List<OrderItem> orderList)` | 查询SQL拼接Order By |
| `com.baomidou.mybatisplus.extension.plugins.inner.PaginationInnerInterceptor` | `boolean willDoQuery(Executor executor,MappedStatement ms,Object parameter,RowBounds rowBounds,ResultHandler resultHandler,BoundSql boundSql)` | 这里进行count,如果count为0这返回false(就是不再执行sql了) |
| `com.baomidou.mybatisplus.extension.plugins.inner.PaginationInnerInterceptor` | `void beforeQuery(Executor executor,MappedStatement ms,Object parameter,RowBounds rowBounds,ResultHandler resultHandler,BoundSql boundSql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.PaginationInnerInterceptor` | `void setProperties(Properties properties)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.ReplacePlaceholderInnerInterceptor` | `void beforeQuery(Executor executor,MappedStatement ms,Object parameter,RowBounds rowBounds,ResultHandler resultHandler,BoundSql boundSql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.TenantLineInnerInterceptor` | `Expression buildTableExpression(final Table table,final Expression where,final String whereSegment)` | 构建租户条件表达式 |
| `com.baomidou.mybatisplus.extension.plugins.inner.TenantLineInnerInterceptor` | `void beforePrepare(StatementHandler sh,Connection connection,Integer transactionTimeout)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.TenantLineInnerInterceptor` | `void beforeQuery(Executor executor,MappedStatement ms,Object parameter,RowBounds rowBounds,ResultHandler resultHandler,BoundSql boundSql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.inner.TenantLineInnerInterceptor` | `void setProperties(Properties properties)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
