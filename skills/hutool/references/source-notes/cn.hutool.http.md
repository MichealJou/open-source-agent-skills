# cn.hutool.http

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.http.ContentType` | `ContentType get(String body)` | 从请求参数的body中判断请求的Content-Type类型，支持的类型有： |
| `cn.hutool.http.ContentType` | `String build(ContentType contentType,Charset charset)` | 输出Content-Type字符串，附带编码信息 |
| `cn.hutool.http.ContentType` | `String build(String contentType,Charset charset)` | 输出Content-Type字符串，附带编码信息 |
| `cn.hutool.http.ContentType` | `String getValue()` | 获取value值 |
| `cn.hutool.http.ContentType` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.ContentType` | `String toString(Charset charset)` | 输出Content-Type字符串，附带编码信息 |
| `cn.hutool.http.ContentType` | `boolean isDefault(String contentType)` | 是否为默认Content-Type，默认包括null和application/x-www-form-urlencoded |
| `cn.hutool.http.ContentType` | `boolean isFormUrlEncode(String contentType)` | 是否为application/x-www-form-urlencoded |
| `cn.hutool.http.GlobalHeaders` | `GlobalHeaders clearHeaders()` | 清除所有头信息，包括全局头信息 |
| `cn.hutool.http.GlobalHeaders` | `GlobalHeaders header(Header name,String value)` | 设置一个header 覆盖模式，则替换之前的值 |
| `cn.hutool.http.GlobalHeaders` | `GlobalHeaders header(Header name,String value,boolean isOverride)` | 设置一个header 如果覆盖模式，则替换之前的值，否则加入到值列表中 |
| `cn.hutool.http.GlobalHeaders` | `GlobalHeaders header(Map<String, List<String>> headers)` | 设置请求头 不覆盖原有请求头 |
| `cn.hutool.http.GlobalHeaders` | `GlobalHeaders header(String name,String value)` | 设置一个header 覆盖模式，则替换之前的值 |
| `cn.hutool.http.GlobalHeaders` | `GlobalHeaders header(String name,String value,boolean isOverride)` | 设置一个header 如果覆盖模式，则替换之前的值，否则加入到值列表中 |
| `cn.hutool.http.GlobalHeaders` | `GlobalHeaders putDefault(boolean isReset)` | 加入默认的头部信息 |
| `cn.hutool.http.GlobalHeaders` | `GlobalHeaders removeHeader(Header name)` | 移除一个头信息 |
| `cn.hutool.http.GlobalHeaders` | `GlobalHeaders removeHeader(String name)` | 移除一个头信息 |
| `cn.hutool.http.GlobalHeaders` | `List<String> headerList(String name)` | 根据name获取头信息列表 |
| `cn.hutool.http.GlobalHeaders` | `Map<String, List<String>> headers()` | 获取headers |
| `cn.hutool.http.GlobalHeaders` | `String header(Header name)` | 根据name获取头信息 |
| `cn.hutool.http.GlobalHeaders` | `String header(String name)` | 根据name获取头信息 |
| `cn.hutool.http.GlobalInterceptor` | `GlobalInterceptor addRequestInterceptor(HttpInterceptor<HttpRequest> interceptor)` | 设置拦截器，用于在请求前重新编辑请求 |
| `cn.hutool.http.GlobalInterceptor` | `GlobalInterceptor addResponseInterceptor(HttpInterceptor<HttpResponse> interceptor)` | 设置拦截器，用于在响应读取后完成编辑或读取 |
| `cn.hutool.http.GlobalInterceptor` | `GlobalInterceptor clear()` | 清空请求和响应拦截器 |
| `cn.hutool.http.GlobalInterceptor` | `GlobalInterceptor clearRequest()` | 清空请求拦截器 |
| `cn.hutool.http.GlobalInterceptor` | `GlobalInterceptor clearResponse()` | 清空响应拦截器 |
| `cn.hutool.http.HTMLFilter` | `String chr(final int decimal)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HTMLFilter` | `String filter(final String input)` | 【原文待译】given a user submitted input String, filter out any invalid or restricted html. |
| `cn.hutool.http.HTMLFilter` | `String htmlSpecialChars(final String s)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HTMLFilter` | `boolean isAlwaysMakeTags()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HTMLFilter` | `boolean isStripComments()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.Header` | `String getValue()` | 获取值 |
| `cn.hutool.http.Header` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HtmlUtil` | `String cleanEmptyTag(String content)` | 清除所有HTML空标签 例如：<p></p> |
| `cn.hutool.http.HtmlUtil` | `String cleanHtmlTag(String content)` | 清除所有HTML标签，但是不删除标签内的内容 |
| `cn.hutool.http.HtmlUtil` | `String escape(String text)` | 转义文本中的HTML字符为安全的字符，以下字符被转义： ' 替换为 &#039; (&apos; doesn't work in HTML4) " 替换为 &quot; & 替换为 &amp; < 替换为 &lt; > 替换为 &gt; |
| `cn.hutool.http.HtmlUtil` | `String filter(String htmlContent)` | 过滤HTML文本，防止XSS攻击 |
| `cn.hutool.http.HtmlUtil` | `String removeAllHtmlAttr(String content,String... tagNames)` | 去除指定标签的所有属性 |
| `cn.hutool.http.HtmlUtil` | `String removeHtmlAttr(String content,String... attrs)` | 去除HTML标签中的属性，如果多个标签有相同属性，都去除 |
| `cn.hutool.http.HtmlUtil` | `String removeHtmlTag(String content,String... tagNames)` | 清除指定HTML标签和被标签包围的内容 不区分大小写 |
| `cn.hutool.http.HtmlUtil` | `String removeHtmlTag(String content,boolean withTagContent,String... tagNames)` | 清除指定HTML标签 不区分大小写 |
| `cn.hutool.http.HtmlUtil` | `String unescape(String htmlStr)` | 还原被转义的HTML特殊字符 |
| `cn.hutool.http.HtmlUtil` | `String unwrapHtmlTag(String content,String... tagNames)` | 清除指定HTML标签，不包括内容 不区分大小写 |
| `cn.hutool.http.HttpBase` | `List<String> headerList(String name)` | 根据name获取头信息列表 |
| `cn.hutool.http.HttpBase` | `Map<String, List<String>> headers()` | 获取headers |
| `cn.hutool.http.HttpBase` | `String charset()` | 返回字符集 |
| `cn.hutool.http.HttpBase` | `String header(Header name)` | 根据name获取头信息 |
| `cn.hutool.http.HttpBase` | `String header(String name)` | 根据name获取头信息 根据RFC2616规范，header的name不区分大小写 |
| `cn.hutool.http.HttpBase` | `String httpVersion()` | 返回http版本 |
| `cn.hutool.http.HttpBase` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpBase` | `T addHeaders(Map<String, String> headers)` | 新增请求头 不覆盖原有请求头 |
| `cn.hutool.http.HttpBase` | `T charset(Charset charset)` | 设置字符集 |
| `cn.hutool.http.HttpBase` | `T charset(String charset)` | 设置字符集 |
| `cn.hutool.http.HttpBase` | `T clearHeaders()` | 清除所有头信息，包括全局头信息 |
| `cn.hutool.http.HttpBase` | `T header(Header name,String value)` | 设置一个header 覆盖模式，则替换之前的值 |
| `cn.hutool.http.HttpBase` | `T header(Header name,String value,boolean isOverride)` | 设置一个header 如果覆盖模式，则替换之前的值，否则加入到值列表中 |
| `cn.hutool.http.HttpBase` | `T header(Map<String, List<String>> headers)` | 设置请求头 不覆盖原有请求头 |
| `cn.hutool.http.HttpBase` | `T header(Map<String, List<String>> headers,boolean isOverride)` | 设置请求头 |
| `cn.hutool.http.HttpBase` | `T header(String name,String value)` | 设置一个header 覆盖模式，则替换之前的值 |
| `cn.hutool.http.HttpBase` | `T header(String name,String value,boolean isOverride)` | 设置一个header 如果覆盖模式，则替换之前的值，否则加入到值列表中 |
| `cn.hutool.http.HttpBase` | `T headerAggregation(boolean aggregate)` | 设置是否需要聚合重复的请求头，将重复的请求头聚合为,拼接 |
| `cn.hutool.http.HttpBase` | `T headerMap(Map<String, String> headers,boolean isOverride)` | 设置请求头 |
| `cn.hutool.http.HttpBase` | `T httpVersion(String httpVersion)` | 设置http版本，此方法不会影响到实际请求的HTTP版本，只用于帮助判断是否connect:Keep-Alive |
| `cn.hutool.http.HttpBase` | `T removeHeader(Header name)` | 移除一个头信息 |
| `cn.hutool.http.HttpBase` | `T removeHeader(String name)` | 移除一个头信息 |
| `cn.hutool.http.HttpBase` | `boolean isHeaderAggregated()` | 获取是否需要聚合请求头状态 |
| `cn.hutool.http.HttpBase` | `byte[] bodyBytes()` | 获取bodyBytes存储字节码 |
| `cn.hutool.http.HttpConfig` | `HttpConfig addRequestInterceptor(HttpInterceptor<HttpRequest> interceptor)` | 设置拦截器，用于在请求前重新编辑请求 |
| `cn.hutool.http.HttpConfig` | `HttpConfig addResponseInterceptor(HttpInterceptor<HttpResponse> interceptor)` | 设置拦截器，用于在请求前重新编辑请求 |
| `cn.hutool.http.HttpConfig` | `HttpConfig create()` | 创建默认Http配置信息 |
| `cn.hutool.http.HttpConfig` | `HttpConfig disableCache()` | 禁用缓存 |
| `cn.hutool.http.HttpConfig` | `HttpConfig setBlockSize(int blockSize)` | 采用流方式上传数据，无需本地缓存数据。 HttpUrlConnection默认是将所有数据读到本地缓存，然后再发送给服务器，这样上传大文件时就会导致内存溢出。 |
| `cn.hutool.http.HttpConfig` | `HttpConfig setConnectionTimeout(int milliseconds)` | 设置连接超时，单位：毫秒 |
| `cn.hutool.http.HttpConfig` | `HttpConfig setDecodeUrl(boolean decodeUrl)` | 设置是否忽略解码URL，包括URL中的Path部分和Param部分。 在构建Http请求时，用户传入的URL可能有编码后和未编码的内容混合在一起，如果此参数为true，则会统一解码编码后的参数， 按照RFC3986规范，在发送请求时，全部编码之。如果为false，则不会解码已经编码的内容，在请求时只编码需要编码的部分。 |
| `cn.hutool.http.HttpConfig` | `HttpConfig setFollowRedirectsCookie(boolean followRedirectsCookie)` | 自动重定向时是否处理cookie |
| `cn.hutool.http.HttpConfig` | `HttpConfig setHostnameVerifier(HostnameVerifier hostnameVerifier)` | 设置域名验证器 只针对HTTPS请求，如果不设置，不做验证，所有域名被信任 |
| `cn.hutool.http.HttpConfig` | `HttpConfig setHttpProxy(String host,int port)` | 设置Http代理 |
| `cn.hutool.http.HttpConfig` | `HttpConfig setIgnoreContentLength(boolean ignoreContentLength)` | 设置是否忽略Content-Length，如果为true，则忽略Content-Length，自动根据响应内容计算Content-Length |
| `cn.hutool.http.HttpConfig` | `HttpConfig setIgnoreEOFError(boolean ignoreEOFError)` | 设置是否忽略响应读取时可能的EOF异常。 在Http协议中，对于Transfer-Encoding: Chunked在正常情况下末尾会写入一个Length为0的的chunk标识完整结束。 如果服务端未遵循这个规范或响应没有正常结束，会报EOF异常，此选项用于是否忽略这个异常。 |
| `cn.hutool.http.HttpConfig` | `HttpConfig setInterceptorOnRedirect(boolean interceptorOnRedirect)` | 重定向时是否使用拦截器 |
| `cn.hutool.http.HttpConfig` | `HttpConfig setMaxRedirectCount(int maxRedirectCount)` | 设置最大重定向次数 如果次数小于1则表示不重定向，大于等于1表示打开重定向 |
| `cn.hutool.http.HttpConfig` | `HttpConfig setProxy(Proxy proxy)` | 设置代理 |
| `cn.hutool.http.HttpConfig` | `HttpConfig setReadTimeout(int milliseconds)` | 设置连接超时，单位：毫秒 |
| `cn.hutool.http.HttpConfig` | `HttpConfig setSSLProtocol(String protocol)` | 设置HTTPS安全连接协议，只针对HTTPS请求，可以使用的协议包括： 此方法调用后#setSSLSocketFactory(SSLSocketFactory) 将被覆盖。 |
| `cn.hutool.http.HttpConfig` | `HttpConfig setSSLSocketFactory(SSLSocketFactory ssf)` | 设置SSLSocketFactory 只针对HTTPS请求，如果不设置，使用默认的SSLSocketFactory 默认SSLSocketFactory为：SSLSocketFactoryBuilder.create().build(); |
| `cn.hutool.http.HttpConfig` | `HttpConfig setUseDefaultContentTypeIfNull(boolean useDefaultContentTypeIfNull)` | 设置是否使用默认Content-Type，如果请求中未设置Content-Type，是否使用默认值 |
| `cn.hutool.http.HttpConfig` | `HttpConfig timeout(int milliseconds)` | 设置超时，单位：毫秒 超时包括： |
| `cn.hutool.http.HttpConnection` | `Charset getCharset()` | 获取字符集编码 从Http连接的头信息中获得字符集 从ContentType中获取 |
| `cn.hutool.http.HttpConnection` | `HttpConnection connect()` | 连接 |
| `cn.hutool.http.HttpConnection` | `HttpConnection create(String urlStr,Proxy proxy)` | 创建HttpConnection |
| `cn.hutool.http.HttpConnection` | `HttpConnection create(URL url,Proxy proxy)` | 创建HttpConnection |
| `cn.hutool.http.HttpConnection` | `HttpConnection disableCache()` | 关闭缓存 |
| `cn.hutool.http.HttpConnection` | `HttpConnection disconnect()` | 断开连接 |
| `cn.hutool.http.HttpConnection` | `HttpConnection disconnectQuietly()` | 静默断开连接。不抛出异常 |
| `cn.hutool.http.HttpConnection` | `HttpConnection header(Header header,String value,boolean isOverride)` | 设置请求头 当请求头存在时，覆盖之 |
| `cn.hutool.http.HttpConnection` | `HttpConnection header(Map<String, List<String>> headerMap,boolean isOverride)` | 设置请求头 不覆盖原有请求头 |
| `cn.hutool.http.HttpConnection` | `HttpConnection header(Map<String, List<String>> headerMap,boolean isOverride,boolean isHeaderAggregated)` | 设置请求头 不覆盖原有请求头并判断是否需要聚合请求头 |
| `cn.hutool.http.HttpConnection` | `HttpConnection header(String header,String value,boolean isOverride)` | 设置请求头 当请求头存在时，覆盖之 |
| `cn.hutool.http.HttpConnection` | `HttpConnection initConn()` | 初始化连接相关信息 |
| `cn.hutool.http.HttpConnection` | `HttpConnection setChunkedStreamingMode(int blockSize)` | 采用流方式上传数据，无需本地缓存数据。 HttpUrlConnection默认是将所有数据读到本地缓存，然后再发送给服务器，这样上传大文件时就会导致内存溢出。 |
| `cn.hutool.http.HttpConnection` | `HttpConnection setConnectTimeout(int timeout)` | 设置连接超时 |
| `cn.hutool.http.HttpConnection` | `HttpConnection setConnectionAndReadTimeout(int timeout)` | 设置连接和读取的超时时间 |
| `cn.hutool.http.HttpConnection` | `HttpConnection setCookie(String cookie)` | 设置Cookie |
| `cn.hutool.http.HttpConnection` | `HttpConnection setFixedLengthStreamingMode(long contentLength)` | 设置固定长度的流模式，会设置HTTP请求头中的Content-Length字段，告知服务器整个请求体的精确字节大小。 这在上传文件或大数据量时非常有用，因为它允许服务器准确地知道何时接收完所有的请求数据，而不需要依赖于连接的关闭来判断数据传输的结束。 |
| `cn.hutool.http.HttpConnection` | `HttpConnection setHttpsInfo(HostnameVerifier hostnameVerifier,SSLSocketFactory ssf)` | 设置https请求参数 有些时候htts请求会出现com.sun.net.ssl.internal.www.protocol.https.HttpsURLConnectionOldImpl的实现，此为sun内部api，按照普通http请求处理 |
| `cn.hutool.http.HttpConnection` | `HttpConnection setInstanceFollowRedirects(boolean isInstanceFollowRedirects)` | 设置自动HTTP 30X跳转 |
| `cn.hutool.http.HttpConnection` | `HttpConnection setMethod(Method method)` | 设置请求方法 |
| `cn.hutool.http.HttpConnection` | `HttpConnection setReadTimeout(int timeout)` | 设置读取超时 |
| `cn.hutool.http.HttpConnection` | `HttpURLConnection getHttpURLConnection()` | 获取HttpURLConnection对象 |
| `cn.hutool.http.HttpConnection` | `InputStream getErrorStream()` | 当返回错误代码时，获得错误内容流 |
| `cn.hutool.http.HttpConnection` | `InputStream getInputStream()` | 获得输入流对象 输入流对象用于读取数据 |
| `cn.hutool.http.HttpConnection` | `Map<String, List<String>> headers()` | 获取所有Http请求头 |
| `cn.hutool.http.HttpConnection` | `Method getMethod()` | 获取请求方法,GET/POST |
| `cn.hutool.http.HttpConnection` | `OutputStream getOutputStream()` | 获取输出流对象 输出流对象用于发送数据 |
| `cn.hutool.http.HttpConnection` | `Proxy getProxy()` | 获得代理 |
| `cn.hutool.http.HttpConnection` | `String getCharsetName()` | 获得字符集编码 从Http连接的头信息中获得字符集 从ContentType中获取 |
| `cn.hutool.http.HttpConnection` | `String header(Header name)` | 获取Http请求头 |
| `cn.hutool.http.HttpConnection` | `String header(String name)` | 获取Http请求头 |
| `cn.hutool.http.HttpConnection` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpConnection` | `URL getUrl()` | 获取请求URL |
| `cn.hutool.http.HttpConnection` | `int responseCode()` | 获取响应码 |
| `cn.hutool.http.HttpDownloader` | `File downloadForFile(String url,File targetFileOrDir,int timeout,StreamProgress streamProgress)` | 下载远程文件，返回文件 |
| `cn.hutool.http.HttpDownloader` | `String downloadString(String url,Charset customCharset,StreamProgress streamPress)` | 下载远程文本 |
| `cn.hutool.http.HttpDownloader` | `byte[] downloadBytes(String url)` | 下载远程文件数据，支持30x跳转 |
| `cn.hutool.http.HttpDownloader` | `byte[] downloadBytes(String url,int timeout)` | 下载远程文件数据，支持30x跳转 |
| `cn.hutool.http.HttpDownloader` | `long download(String url,OutputStream out,boolean isCloseOut,StreamProgress streamProgress)` | 下载远程文件 |
| `cn.hutool.http.HttpDownloader` | `long downloadFile(String url,File targetFileOrDir,String tempFileSuffix,int timeout,StreamProgress streamProgress)` | 下载文件-避免未完成的文件 来自：https://gitee.com/chinabugotech/hutool/pulls/407 此方法原理是先在目标文件同级目录下创建临时文件，下载之，等下载完毕后重命名，避免因下载错误导致的文件不完整。 |
| `cn.hutool.http.HttpDownloader` | `long downloadFile(String url,File targetFileOrDir,int timeout,StreamProgress streamProgress)` | 下载远程文件 |
| `cn.hutool.http.HttpGlobalConfig` | `CookieManager getCookieManager()` | 获取Cookie管理器，用于自定义Cookie管理 |
| `cn.hutool.http.HttpGlobalConfig` | `String getBoundary()` | 获取全局默认的Multipart边界 |
| `cn.hutool.http.HttpGlobalConfig` | `boolean isDecodeUrl()` | 获取是否忽略解码URL，包括URL中的Path部分和Param部分。 在构建Http请求时，用户传入的URL可能有编码后和未编码的内容混合在一起，如果此参数为true，则会统一解码编码后的参数， 按照RFC3986规范，在发送请求时，全部编码之。如果为false，则不会解码已经编码的内容，在请求时只编码需要编码的部分。 |
| `cn.hutool.http.HttpGlobalConfig` | `boolean isIgnoreEOFError()` | 获取是否忽略响应读取时可能的EOF异常。 在Http协议中，对于Transfer-Encoding: Chunked在正常情况下末尾会写入一个Length为0的的chunk标识完整结束。 如果服务端未遵循这个规范或响应没有正常结束，会报EOF异常，此选项用于是否忽略这个异常。 |
| `cn.hutool.http.HttpGlobalConfig` | `boolean isTrustAnyHost()` | 是否信任所有Host |
| `cn.hutool.http.HttpGlobalConfig` | `int getMaxRedirectCount()` | 获取全局默认的最大重定向次数，如设置0表示不重定向 如果设置为1，表示重定向一次，即请求两次 |
| `cn.hutool.http.HttpGlobalConfig` | `int getTimeout()` | 获取全局默认的超时时长 |
| `cn.hutool.http.HttpGlobalConfig` | `void allowPatch()` | 增加支持的METHOD方法 此方法通过注入方式修改HttpURLConnection中的methods静态属性，增加PATCH方法 see: https://stackoverflow.com/questions/25163131/httpurlconnection-invalid-http-method-patch |
| `cn.hutool.http.HttpGlobalConfig` | `void closeCookie()` | 关闭Cookie |
| `cn.hutool.http.HttpGlobalConfig` | `void setBoundary(String customBoundary)` | 设置默认的Multipart边界 |
| `cn.hutool.http.HttpGlobalConfig` | `void setCookieManager(CookieManager customCookieManager)` | 自定义CookieManager |
| `cn.hutool.http.HttpGlobalConfig` | `void setDecodeUrl(boolean customDecodeUrl)` | 设置是否忽略解码URL，包括URL中的Path部分和Param部分。 在构建Http请求时，用户传入的URL可能有编码后和未编码的内容混合在一起，如果此参数为true，则会统一解码编码后的参数， 按照RFC3986规范，在发送请求时，全部编码之。如果为false，则不会解码已经编码的内容，在请求时只编码需要编码的部分。 |
| `cn.hutool.http.HttpGlobalConfig` | `void setIgnoreEOFError(boolean customIgnoreEOFError)` | 设置是否忽略响应读取时可能的EOF异常。 在Http协议中，对于Transfer-Encoding: Chunked在正常情况下末尾会写入一个Length为0的的chunk标识完整结束。 如果服务端未遵循这个规范或响应没有正常结束，会报EOF异常，此选项用于是否忽略这个异常。 |
| `cn.hutool.http.HttpGlobalConfig` | `void setMaxRedirectCount(int customMaxRedirectCount)` | 设置默认全局默认的最大重定向次数，如设置0表示不重定向 如果设置为1，表示重定向一次，即请求两次 |
| `cn.hutool.http.HttpGlobalConfig` | `void setTimeout(int customTimeout)` | 设置默认的连接和读取超时时长 -1: 含义，永不超时。 如果：设置timeout = 3s(3000 ms), 那一次请求最大超时：就是：6s 官方含义：timeout of zero is interpreted as an infinite timeout. （0的超时被解释为无限超时。） 这里实际项目一定要进行修改，防止把系统拖死. 底层调用：HttpURLConnection#setReadTimeout(int) 同时设置: 读取超时 底层调用：HttpURLConnection#setConnectTimeout(int) 同时设置: 连接超时 |
| `cn.hutool.http.HttpGlobalConfig` | `void setTrustAnyHost(boolean customTrustAnyHost)` | 是否信任所有Host 见：https://github.com/chinabugotech/hutool/issues/2042 |
| `cn.hutool.http.HttpInputStream` | `boolean markSupported()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpInputStream` | `int available()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpInputStream` | `int read()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpInputStream` | `int read(byte[] b,int off,int len)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpInputStream` | `long skip(long n)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpInputStream` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpInputStream` | `void mark(int readlimit)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpInputStream` | `void reset()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpInterceptor` | `void process(T httpObj)` | 处理请求 |
| `cn.hutool.http.HttpInterceptor$Chain` | `Chain<T> addChain(HttpInterceptor<T> element)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpInterceptor$Chain` | `Chain<T> clear()` | 清空 |
| `cn.hutool.http.HttpInterceptor$Chain` | `Iterator<HttpInterceptor<T>> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpRequest` | `CookieManager getCookieManager()` | 获取Cookie管理器，用于自定义Cookie管理 |
| `cn.hutool.http.HttpRequest` | `HttpConnection getConnection()` | 获取HttpConnection 在#execute() 执行前此对象为null |
| `cn.hutool.http.HttpRequest` | `HttpRequest addInterceptor(HttpInterceptor<HttpRequest> interceptor)` | 设置拦截器，用于在请求前重新编辑请求 |
| `cn.hutool.http.HttpRequest` | `HttpRequest addRequestInterceptor(HttpInterceptor<HttpRequest> interceptor)` | 设置拦截器，用于在请求前重新编辑请求 |
| `cn.hutool.http.HttpRequest` | `HttpRequest addResponseInterceptor(HttpInterceptor<HttpResponse> interceptor)` | 设置拦截器，用于在请求前重新编辑请求 |
| `cn.hutool.http.HttpRequest` | `HttpRequest auth(String content)` | 验证，简单插入Authorization头 |
| `cn.hutool.http.HttpRequest` | `HttpRequest basicAuth(String username,String password)` | 简单验证，生成的头信息类似于： |
| `cn.hutool.http.HttpRequest` | `HttpRequest basicProxyAuth(String username,String password)` | 简单代理验证，生成的头信息类似于： |
| `cn.hutool.http.HttpRequest` | `HttpRequest bearerAuth(String token)` | 令牌验证，生成的头类似于："Authorization: Bearer XXXXX"，一般用于JWT |
| `cn.hutool.http.HttpRequest` | `HttpRequest body(Resource resource)` | 设置主体字节码 需在此方法调用前使用charset方法设置编码，否则使用默认编码UTF-8 |
| `cn.hutool.http.HttpRequest` | `HttpRequest body(String body)` | 设置内容主体 请求体body参数支持两种类型： |
| `cn.hutool.http.HttpRequest` | `HttpRequest body(String body,String contentType)` | 设置内容主体 请求体body参数支持两种类型： |
| `cn.hutool.http.HttpRequest` | `HttpRequest body(byte[] bodyBytes)` | 设置主体字节码 需在此方法调用前使用charset方法设置编码，否则使用默认编码UTF-8 |
| `cn.hutool.http.HttpRequest` | `HttpRequest contentLength(int value)` | 设置内容长度 |
| `cn.hutool.http.HttpRequest` | `HttpRequest contentType(String contentType)` | 设置contentType |
| `cn.hutool.http.HttpRequest` | `HttpRequest cookie(Collection<HttpCookie> cookies)` | 设置Cookie 自定义Cookie后会覆盖Hutool的默认Cookie行为 |
| `cn.hutool.http.HttpRequest` | `HttpRequest cookie(HttpCookie... cookies)` | 设置Cookie 自定义Cookie后会覆盖Hutool的默认Cookie行为 |
| `cn.hutool.http.HttpRequest` | `HttpRequest cookie(String cookie)` | 设置Cookie 自定义Cookie后会覆盖Hutool的默认Cookie行为 |
| `cn.hutool.http.HttpRequest` | `HttpRequest delete(String url)` | DELETE请求 |
| `cn.hutool.http.HttpRequest` | `HttpRequest disableCache()` | 禁用缓存 |
| `cn.hutool.http.HttpRequest` | `HttpRequest disableCookie()` | 禁用默认Cookie行为，此方法调用后会将Cookie置为空。 如果想重新启用Cookie，请调用：#cookie(String)方法自定义Cookie。 如果想启动默认的Cookie行为（自动回填服务器传回的Cookie），则调用#enableDefaultCookie() |
| `cn.hutool.http.HttpRequest` | `HttpRequest enableDefaultCookie()` | 打开默认的Cookie行为（自动回填服务器传回的Cookie） |
| `cn.hutool.http.HttpRequest` | `HttpRequest form(Map<String, Object> formMap)` | 设置map类型表单数据 |
| `cn.hutool.http.HttpRequest` | `HttpRequest form(String name,File file)` | 文件表单项 一旦有文件加入，表单变为multipart/form-data |
| `cn.hutool.http.HttpRequest` | `HttpRequest form(String name,File file,String fileName)` | 文件表单项 一旦有文件加入，表单变为multipart/form-data |
| `cn.hutool.http.HttpRequest` | `HttpRequest form(String name,File... files)` | 文件表单项 一旦有文件加入，表单变为multipart/form-data |
| `cn.hutool.http.HttpRequest` | `HttpRequest form(String name,Object value)` | 设置表单数据 |
| `cn.hutool.http.HttpRequest` | `HttpRequest form(String name,Object value,Object... parameters)` | 设置表单数据 |
| `cn.hutool.http.HttpRequest` | `HttpRequest form(String name,Resource resource)` | 文件表单项 一旦有文件加入，表单变为multipart/form-data |
| `cn.hutool.http.HttpRequest` | `HttpRequest form(String name,byte[] fileBytes,String fileName)` | 文件byte[]表单项 一旦有文件加入，表单变为multipart/form-data |
| `cn.hutool.http.HttpRequest` | `HttpRequest formStr(Map<String, String> formMapStr)` | 设置map<String, String>类型表单数据 |
| `cn.hutool.http.HttpRequest` | `HttpRequest get(String url)` | GET请求 |
| `cn.hutool.http.HttpRequest` | `HttpRequest head(String url)` | HEAD请求 |
| `cn.hutool.http.HttpRequest` | `HttpRequest keepAlive(boolean isKeepAlive)` | 设置是否为长连接 |
| `cn.hutool.http.HttpRequest` | `HttpRequest method(Method method)` | 设置请求方法 |
| `cn.hutool.http.HttpRequest` | `HttpRequest of(String url)` | 构建一个HTTP请求 对于传入的URL，可以自定义是否解码已经编码的内容，设置见HttpGlobalConfig#setDecodeUrl(boolean) 在构建Http请求时，用户传入的URL可能有编码后和未编码的内容混合在一起，如果HttpGlobalConfig#isDecodeUrl()为true，则会统一解码编码后的参数， 按照RFC3986规范，在发送请求时，全部编码之。如果为false，则不会解码已经编码的内容，在请求时只编码需要编码的部分。 |
| `cn.hutool.http.HttpRequest` | `HttpRequest of(String url,Charset charset)` | 构建一个HTTP请求 对于传入的URL，可以自定义是否解码已经编码的内容。 在构建Http请求时，用户传入的URL可能有编码后和未编码的内容混合在一起，如果charset参数不为null，则会统一解码编码后的参数， 按照RFC3986规范，在发送请求时，全部编码之。如果为false，则不会解码已经编码的内容，在请求时只编码需要编码的部分。 |
| `cn.hutool.http.HttpRequest` | `HttpRequest of(UrlBuilder url)` | 构建一个HTTP请求 |
| `cn.hutool.http.HttpRequest` | `HttpRequest options(String url)` | OPTIONS请求 |
| `cn.hutool.http.HttpRequest` | `HttpRequest patch(String url)` | PATCH请求 |
| `cn.hutool.http.HttpRequest` | `HttpRequest post(String url)` | POST请求 |
| `cn.hutool.http.HttpRequest` | `HttpRequest proxyAuth(String content)` | 验证，简单插入Authorization头 |
| `cn.hutool.http.HttpRequest` | `HttpRequest put(String url)` | PUT请求 |
| `cn.hutool.http.HttpRequest` | `HttpRequest setChunkedStreamingMode(int blockSize)` | 采用流方式上传数据，无需本地缓存数据。 HttpUrlConnection默认是将所有数据读到本地缓存，然后再发送给服务器，这样上传大文件时就会导致内存溢出。 |
| `cn.hutool.http.HttpRequest` | `HttpRequest setConfig(HttpConfig config)` | 将新的配置加入 注意加入的配置可能被修改 |
| `cn.hutool.http.HttpRequest` | `HttpRequest setConnectionTimeout(int milliseconds)` | 设置连接超时，单位：毫秒 |
| `cn.hutool.http.HttpRequest` | `HttpRequest setFixedContentLength(long contentLength)` | 设置固定长度的流模式，会设置HTTP请求头中的Content-Length字段，告知服务器整个请求体的精确字节大小。 这在上传文件或大数据量时非常有用，因为它允许服务器准确地知道何时接收完所有的请求数据，而不需要依赖于连接的关闭来判断数据传输的结束。 |
| `cn.hutool.http.HttpRequest` | `HttpRequest setFollowRedirects(boolean isFollowRedirects)` | 设置是否打开重定向，如果打开默认重定向次数为2 此方法效果与#setMaxRedirectCount(int) 一致 需要注意的是，当设置为true时，如果全局重定向次数非0，直接复用，否则设置默认2次。 当设置为false时，无论全局是否设置次数，都设置为0。 不调用此方法的情况下，使用全局默认的次数。 |
| `cn.hutool.http.HttpRequest` | `HttpRequest setFollowRedirectsCookie(boolean followRedirectsCookie)` | 自动重定向时是否处理cookie |
| `cn.hutool.http.HttpRequest` | `HttpRequest setHostnameVerifier(HostnameVerifier hostnameVerifier)` | 设置域名验证器 只针对HTTPS请求，如果不设置，不做验证，所有域名被信任 |
| `cn.hutool.http.HttpRequest` | `HttpRequest setHttpProxy(String host,int port)` | 设置Http代理 |
| `cn.hutool.http.HttpRequest` | `HttpRequest setMaxRedirectCount(int maxRedirectCount)` | 设置最大重定向次数 如果次数小于1则表示不重定向，大于等于1表示打开重定向 |
| `cn.hutool.http.HttpRequest` | `HttpRequest setMethod(Method method)` | 设置请求方法 |
| `cn.hutool.http.HttpRequest` | `HttpRequest setProxy(Proxy proxy)` | 设置代理 |
| `cn.hutool.http.HttpRequest` | `HttpRequest setReadTimeout(int milliseconds)` | 设置连接超时，单位：毫秒 |
| `cn.hutool.http.HttpRequest` | `HttpRequest setRest(boolean isRest)` | 设置是否rest模式 rest模式下get请求不会把参数附加到URL之后 |
| `cn.hutool.http.HttpRequest` | `HttpRequest setSSLProtocol(String protocol)` | 设置HTTPS安全连接协议，只针对HTTPS请求，可以使用的协议包括： 此方法调用后#setSSLSocketFactory(SSLSocketFactory) 将被覆盖。 |
| `cn.hutool.http.HttpRequest` | `HttpRequest setSSLSocketFactory(SSLSocketFactory ssf)` | 设置SSLSocketFactory 只针对HTTPS请求，如果不设置，使用默认的SSLSocketFactory 默认SSLSocketFactory为：SSLSocketFactoryBuilder.create().build(); |
| `cn.hutool.http.HttpRequest` | `HttpRequest setUrl(String url)` | 设置URL |
| `cn.hutool.http.HttpRequest` | `HttpRequest setUrl(UrlBuilder urlBuilder)` | 设置URL |
| `cn.hutool.http.HttpRequest` | `HttpRequest setUrlHandler(URLStreamHandler urlHandler)` | 设置URLStreamHandler 部分环境下需要单独设置此项，例如当 WebLogic Server 实例充当 SSL 客户端角色（它会尝试通过 SSL 连接到其他服务器或应用程序）时， 它会验证 SSL 服务器在数字证书中返回的主机名是否与用于连接 SSL 服务器的 URL 主机名相匹配。如果主机名不匹配，则删除此连接。 因此weblogic不支持https的sni协议的主机名验证，此时需要将此值设置为sun.net.www.protocol.https.Handler对象。 相关issue见： https://gitee.com/chinabugotech/hutool/issues/… |
| `cn.hutool.http.HttpRequest` | `HttpRequest timeout(int milliseconds)` | 设置超时，单位：毫秒 超时包括： |
| `cn.hutool.http.HttpRequest` | `HttpRequest trace(String url)` | TRACE请求 |
| `cn.hutool.http.HttpRequest` | `HttpResponse execute()` | 执行Reuqest请求 |
| `cn.hutool.http.HttpRequest` | `HttpResponse execute(boolean isAsync)` | 执行Reuqest请求 |
| `cn.hutool.http.HttpRequest` | `HttpResponse executeAsync()` | 异步请求 异步请求后获取的HttpResponse 为异步模式，执行完此方法后发送请求到服务器，但是并不立即读取响应内容。 此时保持Http连接不关闭，直调用获取内容方法为止。 一般执行完execute之后会把响应内容全部读出来放在一个 byte数组里，如果你响应的内容太多内存就爆了，此法是发送完请求不直接读响应内容，等有需要的时候读。 |
| `cn.hutool.http.HttpRequest` | `Map<String, Object> form()` | 获取表单数据 |
| `cn.hutool.http.HttpRequest` | `Map<String, Resource> fileForm()` | 获取文件表单数据 |
| `cn.hutool.http.HttpRequest` | `Method getMethod()` | 获取Http请求方法 |
| `cn.hutool.http.HttpRequest` | `String contentLength()` | 获取内容长度 |
| `cn.hutool.http.HttpRequest` | `String getUrl()` | 获取请求URL |
| `cn.hutool.http.HttpRequest` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpRequest` | `T thenFunction(Function<HttpResponse, T> function)` | 执行Request请求后，对响应内容后续处理 处理结束后关闭连接 |
| `cn.hutool.http.HttpRequest` | `boolean isKeepAlive()` | @return 获取是否为长连接 |
| `cn.hutool.http.HttpRequest` | `void closeCookie()` | 关闭Cookie |
| `cn.hutool.http.HttpRequest` | `void setCookieManager(CookieManager customCookieManager)` | 自定义CookieManager |
| `cn.hutool.http.HttpRequest` | `void setGlobalTimeout(int customTimeout)` | 设置全局默认的连接和读取超时时长 |
| `cn.hutool.http.HttpRequest` | `void then(Consumer<HttpResponse> consumer)` | 执行Request请求后，对响应内容后续处理 处理结束后关闭连接 |
| `cn.hutool.http.HttpResource` | `InputStream getStream()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpResource` | `String getContentType()` | 获取自定义Content-Type类型 |
| `cn.hutool.http.HttpResource` | `String getName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpResource` | `URL getUrl()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpResponse` | `File completeFileNameFromHeader(File targetFileOrDir)` | 从响应头补全下载文件名 |
| `cn.hutool.http.HttpResponse` | `File writeBodyForFile(File targetFileOrDir,StreamProgress streamProgress)` | 将响应内容写出到文件 异步模式下直接读取Http流写出，同步模式下将存储在内存中的响应内容写出 写出后会关闭Http流（异步模式） |
| `cn.hutool.http.HttpResponse` | `HttpCookie getCookie(String name)` | 获取Cookie |
| `cn.hutool.http.HttpResponse` | `HttpResponse body(byte[] bodyBytes)` | 设置主体字节码 需在此方法调用前使用charset方法设置编码，否则使用默认编码UTF-8 |
| `cn.hutool.http.HttpResponse` | `HttpResponse sync()` | 同步 如果为异步状态，则暂时不读取服务器中响应的内容，而是持有Http链接的InputStream。 当调用此方法时，异步状态转为同步状态，此时从Http链接流中读取body内容并暂存在内容中。如果已经是同步状态，则不进行任何操作。 |
| `cn.hutool.http.HttpResponse` | `InputStream bodyStream()` | 获得服务区响应流 异步模式下获取Http原生流，同步模式下获取获取到的在内存中的副本 如果想在同步模式下获取流，请先调用#sync()方法强制同步 流获取后处理完毕需关闭此类 |
| `cn.hutool.http.HttpResponse` | `List<HttpCookie> getCookies()` | 获取Cookie |
| `cn.hutool.http.HttpResponse` | `String body()` | 获取响应主体 |
| `cn.hutool.http.HttpResponse` | `String contentEncoding()` | 获取内容编码 |
| `cn.hutool.http.HttpResponse` | `String getCookieStr()` | 获取本次请求服务器返回的Cookie信息 |
| `cn.hutool.http.HttpResponse` | `String getCookieValue(String name)` | 获取Cookie值 |
| `cn.hutool.http.HttpResponse` | `String getFileNameFromDisposition()` | 从Content-Disposition头中获取文件名 |
| `cn.hutool.http.HttpResponse` | `String getFileNameFromDisposition(String paramName)` | 从Content-Disposition头中获取文件名，以参数名为'filename'为例，规则为： 首先按照RFC5987规范检查'filename*'参数对应的值，即：'filename*="example.txt"'，则获取'example.txt' 如果找不到'filename*'参数，则检查'filename'参数对应的值，即：'filename="example.txt"'，则获取'example.txt' 按照规范，'Content-Disposition'可能返回多个，此处遍历所有返回头，并且'filename*'始终优先获取，即使'filename'存在并更靠前。 参考：ht… |
| `cn.hutool.http.HttpResponse` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpResponse` | `boolean isChunked()` | 是否为Transfer-Encoding:Chunked的内容 |
| `cn.hutool.http.HttpResponse` | `boolean isDeflate()` | 是否为zlib(Deflate)压缩过的内容 |
| `cn.hutool.http.HttpResponse` | `boolean isGzip()` | 是否为gzip压缩过的内容 |
| `cn.hutool.http.HttpResponse` | `boolean isOk()` | 请求是否成功，判断依据为：状态码范围在200~299内。 |
| `cn.hutool.http.HttpResponse` | `byte[] bodyBytes()` | 获取响应流字节码 此方法会转为同步模式 |
| `cn.hutool.http.HttpResponse` | `int getStatus()` | 获取状态码 |
| `cn.hutool.http.HttpResponse` | `long contentLength()` | 获取内容长度，以下情况长度无效： Transfer-Encoding: Chunked Content-Encoding: XXX 参考：https://blog.csdn.net/jiang7701037/article/details/86304302 |
| `cn.hutool.http.HttpResponse` | `long writeBody(File targetFileOrDir)` | 将响应内容写出到文件 异步模式下直接读取Http流写出，同步模式下将存储在内存中的响应内容写出 写出后会关闭Http流（异步模式） |
| `cn.hutool.http.HttpResponse` | `long writeBody(File targetFileOrDir,StreamProgress streamProgress)` | 将响应内容写出到文件 异步模式下直接读取Http流写出，同步模式下将存储在内存中的响应内容写出 写出后会关闭Http流（异步模式） |
| `cn.hutool.http.HttpResponse` | `long writeBody(File targetFileOrDir,String tempFileSuffix,StreamProgress streamProgress)` | 将响应内容写出到文件-避免未完成的文件 异步模式下直接读取Http流写出，同步模式下将存储在内存中的响应内容写出 写出后会关闭Http流（异步模式） 来自：https://gitee.com/chinabugotech/hutool/pulls/407 此方法原理是先在目标文件同级目录下创建临时文件，下载之，等下载完毕后重命名，避免因下载错误导致的文件不完整。 |
| `cn.hutool.http.HttpResponse` | `long writeBody(OutputStream out,boolean isCloseOut,StreamProgress streamProgress)` | 将响应内容写出到OutputStream 异步模式下直接读取Http流写出，同步模式下将存储在内存中的响应内容写出 写出后会关闭Http流（异步模式） |
| `cn.hutool.http.HttpResponse` | `long writeBody(String targetFileOrDir)` | 将响应内容写出到文件 异步模式下直接读取Http流写出，同步模式下将存储在内存中的响应内容写出 写出后会关闭Http流（异步模式） |
| `cn.hutool.http.HttpResponse` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.HttpStatus` | `boolean isRedirected(int responseCode)` | 是否为重定向状态码 |
| `cn.hutool.http.HttpUtil` | `File downloadFileFromUrl(String url,File destFile)` | 下载远程文件 |
| `cn.hutool.http.HttpUtil` | `File downloadFileFromUrl(String url,File destFile,StreamProgress streamProgress)` | 下载远程文件 |
| `cn.hutool.http.HttpUtil` | `File downloadFileFromUrl(String url,File destFile,int timeout)` | 下载远程文件 |
| `cn.hutool.http.HttpUtil` | `File downloadFileFromUrl(String url,File destFile,int timeout,StreamProgress streamProgress)` | 下载远程文件 |
| `cn.hutool.http.HttpUtil` | `File downloadFileFromUrl(String url,String dest)` | 下载远程文件 |
| `cn.hutool.http.HttpUtil` | `HttpRequest createGet(String url)` | 创建Http GET请求对象 |
| `cn.hutool.http.HttpUtil` | `HttpRequest createGet(String url,boolean isFollowRedirects)` | 创建Http GET请求对象 |
| `cn.hutool.http.HttpUtil` | `HttpRequest createPost(String url)` | 创建Http POST请求对象 |
| `cn.hutool.http.HttpUtil` | `HttpRequest createRequest(Method method,String url)` | 创建Http请求对象 |
| `cn.hutool.http.HttpUtil` | `Map<String, List<String>> decodeParams(String paramsStr,Charset charset)` | 将URL QueryString参数解析为Map |
| `cn.hutool.http.HttpUtil` | `Map<String, List<String>> decodeParams(String paramsStr,Charset charset,boolean isFormUrlEncoded)` | 将URL参数解析为Map（也可以解析Post中的键值对参数） |
| `cn.hutool.http.HttpUtil` | `Map<String, List<String>> decodeParams(String paramsStr,String charset)` | 将URL参数解析为Map（也可以解析Post中的键值对参数） |
| `cn.hutool.http.HttpUtil` | `Map<String, List<String>> decodeParams(String paramsStr,String charset,boolean isFormUrlEncoded)` | 将URL参数解析为Map（也可以解析Post中的键值对参数） |
| `cn.hutool.http.HttpUtil` | `Map<String, String> decodeParamMap(String paramsStr,Charset charset)` | 将URL参数解析为Map（也可以解析Post中的键值对参数） |
| `cn.hutool.http.HttpUtil` | `SimpleServer createServer(int port)` | 创建简易的Http服务器 |
| `cn.hutool.http.HttpUtil` | `String buildBasicAuth(String username,String password,Charset charset)` | 构建简单的账号秘密验证信息，构建后类似于： |
| `cn.hutool.http.HttpUtil` | `String downloadString(String url,Charset customCharset)` | 下载远程文本 |
| `cn.hutool.http.HttpUtil` | `String downloadString(String url,Charset customCharset,StreamProgress streamPress)` | 下载远程文本 |
| `cn.hutool.http.HttpUtil` | `String downloadString(String url,String customCharsetName)` | 下载远程文本 |
| `cn.hutool.http.HttpUtil` | `String encodeParams(String urlWithParams,Charset charset)` | 对URL参数做编码，只编码键和值 提供的值可以是url附带参数，但是不能只是url 注意，此方法只能标准化整个URL，并不适合于单独编码参数值 |
| `cn.hutool.http.HttpUtil` | `String get(String urlString)` | 发送get请求 |
| `cn.hutool.http.HttpUtil` | `String get(String urlString,Charset customCharset)` | 发送get请求 |
| `cn.hutool.http.HttpUtil` | `String get(String urlString,Map<String, Object> paramMap)` | 发送get请求 |
| `cn.hutool.http.HttpUtil` | `String get(String urlString,Map<String, Object> paramMap,int timeout)` | 发送get请求 |
| `cn.hutool.http.HttpUtil` | `String get(String urlString,int timeout)` | 发送get请求 |
| `cn.hutool.http.HttpUtil` | `String getCharset(HttpURLConnection conn)` | 从Http连接的头信息中获得字符集 从ContentType中获取 |
| `cn.hutool.http.HttpUtil` | `String getCharset(String contentType)` | 从Http连接的头信息中获得字符集 从ContentType中获取 |
| `cn.hutool.http.HttpUtil` | `String getContentTypeByRequestBody(String body)` | 从请求参数的body中判断请求的Content-Type类型，支持的类型有： |
| `cn.hutool.http.HttpUtil` | `String getMimeType(String filePath)` | 根据文件扩展名获得MimeType |
| `cn.hutool.http.HttpUtil` | `String getMimeType(String filePath,String defaultValue)` | 根据文件扩展名获得MimeType |
| `cn.hutool.http.HttpUtil` | `String getString(InputStream in,Charset charset,boolean isGetCharsetFromContent)` | 从流中读取内容 首先尝试使用charset编码读取内容（如果为空默认UTF-8），如果isGetCharsetFromContent为true，则通过正则在正文中获取编码信息，转换为指定编码； |
| `cn.hutool.http.HttpUtil` | `String getString(byte[] contentBytes,Charset charset,boolean isGetCharsetFromContent)` | 从流中读取内容 首先尝试使用charset编码读取内容（如果为空默认UTF-8），如果isGetCharsetFromContent为true，则通过正则在正文中获取编码信息，转换为指定编码； |
| `cn.hutool.http.HttpUtil` | `String normalizeParams(String paramPart,Charset charset)` | 标准化参数字符串，即URL中？后的部分 注意，此方法只能标准化整个URL，并不适合于单独编码参数值 |
| `cn.hutool.http.HttpUtil` | `String post(String urlString,Map<String, Object> paramMap)` | 发送post请求 |
| `cn.hutool.http.HttpUtil` | `String post(String urlString,Map<String, Object> paramMap,int timeout)` | 发送post请求 |
| `cn.hutool.http.HttpUtil` | `String post(String urlString,String body)` | 发送post请求 请求体body参数支持两种类型： |
| `cn.hutool.http.HttpUtil` | `String post(String urlString,String body,int timeout)` | 发送post请求 请求体body参数支持两种类型： |
| `cn.hutool.http.HttpUtil` | `String toParams(Map<String, ?> paramMap)` | 将Map形式的Form表单数据转换为Url参数形式，会自动url编码键和值 |
| `cn.hutool.http.HttpUtil` | `String toParams(Map<String, ?> paramMap,Charset charset)` | 将Map形式的Form表单数据转换为Url参数形式 paramMap中如果key为空（null和""）会被忽略，如果value为null，会被做为空白符（""） 会自动url编码键和值 此方法用于拼接URL中的Query部分，并不适用于POST请求中的表单 |
| `cn.hutool.http.HttpUtil` | `String toParams(Map<String, ?> paramMap,Charset charset,boolean isFormUrlEncoded)` | 将Map形式的Form表单数据转换为Url参数形式 paramMap中如果key为空（null和""）会被忽略，如果value为null，会被做为空白符（""） 会自动url编码键和值 |
| `cn.hutool.http.HttpUtil` | `String toParams(Map<String, Object> paramMap,String charsetName)` | 将Map形式的Form表单数据转换为Url参数形式 编码键和值对 |
| `cn.hutool.http.HttpUtil` | `String urlWithForm(String url,Map<String, Object> form,Charset charset,boolean isEncodeParams)` | 将表单数据加到URL中（用于GET表单提交） 表单的键值对会被url编码，但是url中原参数不会被编码 |
| `cn.hutool.http.HttpUtil` | `String urlWithForm(String url,String queryString,Charset charset,boolean isEncode)` | 将表单数据字符串加到URL中（用于GET表单提交） |
| `cn.hutool.http.HttpUtil` | `String urlWithFormUrlEncoded(String url,Map<String, Object> form,Charset charset)` | 将表单数据加到URL中（用于GET表单提交） 表单的键值对会被url编码，但是url中原参数不会被编码 且对form参数进行 FormUrlEncoded ，x-www-form-urlencoded模式，此模式下空格会编码为'+' |
| `cn.hutool.http.HttpUtil` | `boolean isHttp(String url)` | 检测是否http |
| `cn.hutool.http.HttpUtil` | `boolean isHttps(String url)` | 检测是否https |
| `cn.hutool.http.HttpUtil` | `byte[] downloadBytes(String url)` | 下载远程文件数据，支持30x跳转 |
| `cn.hutool.http.HttpUtil` | `long download(String url,OutputStream out,boolean isCloseOut)` | 下载远程文件 |
| `cn.hutool.http.HttpUtil` | `long download(String url,OutputStream out,boolean isCloseOut,StreamProgress streamProgress)` | 下载远程文件 |
| `cn.hutool.http.HttpUtil` | `long downloadFile(String url,File destFile)` | 下载远程文件 |
| `cn.hutool.http.HttpUtil` | `long downloadFile(String url,File destFile,StreamProgress streamProgress)` | 下载远程文件 |
| `cn.hutool.http.HttpUtil` | `long downloadFile(String url,File destFile,int timeout)` | 下载远程文件 |
| `cn.hutool.http.HttpUtil` | `long downloadFile(String url,File destFile,int timeout,StreamProgress streamProgress)` | 下载远程文件 |
| `cn.hutool.http.HttpUtil` | `long downloadFile(String url,String dest)` | 下载远程文件 |
| `cn.hutool.http.HttpUtil` | `void closeCookie()` | 关闭Cookie |
| `cn.hutool.http.MultipartOutputStream` | `MultipartOutputStream write(String formFieldName,Object value)` | 添加Multipart表单的数据项 |
| `cn.hutool.http.MultipartOutputStream` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.MultipartOutputStream` | `void finish()` | 上传表单结束 |
| `cn.hutool.http.MultipartOutputStream` | `void write(int b)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
