# com.feilong.context.invoker

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.context.invoker.AbstractResponseCommandBuilder` | `T build(R request)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.invoker.AbstractResponseStringBuilder` | `String build(T request)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.invoker.AbstractResponseStringBuilder` | `void setFormat(String format)` | 字符串格式化,用来简化 StringFormatter 配置. 优先级 stringFormatter> format |
| `com.feilong.context.invoker.AbstractResponseStringBuilder` | `void setResponseStringRebuilder(Rebuilder<String> responseStringRebuilder)` | 再加工器. 一般情况下用不到 支持在获得 responseString 之后,再次加工 典型应用,cc 视频, 返回 |
| `com.feilong.context.invoker.AbstractResponseStringBuilder` | `void setStringFormatter(StringFormatter stringFormatter)` | 设置 字符串格式化器. |
| `com.feilong.context.invoker.DataAndInvokerResultHandler` | `void handle(D data,I invokerResult)` | 【原文待译】Handler. |
| `com.feilong.context.invoker.DefaultRequestResultInvoker` | `N doHandler(R request)` | 【原文待译】Do handler. |
| `com.feilong.context.invoker.DefaultRequestResultInvoker` | `N invoke(R queryRequest)` | 【原文待译】Invoke. |
| `com.feilong.context.invoker.DefaultRequestResultInvoker` | `void setInvokerRequestValidator(InvokerRequestValidator<R> invokerRequestValidator)` | 设置 请求参数自定义校验. |
| `com.feilong.context.invoker.DefaultRequestResultInvoker` | `void setInvokerResultConverter(InvokerResultConverter<R, T, N> invokerResultConverter)` | 设置 将对象转换成 InvokerResult. |
| `com.feilong.context.invoker.DefaultRequestResultInvoker` | `void setResponseStringBuilder(ResponseStringBuilder<R> responseStringBuilder)` | 设置 调用结果构造器. |
| `com.feilong.context.invoker.DefaultRequestResultInvoker` | `void setStringToBeanConverter(StringToBeanConverter<T> stringToBeanConverter)` | 设置 字符串转换成bean 转换器. |
| `com.feilong.context.invoker.DefaultResponseCommandBuilder` | `void setResponseStringBuilder(ResponseStringBuilder<R> responseStringBuilder)` | 设置 响应结果字符串构造器. |
| `com.feilong.context.invoker.DefaultResponseCommandBuilder` | `void setStringToBeanConverter(StringToBeanConverter<T> stringToBeanConverter)` | 设置 字符串转换成bean 转换器. |
| `com.feilong.context.invoker.DefaultResponseHandler` | `void handle(R request)` | 【原文待译】Handle. |
| `com.feilong.context.invoker.DefaultResponseHandler` | `void setResponseStringBuilder(ResponseStringBuilder<R> responseStringBuilder)` | 设置 响应结果字符串构造器. |
| `com.feilong.context.invoker.DefaultResponseHandler` | `void setResponseStringHandler(ResponseStringHandler<R> responseStringHandler)` | 设置 处理响应字符串和请求对象. |
| `com.feilong.context.invoker.InvokerRequestValidator` | `void validate(T request)` | Validate. 失败请自行抛出异常 |
| `com.feilong.context.invoker.InvokerResultConverter` | `N convert(R request,String invokerResponse,T t)` | 将请求 request , 接口响应的字符串 invokerResponse , 以及字符串转后的对象 t , 转成 指定的结果类型. |
| `com.feilong.context.invoker.RequestArrayParamsBuilder` | `Object[] build(T request)` | 用来基于 request 构造 Object 数组的方法. 常用于 com.feilong.context.invoker.jaxws.JaxWsDynamicResponseStringBuilder |
| `com.feilong.context.invoker.RequestParamsBuilder` | `Map<String, String> build(T request)` | 用来基于 request 构造 Map 参数的方法. 常用于 com.feilong.context.invoker.http.DefaultHttpRequestBuilder |
| `com.feilong.context.invoker.RequestResultInvoker` | `K invoke(T request)` | 调用. |
| `com.feilong.context.invoker.ResponseCommandBuilder` | `T build(R request)` | 通过发送请求,得到响应的对象. |
| `com.feilong.context.invoker.ResponseHandler` | `void handle(R request)` | 处理某个请求. |
| `com.feilong.context.invoker.ResponseStringBuilder` | `String build(T request)` | 通过发送请求,得到响应的字符串. |
| `com.feilong.context.invoker.ResponseStringHandler` | `void handle(String responseString,R request)` | 处理响应字符串和 请求request. |
| `com.feilong.context.invoker.SimpleHttpAndJsonResponseCommandBuilder` | `void setHeaderMap(Map<String, String> headerMap)` | 设置 http请求头. |
| `com.feilong.context.invoker.SimpleHttpAndJsonResponseCommandBuilder` | `void setMethod(String method)` | 设置 http请求method. |
| `com.feilong.context.invoker.SimpleHttpAndJsonResponseCommandBuilder` | `void setRequestBodyBuilder(RequestBodyBuilder<R> requestBodyBuilder)` | 设置 请求体构造器. |
| `com.feilong.context.invoker.SimpleHttpAndJsonResponseCommandBuilder` | `void setRequestParamsBuilder(RequestParamsBuilder<R> requestParamsBuilder)` | 设置 请求参数构造器. |
| `com.feilong.context.invoker.SimpleHttpAndJsonResponseCommandBuilder` | `void setResponseCommandRootClass(Class<T> rootClass)` | 设置 结果转换的类型. |
| `com.feilong.context.invoker.SimpleHttpAndJsonResponseCommandBuilder` | `void setUri(String uri)` | 设置 提交地址. |
