# com.feilong.servlet.http

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.servlet.http.CookieUtil` | `Cookie getCookie(HttpServletRequest request,String cookieName)` | 获得 Cookie对象. 循环遍历 HttpServletRequest#getCookies(),找到 Cookie#getName()是 cookieName 的 Cookie |
| `com.feilong.servlet.http.CookieUtil` | `Integer getCookieIntegerValue(HttpServletRequest request,String cookieName)` | 取指定 cookieName 的 Cookie值转成Integer类型返回. |
| `com.feilong.servlet.http.CookieUtil` | `Long getCookieLongValue(HttpServletRequest request,String cookieName)` | 取指定 cookieName 的 Cookie值转成Long类型返回. |
| `com.feilong.servlet.http.CookieUtil` | `Map<String, String> getCookieMap(HttpServletRequest request)` | 将Cookie的 key 和value转成 map(TreeMap). |
| `com.feilong.servlet.http.CookieUtil` | `String getCookieValue(HttpServletRequest request,String cookieName)` | 取指定 cookieName 的 Cookie值. |
| `com.feilong.servlet.http.CookieUtil` | `void addCookie(CookieEntity cookieEntity,HttpServletResponse response)` | 创建cookie. 如果 cookieEntity 是null,抛出 NullPointerException 如果 cookieEntity.cookieName 是null,抛出 NullPointerException 如果 cookieEntity.cookieName 是blank,抛出 IllegalArgumentException |
| `com.feilong.servlet.http.CookieUtil` | `void addCookie(String cookieName,String value,HttpServletResponse response)` | 创建cookie. 注意:该方法创建的cookie,有效期是默认值 -1,即浏览器退出就删除 如果 cookieName 是null,抛出 NullPointerException 如果 cookieName 是blank,抛出 IllegalArgumentException |
| `com.feilong.servlet.http.CookieUtil` | `void addCookie(String cookieName,String value,int maxAge,HttpServletResponse response)` | 创建cookie. 如果 cookieName 是null,抛出 NullPointerException 如果 cookieName 是blank,抛出 IllegalArgumentException |
| `com.feilong.servlet.http.CookieUtil` | `void deleteCookie(CookieEntity cookieEntity,HttpServletResponse response)` | 删除cookie. 删除 Cookie的时候,path必须保持一致 |
| `com.feilong.servlet.http.CookieUtil` | `void deleteCookie(String cookieName,HttpServletResponse response)` | 删除Cookie. 删除Cookie的时候,path必须保持一致; 如果path不一致,请使用 CookieUtil#deleteCookie(CookieEntity, HttpServletResponse) |
| `com.feilong.servlet.http.RequestUtil` | `Integer getHeaderIntegerValue(HttpServletRequest request,String headerName)` | 取指定 headerName 的 header 值转成Integer类型返回. |
| `com.feilong.servlet.http.RequestUtil` | `Integer getParameterPageNo(HttpServletRequest request,String paramName)` | 获得request中的请求分页页码参数,如果不存在或者是empty,那么使用默认值 defaultValue . |
| `com.feilong.servlet.http.RequestUtil` | `Integer getParameterPageSize(HttpServletRequest request,String paramName,Integer defaultValue)` | 获得request中的请求分页size参数值,如果不存在或者是empty,那么使用默认值 defaultValue . |
| `com.feilong.servlet.http.RequestUtil` | `Long getHeaderLongValue(HttpServletRequest request,String headerName)` | 取指定 cookieName 的 Cookie值转成Long类型返回. |
| `com.feilong.servlet.http.RequestUtil` | `Map<String, Object> getAttributeMap(HttpServletRequest request)` | 遍历显示request的attribute,将 name /attributeValue 存入到map(TreeMap). |
| `com.feilong.servlet.http.RequestUtil` | `Map<String, Object> getRequestInfoFullMapForLog(HttpServletRequest request)` | 将request full相关属性,数据转成json格式 以便log显示(目前仅作log使用). |
| `com.feilong.servlet.http.RequestUtil` | `Map<String, Object> getRequestInfoMapForLog(HttpServletRequest request)` | 将 HttpServletRequest 相关属性,数据转成json格式 以便log显示(目前仅作log使用). 默认使用 RequestLogSwitch#NORMAL |
| `com.feilong.servlet.http.RequestUtil` | `Map<String, Object> getRequestInfoMapForLog(HttpServletRequest request,RequestLogSwitch requestLogSwitch)` | 将request 相关属性,数据转成json格式 以便log显示(目前仅作log使用). |
| `com.feilong.servlet.http.RequestUtil` | `Map<String, String> getHeaderMap(HttpServletRequest request)` | 遍历显示request的header. 将 request header name 和value 封装到TreeMap. |
| `com.feilong.servlet.http.RequestUtil` | `Map<String, String> getParameterSingleValueMap(HttpServletRequest request)` | 获得请求参数和单值map. 由于调用的 #getParameterMap(HttpServletRequest)结果是 有序的 , 此方法返回的map也是 有序的 由于j2eeServletRequest#getParameterMap()返回的map值是数组形式, 对于一些确认是单值的请求(比如支付宝notify/return request),不便后续处理 |
| `com.feilong.servlet.http.RequestUtil` | `Map<String, String[]> getParameterMap(HttpServletRequest request)` | 获得参数map(结果转成了key自然排序的TreeMap). 此方式会将tomcat返回的map 转成TreeMap 返回,便于log; 也可以 对这个返回的map进行操作 |
| `com.feilong.servlet.http.RequestUtil` | `String decodeISO88591String(String str,String charsetType)` | CharsetType#ISO_8859_1 的方式去除乱码. CharsetType#ISO_8859_1 是JAVA网络传输使用的标准 字符集 |
| `com.feilong.servlet.http.RequestUtil` | `String getClientIp(HttpServletRequest request)` | 获得客户端真实ip地址. 这样做的好处是,对开发透明 |
| `com.feilong.servlet.http.RequestUtil` | `String getHeader(HttpServletRequest request,String headerName)` | 取指定 headerName 的 header 值. |
| `com.feilong.servlet.http.RequestUtil` | `String getHeaderOrigin(HttpServletRequest request)` | 1、Origin字段里只包含是谁发起的请求,并没有其他信息 (通常情况下是方案,主机和活动文档URL的端口). 跟Referer不一样的是,Origin字段并没有包含涉及到用户隐私的URL路径和请求内容,这个尤其重要. 2、Origin字段只存在于POST请求,而Referer则存在于所有类型的请求. |
| `com.feilong.servlet.http.RequestUtil` | `String getHeaderReferer(HttpServletRequest request)` | 获得上个请求的URL. referer是浏览器在用户提交请求当前页面中的一个链接时,将当前页面的URL放在头域中提交给服务端的,如当前页面为a.html, 它里面有一个b.html的链接,当用户要访问b.html时浏览器就会把a.html作为referer发给服务端. |
| `com.feilong.servlet.http.RequestUtil` | `String getHeaderUserAgent(HttpServletRequest request)` | User Agent中文名为用户代理,简称 UA. 它是一个特殊字符串头,使得服务器能够识别客户使用的操作系统及版本、CPU 类型、浏览器及版本、浏览器渲染引擎、浏览器语言、浏览器插件等. |
| `com.feilong.servlet.http.RequestUtil` | `String getOriginatingServletPath(HttpServletRequest request)` | 【原文待译】Return the servlet path for the given request, detecting an include request URL if called within a RequestDispatcher include. |
| `com.feilong.servlet.http.RequestUtil` | `String getParameter(HttpServletRequest request,String paramName)` | 获得request中的请求参数值. |
| `com.feilong.servlet.http.RequestUtil` | `String getParameterDefaultValue(HttpServletRequest request,String paramName,String defaultValue)` | 获得request中的请求参数值,如果不存在或者是empty,那么使用默认值 defaultValue . |
| `com.feilong.servlet.http.RequestUtil` | `String getRequestBody(HttpServletRequest request)` | 获取request body中的内容. |
| `com.feilong.servlet.http.RequestUtil` | `String getRequestFullURL(HttpServletRequest request)` | 获得请求的全地址. |
| `com.feilong.servlet.http.RequestUtil` | `String getRequestFullURL(HttpServletRequest request,String charsetType)` | 获得请求的全地址. |
| `com.feilong.servlet.http.RequestUtil` | `String getRequestURL(HttpServletRequest request)` | 获得请求的?部分前面的地址. 自动识别 request 是否 forword ,如果是forword过来的,那么取 RequestAttributes#FORWARD_REQUEST_URI变量 |
| `com.feilong.servlet.http.RequestUtil` | `String getServerRootWithContextPath(HttpServletRequest request)` | scheme+serverName+port+getContextPath. 区分 http 和https. |
| `com.feilong.servlet.http.RequestUtil` | `String parseParamsToQueryString(HttpServletRequest request)` | 提取参数,转成类似于queryString字符串. 如果request是get 请求,那么直接返回 request.getQueryString() 如果request不是get,那么提取参数组装成字符串返回 |
| `com.feilong.servlet.http.RequestUtil` | `T getAttribute(HttpServletRequest request,String attributeName)` | 获得 attribute. |
| `com.feilong.servlet.http.RequestUtil` | `T getAttribute(HttpServletRequest request,String attributeName,T defaultValue)` | 获得 attribute,如果值是null 或者没有相关属性,那么返回 defaultValue . |
| `com.feilong.servlet.http.RequestUtil` | `T getAttribute(HttpServletRequest request,String name,Class<T> klass)` | 取到request里面的属性值, 转换类型成指定的参数 klass . |
| `com.feilong.servlet.http.RequestUtil` | `T getAttribute(HttpServletRequest request,String name,Class<T> klass,T defaultValue)` | 取到request里面的属性值, 转换类型成指定的参数 klass . 如果值是null 或者没有相关属性,那么返回 defaultValue . |
| `com.feilong.servlet.http.RequestUtil` | `T getParameterDefaultValue(HttpServletRequest request,String paramName,Class<T> convertClass,T defaultValue)` | 获得request中的请求参数值,如果不存在或者是empty,那么使用默认值 defaultValue . |
| `com.feilong.servlet.http.RequestUtil` | `boolean containsParam(HttpServletRequest request,String paramName)` | 请求路径中是否包含某个参数名称 (注意:这是判断是否包含参数,而不是判断参数值是否为空). |
| `com.feilong.servlet.http.RequestUtil` | `boolean isAjaxRequest(HttpServletRequest request)` | 判断一个请求是否是ajax请求. |
| `com.feilong.servlet.http.RequestUtil` | `boolean isGetMethod(HttpServletRequest request)` | 判断一个请求是不是get method. |
| `com.feilong.servlet.http.RequestUtil` | `boolean isNotAjaxRequest(HttpServletRequest request)` | 判断一个请求 ,不是ajax 请求. |
| `com.feilong.servlet.http.RequestUtil` | `boolean isNotWechatMiniProgramRequest(HttpServletRequest request)` | 判断一个请求 不是 微信小程序 的请求. 注意:此方法目前android weixin userAgent 会带特殊字符,IOS环境没有, ios微信web-view的user-agent缺失miniprogram 请谨慎使用,为了将来扩展,暂时保留此方法 |
| `com.feilong.servlet.http.RequestUtil` | `boolean isNotWechatRequest(HttpServletRequest request)` | 判断一个请求不是 微信浏览器 的请求. |
| `com.feilong.servlet.http.RequestUtil` | `boolean isPostMethod(HttpServletRequest request)` | 判断一个请求是不是post method. |
| `com.feilong.servlet.http.RequestUtil` | `boolean isStaticResource(String requestURI)` | 判断请求是否是静态资源. |
| `com.feilong.servlet.http.RequestUtil` | `boolean isSupportMethod(String[] supportHttpMethods,String method)` | 判断传入的 method 是否在 支持的 supportHttpMethods 数组中. |
| `com.feilong.servlet.http.RequestUtil` | `boolean isWechatMiniProgramRequest(HttpServletRequest request)` | 判断一个请求是否是 微信小程序 的请求. 注意:此方法目前android weixin userAgent 会带特殊字符,IOS环境没有, ios微信web-view的user-agent缺失miniprogram 请谨慎使用,为了将来扩展,暂时保留此方法 |
| `com.feilong.servlet.http.RequestUtil` | `boolean isWechatRequest(HttpServletRequest request)` | 判断一个请求是否是 微信浏览器 的请求. |
| `com.feilong.servlet.http.RequestUtil` | `void forward(String path,HttpServletRequest request,HttpServletResponse response)` | 用于将请求转发到 RequestDispatcher 对象封装的资源,Servlet程序在调用该方法转发之前可以对请求进行前期预处理. 该方法将 checked exception 转成了 unchecked exception,方便书写和调用 Forwards a request from a servlet to another resource (servlet, JSP file, or HTML file) on the server. This method allows one servlet to do preliminary processing of a request a… |
| `com.feilong.servlet.http.RequestUtil` | `void include(String path,HttpServletRequest request,HttpServletResponse response)` | 用于将 RequestDispatcher 对象封装的资源内容作为当前响应内容的一部分包含进来,从而实现可编程服务器的服务器端包含功能. 该方法将 checked exception 转成了 unchecked exception,方便书写和调用 Includes the content of a resource (servlet, JSP page,HTML file) in the response. In essence, this method enables programmatic server-side includes. 注:被包含的Servlet程序不能改变响应信息的状态码… |
| `com.feilong.servlet.http.ResponseDownloadUtil` | `void download(File file,HttpServletRequest request,HttpServletResponse response)` | 下载文件. |
| `com.feilong.servlet.http.ResponseDownloadUtil` | `void download(String pathname,HttpServletRequest request,HttpServletResponse response)` | 下载文件. |
| `com.feilong.servlet.http.ResponseDownloadUtil` | `void download(String saveFileName,InputStream inputStream,Number contentLength,HttpServletRequest request,HttpServletResponse response)` | 下载(以 contentType=application/force-download) 强制下载. |
| `com.feilong.servlet.http.ResponseDownloadUtil` | `void download(String saveFileName,InputStream inputStream,Number contentLength,String contentType,String contentDisposition,HttpServletRequest request,HttpServletResponse response)` | 下载. |
| `com.feilong.servlet.http.ResponseUtil` | `Map<String, Object> getResponseInfoMapForLog(HttpServletResponse response)` | 获得 response info map for log. |
| `com.feilong.servlet.http.ResponseUtil` | `void sendError(HttpServletResponse response,int errorStatusCode)` | 【原文待译】Sends an error response to the client using the specified status code and clears the buffer. The server will preserve cookies and may clear or update any headers needed to serve the error page as a valid response. If an error-page declaration has been made for the web application corresponding to th… |
| `com.feilong.servlet.http.ResponseUtil` | `void sendError(HttpServletResponse response,int errorStatusCode,String errorMessage)` | 【原文待译】Sends an error response to the client using the specified status and clears the buffer. The server defaults to creating the response to look like an HTML-formatted server error page containing the specified message, setting the content type to "text/html". The server will preserve cookies and may cl… |
| `com.feilong.servlet.http.ResponseUtil` | `void sendRedirect(HttpServletResponse response,String url)` | 跳转. HttpServletResponse#sendRedirect(String)方法用于生成302响应码和Location响应头,从而通知客户端重新访问Location响应头指定的URL. 在 HttpServletResponse#sendRedirect(String)之后, 应该紧跟一句return; ; 我们已知道 HttpServletResponse#sendRedirect(String)是通过浏览器来做转向的,所以只有在页面处理完成后,才会有实际的动作. 既然您已要做转向了,那么后的输出更有什么意义呢？而且有可能会因为后面的输出导致转向失败. 如果 url 是null,… |
| `com.feilong.servlet.http.ResponseUtil` | `void setCacheHeader(HttpServletResponse response,int cacheTime)` | 设置页面缓存. 过期时间 = max-age 属性,单位 秒 . |
| `com.feilong.servlet.http.ResponseUtil` | `void setNoCacheHeader(HttpServletResponse response)` | 设置页面不缓存. 当HTTP1.1服务器指定 CacheControl = no-cache时,浏览器就不会缓存该网页. 旧式 HTTP1.0 服务器不能使用 Cache-Control 标题 |
| `com.feilong.servlet.http.ResponseUtil` | `void write(HttpServletResponse response,Object content)` | 输出. 默认 utf-8编码格式输出,如果你需要修改编码格式,可以使用 #write(HttpServletResponse, Object, String, String)方法 |
| `com.feilong.servlet.http.ResponseUtil` | `void write(HttpServletResponse response,Object content,String contentType,String characterEncoding)` | 输出. |
| `com.feilong.servlet.http.ResponseUtil` | `void writeJson(HttpServletResponse response,Object json)` | 以json的方式输出. 默认 utf-8编码格式输出,如果你需要修改编码格式,可以使用 #writeJson(HttpServletResponse, Object, String)方法 |
| `com.feilong.servlet.http.ResponseUtil` | `void writeJson(HttpServletResponse response,Object json,String characterEncoding)` | 以json的方式输出. 如果 characterEncoding 是null或者blank,默认使用utf-8 |
| `com.feilong.servlet.http.ResponseUtil` | `void writeText(HttpServletResponse response,Object text)` | 以text的方式输出. 默认 utf-8编码格式输出,如果你需要修改编码格式,可以使用 #writeText(HttpServletResponse, Object, String)方法 |
| `com.feilong.servlet.http.ResponseUtil` | `void writeText(HttpServletResponse response,Object text,String characterEncoding)` | 以text的方式输出. 如果 characterEncoding 是null或者blank,默认使用utf-8 |
| `com.feilong.servlet.http.SessionUtil` | `HttpSession replaceSession(HttpServletRequest request)` | 替换session,防止利用JSESSIONID 伪造url进行session hack. |
| `com.feilong.servlet.http.SessionUtil` | `Map<String, Object> getSessionInfoMapForLog(HttpSession session)` | 获得常用的session 属性值 map(仅仅用于log和debug使用). |
| `com.feilong.servlet.http.SessionUtil` | `Map<String, Serializable> getAttributeMap(HttpSession session)` | 遍历session的attribute,将 name /attributeValue 存入到map里. |
| `com.feilong.servlet.http.SessionUtil` | `String getSessionId(HttpServletRequest request)` | 获得给定request的session id,如果有的话. |
| `com.feilong.servlet.http.SessionUtil` | `T getAttribute(HttpServletRequest request,String attributeName)` | 从指定的request 对应的session中获取指定的属性. |
| `com.feilong.servlet.http.SessionUtil` | `T getRequiredAttribute(HttpServletRequest request,String attributeName)` | 从指定的request 对应的session中获取指定的属性. |
| `com.feilong.servlet.http.SessionUtil` | `void removeAttribute(HttpServletRequest request,String attributeName)` | 删除session 中指定的属性. |
| `com.feilong.servlet.http.SessionUtil` | `void setAttribute(HttpServletRequest request,String attributeName,Serializable attributeValue)` | 设置 the session attribute with the given name to the given value. |
