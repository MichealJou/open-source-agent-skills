# com.baomidou.mybatisplus.core.plugins

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `IgnoreStrategy findIgnoreStrategy(Class<?> clz,Method method)` | 通过方法获取策略信息(优先级方法注解>当前类注解) |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `IgnoreStrategy getIgnoreStrategy(String key)` | 获取忽略策略缓存信息 |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `IgnoreStrategy initSqlParserInfoCache(Class<?> mapperClass)` | 初始化缓存 Mapper 上 InterceptorIgnore 注解信息 |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `T execute(IgnoreStrategy ignoreStrategy,Supplier<T> supplier)` | 按指定策略执行指定方法 (忽略线程级别,参数执行级使用最高) 方法执行完成后后释放掉当前线程上的忽略策略. 注意: 1.不要和#handle(IgnoreStrategy)一起混合使用,此方法只是简化操作,防止未释放掉资源造成的错误 2.不要和InterceptorIgnore 注解一起搭配使用,例如在mapper上的default方法里再调用此方法,最终优先级还是以此方法为准 3.记住,一旦调用了此方法,开始会覆盖你当前执行线程上的策略,结束必定会释放掉当前线程上的策略 |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `boolean hasIgnoreStrategy()` | 判断当前线程是否有忽略策略 |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `boolean willIgnore(String id,Function<IgnoreStrategy, Boolean> function)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `boolean willIgnoreBlockAttack(String id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `boolean willIgnoreDataPermission(String id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `boolean willIgnoreDynamicTableName(String id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `boolean willIgnoreIllegalSql(String id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `boolean willIgnoreOthersByKey(String id,String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `boolean willIgnoreTenantLine(String id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `void clearIgnoreStrategy()` | 清空本地忽略策略 |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `void execute(IgnoreStrategy ignoreStrategy,Runnable runnable)` | 按指定策略执行指定方法 (忽略线程级别,参数执行级使用最高) 方法执行完成后后释放掉当前线程上的忽略策略. 注意: 1.不要和#handle(IgnoreStrategy)一起混合使用,此方法只是简化操作,防止未释放掉资源造成的错误 2.不要和InterceptorIgnore 注解一起搭配使用,例如在mapper上的default方法里再调用此方法,最终优先级还是以此方法为准 3.记住,一旦调用了此方法,开始会覆盖你当前执行线程上的策略,结束必定会释放掉当前线程上的策略 |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `void handle(IgnoreStrategy ignoreStrategy)` | 手动设置拦截器忽略执行策略，权限大于注解权限 InterceptorIgnoreHelper.handle(IgnoreStrategy.builder().tenantLine(true).build()); 注意，需要手动关闭调用方法 #clearIgnoreStrategy() 简化操作可请使用#execute(IgnoreStrategy, Supplier) |
| `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper` | `void initSqlParserInfoCache(IgnoreStrategy mapperAnnotation,String mapperClassName,Method method)` | 初始化缓存 Mapper#method 上 InterceptorIgnore 注解信息 |
