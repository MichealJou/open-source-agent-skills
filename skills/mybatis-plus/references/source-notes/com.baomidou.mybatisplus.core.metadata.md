# com.baomidou.mybatisplus.core.metadata

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `IPage<R> convert(Function<? super T, ? extends R> mapper)` | IPage 的泛型转换 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `IPage<T> setCurrent(long current)` | 设置当前页 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `IPage<T> setPages(long pages)` | 内部什么也不干 只是为了 json 反序列化时不报错 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `IPage<T> setRecords(List<T> records)` | 设置分页记录列表 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `IPage<T> setSize(long size)` | 设置每页显示条数 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `IPage<T> setTotal(long total)` | 设置当前满足条件总行数 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `List<OrderItem> orders()` | 获取排序信息，排序的字段和正反序 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `List<T> getRecords()` | 分页记录列表 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `Long maxLimit()` | 最大每页分页数限制,优先级高于分页插件内的 maxLimit |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `String countId()` | 老分页插件不支持 MappedStatement 的 id |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `boolean optimizeCountSql()` | 自动优化 COUNT SQL【 默认：true 】 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `boolean optimizeJoinOfCountSql()` | com.baomidou.mybatisplus.extension.plugins.inner.PaginationInnerInterceptor#isOptimizeJoin() 两个参数都为 true 才会进行sql处理 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `boolean searchCount()` | 进行 count 查询 【 默认: true 】 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `long getCurrent()` | 当前页 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `long getPages()` | 当前分页总页数 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `long getSize()` | 获取每页显示条数 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `long getTotal()` | 当前满足条件总行数 |
| `com.baomidou.mybatisplus.core.metadata.IPage` | `long offset()` | 计算当前分页偏移量 |
| `com.baomidou.mybatisplus.core.metadata.MapperProxyMetadata` | `Class<?> getMapperInterface()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.metadata.MapperProxyMetadata` | `SqlSession getSqlSession()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.metadata.MapperProxyMetadata` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.metadata.OrderItem` | `List<OrderItem> ascs(String... columns)` | 根据指定字段列表进行升序排序 |
| `com.baomidou.mybatisplus.core.metadata.OrderItem` | `List<OrderItem> descs(String... columns)` | 根据指定字段列表进行降序排序 |
| `com.baomidou.mybatisplus.core.metadata.OrderItem` | `OrderItem asc(String column)` | 根据指定字段升序排序 |
| `com.baomidou.mybatisplus.core.metadata.OrderItem` | `OrderItem desc(String column)` | 根据指定字段降序排序 |
| `com.baomidou.mybatisplus.core.metadata.OrderItem` | `OrderItem setAsc(boolean asc)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.metadata.OrderItem` | `OrderItem setColumn(String column)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.metadata.OrderItem` | `OrderItem withExpression(String expression)` | 根据表达式排序 任意表达式语句,自行控制SQL注入 不适用与反序列 |
| `com.baomidou.mybatisplus.core.metadata.OrderItem` | `OrderItem withExpression(String expression,boolean asc)` | 根据表达式排序 任意表达式语句,自行控制SQL注入 不适用与反序列 |
| `com.baomidou.mybatisplus.core.metadata.OrderItem` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.metadata.TableFieldInfo` | `String getInsertSqlColumn()` | 获取 insert 时候字段 sql 脚本片段 insert into table (字段) values (值) 位于 "字段" 部位 不生成 if 标签 |
| `com.baomidou.mybatisplus.core.metadata.TableFieldInfo` | `String getInsertSqlColumnMaybeIf(final String prefix)` | 获取 insert 时候字段 sql 脚本片段 insert into table (字段) values (值) 位于 "字段" 部位 根据规则会生成 if 标签 |
| `com.baomidou.mybatisplus.core.metadata.TableFieldInfo` | `String getInsertSqlProperty(final String prefix)` | 获取 insert 时候插入值 sql 脚本片段 insert into table (字段) values (值) 位于 "值" 部位 不生成 if 标签 |
| `com.baomidou.mybatisplus.core.metadata.TableFieldInfo` | `String getInsertSqlPropertyMaybeIf(final String prefix)` | 获取 insert 时候插入值 sql 脚本片段 insert into table (字段) values (值) 位于 "值" 部位 根据规则会生成 if 标签 |
| `com.baomidou.mybatisplus.core.metadata.TableFieldInfo` | `String getSqlSet(final String prefix)` | 获取 set sql 片段 |
| `com.baomidou.mybatisplus.core.metadata.TableFieldInfo` | `String getSqlSet(final boolean ignoreIf,final String prefix)` | 获取 set sql 片段 |
| `com.baomidou.mybatisplus.core.metadata.TableFieldInfo` | `String getSqlWhere(final String prefix)` | 获取 查询的 sql 片段 |
| `com.baomidou.mybatisplus.core.metadata.TableFieldInfo` | `String getVersionOli(final String alias,final String prefix)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `List<OrderFieldInfo> getOrderByFields()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `List<TableFieldInfo> getFieldList()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `Object getPropertyValue(Object entity,String property)` | 获取对象属性值 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `String chooseSelect(Predicate<TableFieldInfo> predicate)` | 获取需要进行查询的 select sql 片段 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `String chooseSelect(Predicate<TableFieldInfo> predicate,List<String> noSelectProperty)` | 获取需要进行查询的 select sql 片段 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `String getAllInsertSqlColumnMaybeIf(final String prefix)` | 获取 insert 时候字段 sql 脚本片段 insert into table (字段) values (值) 位于 "字段" 部位 自动选部位,根据规则会生成 if 标签 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `String getAllInsertSqlColumnMaybeIf(final String prefix,boolean ignoreAutoIncrementColumn)` | 获取 insert 时候字段 sql 脚本片段 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `String getAllInsertSqlPropertyMaybeIf(final String prefix)` | 获取所有 insert 时候插入值 sql 脚本片段 insert into table (字段) values (值) 位于 "值" 部位 自动选部位,根据规则会生成 if 标签 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `String getAllInsertSqlPropertyMaybeIf(final String prefix,boolean ignoreAutoIncrementColumn)` | 获取所有 insert 时候插入值 sql 脚本片段 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `String getAllSqlSelect()` | 获取包含主键及字段的 select sql 片段 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `String getAllSqlSet(boolean ignoreLogicDelFiled,final String prefix)` | 获取所有的 sql set 片段 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `String getAllSqlWhere(boolean fistAnd,boolean ignoreLogicDelFiled,boolean withId,final String prefix)` | 获取所有的查询的 sql 片段 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `String getKeyInsertSqlColumn(final boolean batch,final String prefix,final boolean newLine)` | 获取 insert 时候主键 sql 脚本片段 insert into table (字段) values (值) 位于 "字段" 部位 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `String getKeyInsertSqlProperty(final boolean batch,final String prefix,final boolean newLine)` | 获取 insert 时候主键 sql 脚本片段 insert into table (字段) values (值) 位于 "值" 部位 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `String getKeySqlSelect()` | 获取主键的 select sql 片段 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `String getLogicDeleteSql(boolean startWithAnd,boolean isWhere)` | 获取逻辑删除字段的 sql 脚本 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `String getSqlStatement(String sqlMethod)` | 获得注入的 SQL Statement |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `T newInstance()` | 创建实例 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `boolean havePK()` | 是否有主键 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `boolean isLogicDelete()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.metadata.TableInfo` | `void setPropertyValue(Object entity,String property,Object... values)` | 设置对象属性值 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `KeyGenerator genKeyGenerator(String baseStatementId,TableInfo tableInfo,MapperBuilderAssistant builderAssistant)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `List<Field> getAllFields(Class<?> clazz)` | 获取该类的所有属性列表 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `List<Field> getAllFields(Class<?> clazz,AnnotationHandler annotationHandler)` | 获取该类的所有属性列表 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `List<TableInfo> getTableInfos()` | 获取所有实体映射表信息 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `TableInfo getTableInfo(Class<?> clazz)` | 获取实体映射表信息 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `TableInfo getTableInfo(String tableName)` | 根据表名获取实体映射表信息 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `TableInfo initTableInfo(MapperBuilderAssistant builderAssistant,Class<?> clazz)` | 实体类反射获取表信息【初始化】 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `boolean checkRelated(boolean underCamel,String property,String column)` | 判定 related 的值 为 true 表示不符合规则 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `boolean isExistOrderBy(Class<?> clazz,List<Field> list)` | 判断排序注解是否存在 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `boolean isExistOrderBy(List<Field> list,AnnotationHandler annotationHandler)` | 判断排序注解是否存在 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `boolean isExistTableId(Class<?> clazz,List<Field> list)` | 判断主键注解是否存在 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `boolean isExistTableId(List<Field> list,AnnotationHandler annotationHandler)` | 判断主键注解是否存在 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `boolean isExistTableLogic(Class<?> clazz,List<Field> list)` | 判断逻辑删除注解是否存在 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `boolean isExistTableLogic(List<Field> list,AnnotationHandler annotationHandler)` | 判断逻辑删除注解是否存在 |
| `com.baomidou.mybatisplus.core.metadata.TableInfoHelper` | `void remove(Class<?> entityClass)` | 清空实体表映射缓存信息 |
