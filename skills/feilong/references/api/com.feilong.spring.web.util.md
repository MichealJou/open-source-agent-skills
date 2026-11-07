# com.feilong.spring.web.util

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.spring.web.util.WebSpringUtil`

```java
public final class com.feilong.spring.web.util.WebSpringUtil {
  public static javax.servlet.http.HttpServletRequest getRequest();
  public static <T> T getBean(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static <T> T getBean(javax.servlet.http.HttpServletRequest, java.lang.Class<T>);
  public static <T> T getBean(javax.servlet.ServletContext, java.lang.String);
  public static <T> T getBean(javax.servlet.ServletContext, java.lang.Class<T>);
  public static <T> T getRequiredBean(javax.servlet.ServletContext, java.lang.String);
  public static <T> T getRequiredBean(javax.servlet.ServletContext, java.lang.Class<T>);
  public static org.springframework.web.context.WebApplicationContext getWebApplicationContext(javax.servlet.ServletContext);
  public static org.springframework.web.context.WebApplicationContext getRequiredWebApplicationContext(javax.servlet.ServletContext);
  public static org.springframework.web.context.WebApplicationContext getWebApplicationContext(javax.servlet.http.HttpServletRequest);
}
```
