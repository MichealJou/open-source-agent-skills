# com.feilong.taglib.display.httpconcat

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.taglib.display.httpconcat.HttpConcatTag` | `String buildCacheTagKey()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.display.httpconcat.HttpConcatTag` | `void setDomain(String domain)` | 域名,如果没有设置,将自动使用 HttpServletRequest#getContextPath(). |
| `com.feilong.taglib.display.httpconcat.HttpConcatTag` | `void setHttpConcatSupport(Boolean httpConcatSupport)` | 设置 是否支持 http concat(如果设置这个参数,本次渲染将会覆盖全局变量). |
| `com.feilong.taglib.display.httpconcat.HttpConcatTag` | `void setRoot(String root)` | Sets the 根目录. 如果设置root为'/script' 会拼成http://staging. |
| `com.feilong.taglib.display.httpconcat.HttpConcatTag` | `void setType(String type)` | Sets the 类型css/js. |
| `com.feilong.taglib.display.httpconcat.HttpConcatTag` | `void setVersion(String version)` | Sets the 版本号. |
| `com.feilong.taglib.display.httpconcat.HttpConcatUtil` | `String getWriteContent(HttpConcatParam httpConcatParam)` | 获得解析的内容. |
