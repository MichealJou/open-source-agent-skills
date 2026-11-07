# cn.hutool.extra.servlet

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `Cookie getCookie(HttpServletRequest httpServletRequest,String name)` | 获得指定的Cookie |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `Map<String, Collection<String>> getHeadersMap(final HttpServletResponse response)` | 获取响应所有的头（header）信息 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `Map<String, Cookie> readCookieMap(HttpServletRequest httpServletRequest)` | 将cookie封装到Map里面 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `Map<String, List<String>> getHeadersMap(final HttpServletRequest request)` | 获取请求所有的头（header）信息 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `Map<String, String> getHeaderMap(HttpServletRequest request)` | 获取请求所有的头（header）信息 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `Map<String, String> getParamMap(ServletRequest request)` | 获得所有请求参数 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `Map<String, String[]> getParams(ServletRequest request)` | 获得所有请求参数 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `MultipartFormData getMultipart(ServletRequest request)` | 获得MultiPart表单内容，多用于获得上传的文件 在同一次请求中，此方法只能被执行一次！ |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `MultipartFormData getMultipart(ServletRequest request,UploadSetting uploadSetting)` | 获得multipart/form-data 表单内容 包括文件和普通表单数据 在同一次请求中，此方法只能被执行一次！ |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `PrintWriter getWriter(HttpServletResponse response)` | 获得PrintWriter |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `String getBody(ServletRequest request)` | 获取请求体 调用该方法后，getParam方法将失效 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `String getClientIP(HttpServletRequest request,String... otherHeaderNames)` | 获取客户端IP 默认检测的Header: |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `String getClientIPByHeader(HttpServletRequest request,String... headerNames)` | 获取客户端IP headerNames参数用于自定义检测的Header 需要注意的是，使用此方法获取的客户IP地址必须在Http服务器（例如Nginx）中配置头信息，否则容易造成IP伪造。 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `String getHeader(HttpServletRequest request,String name,Charset charset)` | 获得请求header中的信息 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `String getHeader(HttpServletRequest request,String name,String charsetName)` | 获得请求header中的信息 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `String getHeaderIgnoreCase(HttpServletRequest request,String nameIgnoreCase)` | 忽略大小写获得请求header中的信息 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `T fillBean(ServletRequest request,T bean,boolean isIgnoreError)` | ServletRequest 参数转Bean |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `T fillBean(final ServletRequest request,T bean,CopyOptions copyOptions)` | ServletRequest 参数转Bean |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `T toBean(ServletRequest request,Class<T> beanClass,boolean isIgnoreError)` | ServletRequest 参数转Bean |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `boolean isGetMethod(HttpServletRequest request)` | 是否为GET请求 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `boolean isIE(HttpServletRequest request)` | 客户浏览器是否为IE |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `boolean isMultipart(HttpServletRequest request)` | 是否为Multipart类型表单，此类型表单用于文件上传 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `boolean isPostMethod(HttpServletRequest request)` | 是否为POST请求 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `byte[] getBodyBytes(ServletRequest request)` | 获取请求体byte[] 调用该方法后，getParam方法将失效 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `void addCookie(HttpServletResponse response,Cookie cookie)` | 设定返回给客户端的Cookie |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `void addCookie(HttpServletResponse response,String name,String value)` | 设定返回给客户端的Cookie |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `void addCookie(HttpServletResponse response,String name,String value,int maxAgeInSeconds)` | 设定返回给客户端的Cookie Path: "/" No Domain |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `void addCookie(HttpServletResponse response,String name,String value,int maxAgeInSeconds,String path,String domain)` | 设定返回给客户端的Cookie |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `void setHeader(HttpServletResponse response,String name,Object value)` | 设置响应的Header |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `void write(HttpServletResponse response,File file)` | 返回文件给客户端 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `void write(HttpServletResponse response,InputStream in)` | 返回数据给客户端 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `void write(HttpServletResponse response,InputStream in,String contentType)` | 返回数据给客户端 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `void write(HttpServletResponse response,InputStream in,String contentType,String fileName)` | 返回数据给客户端 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `void write(HttpServletResponse response,InputStream in,int bufferSize)` | 返回数据给客户端 |
| `cn.hutool.extra.servlet.JakartaServletUtil` | `void write(HttpServletResponse response,String text,String contentType)` | 返回数据给客户端 |
| `cn.hutool.extra.servlet.ServletUtil` | `Cookie getCookie(HttpServletRequest httpServletRequest,String name)` | 获得指定的Cookie |
| `cn.hutool.extra.servlet.ServletUtil` | `Map<String, Collection<String>> getHeadersMap(HttpServletResponse response)` | 获取响应所有的头（header）信息 |
| `cn.hutool.extra.servlet.ServletUtil` | `Map<String, Cookie> readCookieMap(HttpServletRequest httpServletRequest)` | 将cookie封装到Map里面 |
| `cn.hutool.extra.servlet.ServletUtil` | `Map<String, List<String>> getHeadersMap(final HttpServletRequest request)` | 获取请求所有的头（header）信息 |
| `cn.hutool.extra.servlet.ServletUtil` | `Map<String, String> getHeaderMap(HttpServletRequest request)` | 获取请求所有的头（header）信息 |
| `cn.hutool.extra.servlet.ServletUtil` | `Map<String, String> getParamMap(ServletRequest request)` | 获得所有请求参数 |
| `cn.hutool.extra.servlet.ServletUtil` | `Map<String, String[]> getParams(ServletRequest request)` | 获得所有请求参数 |
| `cn.hutool.extra.servlet.ServletUtil` | `MultipartFormData getMultipart(ServletRequest request)` | 获得MultiPart表单内容，多用于获得上传的文件 在同一次请求中，此方法只能被执行一次！ |
| `cn.hutool.extra.servlet.ServletUtil` | `MultipartFormData getMultipart(ServletRequest request,UploadSetting uploadSetting)` | 获得multipart/form-data 表单内容 包括文件和普通表单数据 在同一次请求中，此方法只能被执行一次！ |
| `cn.hutool.extra.servlet.ServletUtil` | `PrintWriter getWriter(HttpServletResponse response)` | 获得PrintWriter |
| `cn.hutool.extra.servlet.ServletUtil` | `String getBody(ServletRequest request)` | 获取请求体 调用该方法后，getParam方法将失效 |
| `cn.hutool.extra.servlet.ServletUtil` | `String getClientIP(HttpServletRequest request,String... otherHeaderNames)` | 获取客户端IP 默认检测的Header: |
| `cn.hutool.extra.servlet.ServletUtil` | `String getClientIPByHeader(HttpServletRequest request,String... headerNames)` | 获取客户端IP headerNames参数用于自定义检测的Header 需要注意的是，使用此方法获取的客户IP地址必须在Http服务器（例如Nginx）中配置头信息，否则容易造成IP伪造。 |
| `cn.hutool.extra.servlet.ServletUtil` | `String getHeader(HttpServletRequest request,String name,Charset charset)` | 获得请求header中的信息 |
| `cn.hutool.extra.servlet.ServletUtil` | `String getHeader(HttpServletRequest request,String name,String charsetName)` | 获得请求header中的信息 |
| `cn.hutool.extra.servlet.ServletUtil` | `String getHeaderIgnoreCase(HttpServletRequest request,String nameIgnoreCase)` | 忽略大小写获得请求header中的信息 |
| `cn.hutool.extra.servlet.ServletUtil` | `T fillBean(ServletRequest request,T bean,boolean isIgnoreError)` | ServletRequest 参数转Bean |
| `cn.hutool.extra.servlet.ServletUtil` | `T fillBean(final ServletRequest request,T bean,CopyOptions copyOptions)` | ServletRequest 参数转Bean |
| `cn.hutool.extra.servlet.ServletUtil` | `T toBean(ServletRequest request,Class<T> beanClass,boolean isIgnoreError)` | ServletRequest 参数转Bean |
| `cn.hutool.extra.servlet.ServletUtil` | `boolean isGetMethod(HttpServletRequest request)` | 是否为GET请求 |
| `cn.hutool.extra.servlet.ServletUtil` | `boolean isIE(HttpServletRequest request)` | 客户浏览器是否为IE |
| `cn.hutool.extra.servlet.ServletUtil` | `boolean isMultipart(HttpServletRequest request)` | 是否为Multipart类型表单，此类型表单用于文件上传 |
| `cn.hutool.extra.servlet.ServletUtil` | `boolean isPostMethod(HttpServletRequest request)` | 是否为POST请求 |
| `cn.hutool.extra.servlet.ServletUtil` | `byte[] getBodyBytes(ServletRequest request)` | 获取请求体byte[] 调用该方法后，getParam方法将失效 |
| `cn.hutool.extra.servlet.ServletUtil` | `void addCookie(HttpServletResponse response,Cookie cookie)` | 设定返回给客户端的Cookie |
| `cn.hutool.extra.servlet.ServletUtil` | `void addCookie(HttpServletResponse response,String name,String value)` | 设定返回给客户端的Cookie |
| `cn.hutool.extra.servlet.ServletUtil` | `void addCookie(HttpServletResponse response,String name,String value,int maxAgeInSeconds)` | 设定返回给客户端的Cookie Path: "/" No Domain |
| `cn.hutool.extra.servlet.ServletUtil` | `void addCookie(HttpServletResponse response,String name,String value,int maxAgeInSeconds,String path,String domain)` | 设定返回给客户端的Cookie |
| `cn.hutool.extra.servlet.ServletUtil` | `void setHeader(HttpServletResponse response,String name,Object value)` | 设置响应的Header |
| `cn.hutool.extra.servlet.ServletUtil` | `void write(HttpServletResponse response,File file)` | 返回文件给客户端 |
| `cn.hutool.extra.servlet.ServletUtil` | `void write(HttpServletResponse response,InputStream in)` | 返回数据给客户端 |
| `cn.hutool.extra.servlet.ServletUtil` | `void write(HttpServletResponse response,InputStream in,String contentType)` | 返回数据给客户端 |
| `cn.hutool.extra.servlet.ServletUtil` | `void write(HttpServletResponse response,InputStream in,String contentType,String fileName)` | 返回数据给客户端 |
| `cn.hutool.extra.servlet.ServletUtil` | `void write(HttpServletResponse response,InputStream in,int bufferSize)` | 返回数据给客户端 |
| `cn.hutool.extra.servlet.ServletUtil` | `void write(HttpServletResponse response,String text,String contentType)` | 返回数据给客户端 |
