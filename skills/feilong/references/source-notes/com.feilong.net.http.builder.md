# com.feilong.net.http.builder

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.http.builder.HttpClientBuilder` | `HttpClient build(String logTraceContext,ConnectionConfig connectionConfig)` | 创造 HttpClient. |
| `com.feilong.net.http.builder.HttpRequestExecuter` | `T execute(HttpRequest httpRequest,ConnectionConfig connectionConfig,ResultCallback<T> resultCallback)` | 【原文待译】Execute. |
| `com.feilong.net.http.builder.HttpResponseUtil` | `String getResultString(HttpResponse httpResponse)` | 从HttpResponse中提取result 字符串 . |
| `com.feilong.net.http.builder.HttpUriRequestBuilder` | `HttpUriRequest build(HttpRequest httpRequest,ConnectionConfig connectionConfig)` | 基于 httpRequest 和 connectionConfig 构造 HttpUriRequest. |
| `com.feilong.net.http.builder.RequestConfigBuilder` | `RequestConfig build(ConnectionConfig connectionConfig)` | 【原文待译】Builds the RequestConfig. |
| `com.feilong.net.http.builder.SpecialHttpRequestRetryHandler` | `boolean retryRequest(final IOException exception,final int executionCount,final HttpContext context)` | 【原文待译】Used retryCount and requestSentRetryEnabled to determine if the given method should be retried. |
| `com.feilong.net.http.builder.SpecialHttpRequestRetryHandler` | `void setLogTraceContext(String logTraceContext)` | 【原文待译】@param logTraceContext the logTraceContext to set |
