# com.baomidou.mybatisplus.extension.conditions.update

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.conditions.update.ChainUpdate` | `boolean remove()` | 删除数据 |
| `com.baomidou.mybatisplus.extension.conditions.update.ChainUpdate` | `boolean update()` | 更新数据 此方法无法进行自动填充,如需自动填充请使用#update(Object) |
| `com.baomidou.mybatisplus.extension.conditions.update.ChainUpdate` | `boolean update(T entity)` | 更新数据 |
| `com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper` | `BaseMapper<T> getBaseMapper()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper` | `Class<T> getEntityClass()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper` | `LambdaUpdateChainWrapper<T> set(boolean condition,SFunction<T, ?> column,Object val,String mapping)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper` | `LambdaUpdateChainWrapper<T> setDecrBy(boolean condition,SFunction<T, ?> column,Number val)` | 字段自减变量 val 值 |
| `com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper` | `LambdaUpdateChainWrapper<T> setIncrBy(boolean condition,SFunction<T, ?> column,Number val)` | 字段自增变量 val 值 |
| `com.baomidou.mybatisplus.extension.conditions.update.LambdaUpdateChainWrapper` | `LambdaUpdateChainWrapper<T> setSql(boolean condition,String setSql,Object... params)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper` | `BaseMapper<T> getBaseMapper()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper` | `Class<T> getEntityClass()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper` | `LambdaUpdateChainWrapper<T> lambda()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper` | `String getSqlSet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper` | `UpdateChainWrapper<T> set(boolean condition,String column,Object val,String mapping)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper` | `UpdateChainWrapper<T> setDecrBy(boolean condition,String column,Number val)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper` | `UpdateChainWrapper<T> setIncrBy(boolean condition,String column,Number val)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.update.UpdateChainWrapper` | `UpdateChainWrapper<T> setSql(boolean condition,String setSql,Object... params)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
