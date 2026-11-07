# com.baomidou.mybatisplus.extension.plugins.handler

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.plugins.handler.DataPermissionHandler` | `Expression getSqlSegment(Expression where,String mappedStatementId)` | 获取数据权限 SQL 片段 |
| `com.baomidou.mybatisplus.extension.plugins.handler.MultiDataPermissionHandler` | `Expression getSqlSegment(Expression where,String mappedStatementId)` | 为兼容旧版数据权限处理器，继承了 DataPermissionHandler 但是新的多表数据权限处理又不会调用此方法，因此标记过时 |
| `com.baomidou.mybatisplus.extension.plugins.handler.MultiDataPermissionHandler` | `Expression getSqlSegment(final Table table,final Expression where,final String mappedStatementId)` | 获取数据权限 SQL 片段。 旧的 MultiDataPermissionHandler#getSqlSegment(Expression, String) 方法第一个参数包含所有的 where 条件信息，如果 return 了 null 会覆盖原有的 where 数据， 新版的 MultiDataPermissionHandler#getSqlSegment(Table, Expression, String) 方法不能覆盖原有的 where 数据，如果 return 了 null 则表示不追加任何 where 条件 |
| `com.baomidou.mybatisplus.extension.plugins.handler.TableNameHandler` | `String dynamicTableName(String sql,String tableName)` | 生成动态表名 |
| `com.baomidou.mybatisplus.extension.plugins.handler.TenantLineHandler` | `Expression getTenantId()` | 获取租户 ID 值表达式，只支持单个 ID 值 |
| `com.baomidou.mybatisplus.extension.plugins.handler.TenantLineHandler` | `String getTenantIdColumn()` | 获取租户字段名 默认字段名叫: tenant_id |
| `com.baomidou.mybatisplus.extension.plugins.handler.TenantLineHandler` | `boolean ignoreInsert(List<Column> columns,String tenantIdColumn)` | 忽略插入租户字段逻辑 |
| `com.baomidou.mybatisplus.extension.plugins.handler.TenantLineHandler` | `boolean ignoreTable(String tableName)` | 根据表名判断是否忽略拼接多租户条件 默认都要进行解析并拼接多租户条件 |
