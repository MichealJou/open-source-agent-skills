# com.baomidou.mybatisplus.extension.ddl

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.ddl.DdlHelper` | `InputStream getInputStream(String path)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.DdlHelper` | `ScriptRunner getScriptRunner(Connection connection,boolean autoCommit)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.DdlHelper` | `String getDatabase(String jdbcUrl)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.DdlHelper` | `void runScript(IDdlGenerator ddlGenerator,Connection connection,List<String> sqlFiles,Consumer<ScriptRunner> scriptRunnerConsumer,DdlScriptErrorHandler ddlScriptErrorHandler)` | 运行 SQL 脚本文件 |
| `com.baomidou.mybatisplus.extension.ddl.DdlHelper` | `void runScript(IDdlGenerator ddlGenerator,Connection connection,List<String> sqlFiles,Consumer<ScriptRunner> scriptRunnerConsumer,boolean autoCommit,DdlScriptErrorHandler ddlScriptErrorHandler)` | 运行 SQL 脚本文件 |
| `com.baomidou.mybatisplus.extension.ddl.DdlHelper` | `void runScript(IDdlGenerator ddlGenerator,Connection connection,List<String> sqlFiles,boolean autoCommit)` | 运行 SQL 脚本文件 |
| `com.baomidou.mybatisplus.extension.ddl.DdlHelper` | `void runScript(IDdlGenerator ddlGenerator,Connection connection,List<String> sqlFiles,boolean autoCommit,DdlScriptErrorHandler ddlScriptErrorHandler)` | 运行 SQL 脚本文件 |
| `com.baomidou.mybatisplus.extension.ddl.DdlHelper` | `void runScript(IDdlGenerator ddlGenerator,DataSource dataSource,List<String> sqlFiles,Consumer<ScriptRunner> scriptRunnerConsumer,DdlScriptErrorHandler ddlScriptErrorHandler)` | 运行 SQL 脚本文件 |
| `com.baomidou.mybatisplus.extension.ddl.DdlHelper` | `void runScript(IDdlGenerator ddlGenerator,DataSource dataSource,List<String> sqlFiles,Consumer<ScriptRunner> scriptRunnerConsumer,boolean autoCommit,DdlScriptErrorHandler ddlScriptErrorHandler)` | 运行 SQL 脚本文件 |
| `com.baomidou.mybatisplus.extension.ddl.DdlHelper` | `void runScript(IDdlGenerator ddlGenerator,DataSource dataSource,List<String> sqlFiles,boolean autoCommit)` | 运行 SQL 脚本文件 |
| `com.baomidou.mybatisplus.extension.ddl.DdlHelper` | `void runScript(IDdlGenerator ddlGenerator,DataSource dataSource,List<String> sqlFiles,boolean autoCommit,DdlScriptErrorHandler ddlScriptErrorHandler)` | 运行 SQL 脚本文件 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScript` | `DdlScript scriptRunner(Consumer<ScriptRunner> scriptRunnerConsumer)` | 自定义 ScriptRunner |
| `com.baomidou.mybatisplus.extension.ddl.DdlScript` | `boolean execute(final String driverClassName,final String url,final String user,final String password,final String sqlScript,Consumer<String> exceptionConsumer)` | 以默认分隔符(;) 执行 SQL 脚本 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScript` | `boolean execute(final String driverClassName,final String url,final String user,final String password,final String sqlScript,String delimiter,Consumer<String> exceptionConsumer)` | 以指定分隔符 执行 SQL 脚本 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScript` | `boolean run(String sqlScript,Consumer<String> exceptionConsumer)` | 以默认分隔符(;) 执行 SQL 脚本 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScript` | `boolean run(String sqlScript,String delimiter,Consumer<String> exceptionConsumer)` | 以指定分隔符 执行 SQL 脚本 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScript` | `void run(Connection connection,Reader reader,boolean autoCommit,String delimiter)` | 执行 SQL 脚本 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScript` | `void run(List<String> sqlFiles)` | 执行 SQL 脚本文件 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScript` | `void run(List<String> sqlFiles,boolean autoCommit)` | 执行 SQL 脚本文件 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScript` | `void run(Reader reader)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScript` | `void run(Reader reader,boolean autoCommit)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScript` | `void run(Reader reader,boolean autoCommit,String delimiter)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScript` | `void run(String sqlScript)` | 运行 SQL 脚本 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScript` | `void run(String sqlScript,String delimiter)` | 执行 SQL 脚本 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler` | `void handle(String sqlFile,Exception exception)` | 错误处理 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler$PrintlnLogErrorHandler` | `void handle(String sqlFile,Exception throwable)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler$ThrowsErrorHandler` | `void handle(String sqlFile,Exception throwable)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.IDdl` | `IDdlGenerator getDdlGenerator()` | DDL 生成器 |
| `com.baomidou.mybatisplus.extension.ddl.IDdl` | `List<String> getSqlFiles()` | 执行 SQL 脚本 Resources.getResourceAsReader("db/test.sql") |
| `com.baomidou.mybatisplus.extension.ddl.IDdl` | `void runScript(Consumer<DataSource> consumer)` | 执行 SQL 脚本 |
| `com.baomidou.mybatisplus.extension.ddl.SimpleDdl` | `List<String> getSqlFiles()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.ddl.SimpleDdl` | `void runScript(Consumer<DataSource> consumer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
