# com.baomidou.mybatisplus.core.toolkit.sql

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlInjectionUtils` | `String removeEscapeCharacter(String text)` | 刪除字段转义符单引号双引号 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlInjectionUtils` | `boolean check(String value)` | 检查参数是否存在 SQL 注入 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils` | `String convertChoose(final String whenTest,final String whenSqlScript,final String otherwise)` | 生成 choose 标签的脚本 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils` | `String convertForeach(final String sqlScript,final String collection,final String index,final String item,final String separator)` | 生成 foreach 标签的脚本 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils` | `String convertIf(final String sqlScript,final String ifTest,boolean newLine)` | 获取 带 if 标签的脚本 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils` | `String convertParamMapping(Class<? extends TypeHandler<?>> typeHandler,JdbcType jdbcType,Integer numericScale)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils` | `String convertSet(final String sqlScript)` | 生成 set 标签的脚本 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils` | `String convertTrim(final String sqlScript,final String prefix,final String suffix,final String prefixOverrides,final String suffixOverrides)` | 获取 带 trim 标签的脚本 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils` | `String convertWhere(final String sqlScript)` | 生成 where 标签的脚本 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils` | `String mappingJdbcType(JdbcType jdbcType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils` | `String mappingNumericScale(Integer numericScale)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils` | `String mappingTypeHandler(Class<? extends TypeHandler<?>> typeHandler)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils` | `String safeParam(final String param)` | 安全入参: #{入参} |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils` | `String safeParam(final String param,final String mapping)` | 安全入参: #{入参,mapping} |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlScriptUtils` | `String unSafeParam(final String param)` | 非安全入参: ${入参} |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlUtils` | `List<String> findPlaceholder(String sql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlUtils` | `String concatLike(Object str,SqlLike type)` | 用%连接like |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlUtils` | `String getNewSelectBody(String selectBody,String alisa,String asAlisa,String escapeSymbol)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlUtils` | `String getSelectBody(String placeHolder,String escapeSymbol)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlUtils` | `String getSelectBody(String tableName,String alisa,String asAlisa,String escapeSymbol)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.sql.SqlUtils` | `String replaceSqlPlaceholder(String sql,List<String> placeHolder,String escapeSymbol)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.toolkit.sql.StringEscape` | `String escapeRawString(String escapeStr)` | 转义字符串。纯转义，不添加单引号。 |
| `com.baomidou.mybatisplus.core.toolkit.sql.StringEscape` | `String escapeString(String escapeStr)` | 转义字符串 |
