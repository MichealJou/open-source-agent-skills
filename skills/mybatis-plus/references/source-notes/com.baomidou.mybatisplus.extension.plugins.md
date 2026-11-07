# com.baomidou.mybatisplus.extension.plugins

版本 3.5.16。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.baomidou.mybatisplus.extension.plugins.MybatisPlusInterceptor` | `List<InnerInterceptor> getInterceptors()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.MybatisPlusInterceptor` | `Object intercept(Invocation invocation)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.MybatisPlusInterceptor` | `Object plugin(Object target)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.MybatisPlusInterceptor` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.MybatisPlusInterceptor` | `void addInnerInterceptor(InnerInterceptor innerInterceptor)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.baomidou.mybatisplus.extension.plugins.MybatisPlusInterceptor` | `void setProperties(Properties properties)` | 使用内部规则,拿分页插件举个栗子: - key: "@page" ,value: "com.baomidou.mybatisplus.extension.plugins.inner.PaginationInnerInterceptor" - key: "page:limit" ,value: "100" 解读1: key 以 "@" 开头定义了这是一个需要组装的 'InnerInterceptor', 以 "page" 结尾表示别名 value 是 'InnerInterceptor' 的具体的 class 全名 解读2: key 以上面定义的 "别名 + ':'" 开头指这个 'value'… |
