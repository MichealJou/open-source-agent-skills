# com.baomidou.mybatisplus.extension.plugins.pagination

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.plugins.pagination.DialectFactory` | `IDialect getDialect(DbType dbType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel` | `DialectModel setConsumer(boolean isFirstParam)` | 设置消费 List 的方式 不带下标的 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel` | `DialectModel setConsumer(boolean isFirstParam,Function<List<ParameterMapping>, Integer> function)` | 设置消费 List 的方式 带下标的 mark: 标记一下,暂时没看到哪个数据库的分页方言会存在使用该方法 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel` | `DialectModel setConsumerChain()` | 设置消费 List 的方式 不带下标的,两个值都有 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel` | `void consumers(List<ParameterMapping> parameterMappings,Configuration configuration,Map<String, Object> additionalParameters)` | 把内部所有需要消费的都消费掉 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `List<OrderItem> orders()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `List<T> getRecords()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `Long maxLimit()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `Page<T> addOrder(List<OrderItem> items)` | 添加新的排序条件，构造条件可以使用工厂：OrderItem#build(String, boolean) |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `Page<T> addOrder(OrderItem... items)` | 添加新的排序条件，构造条件可以使用工厂：OrderItem#build(String, boolean) |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `Page<T> of(long current,long size)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `Page<T> of(long current,long size,boolean searchCount)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `Page<T> of(long current,long size,long total)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `Page<T> of(long current,long size,long total,boolean searchCount)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `Page<T> setCurrent(long current)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `Page<T> setOptimizeCountSql(boolean optimizeCountSql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `Page<T> setRecords(List<T> records)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `Page<T> setSearchCount(boolean searchCount)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `Page<T> setSize(long size)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `Page<T> setTotal(long total)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `String countId()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `boolean hasNext()` | 是否存在下一页 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `boolean hasPrevious()` | 是否存在上一页 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `boolean optimizeCountSql()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `boolean optimizeJoinOfCountSql()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `boolean searchCount()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `long getCurrent()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `long getPages()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `long getSize()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.Page` | `long getTotal()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO` | `List<OrderItem> getOrders()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO` | `Long getMaxLimit()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO` | `Page<T> of(long current,long size)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO` | `Page<T> of(long current,long size,boolean searchCount)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO` | `Page<T> of(long current,long size,long total)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO` | `Page<T> of(long current,long size,long total,boolean searchCount)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO` | `String getCountId()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO` | `boolean isOptimizeCountSql()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO` | `boolean isOptimizeJoinOfCountSql()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO` | `boolean isSearchCount()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
