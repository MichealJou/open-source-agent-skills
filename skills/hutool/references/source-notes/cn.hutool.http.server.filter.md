# cn.hutool.http.server.filter

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.http.server.filter.DefaultExceptionFilter` | `void afterException(final HttpServerRequest req,final HttpServerResponse res,final Throwable e)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.filter.ExceptionFilter` | `void afterException(final HttpServerRequest req,final HttpServerResponse res,final Throwable e)` | 异常之后的处理逻辑 |
| `cn.hutool.http.server.filter.ExceptionFilter` | `void doFilter(final HttpServerRequest req,final HttpServerResponse res,final Filter.Chain chain)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.filter.HttpFilter` | `void doFilter(HttpServerRequest req,HttpServerResponse res,Filter.Chain chain)` | 执行过滤 |
| `cn.hutool.http.server.filter.SimpleFilter` | `String description()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
