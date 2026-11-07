# cn.hutool.db.meta

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.db.meta.Column` | `Column clone()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.Column` | `Column create(Table table,ResultSet columnMetaRs)` | 创建列对象 |
| `cn.hutool.db.meta.Column` | `Column setAutoIncrement(boolean autoIncrement)` | 设置是否自增 |
| `cn.hutool.db.meta.Column` | `Column setColumnDef(String columnDef)` | 设置默认值 |
| `cn.hutool.db.meta.Column` | `Column setComment(String comment)` | 设置注释 |
| `cn.hutool.db.meta.Column` | `Column setDigit(int digit)` | 设置小数位数 |
| `cn.hutool.db.meta.Column` | `Column setName(String name)` | 设置列名 |
| `cn.hutool.db.meta.Column` | `Column setNullable(boolean isNullable)` | 设置是否为可空 |
| `cn.hutool.db.meta.Column` | `Column setPk(boolean isPk)` | 设置是否主键 |
| `cn.hutool.db.meta.Column` | `Column setSize(int size)` | 设置大小或数据长度 |
| `cn.hutool.db.meta.Column` | `Column setTableName(String tableName)` | 设置表名 |
| `cn.hutool.db.meta.Column` | `Column setType(int type)` | 设置类型，对应java.sql.Types中的类型 |
| `cn.hutool.db.meta.Column` | `Column setTypeName(String typeName)` | 设置类型名称 |
| `cn.hutool.db.meta.Column` | `Integer getDigit()` | 获取小数位数 |
| `cn.hutool.db.meta.Column` | `JdbcType getTypeEnum()` | 获取字段类型的枚举 |
| `cn.hutool.db.meta.Column` | `String getColumnDef()` | 获取默认值 |
| `cn.hutool.db.meta.Column` | `String getComment()` | 获取注释 |
| `cn.hutool.db.meta.Column` | `String getName()` | 获取列名 |
| `cn.hutool.db.meta.Column` | `String getTableName()` | 获取表名 |
| `cn.hutool.db.meta.Column` | `String getTypeName()` | 获取类型名称 |
| `cn.hutool.db.meta.Column` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.Column` | `boolean isAutoIncrement()` | 是否自增 |
| `cn.hutool.db.meta.Column` | `boolean isNullable()` | 是否为可空 |
| `cn.hutool.db.meta.Column` | `boolean isPk()` | 是否主键 |
| `cn.hutool.db.meta.Column` | `int getType()` | 获取类型，对应java.sql.Types中的类型 |
| `cn.hutool.db.meta.Column` | `long getSize()` | 获取大小或数据长度 |
| `cn.hutool.db.meta.Column` | `void init(Table table,ResultSet columnMetaRs)` | 初始化 |
| `cn.hutool.db.meta.ColumnIndexInfo` | `ColumnIndexInfo clone()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.ColumnIndexInfo` | `ColumnIndexInfo create(ResultSet rs)` | 根据DatabaseMetaData#getIndexInfo获取的ResultSet构建索引列信息 |
| `cn.hutool.db.meta.ColumnIndexInfo` | `String getAscOrDesc()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.ColumnIndexInfo` | `String getColumnName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.ColumnIndexInfo` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.ColumnIndexInfo` | `void setAscOrDesc(String ascOrDesc)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.ColumnIndexInfo` | `void setColumnName(String columnName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `IndexInfo clone()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `List<ColumnIndexInfo> getColumnIndexInfoList()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `String getCatalog()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `String getIndexName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `String getSchema()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `String getTableName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `boolean equals(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `boolean isNonUnique()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `void setCatalog(String catalog)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `void setColumnIndexInfoList(List<ColumnIndexInfo> columnIndexInfoList)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `void setIndexName(String indexName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `void setNonUnique(boolean nonUnique)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `void setSchema(String schema)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.IndexInfo` | `void setTableName(String tableName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.JdbcType` | `JdbcType valueOf(int code)` | 通过java.sql.Types中对应int值找到enum值 |
| `cn.hutool.db.meta.MetaUtil` | `DatabaseMetaData getMetaData(final Connection conn)` | 获取数据库连接的元数据信息。 |
| `cn.hutool.db.meta.MetaUtil` | `Entity createLimitedEntity(DataSource ds,String tableName)` | 创建带有字段限制的Entity对象 此方法读取数据库中对应表的字段列表，加入到Entity中，当Entity被设置内容时，会忽略对应表字段外的所有KEY |
| `cn.hutool.db.meta.MetaUtil` | `List<String> getTables(DataSource ds)` | 获得所有表名 |
| `cn.hutool.db.meta.MetaUtil` | `List<String> getTables(DataSource ds,String schema,String tableName,TableType... types)` | 获得所有表名 |
| `cn.hutool.db.meta.MetaUtil` | `List<String> getTables(DataSource ds,String schema,TableType... types)` | 获得所有表名 |
| `cn.hutool.db.meta.MetaUtil` | `List<String> getTables(DataSource ds,TableType... types)` | 获得所有表名 |
| `cn.hutool.db.meta.MetaUtil` | `Map<String, IndexInfo> getIndexInfo(final DatabaseMetaData metaData,final String catalog,final String schema,final String tableName)` | 获取指定表的索引信息。 |
| `cn.hutool.db.meta.MetaUtil` | `Set<String> getPrimaryKeys(final DatabaseMetaData metaData,final String catalog,final String schema,String tableName)` | 获取指定表的主键列名列表。 |
| `cn.hutool.db.meta.MetaUtil` | `String getCataLog(Connection conn)` | 获取catalog，获取失败返回null |
| `cn.hutool.db.meta.MetaUtil` | `String getCatalog(Connection conn)` | 获取catalog，获取失败返回null |
| `cn.hutool.db.meta.MetaUtil` | `String getRemarks(final DatabaseMetaData metaData,final String catalog,final String schema,String tableName)` | 获取指定表的备注信息。 |
| `cn.hutool.db.meta.MetaUtil` | `String getSchema(Connection conn)` | 获取schema，获取失败返回null |
| `cn.hutool.db.meta.MetaUtil` | `String[] getColumnNames(DataSource ds,String tableName)` | 获得表的所有列名 |
| `cn.hutool.db.meta.MetaUtil` | `String[] getColumnNames(ResultSet rs)` | 获得结果集的所有列名 |
| `cn.hutool.db.meta.MetaUtil` | `Table getTableMeta(DataSource ds,String catalog,String schema,String tableName)` | 获得表的元信息 注意如果需要获取注释，某些数据库如MySQL，需要在配置中添加: |
| `cn.hutool.db.meta.MetaUtil` | `Table getTableMeta(DataSource ds,String tableName)` | 获得表的元信息 注意如果需要获取注释，某些数据库如MySQL，需要在配置中添加: |
| `cn.hutool.db.meta.MetaUtil` | `Table getTableMeta(final Connection conn,String catalog,String schema,final String tableName)` | 获得表的元信息 注意如果需要获取注释，某些数据库如MySQL，需要在配置中添加: |
| `cn.hutool.db.meta.MetaUtil` | `boolean isOracle(final DatabaseMetaData metaData)` | 判断当前数据库是否为Oracle。 |
| `cn.hutool.db.meta.Table` | `Collection<Column> getColumns()` | 获取所有字段元信息 |
| `cn.hutool.db.meta.Table` | `Column getColumn(String name)` | 获取某列信息 |
| `cn.hutool.db.meta.Table` | `List<IndexInfo> getIndexInfoList()` | 获取索引信息 |
| `cn.hutool.db.meta.Table` | `Set<String> getPkNames()` | 获取主键列表 |
| `cn.hutool.db.meta.Table` | `String getCatalog()` | 获取catalog |
| `cn.hutool.db.meta.Table` | `String getComment()` | 获取注释 |
| `cn.hutool.db.meta.Table` | `String getSchema()` | 获取 schema |
| `cn.hutool.db.meta.Table` | `String getTableName()` | 获取表名 |
| `cn.hutool.db.meta.Table` | `Table addPk(String pkColumnName)` | 添加主键 |
| `cn.hutool.db.meta.Table` | `Table clone()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.Table` | `Table create(String tableName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.Table` | `Table setCatalog(String catalog)` | 设置catalog |
| `cn.hutool.db.meta.Table` | `Table setColumn(Column column)` | 设置列对象 |
| `cn.hutool.db.meta.Table` | `Table setComment(String comment)` | 设置注释 |
| `cn.hutool.db.meta.Table` | `Table setSchema(String schema)` | 设置schema |
| `cn.hutool.db.meta.Table` | `boolean isPk(String columnName)` | 给定列名是否为主键 |
| `cn.hutool.db.meta.Table` | `void setIndexInfoList(List<IndexInfo> indexInfoList)` | 设置索引信息 |
| `cn.hutool.db.meta.Table` | `void setPkNames(Set<String> pkNames)` | 设置主键列表 |
| `cn.hutool.db.meta.Table` | `void setTableName(String tableName)` | 设置表名 |
| `cn.hutool.db.meta.TableType` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.meta.TableType` | `String value()` | 获取值 |
