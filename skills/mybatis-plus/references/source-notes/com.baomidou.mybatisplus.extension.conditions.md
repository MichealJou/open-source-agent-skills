# com.baomidou.mybatisplus.extension.conditions

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `AbstractWrapper<T, R, Param> getWrapper()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children allEq(boolean condition,BiPredicate<R, V> filter,Map<R, V> params,boolean null2IsNull)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children allEq(boolean condition,Map<R, V> params,boolean null2IsNull)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children and(boolean condition,Consumer<Param> consumer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children apply(boolean condition,String applySql,Object... values)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children between(boolean condition,R column,Object val1,Object val2)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children comment(boolean condition,String comment)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children eq(boolean condition,R column,Object val)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children eqSql(boolean condition,R column,String eqValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children exists(boolean condition,String existsSql,Object... values)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children first(boolean condition,String firstSql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children func(boolean condition,Consumer<Children> consumer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children ge(boolean condition,R column,Object val)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children geSql(boolean condition,R column,String inValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children groupBy(R column,R... columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children groupBy(boolean condition,List<R> columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children groupBy(boolean condition,R column)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children groupBy(boolean condition,R column,List<R> columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children groupBy(boolean condition,R column,R... columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children gt(boolean condition,R column,Object val)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children gtSql(boolean condition,R column,String inValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children having(boolean condition,String sqlHaving,Object... params)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children in(boolean condition,R column,Collection<?> coll)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children in(boolean condition,R column,Object... values)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children inSql(boolean condition,R column,String inValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children isNotNull(boolean condition,R column)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children isNull(boolean condition,R column)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children last(boolean condition,String lastSql)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children le(boolean condition,R column,Object val)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children leSql(boolean condition,R column,String inValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children like(boolean condition,R column,Object val)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children likeLeft(boolean condition,R column,Object val)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children likeRight(boolean condition,R column,Object val)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children lt(boolean condition,R column,Object val)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children ltSql(boolean condition,R column,String inValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children ne(boolean condition,R column,Object val)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children nested(boolean condition,Consumer<Param> consumer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children not(boolean condition,Consumer<Param> consumer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children notBetween(boolean condition,R column,Object val1,Object val2)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children notExists(boolean condition,String existsSql,Object... values)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children notIn(boolean condition,R column,Collection<?> coll)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children notIn(boolean condition,R column,Object... values)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children notInSql(boolean condition,R column,String inValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children notLike(boolean condition,R column,Object val)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children notLikeLeft(boolean condition,R column,Object val)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children notLikeRight(boolean condition,R column,Object val)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children or(boolean condition)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children or(boolean condition,Consumer<Param> consumer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children orderBy(boolean condition,boolean isAsc,List<R> columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children orderBy(boolean condition,boolean isAsc,R column)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children orderBy(boolean condition,boolean isAsc,R column,List<R> columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children orderBy(boolean condition,boolean isAsc,R column,R... columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children orderByAsc(R column,R... columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children orderByAsc(boolean condition,R column,R... columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children orderByDesc(R column,R... columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children orderByDesc(boolean condition,R column,R... columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children setEntity(T entity)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `Children setEntityClass(Class<T> entityClass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `MergeSegments getExpression()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `String getCustomSqlSegment()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `String getSqlComment()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `String getSqlFirst()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `String getSqlSegment()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `String getSqlSelect()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `String getSqlSet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `String getTargetSql()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `T getEntity()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.conditions.ChainWrapper` | `BaseMapper<T> getBaseMapper()` | 获取 BaseMapper |
| `com.baomidou.mybatisplus.extension.conditions.ChainWrapper` | `Class<T> getEntityClass()` | 获取当前实体Class |
| `com.baomidou.mybatisplus.extension.conditions.ChainWrapper` | `R execute(SFunction<BaseMapper<T>, R> function)` | 执行baseMapper操作，有baseMapper操作时使用baseMapper，没有时通过entityClass获取baseMapper，再使用 |
| `com.baomidou.mybatisplus.extension.conditions.ChainWrapper` | `Wrapper<T> getWrapper()` | 获取最终拿去执行的 Wrapper |
