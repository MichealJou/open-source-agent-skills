# com.baomidou.mybatisplus.core.conditions.interfaces

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children allEq(BiPredicate<R, V> filter,Map<R, V> params)` | 字段过滤接口，传入多参数时允许对参数进行过滤 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children allEq(BiPredicate<R, V> filter,Map<R, V> params,boolean null2IsNull)` | 字段过滤接口，传入多参数时允许对参数进行过滤 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children allEq(Map<R, V> params)` | map 所有非空属性等于 = |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children allEq(Map<R, V> params,boolean null2IsNull)` | map 所有非空属性等于 = |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children allEq(boolean condition,BiPredicate<R, V> filter,Map<R, V> params,boolean null2IsNull)` | 字段过滤接口，传入多参数时允许对参数进行过滤 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children allEq(boolean condition,Map<R, V> params,boolean null2IsNull)` | map 所有非空属性等于 = |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children between(R column,Object val1,Object val2)` | BETWEEN 值1 AND 值2 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children between(boolean condition,R column,Object val1,Object val2)` | BETWEEN 值1 AND 值2 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children eq(R column,Object val)` | 等于 = |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children eq(boolean condition,R column,Object val)` | 等于 = |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children ge(R column,Object val)` | 大于等于 >= |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children ge(boolean condition,R column,Object val)` | 大于等于 >= |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children gt(R column,Object val)` | 大于 > |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children gt(boolean condition,R column,Object val)` | 大于 > |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children le(R column,Object val)` | 小于等于 <= |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children le(boolean condition,R column,Object val)` | 小于等于 <= |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children like(R column,Object val)` | LIKE '%值%' |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children like(boolean condition,R column,Object val)` | LIKE '%值%' |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children likeLeft(R column,Object val)` | LIKE '%值' |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children likeLeft(boolean condition,R column,Object val)` | LIKE '%值' |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children likeRight(R column,Object val)` | LIKE '值%' |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children likeRight(boolean condition,R column,Object val)` | LIKE '值%' |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children lt(R column,Object val)` | 小于 < |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children lt(boolean condition,R column,Object val)` | 小于 < |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children ne(R column,Object val)` | 不等于 <> |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children ne(boolean condition,R column,Object val)` | 不等于 <> |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children notBetween(R column,Object val1,Object val2)` | NOT BETWEEN 值1 AND 值2 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children notBetween(boolean condition,R column,Object val1,Object val2)` | NOT BETWEEN 值1 AND 值2 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children notLike(R column,Object val)` | NOT LIKE '%值%' |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children notLike(boolean condition,R column,Object val)` | NOT LIKE '%值%' |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children notLikeLeft(R column,Object val)` | NOT LIKE '%值' |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children notLikeLeft(boolean condition,R column,Object val)` | NOT LIKE '%值' |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children notLikeRight(R column,Object val)` | NOT LIKE '值%' |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Compare` | `Children notLikeRight(boolean condition,R column,Object val)` | NOT LIKE '值%' |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children eqSql(R column,String sql)` | 字段 EQ ( sql语句 ) !! sql 注入方式的 eq 方法 !! 例1: eqSql("id", "1") 例2: eqSql("id", "select MAX(id) from table") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children eqSql(boolean condition,R column,String sql)` | 字段 EQ ( sql语句 ) !! sql 注入方式的 eq 方法 !! 例1: eqSql("id", "1") 例2: eqSql("id", "select MAX(id) from table") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children func(Consumer<Children> consumer)` | 消费函数 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children func(boolean condition,Consumer<Children> consumer)` | 消费函数 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children geSql(R column,String sql)` | 字段 >= ( sql语句 ) 例1: geSql("id", "1") 例1: geSql("id", "select id from table where name = 'JunJun'") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children geSql(boolean condition,R column,String sql)` | 字段 >= ( sql语句 ) 例1: geSql(true, "id", "1") 例1: geSql(true, "id", "select id from table where name = 'JunJun'") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children groupBy(List<R> columns)` | 分组：GROUP BY 字段, ... 例: groupBy(Arrays.asList("id", "name")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children groupBy(R column)` | 分组：GROUP BY 字段, ... 例: groupBy("id") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children groupBy(R column,R... columns)` | 分组：GROUP BY 字段, ... 例: groupBy("id", "name") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children groupBy(boolean condition,List<R> columns)` | 分组：GROUP BY 字段, ... 例: groupBy(true, Arrays.asList("id", "name")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children groupBy(boolean condition,R column)` | 分组：GROUP BY 字段, ... 例: groupBy(true, "id") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children groupBy(boolean condition,R column,List<R> columns)` | 分组：GROUP BY 字段, ... 例: groupBy(true, "id", Arrays.asList("name")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children groupBy(boolean condition,R column,R... columns)` | 分组：GROUP BY 字段, ... 例: groupBy(true, "id", "name") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children gtSql(R column,String sql)` | 字段 > ( sql语句 ) 例1: gtSql("id", "1") 例1: gtSql("id", "select id from table where name = 'JunJun'") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children gtSql(boolean condition,R column,String sql)` | 字段 > ( sql语句 ) 例1: gtSql(true, "id", "1") 例1: gtSql(true, "id", "select id from table where name = 'JunJun'") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children having(String sqlHaving,Object... params)` | HAVING ( sql语句 ) 例1: having("sum(age) > 10") 例2: having("sum(age) > {0}", 10) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children having(boolean condition,String sqlHaving,Object... params)` | HAVING ( sql语句 ) 例1: having(true, "sum(age) > 10") 例2: having(true, "sum(age) > {0}", 10) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children in(R column,Collection<?> coll)` | 字段 IN (value.get(0), value.get(1), ...) 例: in("id", Arrays.asList(1, 2, 3, 4, 5)) 注意！当集合为 空或null 时, sql会拼接为：WHERE (字段名 IN ()), 执行时报错 若要在特定条件下不拼接, 可在 condition 条件中判断 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children in(R column,Object... values)` | 字段 IN (v0, v1, ...) 例: in("id", 1, 2, 3, 4, 5) 注意！当数组为 空或null 时, sql会拼接为：WHERE (字段名 IN ()), 执行时报错 若要在特定条件下不拼接, 可在 condition 条件中判断 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children in(boolean condition,R column,Collection<?> coll)` | 字段 IN (value.get(0), value.get(1), ...) 例: in(true, "id", Arrays.asList(1, 2, 3, 4, 5)) 注意！当集合为 空或null 时, sql会拼接为：WHERE (字段名 IN ()), 执行时报错 若要在特定条件下不拼接, 可在 condition 条件中判断 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children in(boolean condition,R column,Object... values)` | 字段 IN (v0, v1, ...) 例: in(true, "id", 1, 2, 3, 4, 5) 注意！当数组为 空或null 时, sql会拼接为：WHERE (字段名 IN ()), 执行时报错 若要在特定条件下不拼接, 可在 condition 条件中判断 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children inSql(R column,String sql)` | 字段 IN ( sql语句 ) !! sql 注入方式的 in 方法 !! 例1: inSql("id", "1") 例2: inSql("id", "select id from table where id < 3") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children inSql(boolean condition,R column,String sql)` | 字段 IN ( sql语句 ) !! sql 注入方式的 in 方法 !! 例1: inSql(true, "id", "1") 例2: inSql(true, "id", "select id from table where id < 3") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children isNotNull(R column)` | 字段 IS NOT NULL 例: isNotNull("name") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children isNotNull(boolean condition,R column)` | 字段 IS NOT NULL 例: isNotNull(true, "name") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children isNull(R column)` | 字段 IS NULL 例: isNull("name") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children isNull(boolean condition,R column)` | 字段 IS NULL 例: isNull(true, "name") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children leSql(R column,String inValue)` | 字段 例1: leSql("id", "1") 例1: leSql("id", "select id from table where name = 'JunJun'") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children leSql(boolean condition,R column,String sql)` | 字段 例1: leSql(true, "id", "1") 例1: leSql(true ,"id", "select id from table where name = 'JunJun'") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children ltSql(R column,String sql)` | 字段 < ( sql语句 ) 例1: ltSql("id", "1") 例1: ltSql("id", "select id from table where name = 'JunJun'") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children ltSql(boolean condition,R column,String sql)` | 字段 < ( sql语句 ) 例1: ltSql(true, "id", "1") 例1: ltSql(true , "id", "select id from table where name = 'JunJun'") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children notIn(R column,Collection<?> coll)` | 字段 NOT IN (value.get(0), value.get(1), ...) 例: notIn("id", Arrays.asList(1, 2, 3, 4, 5)) 注意！当集合为 空或null 时, sql会拼接为：WHERE (字段名 NOT IN ()), 执行时报错 若要在特定条件下不拼接, 可在 condition 条件中判断 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children notIn(R column,Object... values)` | 字段 NOT IN (v0, v1, ...) 例: notIn("id", 1, 2, 3, 4, 5) 注意！当数组为 空或null 时, sql会拼接为：WHERE (字段名 NOT IN ()), 执行时报错 若要在特定条件下不拼接, 可在 condition 条件中判断 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children notIn(boolean condition,R column,Collection<?> coll)` | 字段 NOT IN (value.get(0), value.get(1), ...) 例: notIn(true, "id", Arrays.asList(1, 2, 3, 4, 5)) 注意！当集合为 空或null 时, sql会拼接为：WHERE (字段名 NOT IN ()), 执行时报错 若要在特定条件下不拼接, 可在 condition 条件中判断 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children notIn(boolean condition,R column,Object... values)` | 字段 NOT IN (v0, v1, ...) 例: notIn(true, "id", 1, 2, 3, 4, 5) 注意！当数组为 空或null 时, sql会拼接为：WHERE (字段名 NOT IN ()), 执行时报错 若要在特定条件下不拼接, 可在 condition 条件中判断 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children notInSql(R column,String inValue)` | 字段 NOT IN ( sql语句 ) !! sql 注入方式的 not in 方法 !! 例1: notInSql("id", "1, 2, 3, 4, 5, 6") 例2: notInSql("id", "select id from table where id < 3") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children notInSql(boolean condition,R column,String inValue)` | 字段 NOT IN ( sql语句 ) !! sql 注入方式的 not in 方法 !! 例1: notInSql(true, "id", "1, 2, 3, 4, 5, 6") 例2: notInSql(true, "id", "select id from table where id < 3") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderBy(boolean condition,boolean isAsc,List<R> columns)` | 排序：ORDER BY 字段, ... 例: orderBy(true, Arrays.asList("id", "name")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderBy(boolean condition,boolean isAsc,R column)` | 排序：ORDER BY 字段, ... 例: orderBy(true, "id") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderBy(boolean condition,boolean isAsc,R column,List<R> columns)` | 排序：ORDER BY 字段, ... |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderBy(boolean condition,boolean isAsc,R column,R... columns)` | 排序：ORDER BY 字段, ... |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderByAsc(List<R> columns)` | 排序：ORDER BY 字段, ... ASC 例: orderByAsc(Arrays.asList("id", "name")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderByAsc(R column)` | 排序：ORDER BY 字段, ... ASC 例: orderByAsc("id") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderByAsc(R column,R... columns)` | 排序：ORDER BY 字段, ... ASC |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderByAsc(boolean condition,List<R> columns)` | 排序：ORDER BY 字段, ... ASC 例: orderByAsc(true, Arrays.asList("id", "name")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderByAsc(boolean condition,R column)` | 排序：ORDER BY 字段, ... ASC 例: orderByAsc(true, "id") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderByAsc(boolean condition,R column,List<R> columns)` | 排序：ORDER BY 字段, ... ASC 例: orderByAsc(true, Arrays.asList("id", "name")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderByAsc(boolean condition,R column,R... columns)` | 排序：ORDER BY 字段, ... ASC |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderByDesc(List<R> columns)` | 排序：ORDER BY 字段, ... DESC |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderByDesc(R column)` | 排序：ORDER BY 字段, ... DESC 例: orderByDesc("id") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderByDesc(R column,R... columns)` | 排序：ORDER BY 字段, ... DESC |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderByDesc(boolean condition,List<R> columns)` | 排序：ORDER BY 字段, ... DESC 例: orderByDesc(true, Arrays.asList("id", "name")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderByDesc(boolean condition,R column)` | 排序：ORDER BY 字段, ... DESC 例: orderByDesc(true, "id") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderByDesc(boolean condition,R column,List<R> columns)` | 排序：ORDER BY 字段, ... DESC |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Func` | `Children orderByDesc(boolean condition,R column,R... columns)` | 排序：ORDER BY 字段, ... DESC |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Join` | `Children apply(String applySql,Object... values)` | 拼接 sql !! 会有 sql 注入风险 !! 例1: apply("id = 1") 例2: apply("date_format(dateColumn,'%Y-%m-%d') = '2008-08-08'") 例3: apply("date_format(dateColumn,'%Y-%m-%d') = {0}", LocalDate.now()) 例4: apply("type={0,javaType=int,jdbcType=NUMERIC,typeHandler=xxx.xxx.MyTypeHandler}", "待处理字符串") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Join` | `Children apply(boolean condition,String applySql,Object... values)` | 拼接 sql !! 会有 sql 注入风险 !! 例1: apply("id = 1") 例2: apply("date_format(dateColumn,'%Y-%m-%d') = '2008-08-08'") 例3: apply("date_format(dateColumn,'%Y-%m-%d') = {0}", LocalDate.now()) 例4: apply("type={0,javaType=int,jdbcType=NUMERIC,typeHandler=xxx.xxx.MyTypeHandler}", "待处理字符串") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Join` | `Children comment(String comment)` | sql 注释(会拼接在 sql 的最后面) 自3.5.6开始,默认不处理转义字符,如有需要,调用com.baomidou.mybatisplus.core.toolkit.sql.StringEscape#escapeRawString(String) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Join` | `Children comment(boolean condition,String comment)` | sql 注释(会拼接在 sql 的最后面) 自3.5.6开始,默认不处理转义字符,如有需要,调用com.baomidou.mybatisplus.core.toolkit.sql.StringEscape#escapeRawString(String) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Join` | `Children exists(String existsSql,Object... values)` | 拼接 EXISTS ( sql语句 ) !! sql 注入方法 !! 例: exists("select id from table where age = 1") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Join` | `Children exists(boolean condition,String existsSql,Object... values)` | 拼接 EXISTS ( sql语句 ) !! sql 注入方法 !! 例: exists("select id from table where age = 1") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Join` | `Children first(String firstSql)` | sql 起始句（会拼接在SQL语句的起始处） 自3.5.6开始,默认不处理转义字符,如有需要,调用com.baomidou.mybatisplus.core.toolkit.sql.StringEscape#escapeRawString(String) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Join` | `Children first(boolean condition,String firstSql)` | sql 起始句（会拼接在SQL语句的起始处） 自3.5.6开始,默认不处理转义字符,如有需要,调用com.baomidou.mybatisplus.core.toolkit.sql.StringEscape#escapeRawString(String) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Join` | `Children last(String lastSql)` | 无视优化规则直接拼接到 sql 的最后(有sql注入的风险,请谨慎使用) 例: last("limit 1") 注意只能调用一次,多次调用以最后一次为准 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Join` | `Children last(boolean condition,String lastSql)` | 无视优化规则直接拼接到 sql 的最后(有sql注入的风险,请谨慎使用) 例: last("limit 1") 注意只能调用一次,多次调用以最后一次为准 |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Join` | `Children notExists(String existsSql,Object... values)` | 拼接 NOT EXISTS ( sql语句 ) !! sql 注入方法 !! 例: notExists("select id from table where age = 1") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Join` | `Children notExists(boolean condition,String existsSql,Object... values)` | 拼接 NOT EXISTS ( sql语句 ) !! sql 注入方法 !! 例: notExists("select id from table where age = 1") |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Join` | `Children or()` | 拼接 OR |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Join` | `Children or(boolean condition)` | 拼接 OR |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Nested` | `Children and(Consumer<Param> consumer)` | AND 嵌套 例: and(i -> i.eq("name", "李白").ne("status", "活着")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Nested` | `Children and(boolean condition,Consumer<Param> consumer)` | AND 嵌套 例: and(i -> i.eq("name", "李白").ne("status", "活着")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Nested` | `Children nested(Consumer<Param> consumer)` | 正常嵌套 不带 AND 或者 OR 例: nested(i -> i.eq("name", "李白").ne("status", "活着")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Nested` | `Children nested(boolean condition,Consumer<Param> consumer)` | 正常嵌套 不带 AND 或者 OR 例: nested(i -> i.eq("name", "李白").ne("status", "活着")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Nested` | `Children not(Consumer<Param> consumer)` | not嵌套 例: not(i -> i.eq("name", "李白").ne("status", "活着")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Nested` | `Children not(boolean condition,Consumer<Param> consumer)` | not嵌套 例: not(i -> i.eq("name", "李白").ne("status", "活着")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Nested` | `Children or(Consumer<Param> consumer)` | OR 嵌套 例: or(i -> i.eq("name", "李白").ne("status", "活着")) |
| `com.baomidou.mybatisplus.core.conditions.interfaces.Nested` | `Children or(boolean condition,Consumer<Param> consumer)` | OR 嵌套 例: or(i -> i.eq("name", "李白").ne("status", "活着")) |
