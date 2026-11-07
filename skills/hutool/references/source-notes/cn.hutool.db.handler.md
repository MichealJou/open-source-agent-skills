# cn.hutool.db.handler

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.db.handler.BeanHandler` | `BeanHandler<E> create(Class<E> beanType)` | 创建一个 BeanHandler对象 |
| `cn.hutool.db.handler.BeanHandler` | `E handle(ResultSet rs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.handler.BeanListHandler` | `BeanListHandler<E> create(Class<E> beanType)` | 创建一个 BeanListHandler对象 |
| `cn.hutool.db.handler.BeanListHandler` | `List<E> handle(ResultSet rs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.handler.EntityHandler` | `Entity handle(ResultSet rs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.handler.EntityHandler` | `EntityHandler create()` | 创建一个 EntityHandler对象 |
| `cn.hutool.db.handler.EntityListHandler` | `EntityListHandler create()` | 创建一个 EntityListHandler对象 |
| `cn.hutool.db.handler.EntityListHandler` | `List<Entity> handle(ResultSet rs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.handler.EntitySetHandler` | `EntitySetHandler create()` | 创建一个 EntityHandler对象 |
| `cn.hutool.db.handler.EntitySetHandler` | `LinkedHashSet<Entity> handle(ResultSet rs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.handler.HandleHelper` | `Entity handleRow(ResultSet rs)` | 处理单条数据 |
| `cn.hutool.db.handler.HandleHelper` | `Entity handleRow(int columnCount,ResultSetMetaData meta,ResultSet rs)` | 处理单条数据 |
| `cn.hutool.db.handler.HandleHelper` | `Entity handleRow(int columnCount,ResultSetMetaData meta,ResultSet rs,boolean caseInsensitive)` | 处理单条数据 |
| `cn.hutool.db.handler.HandleHelper` | `List<Object> handleRowToList(ResultSet rs)` | 处理单行数据 |
| `cn.hutool.db.handler.HandleHelper` | `T handleRow(T row,int columnCount,ResultSetMetaData meta,ResultSet rs,boolean withMetaInfo)` | 处理单条数据 |
| `cn.hutool.db.handler.HandleHelper` | `T handleRow(int columnCount,ResultSetMetaData meta,ResultSet rs,Class<T> beanClass)` | 处理单条数据 |
| `cn.hutool.db.handler.HandleHelper` | `T handleRow(int columnCount,ResultSetMetaData meta,ResultSet rs,T bean)` | 处理单条数据 |
| `cn.hutool.db.handler.HandleHelper` | `T handleRs(ResultSet rs,T collection)` | 处理多条数据 |
| `cn.hutool.db.handler.HandleHelper` | `T handleRs(ResultSet rs,T collection,boolean caseInsensitive)` | 处理多条数据 |
| `cn.hutool.db.handler.HandleHelper` | `T handleRsToBeanList(ResultSet rs,T collection,Class<E> elementBeanType)` | 处理多条数据并返回一个Bean列表 |
| `cn.hutool.db.handler.NumberHandler` | `Number handle(ResultSet rs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.handler.NumberHandler` | `NumberHandler create()` | 创建一个 NumberHandler对象 |
| `cn.hutool.db.handler.PageResultHandler` | `PageResult<Entity> handle(ResultSet rs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.handler.PageResultHandler` | `PageResultHandler create(PageResult<Entity> pageResult)` | 创建一个 EntityHandler对象 结果集根据给定的分页对象查询数据库，填充结果 |
| `cn.hutool.db.handler.RsHandler` | `T handle(ResultSet rs)` | 处理结果集 结果集处理后不需要关闭 |
| `cn.hutool.db.handler.StringHandler` | `String handle(ResultSet rs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.handler.StringHandler` | `StringHandler create()` | 创建一个 NumberHandler对象 |
| `cn.hutool.db.handler.ValueListHandler` | `List<List<Object>> handle(ResultSet rs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.handler.ValueListHandler` | `ValueListHandler create()` | 创建一个 EntityListHandler对象 |
