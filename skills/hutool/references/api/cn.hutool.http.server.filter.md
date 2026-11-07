# cn.hutool.http.server.filter

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.http.server.filter.DefaultExceptionFilter`

```java
public class cn.hutool.http.server.filter.DefaultExceptionFilter extends cn.hutool.http.server.filter.ExceptionFilter {
  public cn.hutool.http.server.filter.DefaultExceptionFilter();
  public void afterException(cn.hutool.http.server.HttpServerRequest, cn.hutool.http.server.HttpServerResponse, java.lang.Throwable);
}
```

## `cn.hutool.http.server.filter.ExceptionFilter`

```java
public abstract class cn.hutool.http.server.filter.ExceptionFilter implements cn.hutool.http.server.filter.HttpFilter {
  public cn.hutool.http.server.filter.ExceptionFilter();
  public void doFilter(cn.hutool.http.server.HttpServerRequest, cn.hutool.http.server.HttpServerResponse, com.sun.net.httpserver.Filter$Chain);
  public abstract void afterException(cn.hutool.http.server.HttpServerRequest, cn.hutool.http.server.HttpServerResponse, java.lang.Throwable);
}
```

## `cn.hutool.http.server.filter.HttpFilter`

```java
public interface cn.hutool.http.server.filter.HttpFilter {
  public abstract void doFilter(cn.hutool.http.server.HttpServerRequest, cn.hutool.http.server.HttpServerResponse, com.sun.net.httpserver.Filter$Chain) throws java.io.IOException;
}
```

## `cn.hutool.http.server.filter.SimpleFilter`

```java
public abstract class cn.hutool.http.server.filter.SimpleFilter extends com.sun.net.httpserver.Filter {
  public cn.hutool.http.server.filter.SimpleFilter();
  public java.lang.String description();
}
```
