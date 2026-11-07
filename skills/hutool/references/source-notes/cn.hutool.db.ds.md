# cn.hutool.db.ds

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.db.ds.AbstractDSFactory` | `DataSource getDataSource(String group)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.AbstractDSFactory` | `Setting getSetting()` | 获取配置，用于自定义添加配置项 |
| `cn.hutool.db.ds.AbstractDSFactory` | `boolean equals(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.AbstractDSFactory` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.AbstractDSFactory` | `void close(String group)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.AbstractDSFactory` | `void destroy()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.DSFactory` | `DSFactory create(Setting setting)` | 创建数据源实现工厂 此方法通过“试错”方式查找引入项目的连接池库，按照优先级寻找，一旦寻找到则创建对应的数据源工厂 连接池优先级：Hikari > Druid > Tomcat > Dbcp > C3p0 > Hutool Pooled |
| `cn.hutool.db.ds.DSFactory` | `DSFactory setCurrentDSFactory(DSFactory dsFactory)` | 设置全局的数据源工厂 在项目中存在多个连接池库的情况下，我们希望使用低优先级的库时使用此方法自定义之 重新定义全局的数据源工厂此方法可在以下两种情况下调用： |
| `cn.hutool.db.ds.DSFactory` | `DataSource get()` | 获得数据源 使用默认配置文件的无分组配置 |
| `cn.hutool.db.ds.DSFactory` | `DataSource get(String group)` | 获得数据源 |
| `cn.hutool.db.ds.DSFactory` | `DataSource getDataSource()` | 获得默认数据源 |
| `cn.hutool.db.ds.DSFactory` | `DataSource getDataSource(String group)` | 获得分组对应数据源 |
| `cn.hutool.db.ds.DSFactory` | `void close()` | 关闭默认数据源（空组） |
| `cn.hutool.db.ds.DSFactory` | `void close(String group)` | 关闭对应数据源 |
| `cn.hutool.db.ds.DSFactory` | `void destroy()` | 销毁工厂类，关闭所有数据源 |
| `cn.hutool.db.ds.DataSourceWrapper` | `Connection getConnection()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.DataSourceWrapper` | `Connection getConnection(String username,String password)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.DataSourceWrapper` | `DataSource getRaw()` | 获取原始的数据源 |
| `cn.hutool.db.ds.DataSourceWrapper` | `DataSourceWrapper clone()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.DataSourceWrapper` | `DataSourceWrapper wrap(DataSource ds,String driver)` | 包装指定的DataSource |
| `cn.hutool.db.ds.DataSourceWrapper` | `Logger getParentLogger()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.DataSourceWrapper` | `PrintWriter getLogWriter()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.DataSourceWrapper` | `String getDriver()` | 获取驱动名 |
| `cn.hutool.db.ds.DataSourceWrapper` | `T unwrap(Class<T> iface)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.DataSourceWrapper` | `boolean isWrapperFor(Class<?> iface)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.DataSourceWrapper` | `int getLoginTimeout()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.DataSourceWrapper` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.DataSourceWrapper` | `void setLogWriter(PrintWriter out)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.DataSourceWrapper` | `void setLoginTimeout(int seconds)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.db.ds.GlobalDSFactory` | `DSFactory get()` | 获取默认的数据源工厂，读取默认数据库配置文件 此处使用懒加载模式，在第一次调用此方法时才创建默认数据源工厂 如果想自定义全局的数据源工厂，请在第一次调用此方法前调用#set(DSFactory) 方法自行定义 |
| `cn.hutool.db.ds.GlobalDSFactory` | `DSFactory set(DSFactory customDSFactory)` | 设置全局的数据源工厂 在项目中存在多个连接池库的情况下，我们希望使用低优先级的库时使用此方法自定义之 重新定义全局的数据源工厂此方法可在以下两种情况下调用： |
