# cn.hutool.http.server

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.http.server.HttpExchangeWrapper` | `Headers getRequestHeaders()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `Headers getResponseHeaders()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `HttpContext getHttpContext()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `HttpExchange getRaw()` | 获取原始对象 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `HttpPrincipal getPrincipal()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `HttpServerRequest getRequest()` | 获取请求 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `HttpServerResponse getResponse()` | 获取响应 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `InetSocketAddress getLocalAddress()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `InetSocketAddress getRemoteAddress()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `InputStream getRequestBody()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `Object getAttribute(final String name)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `OutputStream getResponseBody()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `String getProtocol()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `String getRequestMethod()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `URI getRequestURI()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `int getResponseCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `void sendResponseHeaders(final int rCode,final long responseLength)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `void setAttribute(final String name,final Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpExchangeWrapper` | `void setStreams(final InputStream i,final OutputStream o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.server.HttpServerBase` | `HttpContext getHttpContext()` | 获取HttpContext |
| `cn.hutool.http.server.HttpServerBase` | `HttpExchange getHttpExchange()` | 获取HttpExchange对象 |
| `cn.hutool.http.server.HttpServerBase` | `void close()` | 调用HttpExchange#close()，关闭请求流和响应流 |
| `cn.hutool.http.server.HttpServerRequest` | `Charset getCharset()` | 获取编码，获取失败默认使用UTF-8，获取规则如下： |
| `cn.hutool.http.server.HttpServerRequest` | `Collection<HttpCookie> getCookies()` | 获得Cookie信息列表 |
| `cn.hutool.http.server.HttpServerRequest` | `Headers getHeaders()` | 获得请求header中的信息 |
| `cn.hutool.http.server.HttpServerRequest` | `HttpCookie getCookie(String cookieName)` | 获得指定Cookie名对应的HttpCookie对象 |
| `cn.hutool.http.server.HttpServerRequest` | `InputStream getBodyStream()` | 获取请求体的流，流中可以读取请求内容，包括请求表单数据或文件上传数据 |
| `cn.hutool.http.server.HttpServerRequest` | `List<String> getParams(String name)` | 获取指定名称的参数值 |
| `cn.hutool.http.server.HttpServerRequest` | `ListValueMap<String, String> getParams()` | 获取参数Map |
| `cn.hutool.http.server.HttpServerRequest` | `Map<String, HttpCookie> getCookieMap()` | 获得Cookie信息Map，键为Cookie名，值为HttpCookie对象 |
| `cn.hutool.http.server.HttpServerRequest` | `MultipartFormData getMultipart()` | 获得MultiPart表单内容，多用于获得上传的文件 |
| `cn.hutool.http.server.HttpServerRequest` | `MultipartFormData parseMultipart(UploadSetting uploadSetting)` | 获得multipart/form-data 表单内容 包括文件和普通表单数据 在同一次请求中，此方法只能被执行一次！ |
| `cn.hutool.http.server.HttpServerRequest` | `String getBody()` | 获取请求体文本，可以是form表单、json、xml等任意内容 使用#getCharset()判断编码，判断失败使用UTF-8编码 |
| `cn.hutool.http.server.HttpServerRequest` | `String getBody(Charset charset)` | 获取请求体文本，可以是form表单、json、xml等任意内容 |
| `cn.hutool.http.server.HttpServerRequest` | `String getClientIP(String... otherHeaderNames)` | 获取客户端IP 默认检测的Header: |
| `cn.hutool.http.server.HttpServerRequest` | `String getClientIPByHeader(String... headerNames)` | 获取客户端IP headerNames参数用于自定义检测的Header 需要注意的是，使用此方法获取的客户IP地址必须在Http服务器（例如Nginx）中配置头信息，否则容易造成IP伪造。 |
| `cn.hutool.http.server.HttpServerRequest` | `String getContentType()` | 获取Content-Type头信息 |
| `cn.hutool.http.server.HttpServerRequest` | `String getCookiesStr()` | 获得Cookie信息字符串 |
| `cn.hutool.http.server.HttpServerRequest` | `String getHeader(Header headerKey)` | 获得请求header中的信息 |
| `cn.hutool.http.server.HttpServerRequest` | `String getHeader(String headerKey)` | 获得请求header中的信息 |
| `cn.hutool.http.server.HttpServerRequest` | `String getHeader(String headerKey,Charset charset)` | 获得请求header中的信息 |
| `cn.hutool.http.server.HttpServerRequest` | `String getMethod()` | 获得Http Method |
| `cn.hutool.http.server.HttpServerRequest` | `String getParam(String name)` | 获取指定名称的参数值，取第一个值 |
| `cn.hutool.http.server.HttpServerRequest` | `String getPath()` | 获得请求路径Path |
| `cn.hutool.http.server.HttpServerRequest` | `String getQuery()` | 获取请求参数 |
| `cn.hutool.http.server.HttpServerRequest` | `String getUserAgentStr()` | 获得User-Agent |
| `cn.hutool.http.server.HttpServerRequest` | `URI getURI()` | 获得请求URI |
| `cn.hutool.http.server.HttpServerRequest` | `UserAgent getUserAgent()` | 获得User-Agent，未识别返回null |
| `cn.hutool.http.server.HttpServerRequest` | `boolean isGetMethod()` | 是否为GET请求 |
| `cn.hutool.http.server.HttpServerRequest` | `boolean isMultipart()` | 是否为Multipart类型表单，此类型表单用于文件上传 |
| `cn.hutool.http.server.HttpServerRequest` | `boolean isPostMethod()` | 是否为POST请求 |
| `cn.hutool.http.server.HttpServerRequest` | `byte[] getBodyBytes()` | 获取body的bytes数组 |
| `cn.hutool.http.server.HttpServerResponse` | `Headers getHeaders()` | 获得所有响应头，获取后可以添加新的响应头 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse addHeader(String header,String value)` | 添加响应头，如果已经存在，则追加 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse send(int httpStatusCode)` | 发送HTTP状态码，Content-Length为0不定长度，会输出Transfer-encoding: chunked |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse send(int httpStatusCode,long bodyLength)` | 发送HTTP状态码 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse send404(String content)` | 发送404错误页 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse sendError(int errorCode,String content)` | 发送错误页 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse sendOk()` | 发送成功状态码 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse sendOk(int bodyLength)` | 发送成功状态码 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse setAttr(String name,Object value)` | 设置属性 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse setCharset(Charset charset)` | 设置响应的编码 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse setContentLength(long contentLength)` | 设置Content-Length头 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse setContentType(String contentType)` | 设置Content-Type头，类似于:text/html;charset=utf-8 如果用户传入的信息无charset信息，自动根据charset补充，charset设置见#setCharset(Charset) |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse setHeader(Header header,String value)` | 设置响应头，如果已经存在，则覆盖 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse setHeader(String header,List<String> value)` | 设置响应头，如果已经存在，则覆盖 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse setHeader(String header,String value)` | 设置响应头，如果已经存在，则覆盖 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse setHeaders(Map<String, List<String>> headers)` | 设置所有响应头，如果已经存在，则覆盖 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse write(File file)` | 返回文件给客户端（文件下载） |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse write(File file,String fileName)` | 返回文件给客户端（文件下载） |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse write(InputStream in)` | 写出数据到客户端 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse write(InputStream in,String contentType)` | 返回数据给客户端 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse write(InputStream in,int length)` | 写出数据到客户端 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse write(InputStream in,int length,String contentType)` | 返回数据给客户端 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse write(InputStream in,int length,String contentType,String fileName)` | 返回文件数据给客户端（文件下载） |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse write(String data)` | 写出数据到客户端 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse write(String data,String contentType)` | 写出数据到客户端 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse write(byte[] data)` | 写出数据到客户端 |
| `cn.hutool.http.server.HttpServerResponse` | `HttpServerResponse write(byte[] data,String contentType)` | 写出数据到客户端 |
| `cn.hutool.http.server.HttpServerResponse` | `OutputStream getOut()` | 获取响应数据流 |
| `cn.hutool.http.server.HttpServerResponse` | `PrintWriter getWriter()` | 获取响应数据流 |
| `cn.hutool.http.server.HttpServerResponse` | `void write(InputStream in,String contentType,String fileName)` | 返回文件数据给客户端（文件下载） |
| `cn.hutool.http.server.SimpleServer` | `HttpContext createContext(String path,HttpHandler handler)` | 创建请求映射上下文，创建后，用户访问指定路径可使用HttpHandler 中的规则进行处理 |
| `cn.hutool.http.server.SimpleServer` | `HttpServer getRawServer()` | 获得原始HttpServer对象 |
| `cn.hutool.http.server.SimpleServer` | `InetSocketAddress getAddress()` | 获取服务器地址信息 |
| `cn.hutool.http.server.SimpleServer` | `SimpleServer addAction(String path,Action action)` | 增加请求处理规则 |
| `cn.hutool.http.server.SimpleServer` | `SimpleServer addFilter(Filter filter)` | 增加请求过滤器，此过滤器对所有请求有效 此方法需在以下方法前之前调用： #setRoot(File) #setRoot(String) #createContext(String, HttpHandler) #addHandler(String, HttpHandler) #addAction(String, Action) |
| `cn.hutool.http.server.SimpleServer` | `SimpleServer addFilter(HttpFilter filter)` | 增加请求过滤器，此过滤器对所有请求有效 此方法需在以下方法前之前调用： #setRoot(File) #setRoot(String) #createContext(String, HttpHandler) #addHandler(String, HttpHandler) #addAction(String, Action) |
| `cn.hutool.http.server.SimpleServer` | `SimpleServer addHandler(String path,HttpHandler handler)` | 增加请求处理规则 |
| `cn.hutool.http.server.SimpleServer` | `SimpleServer setExecutor(Executor executor)` | 设置自定义线程池 |
| `cn.hutool.http.server.SimpleServer` | `SimpleServer setRoot(File root)` | 设置根目录，默认的页面从root目录中读取解析返回 |
| `cn.hutool.http.server.SimpleServer` | `SimpleServer setRoot(String root)` | 设置根目录，默认的页面从root目录中读取解析返回 |
| `cn.hutool.http.server.SimpleServer` | `void start()` | 启动Http服务器，启动后会阻塞当前线程 |
