# com.feilong.servlet

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.servlet.ServletContextUtil` | `Map<String, Object> getAttributeMap(ServletContext servletContext)` | 遍历显示servletContext的 javax.servlet.ServletContext#getAttributeNames() ServletContext.getAttributeNames(),将 name/attributeValue 存入到map. |
| `com.feilong.servlet.ServletContextUtil` | `Map<String, Object> getAttributeMap(ServletContext servletContext,boolean ignoreContainerAttribute)` | 遍历显示servletContext的 javax.servlet.ServletContext#getAttributeNames() ServletContext.getAttributeNames(),将 name/attributeValue 存入到map. |
| `com.feilong.servlet.ServletContextUtil` | `Map<String, Object> getServletContextInfoMapForLog(ServletContext servletContext)` | servletContext.log servletContext相关信息,一般启动时调用. |
| `com.feilong.servlet.ServletContextUtil` | `Map<String, String> getInitParameterMap(ServletContext servletContext)` | 遍历显示servletContext的 ServletContext#getInitParameterNames(),将 name /attributeValue 存入到map返回. |
| `com.feilong.servlet.ServletContextUtil` | `String[] getIgnoreKeys()` | 获取要忽略的keys. |
