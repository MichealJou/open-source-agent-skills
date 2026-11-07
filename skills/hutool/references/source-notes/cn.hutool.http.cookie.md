# cn.hutool.http.cookie

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.http.cookie.GlobalCookieManager` | `CookieManager getCookieManager()` | 获取全局CookieManager |
| `cn.hutool.http.cookie.GlobalCookieManager` | `List<HttpCookie> getCookies(HttpConnection conn)` | 获取指定域名下所有Cookie信息 |
| `cn.hutool.http.cookie.GlobalCookieManager` | `void add(HttpConnection conn)` | 将本地存储的Cookie信息附带到Http请求中，不覆盖用户定义好的Cookie |
| `cn.hutool.http.cookie.GlobalCookieManager` | `void setCookieManager(CookieManager customCookieManager)` | 自定义CookieManager |
| `cn.hutool.http.cookie.GlobalCookieManager` | `void store(HttpConnection conn)` | 存储响应的Cookie信息到本地 |
| `cn.hutool.http.cookie.ThreadLocalCookieStore` | `CookieStore getCookieStore()` | 获取本线程下的CookieStore |
| `cn.hutool.http.cookie.ThreadLocalCookieStore` | `List<HttpCookie> get(URI uri)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.cookie.ThreadLocalCookieStore` | `List<HttpCookie> getCookies()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.cookie.ThreadLocalCookieStore` | `List<URI> getURIs()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.cookie.ThreadLocalCookieStore` | `ThreadLocalCookieStore removeCurrent()` | 移除当前线程的Cookie |
| `cn.hutool.http.cookie.ThreadLocalCookieStore` | `boolean remove(URI uri,HttpCookie cookie)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.cookie.ThreadLocalCookieStore` | `boolean removeAll()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.cookie.ThreadLocalCookieStore` | `void add(URI uri,HttpCookie cookie)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
