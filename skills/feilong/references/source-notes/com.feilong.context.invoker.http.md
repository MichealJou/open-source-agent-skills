# com.feilong.context.invoker.http

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.context.invoker.http.ConnectionConfigBuilder` | `ConnectionConfig build(T request)` | 【原文待译】Builds the. |
| `com.feilong.context.invoker.http.DefaultHttpRequestBuilder` | `HttpRequest build(T request)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.invoker.http.DefaultHttpRequestBuilder` | `void setHttpRequestRebuilder(Rebuilder<HttpRequest> rebuilder)` | 再加工器. 支持在组装完 HttpRequest 之后,再次加工 典型应用在于, 某接口传递了requestbody 属性之后, 还需要额外在uri中加入参数 sign , 值是 requestbody 再次ase加密之后的结果 一般情况下用不到 |
| `com.feilong.context.invoker.http.DefaultHttpRequestBuilder` | `void setHttpTypeBeanProperty(HttpTypeBeanProperty httpTypeBeanProperty)` | 设置 http请求类型的bean属性. |
| `com.feilong.context.invoker.http.DefaultHttpRequestBuilder` | `void setRequestBodyBuilder(RequestBodyBuilder<T> requestBodyBuilder)` | 设置 requestBody构造器. |
| `com.feilong.context.invoker.http.DefaultHttpRequestBuilder` | `void setRequestHeaderBuilder(RequestHeaderBuilder<T> requestHeaderBuilder)` | 设置 头构造器. |
| `com.feilong.context.invoker.http.DefaultHttpRequestBuilder` | `void setRequestParamsBuilder(RequestParamsBuilder<T> requestParamsBuilder)` | 设置 参数构造器. |
| `com.feilong.context.invoker.http.HttpRequestBuilder` | `HttpRequest build(T request)` | 【原文待译】Builds the. |
| `com.feilong.context.invoker.http.HttpResponseStringBuilder` | `void setConnectionConfigBuilder(ConnectionConfigBuilder<T> connectionConfigBuilder)` | 设置 配置构造器. |
| `com.feilong.context.invoker.http.HttpResponseStringBuilder` | `void setHttpRequestBuilder(HttpRequestBuilder<T> httpRequestBuilder)` | 设置 请求参数构造器. |
| `com.feilong.context.invoker.http.RequestBodyBuilder` | `String build(T request)` | 【原文待译】Builds the. |
| `com.feilong.context.invoker.http.RequestHeaderBuilder` | `Map<String, String> build(T request)` | 【原文待译】Builds the. |
| `com.feilong.context.invoker.http.SimpleJsonRequestBodyBuilder` | `JavaToJsonConfig getJavaToJsonConfig()` | 获得 java格式化成json的一些配置. |
| `com.feilong.context.invoker.http.SimpleJsonRequestBodyBuilder` | `String build(T request)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.invoker.http.SimpleJsonRequestBodyBuilder` | `void setJavaToJsonConfig(JavaToJsonConfig javaToJsonConfig)` | 设置 java格式化成json的一些配置. |
| `com.feilong.context.invoker.http.SimpleMapRequestHeaderBuilder` | `Map<String, String> build(T request)` | 【原文待译】Builds the. |
| `com.feilong.context.invoker.http.SimpleMapRequestHeaderBuilder` | `Map<String, String> getHeaderMap()` | 获得 header map. |
| `com.feilong.context.invoker.http.SimpleMapRequestHeaderBuilder` | `void setHeaderMap(Map<String, String> headerMap)` | 设置 header map. |
