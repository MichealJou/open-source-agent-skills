# com.baomidou.mybatisplus.core.conditions.query

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper` | `LambdaQueryWrapper<T> select(Class<T> entityClass,Predicate<TableFieldInfo> predicate)` | 过滤查询的字段信息(主键除外!) 例1: 只要 java 字段名以 "test" 开头的 -> select(i -> i.getProperty().startsWith("test")) 例2: 只要 java 字段属性是 CharSequence 类型的 -> select(TableFieldInfo::isCharSequence) 例3: 只要 java 字段没有填充策略的 -> select(i -> i.getFieldFill() == FieldFill.DEFAULT) 例4: 要全部字段 -> select(i -> true) 例5: 只要主键字段 -> select… |
| `com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper` | `LambdaQueryWrapper<T> select(SFunction<T, ?>... columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper` | `LambdaQueryWrapper<T> select(boolean condition,List<SFunction<T, ?>> columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper` | `LambdaQueryWrapper<T> select(boolean condition,SFunction<T, ?>... columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper` | `String getSqlSelect()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.conditions.query.Query` | `Children select(Class<T> entityClass,Predicate<TableFieldInfo> predicate)` | 过滤查询的字段信息(主键除外!) 例1: 只要 java 字段名以 "test" 开头的 -> select(i -> i.getProperty().startsWith("test")) 例2: 只要 java 字段属性是 CharSequence 类型的 -> select(TableFieldInfo::isCharSequence) 例3: 只要 java 字段没有填充策略的 -> select(i -> i.getFieldFill() == FieldFill.DEFAULT) 例4: 要全部字段 -> select(i -> true) 例5: 只要主键字段 -> select… |
| `com.baomidou.mybatisplus.core.conditions.query.Query` | `Children select(List<R> columns)` | 指定查询字段 |
| `com.baomidou.mybatisplus.core.conditions.query.Query` | `Children select(Predicate<TableFieldInfo> predicate)` | 过滤查询的字段信息(主键除外!) 注意只有内部有 entity 才能使用该方法 |
| `com.baomidou.mybatisplus.core.conditions.query.Query` | `Children select(R... columns)` | 指定查询字段 |
| `com.baomidou.mybatisplus.core.conditions.query.Query` | `Children select(boolean condition,List<R> columns)` | 指定查询字段 |
| `com.baomidou.mybatisplus.core.conditions.query.Query` | `Children select(boolean condition,R... columns)` | 指定查询字段 |
| `com.baomidou.mybatisplus.core.conditions.query.Query` | `String getSqlSelect()` | 查询条件 SQL 片段 |
| `com.baomidou.mybatisplus.core.conditions.query.QueryWrapper` | `LambdaQueryWrapper<T> lambda()` | 返回一个支持 lambda 函数写法的 wrapper |
| `com.baomidou.mybatisplus.core.conditions.query.QueryWrapper` | `QueryWrapper<T> checkSqlInjection()` | 开启检查 SQL 注入 |
| `com.baomidou.mybatisplus.core.conditions.query.QueryWrapper` | `QueryWrapper<T> select(Class<T> entityClass,Predicate<TableFieldInfo> predicate)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.conditions.query.QueryWrapper` | `QueryWrapper<T> select(boolean condition,List<String> columns)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.conditions.query.QueryWrapper` | `String getSqlSelect()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.conditions.query.QueryWrapper` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
