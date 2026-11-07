# com.baomidou.mybatisplus.core.incrementer

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.incrementer.DefaultIdentifierGenerator` | `DefaultIdentifierGenerator getInstance()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.incrementer.DefaultIdentifierGenerator` | `IdentifierGenerator getFixedIdentifierGenerator(Log log)` | 获取固定的生成器实例 当无法通过网卡信息获取时，使用固定的一个主键生成器实例. |
| `com.baomidou.mybatisplus.core.incrementer.DefaultIdentifierGenerator` | `Long nextId(Object entity)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.incrementer.IKeyGenerator` | `DbType dbType()` | 数据库类型 |
| `com.baomidou.mybatisplus.core.incrementer.IKeyGenerator` | `String executeSql(String incrementerName)` | 执行 key 生成 SQL |
| `com.baomidou.mybatisplus.core.incrementer.IdentifierGenerator` | `Number nextId(Object entity)` | 生成Id |
| `com.baomidou.mybatisplus.core.incrementer.IdentifierGenerator` | `String nextUUID(Object entity)` | 生成uuid |
| `com.baomidou.mybatisplus.core.incrementer.IdentifierGenerator` | `boolean assignId(Object idValue)` | 判断是否分配 ID |
| `com.baomidou.mybatisplus.core.incrementer.ImadcnIdentifierGenerator` | `Number nextId(Object entity)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.incrementer.ImadcnIdentifierGenerator` | `String nextUUID(Object entity)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.incrementer.ImadcnIdentifierGenerator` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
