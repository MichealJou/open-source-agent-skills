# com.feilong.servlet.http.entity

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.servlet.http.entity.CookieEntity` | `String getComment()` | 获得 ;Comment=VALUE . |
| `com.feilong.servlet.http.entity.CookieEntity` | `String getDomain()` | 获得 ;Domain=VALUE. 和路径类似,主机名是指同一个域下的不同主机,例如:www.google.com和gmail.google.com就是两个不同的主机名. 默认情况下,一个主机中创建的cookie在另一个主机下是不能被访问的, 但可以通过domain参数来实现对其的控制, 其语法格式为: document.cookie="name=value; domain=cookieDomain"; |
| `com.feilong.servlet.http.entity.CookieEntity` | `String getName()` | Gets the name名称,名字和值都不能包含空白字符以及下列字符: @ : ;? , " / [ ] ( ) = 这些符号. |
| `com.feilong.servlet.http.entity.CookieEntity` | `String getPath()` | 获得 ;Path=VALUE . ;Path=VALUE ... URLs that see the cookie 当不设置值的时候(tomcat默认情况),如果在某个页面创建了一个cookie,那么该页面所在目录中的其他页面也可以访问该cookie,如果这个目录下还有子目录,则在子目录中也可以访问. 为了方便使用cookie,特意将此默认值设置为/,表示所有页面均可读取改cookie |
| `com.feilong.servlet.http.entity.CookieEntity` | `String getValue()` | value,名字和值都不能包含空白字符以及下列字符: @ : ;? , " / [ ] ( ) = 这些符号. 注意:如果值长度超过4K,浏览器会忽略,不会执行记录的操作 |
| `com.feilong.servlet.http.entity.CookieEntity` | `boolean getHttpOnly()` | Not in cookie specs, but supported by browsers. 如果在Cookie中设置了"HttpOnly"属性,那么通过程序(JS脚本、Applet等)将无法读取到Cookie信息,这样能有效的防止XSS攻击. |
| `com.feilong.servlet.http.entity.CookieEntity` | `boolean getSecure()` | ;Secure ... e.g. use SSL. 指定是否cookie应该只通过安全协议,例如HTTPS或SSL,传送给浏览器. secure值为true时,在http中是无效的; 在https中才有效 keep cookie communication limited to encrypted transmission, directing browsers to use cookies only via secure/encrypted connections. However, if a web server sets a cookie with a secure attribute … |
| `com.feilong.servlet.http.entity.CookieEntity` | `int getMaxAge()` | 获得 设置存活时间,单位秒. |
| `com.feilong.servlet.http.entity.CookieEntity` | `int getVersion()` | 【原文待译】supports both the Version 0 (by Netscape) and Version 1 (by RFC 2109) cookie specifications. By default, cookies are created using Version 0 to ensure the best interoperability. ;Version=1 ... means RFC 2109++ style |
| `com.feilong.servlet.http.entity.CookieEntity` | `void setComment(String comment)` | 设置 ;Comment=VALUE . |
| `com.feilong.servlet.http.entity.CookieEntity` | `void setDomain(String domain)` | 设置 ;Domain=VALUE . 和路径类似,主机名是指同一个域下的不同主机,例如:www.google.com和gmail.google.com就是两个不同的主机名. 默认情况下,一个主机中创建的cookie在另一个主机下是不能被访问的, 但可以通过domain参数来实现对其的控制, 其语法格式为: document.cookie="name=value; domain=cookieDomain"; |
| `com.feilong.servlet.http.entity.CookieEntity` | `void setHttpOnly(boolean httpOnly)` | Not in cookie specs, but supported by browsers. 如果在Cookie中设置了"HttpOnly"属性,那么通过程序(JS脚本、Applet等)将无法读取到Cookie信息,这样能有效的防止XSS攻击. |
| `com.feilong.servlet.http.entity.CookieEntity` | `void setMaxAge(int maxAge)` | 设置 设置存活时间,单位秒. |
| `com.feilong.servlet.http.entity.CookieEntity` | `void setName(String name)` | Sets the name名称,名字和值都不能包含空白字符以及下列字符: @ : ;? , " / [ ] ( ) = 这些符号. |
| `com.feilong.servlet.http.entity.CookieEntity` | `void setPath(String path)` | 设置 ;Path=VALUE . ;Path=VALUE ... URLs that see the cookie 当不设置值的时候(tomcat默认情况),如果在某个页面创建了一个cookie,那么该页面所在目录中的其他页面也可以访问该cookie,如果这个目录下还有子目录,则在子目录中也可以访问. 为了方便使用cookie,特意将此默认值设置为/,表示所有页面均可读取改cookie |
| `com.feilong.servlet.http.entity.CookieEntity` | `void setSecure(boolean secure)` | ;Secure ... e.g. use SSL. 指定是否cookie应该只通过安全协议,例如HTTPS或SSL,传送给浏览器. secure值为true时,在http中是无效的; 在https中才有效 keep cookie communication limited to encrypted transmission, directing browsers to use cookies only via secure/encrypted connections. However, if a web server sets a cookie with a secure attribute … |
| `com.feilong.servlet.http.entity.CookieEntity` | `void setValue(String value)` | value,名字和值都不能包含空白字符以及下列字符: @ : ;? , " / [ ] ( ) = 这些符号. 注意:如果值长度超过4K,浏览器会忽略,不会执行记录的操作 |
| `com.feilong.servlet.http.entity.CookieEntity` | `void setVersion(int version)` | 【原文待译】supports both the Version 0 (by Netscape) and Version 1 (by RFC 2109) cookie specifications. By default, cookies are created using Version 0 to ensure the best interoperability. ;Version=1 ... means RFC 2109++ style |
| `com.feilong.servlet.http.entity.RequestIdentity` | `String getClientIP()` | 获得 用户客户端ip. |
| `com.feilong.servlet.http.entity.RequestIdentity` | `String getSessionId()` | 获得 用户 sessionId. |
| `com.feilong.servlet.http.entity.RequestIdentity` | `String getUserAgent()` | 获得 用户userAgent. |
| `com.feilong.servlet.http.entity.RequestIdentity` | `void setClientIP(String clientIP)` | 设置 用户客户端ip. |
| `com.feilong.servlet.http.entity.RequestIdentity` | `void setSessionId(String sessionId)` | 设置 用户 sessionId. |
| `com.feilong.servlet.http.entity.RequestIdentity` | `void setUserAgent(String userAgent)` | 设置 用户userAgent. |
| `com.feilong.servlet.http.entity.RequestLogSwitch` | `boolean getShowCookies()` | Gets the 显示cookie. |
| `com.feilong.servlet.http.entity.RequestLogSwitch` | `boolean getShowElses()` | Gets the 显示和else相关. |
| `com.feilong.servlet.http.entity.RequestLogSwitch` | `boolean getShowErrors()` | 显示和Error相关. |
| `com.feilong.servlet.http.entity.RequestLogSwitch` | `boolean getShowForwardInfos()` | 获得 显示和forward相关. |
| `com.feilong.servlet.http.entity.RequestLogSwitch` | `boolean getShowFullURL()` | Gets the 显示和FullURL相关. |
| `com.feilong.servlet.http.entity.RequestLogSwitch` | `boolean getShowHeaders()` | Gets the 显示和Header相关. |
| `com.feilong.servlet.http.entity.RequestLogSwitch` | `boolean getShowIPs()` | Gets the 显示和ip相关. |
| `com.feilong.servlet.http.entity.RequestLogSwitch` | `boolean getShowIdentity()` | 获得 显示IDENTITY(包含ip以及UA). |
| `com.feilong.servlet.http.entity.RequestLogSwitch` | `boolean getShowIncludeInfos()` | 获得 显示和include相关信息. |
| `com.feilong.servlet.http.entity.RequestLogSwitch` | `boolean getShowMethod()` | Gets the 显示和Method. |
| `com.feilong.servlet.http.entity.RequestLogSwitch` | `boolean getShowParams()` | Gets the 显示参数. |
| `com.feilong.servlet.http.entity.RequestLogSwitch` | `boolean getShowPorts()` | Gets the 显示和Port相关. |
| `com.feilong.servlet.http.entity.RequestLogSwitch` | `boolean getShowURLs()` | Gets the 显示和url相关. |
