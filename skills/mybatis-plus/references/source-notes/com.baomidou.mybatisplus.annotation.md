# com.baomidou.mybatisplus.annotation

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.annotation.DbType` | `DbType getDbType(String dbType)` | 获取数据库类型 |
| `com.baomidou.mybatisplus.annotation.DbType` | `boolean mysqlSameType()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.annotation.DbType` | `boolean oracleSameType()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.annotation.DbType` | `boolean postgresqlSameType()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.annotation.IEnum` | `T getValue()` | 枚举数据库存储值 |
| `com.baomidou.mybatisplus.annotation.InterceptorIgnore` | `String blockAttack()` | 攻击 SQL 阻断解析器,防止全表更新与删除 com.baomidou.mybatisplus.extension.plugins.inner.BlockAttackInnerInterceptor |
| `com.baomidou.mybatisplus.annotation.InterceptorIgnore` | `String dataPermission()` | 数据权限 com.baomidou.mybatisplus.extension.plugins.inner.DataPermissionInterceptor 默认关闭，需要注解打开 |
| `com.baomidou.mybatisplus.annotation.InterceptorIgnore` | `String dynamicTableName()` | 动态表名 com.baomidou.mybatisplus.extension.plugins.inner.DynamicTableNameInnerInterceptor |
| `com.baomidou.mybatisplus.annotation.InterceptorIgnore` | `String illegalSql()` | 垃圾SQL拦截 com.baomidou.mybatisplus.extension.plugins.inner.IllegalSQLInnerInterceptor |
| `com.baomidou.mybatisplus.annotation.InterceptorIgnore` | `String tenantLine()` | 行级租户 com.baomidou.mybatisplus.extension.plugins.inner.TenantLineInnerInterceptor |
| `com.baomidou.mybatisplus.annotation.InterceptorIgnore` | `String[] others()` | 其他的 格式应该为: "key"+"@"+可选项[false,true,1,0,on,off] 例如: "xxx@1" 或 "xxx@true" 或 "xxx@on" 如果配置了该属性的注解是注解在 Mapper 上的,则如果该 Mapper 的一部分 Method 需要取反则需要在 Method 上注解并配置此属性为反值 例如: "xxx@1" 在 Mapper 上, 则 Method 上需要 "xxx@0" |
| `com.baomidou.mybatisplus.annotation.KeySequence` | `DbType dbType()` | 数据库类型，未配置默认使用注入 IKeyGenerator 实现，多个实现必须指定 |
| `com.baomidou.mybatisplus.annotation.KeySequence` | `String value()` | 序列名 |
| `com.baomidou.mybatisplus.annotation.OrderBy` | `boolean asc()` | 默认倒序，设置 true 顺序 |
| `com.baomidou.mybatisplus.annotation.OrderBy` | `short sort()` | 数字越小越靠前 |
| `com.baomidou.mybatisplus.annotation.TableField` | `Class<? extends TypeHandler> typeHandler()` | 类型处理器 (该默认值不代表会按照该值生效), 只生效于 mp 自动注入的 method, 建议配合 TableName#autoResultMap() 一起使用 ResultMapping#typeHandler and ParameterMapping#typeHandler |
| `com.baomidou.mybatisplus.annotation.TableField` | `FieldFill fill()` | 字段自动填充策略 在对应模式下将会忽略 insertStrategy 或 updateStrategy 的配置,等于断言该字段必有值 |
| `com.baomidou.mybatisplus.annotation.TableField` | `FieldStrategy insertStrategy()` | 字段验证策略之 insert: 当insert操作时，该字段拼接insert语句时的策略 ALWAYS: 直接拼接 insert into table_a(column) values (#{columnProperty}); NOT_NULL: insert into table_a( column ) values ( #{columnProperty} ) NOT_EMPTY: insert into table_a( column ) values ( #{columnProperty} ) NEVER: 该字段不参加 insert 语句 NOT_EMPTY 如果针对的是非 CharS… |
| `com.baomidou.mybatisplus.annotation.TableField` | `FieldStrategy updateStrategy()` | 字段验证策略之 update: 当更新操作时，该字段拼接set语句时的策略 ALWAYS: 直接拼接 update table_a set column=#{columnProperty}, 属性为null/空string都会被set进去 NOT_NULL: update table_a set column=#{columnProperty} NOT_EMPTY: update table_a set column=#{columnProperty} NEVER: 该字段不参加 update 语句 NOT_EMPTY 如果针对的是非 CharSequence 类型的字段则效果等于 NOT_N… |
| `com.baomidou.mybatisplus.annotation.TableField` | `FieldStrategy whereStrategy()` | 字段验证策略之 where: 表示该字段在拼接where条件时的策略 ALWAYS: 直接拼接 column=#{columnProperty} NOT_NULL: column=#{columnProperty} NOT_EMPTY: column=#{columnProperty} NEVER: 该字段不参加 where 语句 NOT_EMPTY 如果针对的是非 CharSequence 类型的字段则效果等于 NOT_NULL |
| `com.baomidou.mybatisplus.annotation.TableField` | `JdbcType jdbcType()` | JDBC类型 (该默认值不代表会按照该值生效), 只生效于 mp 自动注入的 method, 建议配合 TableName#autoResultMap() 一起使用 ResultMapping#jdbcType and ParameterMapping#jdbcType |
| `com.baomidou.mybatisplus.annotation.TableField` | `String condition()` | 字段 where 实体查询比较条件 默认 SqlCondition#EQUAL |
| `com.baomidou.mybatisplus.annotation.TableField` | `String numericScale()` | 指定小数点后保留的位数, 只生效于 mp 自动注入的 method, 建议配合 TableName#autoResultMap() 一起使用 ParameterMapping#numericScale |
| `com.baomidou.mybatisplus.annotation.TableField` | `String property()` | 【原文待译】ResultMapping#property and ParameterMapping#property |
| `com.baomidou.mybatisplus.annotation.TableField` | `String update()` | 字段 update set 部分注入, 该注解优于 el 注解使用 例1：@TableField(.. , update="%s+1") 其中 %s 会填充为字段 输出 SQL 为：update 表 set 字段=字段+1 where ... 例2：@TableField(.. , update="now()") 使用数据库时间 输出 SQL 为：update 表 set 字段=now() where ... |
| `com.baomidou.mybatisplus.annotation.TableField` | `String value()` | 数据库字段值 不需要配置该值的情况: 当 com.baomidou.mybatisplus.core.MybatisConfiguration#mapUnderscoreToCamelCase 为 true 时, (mp下默认是true,mybatis默认是false), 数据库字段值.replace("_","").toUpperCase() == 实体属性名.toUpperCase() 当 com.baomidou.mybatisplus.core.MybatisConfiguration#mapUnderscoreToCamelCase 为 false 时, 数据库字段值.toUpper… |
| `com.baomidou.mybatisplus.annotation.TableField` | `boolean exist()` | 是否为数据库表字段 默认 true 存在，false 不存在 |
| `com.baomidou.mybatisplus.annotation.TableField` | `boolean javaType()` | 只在使用了 #typeHandler() 时判断是否辅助追加 javaType 一般情况下不推荐使用 ParameterMapping#javaType |
| `com.baomidou.mybatisplus.annotation.TableField` | `boolean keepGlobalFormat()` | 是否保持使用全局的 columnFormat 的值 只生效于 既设置了全局的 columnFormat 也设置了上面 #value() 的值 如果是 false , 全局的 columnFormat 不生效 |
| `com.baomidou.mybatisplus.annotation.TableField` | `boolean select()` | 是否进行 select 查询 大字段可设置为 false 不加入 select 查询范围 |
| `com.baomidou.mybatisplus.annotation.TableId` | `IdType type()` | 主键类型 IdType |
| `com.baomidou.mybatisplus.annotation.TableId` | `String value()` | 字段名（该值可无） |
| `com.baomidou.mybatisplus.annotation.TableLogic` | `String delval()` | 默认逻辑删除值（该值可无、会自动获取全局配置） |
| `com.baomidou.mybatisplus.annotation.TableLogic` | `String value()` | 默认逻辑未删除值（该值可无、会自动获取全局配置） |
| `com.baomidou.mybatisplus.annotation.TableName` | `String resultMap()` | 实体映射结果集, 只生效于 mp 自动注入的 method |
| `com.baomidou.mybatisplus.annotation.TableName` | `String schema()` | schema 配置此值将覆盖全局配置的 schema |
| `com.baomidou.mybatisplus.annotation.TableName` | `String value()` | 实体对应的表名 |
| `com.baomidou.mybatisplus.annotation.TableName` | `String[] excludeProperty()` | 需要排除的属性名 与#properties() 二选一配置,都配置了则#properties() 配置生效 |
| `com.baomidou.mybatisplus.annotation.TableName` | `String[] properties()` | 只需要的属性名 与#excludeProperty() 二选一配置,都配置了则只有此配置生效 |
| `com.baomidou.mybatisplus.annotation.TableName` | `boolean autoResultMap()` | 是否自动构建 resultMap 并使用, 只生效于 mp 自动注入的 method, 如果设置 resultMap 则不会进行 resultMap 的自动构建并注入, 只适合个别字段 设置了 typeHandler 或 jdbcType 的情况 |
| `com.baomidou.mybatisplus.annotation.TableName` | `boolean keepGlobalPrefix()` | 是否保持使用全局的 tablePrefix 的值 只生效于 既设置了全局的 tablePrefix 也设置了上面 #value() 的值 如果是 false , 全局的 tablePrefix 不生效 |
