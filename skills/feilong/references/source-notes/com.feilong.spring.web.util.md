# com.feilong.spring.web.util

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.spring.web.util.WebSpringUtil` | `HttpServletRequest getRequest()` | 获得 request. |
| `com.feilong.spring.web.util.WebSpringUtil` | `T getBean(HttpServletRequest request,Class<T> requiredType)` | Gets the bean. 此方法底层调用的是 RequestContextUtils#getWebApplicationContext(ServletRequest, ServletContext) ,会从spingmvc 以及spring ApplicationContext 查找bean |
| `com.feilong.spring.web.util.WebSpringUtil` | `T getBean(HttpServletRequest request,String beanName)` | 普通类获得spring 注入的类方法. 此方法底层调用的是 RequestContextUtils#getWebApplicationContext(ServletRequest, ServletContext) ,会从spingmvc 以及spring ApplicationContext 查找bean |
| `com.feilong.spring.web.util.WebSpringUtil` | `T getBean(ServletContext servletContext,Class<T> requiredType)` | 【原文待译】Gets the bean. |
| `com.feilong.spring.web.util.WebSpringUtil` | `T getBean(ServletContext servletContext,String beanName)` | 普通类获得spring 注入的类方法. 注意: (如果找不到bean,返回null) . |
| `com.feilong.spring.web.util.WebSpringUtil` | `T getRequiredBean(ServletContext servletContext,Class<T> requiredType)` | 【原文待译】Gets the required bean. |
| `com.feilong.spring.web.util.WebSpringUtil` | `T getRequiredBean(ServletContext servletContext,String beanName)` | 【原文待译】Gets the required bean. |
| `com.feilong.spring.web.util.WebSpringUtil` | `WebApplicationContext getRequiredWebApplicationContext(ServletContext servletContext)` | 获得 web application context. |
| `com.feilong.spring.web.util.WebSpringUtil` | `WebApplicationContext getWebApplicationContext(HttpServletRequest request)` | 获得 web application context. 此方法可以得到springmvc 的bean |
| `com.feilong.spring.web.util.WebSpringUtil` | `WebApplicationContext getWebApplicationContext(ServletContext servletContext)` | 【原文待译】Find the root WebApplicationContext for this web app, typically loaded via org.springframework.web.context.ContextLoaderListener. Will rethrow an exception that happened on root context startup, to differentiate between a failed context startup and no context at all. |
