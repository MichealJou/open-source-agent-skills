# com.baomidou.mybatisplus.extension.ddl.history

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator` | `String createDdlHistory()` | 【原文待译】ddl_history sql |
| `com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator` | `String getDdlHistory()` | 返回 DDL_HISTORY 表名 |
| `com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator` | `String insertDdlHistory(String script,String type,String version)` | 【原文待译】insert ddl_history sql |
| `com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator` | `String selectDdlHistory(String script,String type)` | 【原文待译】select ddl_history sql |
| `com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator` | `boolean existTable(Connection connection)` | 检查#getDdlHistory()表是否存在 |
| `com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator` | `boolean existTable(String databaseName,Function<String, Boolean> executeFunction)` | 表是否存在 |
| `com.baomidou.mybatisplus.extension.ddl.history.MysqlDdlGenerator` | `IDdlGenerator newInstance()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.history.MysqlDdlGenerator` | `String createDdlHistory()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.history.MysqlDdlGenerator` | `boolean existTable(String databaseName,Function<String, Boolean> executeFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.history.OracleDdlGenerator` | `IDdlGenerator newInstance()` | 基于当前用户模式实例 |
| `com.baomidou.mybatisplus.extension.ddl.history.OracleDdlGenerator` | `String createDdlHistory()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.history.OracleDdlGenerator` | `String getDdlHistory()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.history.OracleDdlGenerator` | `boolean existTable(Connection connection)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.history.OracleDdlGenerator` | `boolean existTable(String databaseName,Function<String, Boolean> executeFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.history.PostgreDdlGenerator` | `IDdlGenerator newInstance()` | 默认实例 (基于public模式) |
| `com.baomidou.mybatisplus.extension.ddl.history.PostgreDdlGenerator` | `IDdlGenerator newInstanceWithAutoSchema()` | 基于数据库连接自动识别schema |
| `com.baomidou.mybatisplus.extension.ddl.history.PostgreDdlGenerator` | `IDdlGenerator newInstanceWithSchema(String schema)` | 手动指定schema |
| `com.baomidou.mybatisplus.extension.ddl.history.PostgreDdlGenerator` | `String createDdlHistory()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.history.PostgreDdlGenerator` | `String getDdlHistory()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.history.PostgreDdlGenerator` | `boolean existTable(Connection connection)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.history.PostgreDdlGenerator` | `boolean existTable(String databaseName,Function<String, Boolean> executeFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.history.SQLiteDdlGenerator` | `IDdlGenerator newInstance()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.history.SQLiteDdlGenerator` | `String createDdlHistory()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.history.SQLiteDdlGenerator` | `boolean existTable(String databaseName,Function<String, Boolean> executeFunction)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
