# cn.hutool.db.dialect

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.db.dialect.Dialect` | `PreparedStatement psForCount(Connection conn,Query query)` | 构建用于查询行数的PreparedStatement 用户实现需按照数据库方言格式，将Query转换为带有占位符的SQL语句及参数列表 Query中包含了表名、查询条件等信息，可借助SqlBuilder完成SQL语句生成。 |
| `cn.hutool.db.dialect.Dialect` | `PreparedStatement psForCount(Connection conn,SqlBuilder sqlBuilder)` | 构建用于查询行数的PreparedStatement 用户实现需按照数据库方言格式，将Query转换为带有占位符的SQL语句及参数列表 Query中包含了表名、查询条件等信息，可借助SqlBuilder完成SQL语句生成。 |
| `cn.hutool.db.dialect.Dialect` | `PreparedStatement psForDelete(Connection conn,Query query)` | 构建用于删除的PreparedStatement 用户实现需按照数据库方言格式，将Query转换为带有占位符的SQL语句及参数列表 Query中包含了删除所需的表名、查询条件等信息，可借助SqlBuilder完成SQL语句生成。 |
| `cn.hutool.db.dialect.Dialect` | `PreparedStatement psForFind(Connection conn,Query query)` | 构建用于获取多条记录的PreparedStatement 用户实现需按照数据库方言格式，将Query转换为带有占位符的SQL语句及参数列表 Query中包含了查询所需的表名、查询条件等信息，可借助SqlBuilder完成SQL语句生成。 |
| `cn.hutool.db.dialect.Dialect` | `PreparedStatement psForInsert(Connection conn,Entity entity)` | 构建用于插入的PreparedStatement 用户实现需按照数据库方言格式，将Entity转换为带有占位符的SQL语句及参数列表 |
| `cn.hutool.db.dialect.Dialect` | `PreparedStatement psForInsertBatch(Connection conn,Entity... entities)` | 构建用于批量插入的PreparedStatement 用户实现需按照数据库方言格式，将Entity转换为带有占位符的SQL语句及参数列表 |
| `cn.hutool.db.dialect.Dialect` | `PreparedStatement psForPage(Connection conn,Query query)` | 构建用于分页查询的PreparedStatement 用户实现需按照数据库方言格式，将Query转换为带有占位符的SQL语句及参数列表 Query中包含了分页查询所需的表名、查询条件、分页等信息，可借助SqlBuilder完成SQL语句生成。 |
| `cn.hutool.db.dialect.Dialect` | `PreparedStatement psForPage(Connection conn,SqlBuilder sqlBuilder,Page page)` | 构建用于分页查询的PreparedStatement 可以在此方法中使用SqlBuilder#orderBy(Order...)方法加入排序信息， 排序信息通过Page#getOrders()获取 |
| `cn.hutool.db.dialect.Dialect` | `PreparedStatement psForUpdate(Connection conn,Entity entity,Query query)` | 构建用于更新的PreparedStatement 用户实现需按照数据库方言格式，将Entity配合Query转换为带有占位符的SQL语句及参数列表 其中Entity中包含需要更新的数据信息，Query包含更新的查找条件信息。 |
| `cn.hutool.db.dialect.Dialect` | `PreparedStatement psForUpsert(Connection conn,Entity entity,String... keys)` | 构建用于upsert的PreparedStatement 方言实现需实现此默认方法，如果没有实现，抛出SQLException |
| `cn.hutool.db.dialect.Dialect` | `String dialectName()` | 方言名 |
| `cn.hutool.db.dialect.Dialect` | `Wrapper getWrapper()` | @return 包装器 |
| `cn.hutool.db.dialect.Dialect` | `void setWrapper(Wrapper wrapper)` | 设置包装器 |
| `cn.hutool.db.dialect.DialectFactory` | `Dialect getDialect(DataSource ds)` | 获取共享方言 |
| `cn.hutool.db.dialect.DialectFactory` | `Dialect newDialect(Connection conn)` | 创建方言 |
| `cn.hutool.db.dialect.DialectFactory` | `Dialect newDialect(DataSource ds)` | 创建方言 |
| `cn.hutool.db.dialect.DialectFactory` | `Dialect newDialect(String driverName)` | 根据驱动名创建方言 驱动名是不分区大小写完全匹配的 |
| `cn.hutool.db.dialect.DialectFactory` | `String identifyDriver(String nameContainsProductInfo)` | 通过JDBC URL等信息识别JDBC驱动名 |
| `cn.hutool.db.dialect.DialectFactory` | `String identifyDriver(String nameContainsProductInfo,ClassLoader classLoader)` | 通过JDBC URL等信息识别JDBC驱动名 |
| `cn.hutool.db.dialect.DialectName` | `boolean match(String dialectName)` | 是否为指定数据库方言，检查时不分区大小写 |
| `cn.hutool.db.dialect.DriverUtil` | `String identifyDriver(Connection conn)` | 识别JDBC驱动名 |
| `cn.hutool.db.dialect.DriverUtil` | `String identifyDriver(DataSource ds)` | 识别JDBC驱动名 |
| `cn.hutool.db.dialect.DriverUtil` | `String identifyDriver(String nameContainsProductInfo)` | 通过JDBC URL等信息识别JDBC驱动名 |
