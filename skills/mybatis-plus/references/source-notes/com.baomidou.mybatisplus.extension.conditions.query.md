# com.baomidou.mybatisplus.extension.conditions.query

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.conditions.query.ChainQuery` | `E page(E page)` | 获取分页数据 |
| `com.baomidou.mybatisplus.extension.conditions.query.ChainQuery` | `List<T> list()` | 获取集合 |
| `com.baomidou.mybatisplus.extension.conditions.query.ChainQuery` | `List<T> list(IPage<T> page)` | 获取集合 |
| `com.baomidou.mybatisplus.extension.conditions.query.ChainQuery` | `Long count()` | 获取 count |
| `com.baomidou.mybatisplus.extension.conditions.query.ChainQuery` | `Optional<T> oneOpt()` | 获取单个 |
| `com.baomidou.mybatisplus.extension.conditions.query.ChainQuery` | `T one()` | 获取单个 |
| `com.baomidou.mybatisplus.extension.conditions.query.ChainQuery` | `boolean exists()` | 判断数据是否存在 |
| `com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper` | `BaseMapper<T> getBaseMapper()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper` | `Class<T> getEntityClass()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper` | `LambdaQueryChainWrapper<T> select(Class<T> entityClass,Predicate<TableFieldInfo> predicate)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper` | `LambdaQueryChainWrapper<T> select(SFunction<T, ?>... columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper` | `LambdaQueryChainWrapper<T> select(boolean condition,List<SFunction<T, ?>> columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper` | `LambdaQueryChainWrapper<T> select(boolean condition,SFunction<T, ?>... columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.query.LambdaQueryChainWrapper` | `String getSqlSelect()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper` | `BaseMapper<T> getBaseMapper()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper` | `Class<T> getEntityClass()` | 获取当前实体Class |
| `com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper` | `LambdaQueryChainWrapper<T> lambda()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper` | `QueryChainWrapper<T> select(Class<T> entityClass,Predicate<TableFieldInfo> predicate)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper` | `QueryChainWrapper<T> select(boolean condition,List<String> columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.query.QueryChainWrapper` | `String getSqlSelect()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
