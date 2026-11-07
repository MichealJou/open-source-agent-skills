# cn.hutool.db.sql

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.db.sql.Condition` | `Condition checkValueNull()` | 检查值是否为null，如果为null转换为 "IS NULL"或"IS NOT NULL"形式 |
| `cn.hutool.db.sql.Condition` | `Condition parse(String field,Object expression)` | 解析为Condition |
| `cn.hutool.db.sql.Condition` | `LogicalOperator getLinkOperator()` | 获取与前一个Condition连接的逻辑运算符，可以是and或or |
| `cn.hutool.db.sql.Condition` | `Object getSecondValue()` | 获得between 类型中第二个值 |
| `cn.hutool.db.sql.Condition` | `Object getValue()` | 获得值 |
| `cn.hutool.db.sql.Condition` | `String getField()` | @return 字段 |
| `cn.hutool.db.sql.Condition` | `String getOperator()` | 获得运算符 大于号，小于号，等于号 等 |
| `cn.hutool.db.sql.Condition` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.Condition` | `String toString(List<Object> paramValues)` | 转换为条件字符串，并回填占位符对应的参数值 |
| `cn.hutool.db.sql.Condition` | `boolean isOperatorBetween()` | 是否 between x and y 类型 |
| `cn.hutool.db.sql.Condition` | `boolean isOperatorIn()` | 是否IN条件 |
| `cn.hutool.db.sql.Condition` | `boolean isOperatorIs()` | 是否IS条件 |
| `cn.hutool.db.sql.Condition` | `boolean isOperatorIsNot()` | 是否 IS NOT条件 |
| `cn.hutool.db.sql.Condition` | `boolean isOperatorLike()` | 是否LIKE条件 |
| `cn.hutool.db.sql.Condition` | `boolean isPlaceHolder()` | 是否使用条件占位符 |
| `cn.hutool.db.sql.Condition` | `void setField(String field)` | 设置字段名 |
| `cn.hutool.db.sql.Condition` | `void setLinkOperator(LogicalOperator linkOperator)` | 设置与前一个Condition连接的逻辑运算符，可以是and或or |
| `cn.hutool.db.sql.Condition` | `void setOperator(String operator)` | 设置运算符 大于号，小于号，等于号 等 |
| `cn.hutool.db.sql.Condition` | `void setPlaceHolder(boolean isPlaceHolder)` | 设置是否使用条件占位符 |
| `cn.hutool.db.sql.Condition` | `void setSecondValue(Object secondValue)` | 设置between 类型中第二个值 |
| `cn.hutool.db.sql.Condition` | `void setValue(Object value)` | 设置值，不解析表达式 |
| `cn.hutool.db.sql.Condition` | `void setValue(Object value,boolean isParse)` | 设置值 |
| `cn.hutool.db.sql.ConditionBuilder` | `ConditionBuilder of(Condition... conditions)` | 创建构建器 |
| `cn.hutool.db.sql.ConditionBuilder` | `List<Object> getParamValues()` | 返回构建后的参数列表 此方法调用前必须调用#build() |
| `cn.hutool.db.sql.ConditionBuilder` | `String build()` | 构建组合条件 例如：name = ? AND type IN (?, ?) AND other LIKE ? |
| `cn.hutool.db.sql.ConditionBuilder` | `String build(List<Object> paramValues)` | 构建组合条件 例如：name = ? AND type IN (?, ?) AND other LIKE ? |
| `cn.hutool.db.sql.ConditionBuilder` | `String toString()` | 构建组合条件 例如：name = ? AND type IN (?, ?) AND other LIKE ? |
| `cn.hutool.db.sql.ConditionGroup` | `String toString(List<Object> paramValues)` | 将条件组转换为条件字符串，使用括号包裹，并回填占位符对应的参数值 |
| `cn.hutool.db.sql.ConditionGroup` | `void addConditions(Condition... conditions)` | 追加条件 |
| `cn.hutool.db.sql.Direction` | `Direction fromString(String value)` | 根据字符串值返回对应Direction值 |
| `cn.hutool.db.sql.LogicalOperator` | `boolean isSame(String logicalOperatorStr)` | 给定字符串逻辑运算符是否与当前逻辑运算符一致，不区分大小写，自动去除两边空白符 |
| `cn.hutool.db.sql.NamedSql` | `List<Object> getParamList()` | 获取参数列表，按照占位符顺序 |
| `cn.hutool.db.sql.NamedSql` | `Object[] getParams()` | 获取参数列表，按照占位符顺序 |
| `cn.hutool.db.sql.NamedSql` | `String getSql()` | 获取SQL |
| `cn.hutool.db.sql.Order` | `Direction getDirection()` | @return 排序方向 |
| `cn.hutool.db.sql.Order` | `String getField()` | @return 排序字段 |
| `cn.hutool.db.sql.Order` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.Order` | `void setDirection(Direction direction)` | 设置排序方向 |
| `cn.hutool.db.sql.Order` | `void setField(String field)` | 设置排序字段 |
| `cn.hutool.db.sql.Query` | `Collection<String> getFields()` | 获得查询的字段名列表 |
| `cn.hutool.db.sql.Query` | `Condition[] getWhere()` | 获得条件语句 |
| `cn.hutool.db.sql.Query` | `Page getPage()` | 获得分页对象，无分页返回null |
| `cn.hutool.db.sql.Query` | `Query of(Entity where)` | 从Entity构建Query |
| `cn.hutool.db.sql.Query` | `Query setFields(Collection<String> fields)` | 设置查询的字段名列表 |
| `cn.hutool.db.sql.Query` | `Query setFields(String... fields)` | 设置查询的字段名列表 |
| `cn.hutool.db.sql.Query` | `Query setPage(Page page)` | 设置分页对象 |
| `cn.hutool.db.sql.Query` | `Query setTableNames(String... tableNames)` | 设置表名 |
| `cn.hutool.db.sql.Query` | `Query setWhere(Condition... where)` | 设置条件语句 |
| `cn.hutool.db.sql.Query` | `String getFirstTableName()` | 获得第一个表名 |
| `cn.hutool.db.sql.Query` | `String[] getTableNames()` | 获得表名数组 |
| `cn.hutool.db.sql.SqlBuilder` | `List<Object> getParamValues()` | 获得占位符对应的值列表 |
| `cn.hutool.db.sql.SqlBuilder` | `Object[] getParamValueArray()` | 获得占位符对应的值列表 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder addParams(Object... params)` | 手动增加参数，调用此方法前需确认SQL中有对应占位符，主要用于自定义SQL片段中有占位符的情况，例如： |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder append(Object sqlFragment)` | 追加SQL其它部分片段，此方法只是简单的追加SQL字符串，空格需手动加入，例如： |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder create()` | 创建SQL构建器 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder create(Wrapper wrapper)` | 创建SQL构建器 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder delete(String tableName)` | 删除 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder format()` | 格式化SQL语句 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder from(String... tableNames)` | 添加 from语句 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder groupBy(String... fields)` | 分组 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder having(Condition... conditions)` | 添加Having语句，所有逻辑之间关系使用Condition#setLinkOperator(LogicalOperator) 定义 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder having(String having)` | 添加Having语句 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder in(String field,T... values)` | 多值选择 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder insert(Entity entity)` | 插入，使用默认的ANSI方言 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder insert(Entity entity,DialectName dialectName)` | 插入 插入会忽略空的字段名及其对应值，但是对于有字段名对应值为null的情况不忽略 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder insert(Entity entity,String dialectName)` | 插入 插入会忽略空的字段名及其对应值，但是对于有字段名对应值为null的情况不忽略 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder insertPreFragment(Object sqlFragment)` | 在SQL的开头补充SQL片段 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder join(String tableName,Join join)` | 多表关联 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder of(CharSequence sql)` | 从已有的SQL中构建一个SqlBuilder |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder on(Condition... conditions)` | 配合JOIN的 ON语句，多表关联的条件语句，所有逻辑之间关系使用Condition#setLinkOperator(LogicalOperator) 定义 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder on(String on)` | 配合JOIN的 ON语句，多表关联的条件语句 只支持单一的逻辑运算符（例如多个条件之间） |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder orderBy(Order... orders)` | 排序 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder query(Query query)` | 构建查询SQL |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder select(Collection<String> fields)` | 查询（非Distinct） |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder select(String... fields)` | 查询（非Distinct） |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder select(boolean isDistinct,Collection<String> fields)` | 查询 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder select(boolean isDistinct,String... fields)` | 查询 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder update(Entity entity)` | 更新 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder where(Condition... conditions)` | 添加Where语句，所有逻辑之间关系使用Condition#setLinkOperator(LogicalOperator) 定义 |
| `cn.hutool.db.sql.SqlBuilder` | `SqlBuilder where(String where)` | 添加Where语句 |
| `cn.hutool.db.sql.SqlBuilder` | `String build()` | 构建，默认打印SQL日志 |
| `cn.hutool.db.sql.SqlBuilder` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.SqlBuilder` | `void validateEntity(Entity entity)` | 验证实体类对象的有效性 |
| `cn.hutool.db.sql.SqlExecutor` | `Long executeForGeneratedKey(Connection conn,String sql,Map<String, Object> paramMap)` | 执行非查询语句，返回主键 发查询语句包括 插入、更新、删除 此方法不会关闭Connection |
| `cn.hutool.db.sql.SqlExecutor` | `Long executeForGeneratedKey(Connection conn,String sql,Object... params)` | 执行非查询语句，返回主键 发查询语句包括 插入、更新、删除 此方法不会关闭Connection |
| `cn.hutool.db.sql.SqlExecutor` | `ResultSet callQuery(Connection conn,String sql,Object... params)` | 执行调用存储过程 此方法不会关闭Connection |
| `cn.hutool.db.sql.SqlExecutor` | `T query(Connection conn,Func1<Connection, PreparedStatement> statementFunc,RsHandler<T> rsh)` | 执行自定义的PreparedStatement，结果使用RsHandler处理 此方法主要用于自定义场景，如游标查询等 |
| `cn.hutool.db.sql.SqlExecutor` | `T query(Connection conn,SqlBuilder sqlBuilder,RsHandler<T> rsh)` | 执行查询语句 此方法不会关闭Connection |
| `cn.hutool.db.sql.SqlExecutor` | `T query(Connection conn,String sql,RsHandler<T> rsh,Map<String, Object> paramMap)` | 执行查询语句，例如：select * from table where field1=:name1 此方法不会关闭Connection |
| `cn.hutool.db.sql.SqlExecutor` | `T query(Connection conn,String sql,RsHandler<T> rsh,Object... params)` | 执行查询语句 此方法不会关闭Connection |
| `cn.hutool.db.sql.SqlExecutor` | `T query(PreparedStatement ps,RsHandler<T> rsh,Object... params)` | 执行查询语句 此方法不会关闭PreparedStatement |
| `cn.hutool.db.sql.SqlExecutor` | `T queryAndClosePs(PreparedStatement ps,RsHandler<T> rsh,Object... params)` | 执行查询语句并关闭PreparedStatement |
| `cn.hutool.db.sql.SqlExecutor` | `boolean call(Connection conn,String sql,Object... params)` | 执行调用存储过程 此方法不会关闭Connection |
| `cn.hutool.db.sql.SqlExecutor` | `boolean execute(PreparedStatement ps,Object... params)` | 可用于执行任何SQL语句，返回一个boolean值，表明执行该SQL语句是否返回了ResultSet。 如果执行后第一个结果是ResultSet，则返回true，否则返回false。 此方法不会关闭PreparedStatement |
| `cn.hutool.db.sql.SqlExecutor` | `int execute(Connection conn,String sql,Map<String, Object> paramMap)` | 执行非查询语句 语句包括 插入、更新、删除 此方法不会关闭Connection |
| `cn.hutool.db.sql.SqlExecutor` | `int execute(Connection conn,String sql,Object... params)` | 执行非查询语句 语句包括 插入、更新、删除 此方法不会关闭Connection |
| `cn.hutool.db.sql.SqlExecutor` | `int executeUpdate(PreparedStatement ps,Object... params)` | 用于执行 INSERT、UPDATE 或 DELETE 语句以及 SQL DDL（数据定义语言）语句，例如 CREATE TABLE 和 DROP TABLE。 INSERT、UPDATE 或 DELETE 语句的效果是修改表中零行或多行中的一列或多列。 executeUpdate 的返回值是一个整数（int），指示受影响的行数（即更新计数）。 对于 CREATE TABLE 或 DROP TABLE 等不操作行的语句，executeUpdate 的返回值总为零。 此方法不会关闭PreparedStatement |
| `cn.hutool.db.sql.SqlExecutor` | `int[] executeBatch(Connection conn,Iterable<String> sqls)` | 批量执行非查询语句 语句包括 插入、更新、删除 此方法不会关闭Connection |
| `cn.hutool.db.sql.SqlExecutor` | `int[] executeBatch(Connection conn,String sql,Iterable<Object[]> paramsBatch)` | 批量执行非查询语句 语句包括 插入、更新、删除 此方法不会关闭Connection |
| `cn.hutool.db.sql.SqlExecutor` | `int[] executeBatch(Connection conn,String sql,Object[]... paramsBatch)` | 批量执行非查询语句 语句包括 插入、更新、删除 此方法不会关闭Connection |
| `cn.hutool.db.sql.SqlExecutor` | `int[] executeBatch(Connection conn,String... sqls)` | 批量执行非查询语句 语句包括 插入、更新、删除 此方法不会关闭Connection |
| `cn.hutool.db.sql.SqlFormatter` | `String format(String source)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.SqlLog` | `void init(boolean isShowSql,boolean isFormatSql,boolean isShowParams,Level level)` | 设置全局配置：是否通过debug日志显示SQL |
| `cn.hutool.db.sql.SqlLog` | `void log(String sql)` | 打印SQL日志 |
| `cn.hutool.db.sql.SqlLog` | `void log(String sql,Object paramValues)` | 打印SQL日志 |
| `cn.hutool.db.sql.SqlLog` | `void logForBatch(String sql)` | 打印批量 SQL日志 |
| `cn.hutool.db.sql.SqlUtil` | `Blob createBlob(Connection conn,InputStream dataStream,boolean closeAfterUse)` | 创建Blob对象 |
| `cn.hutool.db.sql.SqlUtil` | `Blob createBlob(Connection conn,byte[] data)` | 创建Blob对象 |
| `cn.hutool.db.sql.SqlUtil` | `Condition[] buildConditions(Entity entity)` | 通过实体对象构建条件对象 |
| `cn.hutool.db.sql.SqlUtil` | `String blobToStr(Blob blob,Charset charset)` | Blob字段值转字符串 |
| `cn.hutool.db.sql.SqlUtil` | `String buildEqualsWhere(Entity entity,List<Object> paramValues)` | 构件相等条件的where语句 如果没有条件语句，泽返回空串，表示没有条件 |
| `cn.hutool.db.sql.SqlUtil` | `String buildLikeValue(String value,LikeType likeType,boolean withLikeKeyword)` | 创建LIKE语句中的值，创建的结果为： |
| `cn.hutool.db.sql.SqlUtil` | `String clobToStr(Clob clob)` | Clob字段值转字符串 |
| `cn.hutool.db.sql.SqlUtil` | `String formatSql(String sql)` | 格式化SQL |
| `cn.hutool.db.sql.SqlUtil` | `String removeOuterOrderBy(final String selectSql)` | 移除 SQL中的 ORDER BY 子句 |
| `cn.hutool.db.sql.SqlUtil` | `String rowIdToString(RowId rowId)` | 将RowId转为字符串 |
| `cn.hutool.db.sql.SqlUtil` | `boolean isInClause(final CharSequence sql)` | 判断当前上下文是否在 IN 子句中 通过检查变量前的SQL文本，判断是否符合 IN 子句的模式 |
| `cn.hutool.db.sql.SqlUtil` | `java.sql.Date toSqlDate(java.util.Date date)` | 转换为java.sql.Date |
| `cn.hutool.db.sql.SqlUtil` | `java.sql.Timestamp toSqlTimestamp(java.util.Date date)` | 转换为java.sql.Timestamp |
| `cn.hutool.db.sql.StatementWrapper` | `Connection getConnection()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `ParameterMetaData getParameterMetaData()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `ResultSet executeQuery()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `ResultSet executeQuery(String sql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `ResultSet getGeneratedKeys()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `ResultSet getResultSet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `ResultSetMetaData getMetaData()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `SQLWarning getWarnings()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `T unwrap(Class<T> iface)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `boolean execute()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `boolean execute(String sql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `boolean execute(String sql,String[] columnNames)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `boolean execute(String sql,int autoGeneratedKeys)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `boolean execute(String sql,int[] columnIndexes)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `boolean getMoreResults()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `boolean getMoreResults(int current)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `boolean isCloseOnCompletion()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `boolean isClosed()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `boolean isPoolable()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `boolean isWrapperFor(Class<?> iface)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int executeUpdate()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int executeUpdate(String sql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int executeUpdate(String sql,String[] columnNames)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int executeUpdate(String sql,int autoGeneratedKeys)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int executeUpdate(String sql,int[] columnIndexes)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int getFetchDirection()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int getFetchSize()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int getMaxFieldSize()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int getMaxRows()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int getQueryTimeout()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int getResultSetConcurrency()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int getResultSetHoldability()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int getResultSetType()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int getUpdateCount()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `int[] executeBatch()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void addBatch()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void addBatch(String sql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void cancel()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void clearBatch()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void clearParameters()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void clearWarnings()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void closeOnCompletion()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setArray(int parameterIndex,Array x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setAsciiStream(int parameterIndex,InputStream x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setAsciiStream(int parameterIndex,InputStream x,int length)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setAsciiStream(int parameterIndex,InputStream x,long length)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setBigDecimal(int parameterIndex,BigDecimal x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setBinaryStream(int parameterIndex,InputStream x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setBinaryStream(int parameterIndex,InputStream x,int length)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setBinaryStream(int parameterIndex,InputStream x,long length)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setBlob(int parameterIndex,Blob x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setBlob(int parameterIndex,InputStream inputStream)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setBlob(int parameterIndex,InputStream inputStream,long length)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setBoolean(int parameterIndex,boolean x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setByte(int parameterIndex,byte x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setBytes(int parameterIndex,byte[] x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setCharacterStream(int parameterIndex,Reader reader)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setCharacterStream(int parameterIndex,Reader reader,int length)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setCharacterStream(int parameterIndex,Reader reader,long length)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setClob(int parameterIndex,Clob x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setClob(int parameterIndex,Reader reader)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setClob(int parameterIndex,Reader reader,long length)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setCursorName(String name)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setDate(int parameterIndex,Date x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setDate(int parameterIndex,Date x,Calendar cal)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setDouble(int parameterIndex,double x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setEscapeProcessing(boolean enable)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setFetchDirection(int direction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setFetchSize(int rows)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setFloat(int parameterIndex,float x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setInt(int parameterIndex,int x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setLong(int parameterIndex,long x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setMaxFieldSize(int max)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setMaxRows(int max)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setNCharacterStream(int parameterIndex,Reader value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setNCharacterStream(int parameterIndex,Reader value,long length)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setNClob(int parameterIndex,NClob value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setNClob(int parameterIndex,Reader reader)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setNClob(int parameterIndex,Reader reader,long length)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setNString(int parameterIndex,String value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setNull(int parameterIndex,int sqlType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setNull(int parameterIndex,int sqlType,String typeName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setObject(int parameterIndex,Object x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setObject(int parameterIndex,Object x,int targetSqlType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setObject(int parameterIndex,Object x,int targetSqlType,int scaleOrLength)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setPoolable(boolean poolable)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setQueryTimeout(int seconds)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setRef(int parameterIndex,Ref x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setRowId(int parameterIndex,RowId x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setSQLXML(int parameterIndex,SQLXML xmlObject)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setShort(int parameterIndex,short x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setString(int parameterIndex,String x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setTime(int parameterIndex,Time x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setTime(int parameterIndex,Time x,Calendar cal)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setTimestamp(int parameterIndex,Timestamp x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setTimestamp(int parameterIndex,Timestamp x,Calendar cal)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setURL(int parameterIndex,URL x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.StatementWrapper` | `void setUnicodeStream(int parameterIndex,InputStream x,int length)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.sql.Wrapper` | `Collection<String> wrap(Collection<String> fields)` | 包装字段名 有时字段与SQL的某些关键字冲突，导致SQL出错，因此需要将字段名用单引号或者反引号包装起来，避免冲突 |
| `cn.hutool.db.sql.Wrapper` | `Condition[] wrap(Condition... conditions)` | 包装字段名 有时字段与SQL的某些关键字冲突，导致SQL出错，因此需要将字段名用单引号或者反引号包装起来，避免冲突 |
| `cn.hutool.db.sql.Wrapper` | `Entity wrap(Entity entity)` | 包装表名和字段名，此方法返回一个新的Entity实体类 有时字段与SQL的某些关键字冲突，导致SQL出错，因此需要将字段名用单引号或者反引号包装起来，避免冲突 |
| `cn.hutool.db.sql.Wrapper` | `String unWrap(String field)` | 解包装字段名 |
| `cn.hutool.db.sql.Wrapper` | `String wrap(String field)` | 包装字段名 有时字段与SQL的某些关键字冲突，导致SQL出错，因此需要将字段名用单引号或者反引号包装起来，避免冲突 |
| `cn.hutool.db.sql.Wrapper` | `String[] wrap(String... fields)` | 包装字段名 有时字段与SQL的某些关键字冲突，导致SQL出错，因此需要将字段名用单引号或者反引号包装起来，避免冲突 |
| `cn.hutool.db.sql.Wrapper` | `char getPreWrapQuote()` | @return 前置包装符号 |
| `cn.hutool.db.sql.Wrapper` | `char getSufWrapQuote()` | @return 后置包装符号 |
| `cn.hutool.db.sql.Wrapper` | `void setPreWrapQuote(Character preWrapQuote)` | 设置前置包装的符号 |
| `cn.hutool.db.sql.Wrapper` | `void setSufWrapQuote(Character sufWrapQuote)` | 设置后置包装的符号 |
