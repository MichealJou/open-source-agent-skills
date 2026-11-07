# com.baomidou.mybatisplus.core.spi

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.spi.CompatibleHelper` | `CompatibleSet getCompatibleSet()` | 获取com.baomidou.mybatisplus.core.spi.CompatibleSet实例 当为空时会抛出异常,需要检查是否为空请使用#hasCompatibleSet() |
| `com.baomidou.mybatisplus.core.spi.CompatibleHelper` | `boolean hasCompatibleSet()` | 判断是否存在 com.baomidou.mybatisplus.core.spi.CompatibleSet 实例 |
| `com.baomidou.mybatisplus.core.spi.CompatibleHelper` | `void setCompatibleSet(CompatibleSet compatibleSet)` | 手动指定 com.baomidou.mybatisplus.core.spi.CompatibleSet 实例 |
| `com.baomidou.mybatisplus.core.spi.CompatibleSet` | `InputStream getInputStream(String path)` | @deprecated 3.5.12 无需实现 |
| `com.baomidou.mybatisplus.core.spi.CompatibleSet` | `Object getProxyTargetObject(Object mapper)` | 获取真实被代理的对象 (如果没有被代理,请返回原始对象) |
| `com.baomidou.mybatisplus.core.spi.CompatibleSet` | `SqlSession getSqlSession(SqlSessionFactory sessionFactory)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.spi.CompatibleSet` | `T getBean(Class<T> clz)` | 获取容器bean实例 |
| `com.baomidou.mybatisplus.core.spi.CompatibleSet` | `boolean executeBatch(SqlSessionFactory sqlSessionFactory,Log log,Consumer<SqlSession> consumer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.spi.CompatibleSet` | `void closeSqlSession(SqlSession session,SqlSessionFactory sessionFactory)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.spi.CompatibleSet` | `void setContext(Object context)` | 传递上下文对象 |
