# com.baomidou.mybatisplus.core.injector

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.core.injector.AbstractMethod` | `MappedStatement injectMappedStatement(Class<?> mapperClass,Class<?> modelClass,TableInfo tableInfo)` | 注入自定义 MappedStatement |
| `com.baomidou.mybatisplus.core.injector.AbstractMethod` | `SqlSource createSqlSource(Configuration configuration,String script,Class<?> parameterType)` | @param configuration 配置对象 |
| `com.baomidou.mybatisplus.core.injector.AbstractMethod` | `void inject(MapperBuilderAssistant builderAssistant,Class<?> mapperClass,Class<?> modelClass,TableInfo tableInfo)` | 注入自定义方法 |
| `com.baomidou.mybatisplus.core.injector.AbstractSqlInjector` | `List<AbstractMethod> getMethodList(Class<?> mapperClass,TableInfo tableInfo)` | 获取 注入的方法 |
| `com.baomidou.mybatisplus.core.injector.AbstractSqlInjector` | `List<AbstractMethod> getMethodList(Configuration configuration,Class<?> mapperClass,TableInfo tableInfo)` | 获取注入的方法 |
| `com.baomidou.mybatisplus.core.injector.AbstractSqlInjector` | `void inspectInject(MapperBuilderAssistant builderAssistant,Class<?> mapperClass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.injector.DefaultSqlInjector` | `List<AbstractMethod> getMethodList(Configuration configuration,Class<?> mapperClass,TableInfo tableInfo)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.core.injector.ISqlInjector` | `void inspectInject(MapperBuilderAssistant builderAssistant,Class<?> mapperClass)` | 检查SQL是否注入(已经注入过不再注入) |
| `com.baomidou.mybatisplus.core.injector.SqlRunnerInjector` | `void inject(Configuration configuration)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
