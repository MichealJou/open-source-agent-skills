# cn.hutool.db

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.db.AbstractDb` | `AbstractDb disableWrapper()` | 取消包装器 取消自动添加到字段名、表名上的包装符（例如双引号） |
| `cn.hutool.db.AbstractDb` | `AbstractDb setWrapper(Character wrapperChar)` | 设置包装器，包装器用于对表名、字段名进行符号包装（例如双引号），防止关键字与这些表名或字段冲突 |
| `cn.hutool.db.AbstractDb` | `AbstractDb setWrapper(Wrapper wrapper)` | 设置包装器，包装器用于对表名、字段名进行符号包装（例如双引号），防止关键字与这些表名或字段冲突 |
| `cn.hutool.db.AbstractDb` | `Connection getConnection()` | 获得链接。根据实现不同，可以自定义获取连接的方式 |
| `cn.hutool.db.AbstractDb` | `DataSource getDs()` | 获得数据源 |
| `cn.hutool.db.AbstractDb` | `Entity get(Entity where)` | 根据条件实体查询单个记录，当有多条返回时，只显示查询到的第一条 |
| `cn.hutool.db.AbstractDb` | `Entity get(String tableName,String field,T value)` | 根据某个字段（最好是唯一字段）查询单个记录 当有多条返回时，只显示查询到的第一条 |
| `cn.hutool.db.AbstractDb` | `Entity queryOne(String sql,Object... params)` | 查询单条记录 |
| `cn.hutool.db.AbstractDb` | `List<Entity> find(Collection<String> fields,Entity where)` | 查询 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `List<Entity> find(Entity where)` | 查询数据列表，返回字段由where参数指定 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `List<Entity> findAll(Entity where)` | 查询数据列表，返回所有字段 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `List<Entity> findAll(String tableName)` | 查询数据列表，返回所有字段 |
| `cn.hutool.db.AbstractDb` | `List<Entity> findBy(String tableName,Condition... wheres)` | 根据多个条件查询数据列表，返回所有字段 |
| `cn.hutool.db.AbstractDb` | `List<Entity> findBy(String tableName,String field,Object value)` | 根据某个字段名条件查询数据列表，返回所有字段 |
| `cn.hutool.db.AbstractDb` | `List<Entity> findLike(String tableName,String field,String value,LikeType likeType)` | 根据某个字段名条件查询数据列表，返回所有字段 |
| `cn.hutool.db.AbstractDb` | `List<Entity> pageForEntityList(Entity where,Page page)` | 分页查询，结果为Entity列表，不计算总数 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `List<Entity> pageForEntityList(Entity where,int page,int numPerPage)` | 分页查询，结果为Entity列表，不计算总数 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `List<Entity> query(String sql,Map<String, Object> params)` | 查询 |
| `cn.hutool.db.AbstractDb` | `List<Entity> query(String sql,Object... params)` | 查询 |
| `cn.hutool.db.AbstractDb` | `List<Object> insertForGeneratedKeys(Entity record)` | 插入数据 |
| `cn.hutool.db.AbstractDb` | `List<T> find(Entity where,Class<T> beanClass)` | 查询数据列表，返回字段由where参数指定 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `List<T> findAll(Entity where,Class<T> beanClass)` | 查询数据列表，返回所有字段 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `List<T> query(String sql,Class<T> beanClass,Object... params)` | 查询 |
| `cn.hutool.db.AbstractDb` | `Long executeForGeneratedKey(String sql,Object... params)` | 执行非查询语句 语句包括 插入、更新、删除 |
| `cn.hutool.db.AbstractDb` | `Long insertForGeneratedKey(Entity record)` | 插入数据 |
| `cn.hutool.db.AbstractDb` | `Number queryNumber(String sql,Object... params)` | 查询单条单个字段记录,并将其转换为Number |
| `cn.hutool.db.AbstractDb` | `PageResult<Entity> page(CharSequence sql,Page page,Object... params)` | 分页查询 |
| `cn.hutool.db.AbstractDb` | `PageResult<Entity> page(Collection<String> fields,Entity where,Page page)` | 分页查询 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `PageResult<Entity> page(Collection<String> fields,Entity where,int pageNumber,int pageSize)` | 分页查询 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `PageResult<Entity> page(Entity where,Page page)` | 分页查询 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `PageResult<Entity> page(Entity where,int page,int numPerPage)` | 分页查询 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `PageResult<T> page(CharSequence sql,Page page,Class<T> elementBeanType,Object... params)` | 分页查询 |
| `cn.hutool.db.AbstractDb` | `SqlConnRunner getRunner()` | 获取SqlConnRunner |
| `cn.hutool.db.AbstractDb` | `String queryString(String sql,Object... params)` | 查询单条单个字段记录,并将其转换为String |
| `cn.hutool.db.AbstractDb` | `T find(Collection<String> fields,Entity where,RsHandler<T> rsh)` | 查询 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `T find(Entity where,RsHandler<T> rsh,String... fields)` | 查询，返回所有字段 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `T find(Query query,RsHandler<T> rsh)` | 查询 Query为查询所需数据的一个实体类，此对象中可以定义返回字段、查询条件，查询的表、分页等信息 |
| `cn.hutool.db.AbstractDb` | `T page(CharSequence sql,Page page,RsHandler<T> rsh,Object... params)` | 分页查询 |
| `cn.hutool.db.AbstractDb` | `T page(Collection<String> fields,Entity where,Page page,RsHandler<T> rsh)` | 分页查询 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `T page(Collection<String> fields,Entity where,int page,int numPerPage,RsHandler<T> rsh)` | 分页查询 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `T page(Entity where,Page page,RsHandler<T> rsh)` | 分页查询 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `T page(Entity where,int page,int numPerPage,RsHandler<T> rsh)` | 分页查询 查询条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `T page(SqlBuilder sql,Page page,RsHandler<T> rsh)` | 分页查询 |
| `cn.hutool.db.AbstractDb` | `T query(Func1<Connection, PreparedStatement> statementFunc,RsHandler<T> rsh)` | 执行自定义的PreparedStatement，结果使用RsHandler处理 此方法主要用于自定义场景，如游标查询等 |
| `cn.hutool.db.AbstractDb` | `T query(String sql,RsHandler<T> rsh,Map<String, Object> paramMap)` | 支持占位符的查询，例如：select * from table where field1=:name1 |
| `cn.hutool.db.AbstractDb` | `T query(String sql,RsHandler<T> rsh,Object... params)` | 查询 |
| `cn.hutool.db.AbstractDb` | `int del(Entity where)` | 删除数据 |
| `cn.hutool.db.AbstractDb` | `int del(String tableName,String field,Object value)` | 删除数据 |
| `cn.hutool.db.AbstractDb` | `int execute(String sql,Object... params)` | 执行非查询语句 语句包括 插入、更新、删除 |
| `cn.hutool.db.AbstractDb` | `int insert(Entity record)` | 插入数据 |
| `cn.hutool.db.AbstractDb` | `int insertOrUpdate(Entity record,String... keys)` | 插入或更新数据 根据给定的字段名查询数据，如果存在则更新这些数据，否则执行插入 |
| `cn.hutool.db.AbstractDb` | `int update(Entity record,Entity where)` | 更新数据 更新条件为多个key value对表示，默认key = value，如果使用其它条件可以使用：where.put("key", " > 1")，value也可以传Condition对象，key被忽略 |
| `cn.hutool.db.AbstractDb` | `int upsert(Entity record,String... keys)` | 使用upsert语义插入或更新数据 根据给定的字段名查询数据，如果存在则更新这些数据，否则执行插入 如果方言未实现本方法，内部会自动调用insertOrUpdate来实现功能，由于upsert和insert使用有区别，为了兼容性保留原有insertOrUpdate不做变动 |
| `cn.hutool.db.AbstractDb` | `int[] executeBatch(Iterable<String> sqls)` | 批量执行非查询语句 |
| `cn.hutool.db.AbstractDb` | `int[] executeBatch(String sql,Iterable<Object[]> paramsBatch)` | 批量执行非查询语句 |
| `cn.hutool.db.AbstractDb` | `int[] executeBatch(String sql,Object[]... paramsBatch)` | 批量执行非查询语句 |
| `cn.hutool.db.AbstractDb` | `int[] executeBatch(String... sqls)` | 批量执行非查询语句 |
| `cn.hutool.db.AbstractDb` | `int[] insert(Collection<Entity> records)` | 批量插入数据 需要注意的是，批量插入每一条数据结构必须一致。批量插入数据时会获取第一条数据的字段结构，之后的数据会按照这个格式插入。 也就是说假如第一条数据只有2个字段，后边数据多于这两个字段的部分将被抛弃。 |
| `cn.hutool.db.AbstractDb` | `long count(CharSequence selectSql,Object... params)` | 结果的条目数 |
| `cn.hutool.db.AbstractDb` | `long count(Entity where)` | 结果的条目数 |
| `cn.hutool.db.AbstractDb` | `long count(SqlBuilder sql)` | 结果的条目数 |
| `cn.hutool.db.AbstractDb` | `void closeConnection(Connection conn)` | 关闭连接 自定义关闭连接有利于自定义回收连接机制，或者不关闭 |
| `cn.hutool.db.AbstractDb` | `void setCaseInsensitive(boolean caseInsensitive)` | 设置是否在结果中忽略大小写 如果忽略，则在Entity中调用getXXX时，字段值忽略大小写，默认忽略 |
| `cn.hutool.db.AbstractDb` | `void setRunner(SqlConnRunner runner)` | 设置 SqlConnRunner |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity add()` | 根据Entity中现有字段条件从数据库中增加一条数据 |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity addFieldNames(String... fieldNames)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity clone()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity create()` | 创建ActiveEntity |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity create(String tableName)` | 创建ActiveEntity |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity del()` | 根据现有Entity中的条件删除与之匹配的数据库记录 |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity load()` | 根据Entity中现有字段条件从数据库中加载一个Entity对象 |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity parse(T bean)` | 将PO对象转为Entity |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity parse(T bean,boolean isToUnderlineCase,boolean ignoreNullValue)` | 将PO对象转为ActiveEntity |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity parseBean(T bean)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity parseBean(T bean,boolean isToUnderlineCase,boolean ignoreNullValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity parseWithUnderlineCase(T bean)` | 将PO对象转为ActiveEntity,并采用下划线法转换字段 |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity set(String field,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity setFieldNames(Collection<String> fieldNames)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity setFieldNames(String... fieldNames)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity setFields(Func0<?>... fields)` | 通过lambda批量设置值 |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity setIgnoreNull(String field,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity setTableName(String tableName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ActiveEntity` | `ActiveEntity update(String primaryKey)` | 根据现有Entity中的条件删除与之匹配的数据库记录 |
| `cn.hutool.db.DaoTemplate` | `Entity get(Entity where)` | 根据条件实体查询单个记录，当有多条返回时，只显示查询到的第一条 |
| `cn.hutool.db.DaoTemplate` | `Entity get(String field,T value)` | 根据某个字段（最好是唯一字段）查询单个记录 当有多条返回时，只显示查询到的第一条 |
| `cn.hutool.db.DaoTemplate` | `Entity get(T pk)` | 根据主键获取单个记录 |
| `cn.hutool.db.DaoTemplate` | `List<Entity> find(Entity where)` | 根据某个字段值查询结果 |
| `cn.hutool.db.DaoTemplate` | `List<Entity> find(String field,T value)` | 根据某个字段值查询结果 |
| `cn.hutool.db.DaoTemplate` | `List<Entity> findAll()` | 查询当前表的所有记录 |
| `cn.hutool.db.DaoTemplate` | `List<Entity> findBySql(String sql,Object... params)` | 根据SQL语句查询结果 SQL语句可以是非完整SQL语句，可以只提供查询的条件部分（例如WHERE部分） 此方法会自动补全SELECT * FROM [tableName] 部分，这样就无需关心表名，直接提供条件即可 |
| `cn.hutool.db.DaoTemplate` | `List<Object> addForGeneratedKeys(Entity entity)` | 添加 |
| `cn.hutool.db.DaoTemplate` | `Long addForGeneratedKey(Entity entity)` | 添加 |
| `cn.hutool.db.DaoTemplate` | `PageResult<Entity> page(Entity where,Page page)` | 分页 |
| `cn.hutool.db.DaoTemplate` | `PageResult<Entity> page(Entity where,Page page,String... selectFields)` | 分页 |
| `cn.hutool.db.DaoTemplate` | `boolean exist(Entity where)` | 指定条件的数据是否存在 |
| `cn.hutool.db.DaoTemplate` | `int add(Entity entity)` | 添加 |
| `cn.hutool.db.DaoTemplate` | `int addOrUpdate(Entity entity)` | 增加或者更新实体 |
| `cn.hutool.db.DaoTemplate` | `int del(Entity where)` | 删除 |
| `cn.hutool.db.DaoTemplate` | `int del(String field,T value)` | 删除 |
| `cn.hutool.db.DaoTemplate` | `int del(T pk)` | 删除 |
| `cn.hutool.db.DaoTemplate` | `int update(Entity entity)` | 更新 |
| `cn.hutool.db.DaoTemplate` | `int update(Entity record,Entity where)` | 按照条件更新 |
| `cn.hutool.db.DaoTemplate` | `long count(Entity where)` | 满足条件的数据条目数量 |
| `cn.hutool.db.Db` | `Connection getConnection()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Db` | `Db disableWrapper()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Db` | `Db setWrapper(Character wrapperChar)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Db` | `Db setWrapper(Wrapper wrapper)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Db` | `Db tx(TransactionLevel transactionLevel,VoidFunc1<Db> func)` | 执行事务 在同一事务中，所有对数据库操作都是原子的，同时提交或者同时回滚 |
| `cn.hutool.db.Db` | `Db tx(VoidFunc1<Db> func)` | 执行事务，使用默认的事务级别 在同一事务中，所有对数据库操作都是原子的，同时提交或者同时回滚 |
| `cn.hutool.db.Db` | `Db use()` | 创建Db 使用默认数据源，自动探测数据库连接池 |
| `cn.hutool.db.Db` | `Db use(DataSource ds)` | 创建Db 会根据数据源连接的元信息识别目标数据库类型，进而使用合适的数据源 |
| `cn.hutool.db.Db` | `Db use(DataSource ds,Dialect dialect)` | 创建Db |
| `cn.hutool.db.Db` | `Db use(DataSource ds,String driverClassName)` | 创建Db |
| `cn.hutool.db.Db` | `Db use(String group)` | 创建Db 使用默认数据源，自动探测数据库连接池 |
| `cn.hutool.db.Db` | `void closeConnection(Connection conn)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.DbUtil` | `DataSource getDs()` | 获得默认数据源 |
| `cn.hutool.db.DbUtil` | `DataSource getDs(String group)` | 获取指定分组的数据源 |
| `cn.hutool.db.DbUtil` | `DataSource getJndiDs(String jndiName)` | 获得JNDI数据源 |
| `cn.hutool.db.DbUtil` | `DataSource getJndiDsWithLog(String jndiName)` | 获得JNDI数据源 |
| `cn.hutool.db.DbUtil` | `Db use()` | 实例化一个新的Db，使用默认数据源 |
| `cn.hutool.db.DbUtil` | `Db use(DataSource ds)` | 实例化一个新的Db对象 |
| `cn.hutool.db.DbUtil` | `Db use(DataSource ds,Dialect dialect)` | 实例化一个新的SQL运行对象 |
| `cn.hutool.db.DbUtil` | `Session newSession()` | 新建数据库会话，使用默认数据源 |
| `cn.hutool.db.DbUtil` | `Session newSession(DataSource ds)` | 新建数据库会话 |
| `cn.hutool.db.DbUtil` | `SqlConnRunner newSqlConnRunner(Connection conn)` | 实例化一个新的SQL运行对象 |
| `cn.hutool.db.DbUtil` | `SqlConnRunner newSqlConnRunner(DataSource ds)` | 实例化一个新的SQL运行对象 |
| `cn.hutool.db.DbUtil` | `SqlConnRunner newSqlConnRunner(Dialect dialect)` | 实例化一个新的SQL运行对象 |
| `cn.hutool.db.DbUtil` | `void close(Object... objsToClose)` | 连续关闭一系列的SQL相关对象 这些对象必须按照顺序关闭，否则会出错。 |
| `cn.hutool.db.DbUtil` | `void removeShowSqlParams(Setting setting)` | 移除配置文件中的Show SQL相关配置项 此方法用于移除用户配置在分组下的配置项目 |
| `cn.hutool.db.DbUtil` | `void setCaseInsensitiveGlobal(boolean caseInsensitive)` | 设置全局是否在结果中忽略大小写 如果忽略，则在Entity中调用getXXX时，字段值忽略大小写，默认忽略 |
| `cn.hutool.db.DbUtil` | `void setDbSettingPathGlobal(String dbSettingPath)` | 自定义数据库配置文件路径（绝对路径或相对classpath路径） |
| `cn.hutool.db.DbUtil` | `void setReturnGeneratedKeyGlobal(boolean returnGeneratedKey)` | 设置全局是否INSERT语句中默认返回主键（默认返回主键） 如果false，则在Insert操作后，返回影响行数 主要用于某些数据库不支持返回主键的情况 |
| `cn.hutool.db.DbUtil` | `void setShowSqlGlobal(Setting setting)` | 从配置文件中读取SQL打印选项，读取后会去除相应属性 |
| `cn.hutool.db.DbUtil` | `void setShowSqlGlobal(boolean isShowSql,boolean isFormatSql,boolean isShowParams,Level level)` | 设置全局配置：是否通过debug日志显示SQL |
| `cn.hutool.db.DbUtil` | `void setStatementFetchSizeGlobal(Integer fetchSize)` | 设置构造结果集时每次从数据库取到的行数 |
| `cn.hutool.db.DialectRunner` | `Dialect getDialect()` | @return SQL方言 |
| `cn.hutool.db.DialectRunner` | `T find(Connection conn,Query query,RsHandler<T> rsh)` | 查询 此方法不会关闭Connection |
| `cn.hutool.db.DialectRunner` | `T insert(Connection conn,Entity record,RsHandler<T> generatedKeysHandler)` | 插入数据 此方法不会关闭Connection |
| `cn.hutool.db.DialectRunner` | `T page(Connection conn,Query query,RsHandler<T> rsh)` | 分页查询 此方法不会关闭Connection |
| `cn.hutool.db.DialectRunner` | `T page(Connection conn,SqlBuilder sqlBuilder,Page page,RsHandler<T> rsh)` | 分页查询 此方法不会关闭Connection |
| `cn.hutool.db.DialectRunner` | `int del(Connection conn,Entity where)` | 删除数据 此方法不会关闭Connection |
| `cn.hutool.db.DialectRunner` | `int insertOrUpdate(Connection conn,Entity record,String... keys)` | 插入或更新数据 此方法不会关闭Connection |
| `cn.hutool.db.DialectRunner` | `int update(Connection conn,Entity record,Entity where)` | 更新数据 此方法不会关闭Connection |
| `cn.hutool.db.DialectRunner` | `int upsert(Connection conn,Entity record,String... keys)` | 更新或插入数据 此方法不会关闭Connection 如果方言未实现此方法则内部自动使用insertOrUpdate来替代功能 |
| `cn.hutool.db.DialectRunner` | `int[] insert(Connection conn,Entity... records)` | 批量插入数据 批量插入必须严格保持Entity的结构一致，不一致会导致插入数据出现不可预知的结果 此方法不会关闭Connection |
| `cn.hutool.db.DialectRunner` | `long count(Connection conn,Entity where)` | 获取结果总数，生成类似于select count(1) from XXX wher XXX=? and YYY=? |
| `cn.hutool.db.DialectRunner` | `long count(Connection conn,SqlBuilder sqlBuilder)` | 获取查询结果总数，生成类似于 SELECT count(1) from (sql) hutool_alias_count_ 此方法会重新构建SqlBuilder，并去除末尾的order by子句 |
| `cn.hutool.db.DialectRunner` | `void setCaseInsensitive(boolean caseInsensitive)` | 设置是否在结果中忽略大小写 如果忽略，则在Entity中调用getXXX时，字段值忽略大小写，默认忽略 |
| `cn.hutool.db.DialectRunner` | `void setDialect(Dialect dialect)` | 设置SQL方言 |
| `cn.hutool.db.DialectRunner` | `void setWrapper(Character wrapperChar)` | 设置包装器，包装器用于对表名、字段名进行符号包装（例如双引号），防止关键字与这些表名或字段冲突 |
| `cn.hutool.db.DialectRunner` | `void setWrapper(Wrapper wrapper)` | 设置包装器，包装器用于对表名、字段名进行符号包装（例如双引号），防止关键字与这些表名或字段冲突 |
| `cn.hutool.db.Entity` | `Blob getBlob(String field)` | 获得Blob类型结果 |
| `cn.hutool.db.Entity` | `Clob getClob(String field)` | 获得Clob类型结果 |
| `cn.hutool.db.Entity` | `Date getDate(String field)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Entity` | `Entity addCondition(final Condition condition)` | 添加条件 |
| `cn.hutool.db.Entity` | `Entity addFieldNames(String... fieldNames)` | 添加字段列表 |
| `cn.hutool.db.Entity` | `Entity clone()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Entity` | `Entity create()` | 创建Entity |
| `cn.hutool.db.Entity` | `Entity create(String tableName)` | 创建Entity |
| `cn.hutool.db.Entity` | `Entity filter(String... keys)` | 过滤Map保留指定键值对，如果键不存在跳过 |
| `cn.hutool.db.Entity` | `Entity parse(T bean)` | 将PO对象转为Entity |
| `cn.hutool.db.Entity` | `Entity parse(T bean,boolean isToUnderlineCase,boolean ignoreNullValue)` | 将PO对象转为Entity |
| `cn.hutool.db.Entity` | `Entity parseBean(T bean)` | 将值对象转换为Entity 类名会被当作表名，小写第一个字母 |
| `cn.hutool.db.Entity` | `Entity parseBean(T bean,boolean isToUnderlineCase,boolean ignoreNullValue)` | 将值对象转换为Entity 类名会被当作表名，小写第一个字母 |
| `cn.hutool.db.Entity` | `Entity parseWithUnderlineCase(T bean)` | 将PO对象转为Entity,并采用下划线法转换字段 |
| `cn.hutool.db.Entity` | `Entity removeNew(final String... keys)` | 过滤Map去除指定键值对，如果键不存在跳过 |
| `cn.hutool.db.Entity` | `Entity set(String field,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Entity` | `Entity setFieldNames(Collection<String> fieldNames)` | 设置字段列表，用于限制加入的字段的值 |
| `cn.hutool.db.Entity` | `Entity setFieldNames(String... fieldNames)` | 设置字段列表，用于限制加入的字段的值 |
| `cn.hutool.db.Entity` | `Entity setFields(Func0<?>... fields)` | 通过lambda批量设置值 |
| `cn.hutool.db.Entity` | `Entity setIgnoreNull(String field,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Entity` | `Entity setTableName(String tableName)` | 设置表名 |
| `cn.hutool.db.Entity` | `RowId getRowId()` | 获得rowid |
| `cn.hutool.db.Entity` | `RowId getRowId(String field)` | 获得rowid |
| `cn.hutool.db.Entity` | `Set<String> getFieldNames()` | @return 字段集合 |
| `cn.hutool.db.Entity` | `String getStr(String field)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Entity` | `String getStr(String field,Charset charset)` | 获得字符串值 支持Clob、Blob、RowId |
| `cn.hutool.db.Entity` | `String getTableName()` | @return 获得表名 |
| `cn.hutool.db.Entity` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Entity` | `Time getTime(String field)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Entity` | `Timestamp getTimestamp(String field)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.GlobalDbConfig` | `Setting createDbSetting()` | 获取自定义或默认位置数据库配置Setting |
| `cn.hutool.db.GlobalDbConfig` | `void setCaseInsensitive(boolean isCaseInsensitive)` | 设置全局是否在结果中忽略大小写 如果忽略，则在Entity中调用getXXX时，字段值忽略大小写，默认忽略 |
| `cn.hutool.db.GlobalDbConfig` | `void setDbSettingPath(String customDbSettingPath)` | 自定义数据库配置文件路径（绝对路径或相对classpath路径） |
| `cn.hutool.db.GlobalDbConfig` | `void setReturnGeneratedKey(boolean isReturnGeneratedKey)` | 设置全局是否INSERT语句中默认返回主键（默认返回主键） 如果false，则在Insert操作后，返回影响行数 主要用于某些数据库不支持返回主键的情况 |
| `cn.hutool.db.GlobalDbConfig` | `void setShowSql(boolean isShowSql,boolean isFormatSql,boolean isShowParams,Level level)` | 设置全局配置：是否通过debug日志显示SQL |
| `cn.hutool.db.GlobalDbConfig` | `void setStatementFetchSize(Integer statementFetchSize)` | 设置构造结果集时每次从数据库取到的行数 |
| `cn.hutool.db.Page` | `Integer getEndIndex()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Page` | `Integer getStartIndex()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Page` | `Order[] getOrders()` | @return 排序 |
| `cn.hutool.db.Page` | `Page of(int pageNumber,int pageSize)` | 创建Page对象 |
| `cn.hutool.db.Page` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Page` | `int getEndPosition()` | @return 结束位置 |
| `cn.hutool.db.Page` | `int getPageNumber()` | @return 页码，0表示第一页 |
| `cn.hutool.db.Page` | `int getPageSize()` | @return 每页结果数 |
| `cn.hutool.db.Page` | `int getStartPosition()` | @return 开始位置 |
| `cn.hutool.db.Page` | `int[] getStartEnd()` | 开始位置和结束位置 例如： |
| `cn.hutool.db.Page` | `void addOrder(Order... orders)` | 设置排序 |
| `cn.hutool.db.Page` | `void setOrder(Order... orders)` | 设置排序 |
| `cn.hutool.db.Page` | `void setPageNumber(int pageNumber)` | 设置页码，0表示第一页 |
| `cn.hutool.db.Page` | `void setPageSize(int pageSize)` | 设置每页结果数 |
| `cn.hutool.db.PageResult` | `boolean isFirst()` | @return 是否第一页 |
| `cn.hutool.db.PageResult` | `boolean isLast()` | @return 是否最后一页 |
| `cn.hutool.db.PageResult` | `int getPage()` | 页码，0表示第一页 |
| `cn.hutool.db.PageResult` | `int getPageSize()` | @return 每页结果数 |
| `cn.hutool.db.PageResult` | `int getTotal()` | @return 总数 |
| `cn.hutool.db.PageResult` | `int getTotalPage()` | @return 总页数 |
| `cn.hutool.db.PageResult` | `void setPage(int page)` | 设置页码，0表示第一页 |
| `cn.hutool.db.PageResult` | `void setPageSize(int pageSize)` | 设置每页结果数 |
| `cn.hutool.db.PageResult` | `void setTotal(int total)` | 设置总数 |
| `cn.hutool.db.PageResult` | `void setTotalPage(int totalPage)` | 设置总页数 |
| `cn.hutool.db.Session` | `Connection getConnection()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Session` | `Savepoint setSavepoint()` | 设置保存点 |
| `cn.hutool.db.Session` | `Savepoint setSavepoint(String name)` | 设置保存点 |
| `cn.hutool.db.Session` | `Session create()` | 创建默认数据源会话 |
| `cn.hutool.db.Session` | `Session create(DataSource ds)` | 创建会话 |
| `cn.hutool.db.Session` | `Session create(String group)` | 创建会话 |
| `cn.hutool.db.Session` | `Session disableWrapper()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Session` | `Session setWrapper(Character wrapperChar)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Session` | `Session setWrapper(Wrapper wrapper)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Session` | `SqlConnRunner getRunner()` | 获得SqlConnRunner |
| `cn.hutool.db.Session` | `void beginTransaction()` | 开始事务 |
| `cn.hutool.db.Session` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Session` | `void closeConnection(Connection conn)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.Session` | `void commit()` | 提交事务 |
| `cn.hutool.db.Session` | `void quietRollback()` | 静默回滚事务 回滚事务 |
| `cn.hutool.db.Session` | `void quietRollback(Savepoint savepoint)` | 静默回滚到某个保存点，保存点的设置请使用setSavepoint方法 |
| `cn.hutool.db.Session` | `void rollback()` | 回滚事务 |
| `cn.hutool.db.Session` | `void rollback(Savepoint savepoint)` | 回滚到某个保存点，保存点的设置请使用setSavepoint方法 |
| `cn.hutool.db.Session` | `void setTransactionIsolation(int level)` | 设置事务的隔离级别 Connection.TRANSACTION_NONE 驱动不支持事务 Connection.TRANSACTION_READ_UNCOMMITTED 允许脏读、不可重复读和幻读 Connection.TRANSACTION_READ_COMMITTED 禁止脏读，但允许不可重复读和幻读 Connection.TRANSACTION_REPEATABLE_READ 禁止脏读和不可重复读，单运行幻读 Connection.TRANSACTION_SERIALIZABLE 禁止脏读、不可重复读和幻读 |
| `cn.hutool.db.Session` | `void tx(VoidFunc1<Session> func)` | 在事务中执行操作，通过实现VoidFunc1接口的call方法执行多条SQL语句从而完成事务 |
| `cn.hutool.db.SqlConnRunner` | `List<Entity> find(Connection conn,Entity where)` | 查询数据列表，返回字段在where参数中定义 |
| `cn.hutool.db.SqlConnRunner` | `List<Entity> findAll(Connection conn,Entity where)` | 查询数据列表，返回所有字段 |
| `cn.hutool.db.SqlConnRunner` | `List<Entity> findAll(Connection conn,String tableName)` | 查询数据列表，返回所有字段 |
| `cn.hutool.db.SqlConnRunner` | `List<Entity> findBy(Connection conn,String tableName,String field,Object value)` | 根据某个字段名条件查询数据列表，返回所有字段 |
| `cn.hutool.db.SqlConnRunner` | `List<Entity> findIn(Connection conn,String tableName,String field,Object... values)` | 根据某个字段名条件查询数据列表，返回所有字段 |
| `cn.hutool.db.SqlConnRunner` | `List<Entity> findLike(Connection conn,String tableName,String field,String value,LikeType likeType)` | 根据某个字段名条件查询数据列表，返回所有字段 |
| `cn.hutool.db.SqlConnRunner` | `List<Object> insertForGeneratedKeys(Connection conn,Entity record)` | 插入数据 此方法不会关闭Connection |
| `cn.hutool.db.SqlConnRunner` | `Long insertForGeneratedKey(Connection conn,Entity record)` | 插入数据 此方法不会关闭Connection |
| `cn.hutool.db.SqlConnRunner` | `PageResult<Entity> page(Connection conn,Collection<String> fields,Entity where,Page page)` | 分页查询 此方法不会关闭Connection |
| `cn.hutool.db.SqlConnRunner` | `PageResult<Entity> page(Connection conn,Collection<String> fields,Entity where,int page,int numPerPage)` | 分页查询 此方法不会关闭Connection |
| `cn.hutool.db.SqlConnRunner` | `PageResult<Entity> page(Connection conn,Entity where,Page page)` | 分页全字段查询 此方法不会关闭Connection |
| `cn.hutool.db.SqlConnRunner` | `PageResult<Entity> page(Connection conn,SqlBuilder sqlBuilder,Page page)` | 分页查询 此方法不会关闭Connection |
| `cn.hutool.db.SqlConnRunner` | `SqlConnRunner create(DataSource ds)` | 实例化一个新的SQL运行对象 |
| `cn.hutool.db.SqlConnRunner` | `SqlConnRunner create(Dialect dialect)` | 实例化一个新的SQL运行对象 |
| `cn.hutool.db.SqlConnRunner` | `SqlConnRunner create(String driverClassName)` | 实例化一个新的SQL运行对象 |
| `cn.hutool.db.SqlConnRunner` | `T find(Connection conn,Collection<String> fields,Entity where,RsHandler<T> rsh)` | 查询 此方法不会关闭Connection |
| `cn.hutool.db.SqlConnRunner` | `T find(Connection conn,Entity where,RsHandler<T> rsh,String... fields)` | 查询，返回指定字段列表 此方法不会关闭Connection |
| `cn.hutool.db.SqlConnRunner` | `T page(Connection conn,Collection<String> fields,Entity where,Page page,RsHandler<T> handler)` | 分页查询 此方法不会关闭Connection |
| `cn.hutool.db.SqlConnRunner` | `T page(Connection conn,Collection<String> fields,Entity where,int pageNumber,int numPerPage,RsHandler<T> rsh)` | 分页查询 此方法不会关闭Connection |
| `cn.hutool.db.SqlConnRunner` | `int insert(Connection conn,Entity record)` | 插入数据 此方法不会关闭Connection |
| `cn.hutool.db.SqlConnRunner` | `int[] insert(Connection conn,Collection<Entity> records)` | 批量插入数据 需要注意的是，批量插入每一条数据结构必须一致。批量插入数据时会获取第一条数据的字段结构，之后的数据会按照这个格式插入。 也就是说假如第一条数据只有2个字段，后边数据多于这两个字段的部分将被抛弃。 此方法不会关闭Connection |
| `cn.hutool.db.SqlConnRunner` | `long count(Connection conn,CharSequence selectSql,Object... params)` | 获取查询结果总数，生成类似于 SELECT count(1) from (sql) as _count |
| `cn.hutool.db.StatementUtil` | `CallableStatement prepareCall(Connection conn,String sql,Object... params)` | 创建CallableStatement |
| `cn.hutool.db.StatementUtil` | `List<Object> getGeneratedKeys(Statement ps)` | 获得所有主键 |
| `cn.hutool.db.StatementUtil` | `Long getGeneratedKeyOfLong(Statement ps)` | 获得自增键的值 此方法对于Oracle无效（返回null） |
| `cn.hutool.db.StatementUtil` | `PreparedStatement fillParams(PreparedStatement ps,Iterable<?> params)` | 填充SQL的参数。 对于日期对象特殊处理：传入java.util.Date默认按照Timestamp处理 |
| `cn.hutool.db.StatementUtil` | `PreparedStatement fillParams(PreparedStatement ps,Iterable<?> params,Map<Integer, Integer> nullTypeCache)` | 填充SQL的参数。 对于日期对象特殊处理：传入java.util.Date默认按照Timestamp处理 |
| `cn.hutool.db.StatementUtil` | `PreparedStatement fillParams(PreparedStatement ps,Object... params)` | 填充SQL的参数。 |
| `cn.hutool.db.StatementUtil` | `PreparedStatement prepareStatement(Connection conn,SqlBuilder sqlBuilder)` | 创建PreparedStatement |
| `cn.hutool.db.StatementUtil` | `PreparedStatement prepareStatement(Connection conn,String sql,Collection<Object> params)` | 创建PreparedStatement |
| `cn.hutool.db.StatementUtil` | `PreparedStatement prepareStatement(Connection conn,String sql,Object... params)` | 创建PreparedStatement |
| `cn.hutool.db.StatementUtil` | `PreparedStatement prepareStatement(boolean returnGeneratedKey,Connection conn,String sql,Object... params)` | 创建PreparedStatement |
| `cn.hutool.db.StatementUtil` | `PreparedStatement prepareStatementForBatch(Connection conn,String sql,Iterable<Object[]> paramsBatch)` | 创建批量操作的PreparedStatement |
| `cn.hutool.db.StatementUtil` | `PreparedStatement prepareStatementForBatch(Connection conn,String sql,Iterable<String> fields,Entity... entities)` | 创建批量操作的PreparedStatement |
| `cn.hutool.db.StatementUtil` | `PreparedStatement prepareStatementForBatch(Connection conn,String sql,Object[]... paramsBatch)` | 创建批量操作的PreparedStatement |
| `cn.hutool.db.StatementUtil` | `T getGeneratedKeys(Statement statement,RsHandler<T> rsHandler)` | 获取主键，并使用RsHandler 处理后返回 |
| `cn.hutool.db.StatementUtil` | `int getTypeOfNull(PreparedStatement ps,int paramIndex)` | 获取null字段对应位置的数据类型 有些数据库对于null字段必须指定类型，否则会插入报错，此方法用于获取其类型，如果获取失败，使用默认的Types#VARCHAR |
| `cn.hutool.db.StatementUtil` | `void setParam(PreparedStatement ps,int paramIndex,Object param)` | 为PreparedStatement 设置单个参数 |
| `cn.hutool.db.ThreadLocalConnection` | `Connection get(DataSource ds)` | 获取数据源对应的数据库连接 |
| `cn.hutool.db.ThreadLocalConnection` | `void close(DataSource ds)` | 关闭数据库，并从线程池中移除 |
| `cn.hutool.db.ThreadLocalConnection$GroupedConnection` | `Connection get(DataSource ds)` | 获取连接，如果获取的连接为空或者已被关闭，重新创建连接 |
| `cn.hutool.db.ThreadLocalConnection$GroupedConnection` | `GroupedConnection close(DataSource ds)` | 关闭并移除Connection 如果处于事务中，则不进行任何操作 |
| `cn.hutool.db.ThreadLocalConnection$GroupedConnection` | `boolean isEmpty()` | 持有的连接是否为空 |
