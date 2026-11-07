# cn.hutool.db.dialect.impl

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.db.dialect.impl.AnsiSqlDialect` | `PreparedStatement psForDelete(Connection conn,Query query)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.AnsiSqlDialect` | `PreparedStatement psForFind(Connection conn,Query query)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.AnsiSqlDialect` | `PreparedStatement psForInsert(Connection conn,Entity entity)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.AnsiSqlDialect` | `PreparedStatement psForInsertBatch(Connection conn,Entity... entities)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.AnsiSqlDialect` | `PreparedStatement psForPage(Connection conn,Query query)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.AnsiSqlDialect` | `PreparedStatement psForPage(Connection conn,SqlBuilder sqlBuilder,Page page)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.AnsiSqlDialect` | `PreparedStatement psForUpdate(Connection conn,Entity entity,Query query)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.AnsiSqlDialect` | `String dialectName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.AnsiSqlDialect` | `Wrapper getWrapper()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.AnsiSqlDialect` | `void setWrapper(Wrapper wrapper)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.DmDialect` | `PreparedStatement psForUpsert(Connection conn,Entity entity,String... keys)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.DmDialect` | `String dialectName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.H2Dialect` | `PreparedStatement psForUpsert(Connection conn,Entity entity,String... keys)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.H2Dialect` | `String dialectName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.HanaDialect` | `PreparedStatement psForUpsert(Connection conn,Entity entity,String... keys)` | 构建用于upsert的PreparedStatement。 SAP HANA 使用 MERGE INTO 语法来实现 UPSERT 操作。 生成 SQL 语法为： |
| `cn.hutool.db.dialect.impl.HanaDialect` | `String dialectName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.MysqlDialect` | `PreparedStatement psForUpsert(Connection conn,Entity entity,String... keys)` | 构建用于upsert的PreparedStatement MySQL通过主键方式实现Upsert，故keys无效，生成SQL语法为： |
| `cn.hutool.db.dialect.impl.MysqlDialect` | `String dialectName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.OracleDialect` | `String dialectName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.OracleDialect` | `boolean isNextVal(Object value)` | 检查字段值是否为Oracle自增字段，自增字段以'.nextval'结尾 |
| `cn.hutool.db.dialect.impl.PhoenixDialect` | `PreparedStatement psForUpdate(Connection conn,Entity entity,Query query)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.PhoenixDialect` | `PreparedStatement psForUpsert(Connection conn,Entity entity,String... keys)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.PhoenixDialect` | `String dialectName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.PostgresqlDialect` | `PreparedStatement psForUpsert(Connection conn,Entity entity,String... keys)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.PostgresqlDialect` | `String dialectName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.SqlServer2012Dialect` | `String dialectName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.dialect.impl.Sqlite3Dialect` | `String dialectName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
