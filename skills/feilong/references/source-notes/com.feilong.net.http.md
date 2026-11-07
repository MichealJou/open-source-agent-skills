# com.feilong.net.http

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.http.ConnectionConfig` | `Integer getProxyPort()` | 代理端口. A valid port value is between 0 ~ 65535. A port number of zero will let the system pick up an ephemeral port in a bind operation. |
| `com.feilong.net.http.ConnectionConfig` | `String getContentCharset()` | 获得 内容的字符集. |
| `com.feilong.net.http.ConnectionConfig` | `String getPassword()` | Http Basic Authentication 基本认证的密码. 暂时不支持 微软的windows系统使用的一种凭据 如果值是null或者blank,将会自动忽略 |
| `com.feilong.net.http.ConnectionConfig` | `String getProxyAddress()` | 获得 the proxy address. |
| `com.feilong.net.http.ConnectionConfig` | `String getUserName()` | Http Basic Authentication 基本认证的用户名. 暂时不支持 微软的windows系统使用的一种凭据 如果值是null或者blank,将会自动忽略 |
| `com.feilong.net.http.ConnectionConfig` | `String toString()` | 【原文待译】(non-Javadoc) |
| `com.feilong.net.http.ConnectionConfig` | `boolean equals(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.http.ConnectionConfig` | `boolean getIsTimeoutRetry()` | 获得 是否超时重试. |
| `com.feilong.net.http.ConnectionConfig` | `boolean getTurnOffHostnameVerifier()` | 是否关闭 HostnameVerifier essentially turns hostname 校验. 默认 true 表示关闭 |
| `com.feilong.net.http.ConnectionConfig` | `int getConnectTimeout()` | 打开到 URLConnection资源的通信连接时超时值 ( 以毫秒为单位 ). |
| `com.feilong.net.http.ConnectionConfig` | `int getMaxConnPerRoute()` | 针对一个域名,同时正在使用的最多的连接数. httpclient4,系统默认是2, feilong 设置为200 |
| `com.feilong.net.http.ConnectionConfig` | `int getMaxConnTotal()` | 同时间正在用的最多连接数. httpclient4 ,系统默认是20, feilong 设置为1000 |
| `com.feilong.net.http.ConnectionConfig` | `int getReadTimeout()` | 读超时时间,在建立连接后从 Input流读入时的超时时间, 以毫秒为单位 . |
| `com.feilong.net.http.ConnectionConfig` | `int getTimeoutRetryCount()` | 获得 超时重试次数,默认3次. |
| `com.feilong.net.http.ConnectionConfig` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.http.ConnectionConfig` | `void setConnectTimeout(int connectTimeout)` | 打开到 URLConnection资源的通信连接时超时值 ( 以毫秒为单位 ). |
| `com.feilong.net.http.ConnectionConfig` | `void setContentCharset(String contentCharset)` | 设置 内容的字符集. |
| `com.feilong.net.http.ConnectionConfig` | `void setIsTimeoutRetry(boolean isTimeoutRetry)` | 设置 是否超时重试. |
| `com.feilong.net.http.ConnectionConfig` | `void setMaxConnPerRoute(int maxConnPerRoute)` | 针对一个域名,同时正在使用的最多的连接数. httpclient4,系统默认是2, feilong 设置为200 |
| `com.feilong.net.http.ConnectionConfig` | `void setMaxConnTotal(int maxConnTotal)` | 同时间正在用的最多连接数. httpclient4 ,系统默认是20, feilong 设置为1000 |
| `com.feilong.net.http.ConnectionConfig` | `void setPassword(String password)` | Http Basic Authentication 基本认证的密码. 暂时不支持 微软的windows系统使用的一种凭据 如果值是null或者blank,将会自动忽略 |
| `com.feilong.net.http.ConnectionConfig` | `void setProxyAddress(String proxyAddress)` | 设置 the proxy address. |
| `com.feilong.net.http.ConnectionConfig` | `void setProxyPort(Integer proxyPort)` | 代理端口. A valid port value is between 0 ~ 65535. A port number of zero will let the system pick up an ephemeral port in a bind operation. |
| `com.feilong.net.http.ConnectionConfig` | `void setReadTimeout(int readTimeout)` | 读超时时间,在建立连接后从 Input流读入时的超时时间, 以毫秒为单位 . |
| `com.feilong.net.http.ConnectionConfig` | `void setTimeoutRetryCount(int timeoutRetryCount)` | 设置 超时重试次数,默认3次. |
| `com.feilong.net.http.ConnectionConfig` | `void setTurnOffHostnameVerifier(boolean turnOffHostnameVerifier)` | 是否关闭 HostnameVerifier essentially turns hostname 校验. 默认 true 表示关闭 |
| `com.feilong.net.http.ConnectionConfig` | `void setUserName(String userName)` | Http Basic Authentication 基本认证的用户名. 暂时不支持 微软的windows系统使用的一种凭据 如果值是null或者blank,将会自动忽略 |
| `com.feilong.net.http.HttpClientUtil` | `HttpFullInfo<T> getHttpFullInfo(HttpRequest httpRequest,ConnectionConfig connectionConfig,ResultBeanConverter<T> resultBeanConverter)` | http完整信息, 方便在外层做日志或者保存日志到数据库中. |
| `com.feilong.net.http.HttpClientUtil` | `String get(String uri)` | 发送get请求,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String get(String uri,Map<String, String> requestParamMap)` | 发送 get 请求,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String get(String uri,Map<String, String> requestParamMap,Map<String, String> headerMap)` | 发送 get 请求,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String get(String uri,String paramName,String paramValue)` | 发送get请求,获得请求的响应内容. 方便只有1个参数的请求 |
| `com.feilong.net.http.HttpClientUtil` | `String getResponseBodyAsString(HttpRequest httpRequest)` | 发送请求,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String getResponseBodyAsString(HttpRequest httpRequest,ConnectionConfig connectionConfig)` | 发送请求,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String getResponseBodyAsString(String uri,ConnectionConfig connectionConfig)` | 发送请求,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String getResponseBodyAsString(String uri,Map<String, String> requestParamMap,HttpMethodType httpMethodType)` | 发送请求,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String getResponseBodyAsString(String uri,Map<String, String> requestParamMap,String httpMethod)` | 发送请求,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String patch(String uri,String requestBody)` | 发送 patch 请求,并且设置 RequestBody ,以及 headerMap,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String patch(String uri,String requestBody,Map<String, String> headerMap)` | 发送 patch 请求,并且设置 RequestBody ,以及 headerMap,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String post(String uri)` | 发送post请求,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String post(String uri,Map<String, String> requestParamMap)` | 发送 post 请求,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String post(String uri,Map<String, String> requestParamMap,Map<String, String> headerMap)` | 发送 post 请求,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String post(String uri,String paramName,String paramValue)` | 发送post请求,获得请求的响应内容. 方便只有1个参数的请求 |
| `com.feilong.net.http.HttpClientUtil` | `String post(String uri,String requestBody)` | 发送 Post 请求,并且设置 RequestBody ,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String post(String uri,String requestBody,Map<String, String> headerMap)` | 发送 Post 请求,并且设置 RequestBody ,以及 headerMap,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String put(String uri)` | 发送put请求,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String put(String uri,Map<String, String> requestParamMap)` | 发送 put 请求,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String put(String uri,Map<String, String> requestParamMap,Map<String, String> headerMap)` | 发送 put 请求,获得请求的响应内容. |
| `com.feilong.net.http.HttpClientUtil` | `String put(String uri,String paramName,String paramValue)` | 发送put请求,获得请求的响应内容. 方便只有1个参数的请求 |
| `com.feilong.net.http.HttpClientUtil` | `com.feilong.net.http.HttpResponse getHttpResponse(HttpRequest httpRequest)` | 获得 com.feilong.net.http.HttpResponse. |
| `com.feilong.net.http.HttpClientUtil` | `com.feilong.net.http.HttpResponse getHttpResponse(HttpRequest httpRequest,ConnectionConfig connectionConfig)` | 获得 com.feilong.net.http.HttpResponse. |
| `com.feilong.net.http.HttpClientUtil` | `com.feilong.net.http.HttpResponse getHttpResponse(String urlString)` | 获得 com.feilong.net.http.HttpResponse. |
| `com.feilong.net.http.HttpClientUtil` | `com.feilong.net.http.HttpResponse getHttpResponse(String urlString,ConnectionConfig connectionConfig)` | 获得 com.feilong.net.http.HttpResponse. |
| `com.feilong.net.http.HttpClientUtil` | `int getResponseStatusCode(HttpRequest httpRequest,ConnectionConfig connectionConfig)` | 获得请求的响应码. |
| `com.feilong.net.http.HttpClientUtil` | `int getResponseStatusCode(String urlString)` | 获得请求的响应码. 默认 HttpMethodType#GET 请求 |
| `com.feilong.net.http.HttpClientUtil` | `int getResponseStatusCode(String urlString,ConnectionConfig connectionConfig)` | 获得请求的响应码. 默认 HttpMethodType#GET 请求 |
| `com.feilong.net.http.HttpFullInfo` | `ConnectionConfig getConnectionConfig()` | 【原文待译】Gets the connection config. |
| `com.feilong.net.http.HttpFullInfo` | `HttpRequest getHttpRequest()` | 【原文待译】Gets the http request. |
| `com.feilong.net.http.HttpFullInfo` | `HttpResponse getHttpResponse()` | 【原文待译】Gets the http response. |
| `com.feilong.net.http.HttpFullInfo` | `T getResultBean()` | 获得 转换的bean. |
| `com.feilong.net.http.HttpFullInfo` | `UncheckedHttpException getUncheckedHttpException()` | 获得 如果有异常. |
| `com.feilong.net.http.HttpFullInfo` | `void setConnectionConfig(ConnectionConfig connectionConfig)` | 【原文待译】Sets the connection config. |
| `com.feilong.net.http.HttpFullInfo` | `void setHttpRequest(HttpRequest httpRequest)` | 【原文待译】Sets the http request. |
| `com.feilong.net.http.HttpFullInfo` | `void setHttpResponse(HttpResponse httpResponse)` | 【原文待译】Sets the http response. |
| `com.feilong.net.http.HttpFullInfo` | `void setResultBean(T resultBean)` | 设置 转换的bean. |
| `com.feilong.net.http.HttpFullInfo` | `void setUncheckedHttpException(UncheckedHttpException uncheckedHttpException)` | 设置 如果有异常. |
| `com.feilong.net.http.HttpLogHelper` | `String autoLog(HttpRequest httpRequest,ConnectionConfig connectionConfig,String messagePattern,Object... params)` | 自动追加request简单信息. |
| `com.feilong.net.http.HttpLogHelper` | `String autoLog(HttpRequest httpRequest,HttpResponse resultResponse,ConnectionConfig connectionConfig,String messagePattern,Object... params)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.http.HttpLogHelper` | `String autoLog(HttpRequest httpRequest,String messagePattern,Object... params)` | 自动追加request简单信息. |
| `com.feilong.net.http.HttpMethodType` | `HttpMethodType getByMethodValueIgnoreCase(String methodValue)` | 传入一个字符串的 HTTP method,比如 get,得到 HttpMethodType#GET. |
| `com.feilong.net.http.HttpMethodType` | `String getMethod()` | 【原文待译】Gets the method. |
| `com.feilong.net.http.HttpRequest` | `HttpMethodType getHttpMethodType()` | 获得 请求method 类型,默认 HttpMethodType#GET. |
| `com.feilong.net.http.HttpRequest` | `Map<String, String> getHeaderMap()` | 获得 请求头 信息. |
| `com.feilong.net.http.HttpRequest` | `Map<String, String> getParamMap()` | 获得 http 请求 key-value 参数map. |
| `com.feilong.net.http.HttpRequest` | `RequestByteArrayBody getRequestByteArrayBody()` | 获得 二进制数据:请求体可以包含二进制数据，如文件、图像、音频等。 这些数据通常以字节流的形式传递。. |
| `com.feilong.net.http.HttpRequest` | `String getFullEncodedUrl()` | 完整的请求路径. |
| `com.feilong.net.http.HttpRequest` | `String getLogTraceContext()` | 日志追踪上下文. 所有的feilong http此次调用的log 都会拼上改日志字符串 |
| `com.feilong.net.http.HttpRequest` | `String getRequestBody()` | 获得 请求正文,比如 webservice 可以传递 xml/json数据体. |
| `com.feilong.net.http.HttpRequest` | `String getUri()` | 获得 请求的uri地址. 如果uri是null,将返回empty 如果uri中有空格,将会替换成%20 |
| `com.feilong.net.http.HttpRequest` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.http.HttpRequest` | `boolean getIsTrimUri()` | 是否uri trim. 有时候程序员在配置uri 的时候,会误操作 uri 前后会多出空格, 这样会导致一些功能不work,要排查好久, 理论上uri前后是没有空格的, 所以默认为true ,会自动去除前后的空格; 如果真的有特殊需求, 可以设置为false |
| `com.feilong.net.http.HttpRequest` | `void setHeaderMap(Map<String, String> headerMap)` | 设置 请求头 信息. |
| `com.feilong.net.http.HttpRequest` | `void setHttpMethodType(HttpMethodType httpMethodType)` | 设置 请求method 类型,默认 HttpMethodType#GET. |
| `com.feilong.net.http.HttpRequest` | `void setIsTrimUri(boolean isTrimUri)` | 是否uri trim. 有时候程序员在配置uri 的时候,会误操作 uri 前后会多出空格, 这样会导致一些功能不work,要排查好久, 理论上uri前后是没有空格的, 所以默认为true ,会自动去除前后的空格; 如果真的有特殊需求, 可以设置为false |
| `com.feilong.net.http.HttpRequest` | `void setLogTraceContext(String logTraceContext)` | 日志追踪上下文. 所有的feilong http此次调用的log 都会拼上改日志字符串 |
| `com.feilong.net.http.HttpRequest` | `void setParamMap(Map<String, String> paramMap)` | 设置 http 请求 key-value 参数map. |
| `com.feilong.net.http.HttpRequest` | `void setRequestBody(String requestBody)` | 设置 请求正文,比如 webservice 可以传递 xml/json数据体. |
| `com.feilong.net.http.HttpRequest` | `void setRequestByteArrayBody(RequestByteArrayBody requestByteArrayBody)` | 设置 二进制数据:请求体可以包含二进制数据，如文件、图像、音频等。 这些数据通常以字节流的形式传递。. |
| `com.feilong.net.http.HttpRequest` | `void setUri(String uri)` | 设置 请求的uri地址. |
| `com.feilong.net.http.HttpResponse` | `Map<String, String> getHeaderMap()` | 获得 响应头信息. |
| `com.feilong.net.http.HttpResponse` | `String getResultString()` | 获得 响应的结果字符串. |
| `com.feilong.net.http.HttpResponse` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.http.HttpResponse` | `int getStatusCode()` | 获得 响应的状态码. |
| `com.feilong.net.http.HttpResponse` | `long getUseTime()` | 获得 耗时时间, 毫秒 . |
| `com.feilong.net.http.HttpResponse` | `void setHeaderMap(Map<String, String> headerMap)` | 设置 响应头信息. |
| `com.feilong.net.http.HttpResponse` | `void setResultString(String resultString)` | 设置 响应的结果字符串. |
| `com.feilong.net.http.HttpResponse` | `void setStatusCode(int statusCode)` | 设置 响应的状态码. |
| `com.feilong.net.http.HttpResponse` | `void setUseTime(long useTime)` | 设置 耗时时间, 毫秒 . |
| `com.feilong.net.http.RequestByteArrayBody` | `Integer getLength()` | 获得 maximum number of bytes to read from the buffer. |
| `com.feilong.net.http.RequestByteArrayBody` | `Integer getOff()` | 获得 offset in the buffer of the first byte to read. |
| `com.feilong.net.http.RequestByteArrayBody` | `String getMimeType()` | 获得 mime type. |
| `com.feilong.net.http.RequestByteArrayBody` | `byte[] getBuf()` | 获得 an array of bytes that was provided by the creator of the stream. |
| `com.feilong.net.http.RequestByteArrayBody` | `void setBuf(byte[] buf)` | 设置 an array of bytes that was provided by the creator of the stream. |
| `com.feilong.net.http.RequestByteArrayBody` | `void setLength(Integer length)` | 设置 maximum number of bytes to read from the buffer. |
| `com.feilong.net.http.RequestByteArrayBody` | `void setMimeType(String mimeType)` | 设置 mime type. |
| `com.feilong.net.http.RequestByteArrayBody` | `void setOff(Integer off)` | 设置 offset in the buffer of the first byte to read. |
