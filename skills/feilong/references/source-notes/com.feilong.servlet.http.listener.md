# com.feilong.servlet.http.listener

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.servlet.http.listener.AbstractServletContextDestroyedListener` | `void contextDestroyed(ServletContextEvent servletContextEvent)` | 【原文待译】Receives notification that the ServletContext is about to be shut down. All servlets and filters will have been destroyed before any ServletContextListeners are notified of context destruction. |
| `com.feilong.servlet.http.listener.AbstractServletContextDestroyedListener` | `void contextInitialized(ServletContextEvent servletContextEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.AbstractServletContextInitializedListener` | `void contextDestroyed(ServletContextEvent servletContextEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.AbstractServletContextInitializedListener` | `void contextInitialized(ServletContextEvent servletContextEvent)` | 【原文待译】Receives notification that the web application initialization process is starting. All ServletContextListeners are notified of context initialization before any filters or servlets in the web application are initialized. |
| `com.feilong.servlet.http.listener.HttpSessionAttributeLoggingListener` | `void attributeAdded(HttpSessionBindingEvent httpSessionBindingEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.HttpSessionAttributeLoggingListener` | `void attributeRemoved(HttpSessionBindingEvent httpSessionBindingEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.HttpSessionAttributeLoggingListener` | `void attributeReplaced(HttpSessionBindingEvent httpSessionBindingEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.HttpSessionLoggingListener` | `void sessionCreated(HttpSessionEvent httpSessionEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.HttpSessionLoggingListener` | `void sessionDestroyed(HttpSessionEvent httpSessionEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.ServletContextAttributeLoggingListener` | `void attributeAdded(ServletContextAttributeEvent servletContextAttributeEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.ServletContextAttributeLoggingListener` | `void attributeRemoved(ServletContextAttributeEvent servletContextAttributeEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.ServletContextAttributeLoggingListener` | `void attributeReplaced(ServletContextAttributeEvent servletContextAttributeEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.ServletContextLoggingListener` | `void contextDestroyed(ServletContextEvent servletContextEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.ServletContextLoggingListener` | `void contextInitialized(ServletContextEvent servletContextEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.ServletRequestAttributeLoggingListener` | `void attributeAdded(ServletRequestAttributeEvent servletRequestAttributeEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.ServletRequestAttributeLoggingListener` | `void attributeRemoved(ServletRequestAttributeEvent servletRequestAttributeEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.ServletRequestAttributeLoggingListener` | `void attributeReplaced(ServletRequestAttributeEvent servletRequestAttributeEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.ServletRequestLoggingListener` | `void requestDestroyed(ServletRequestEvent servletRequestEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.servlet.http.listener.ServletRequestLoggingListener` | `void requestInitialized(ServletRequestEvent servletRequestEvent)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
