# com.baomidou.mybatisplus.extension.spi

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.spi.CompatibleHelper` | `CompatibleSet getCompatibleSet()` | 获取com.baomidou.mybatisplus.extension.spi.CompatibleSet实例 当为空时会抛出异常,需要检查是否为空请使用#hasCompatibleSet() |
| `com.baomidou.mybatisplus.extension.spi.CompatibleHelper` | `boolean hasCompatibleSet()` | 判断是否存在 com.baomidou.mybatisplus.extension.spi.CompatibleSet 实例 |
| `com.baomidou.mybatisplus.extension.spi.CompatibleHelper` | `void setCompatibleSet(CompatibleSet compatibleSet)` | 手动指定 com.baomidou.mybatisplus.extension.spi.CompatibleSet 实例 |
| `com.baomidou.mybatisplus.extension.spi.SpringCompatibleSet` | `InputStream getInputStream(String path)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.spi.SpringCompatibleSet` | `Object getProxyTargetObject(Object mapper)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.spi.SpringCompatibleSet` | `SqlSession getSqlSession(SqlSessionFactory sessionFactory)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.spi.SpringCompatibleSet` | `T getBean(Class<T> clz)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.spi.SpringCompatibleSet` | `boolean executeBatch(SqlSessionFactory sqlSessionFactory,Log log,Consumer<SqlSession> consumer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.spi.SpringCompatibleSet` | `void closeSqlSession(SqlSession sqlSession,SqlSessionFactory sqlSessionFactory)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.spi.SpringCompatibleSet` | `void setContext(Object context)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
