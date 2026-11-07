# com.feilong.net.http.callback

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.http.callback.AbstractResultCallback` | `T doException(HttpRequest httpRequest,HttpUriRequest httpUriRequest,ConnectionConfig useConnectionConfig,UncheckedHttpException e,Date beginDate)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.http.callback.HttpFullInfoResultCallback` | `HttpFullInfo<T> doException(HttpRequest httpRequest,HttpUriRequest httpUriRequest,ConnectionConfig useConnectionConfig,UncheckedHttpException e,Date beginDate)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.http.callback.HttpFullInfoResultCallback` | `HttpFullInfo<T> on(HttpRequest httpRequest,HttpUriRequest httpUriRequest,HttpResponse httpResponse,ConnectionConfig useConnectionConfig,Date beginDate)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.http.callback.HttpFullInfoResultCallback` | `ResultBeanConverter<T> getResultBeanConverter()` | 【原文待译】@return the resultBeanConverter |
| `com.feilong.net.http.callback.HttpFullInfoResultCallback` | `void setResultBeanConverter(ResultBeanConverter<T> resultBeanConverter)` | 【原文待译】@param resultBeanConverter the resultBeanConverter to set |
| `com.feilong.net.http.callback.HttpResponseResultCallback` | `com.feilong.net.http.HttpResponse on(HttpRequest httpRequest,HttpUriRequest httpUriRequest,HttpResponse httpResponse,ConnectionConfig useConnectionConfig,Date beginDate)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.http.callback.ResponseBodyAsStringResultCallback` | `String on(HttpRequest httpRequest,HttpUriRequest httpUriRequest,HttpResponse httpResponse,ConnectionConfig useConnectionConfig,Date beginDate)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.http.callback.ResultBeanConverter` | `T convert(HttpRequest httpRequest,ConnectionConfig useConnectionConfig,HttpResponse httpResponse)` | 转换数据. 注意:每个参数都不会为null |
| `com.feilong.net.http.callback.ResultCallback` | `T doException(HttpRequest httpRequest,HttpUriRequest httpUriRequest,ConnectionConfig useConnectionConfig,UncheckedHttpException e,Date beginDate)` | 如果出现了异常. |
| `com.feilong.net.http.callback.ResultCallback` | `T on(HttpRequest httpRequest,HttpUriRequest httpUriRequest,HttpResponse httpResponse,ConnectionConfig useConnectionConfig,Date beginDate)` | On. 注意:每个参数都不会为null |
| `com.feilong.net.http.callback.StatusCodeResultCallback` | `Integer on(HttpRequest httpRequest,HttpUriRequest httpUriRequest,HttpResponse httpResponse,ConnectionConfig useConnectionConfig,Date beginDate)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
