# cn.hutool.http.server

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.http.server.HttpExchangeWrapper`

```java
public class cn.hutool.http.server.HttpExchangeWrapper extends com.sun.net.httpserver.HttpExchange {
  public cn.hutool.http.server.HttpExchangeWrapper(com.sun.net.httpserver.HttpExchange);
  public com.sun.net.httpserver.HttpExchange getRaw();
  public cn.hutool.http.server.HttpServerRequest getRequest();
  public cn.hutool.http.server.HttpServerResponse getResponse();
  public com.sun.net.httpserver.Headers getRequestHeaders();
  public com.sun.net.httpserver.Headers getResponseHeaders();
  public java.net.URI getRequestURI();
  public java.lang.String getRequestMethod();
  public com.sun.net.httpserver.HttpContext getHttpContext();
  public void close();
  public java.io.InputStream getRequestBody();
  public java.io.OutputStream getResponseBody();
  public void sendResponseHeaders(int, long) throws java.io.IOException;
  public java.net.InetSocketAddress getRemoteAddress();
  public int getResponseCode();
  public java.net.InetSocketAddress getLocalAddress();
  public java.lang.String getProtocol();
  public java.lang.Object getAttribute(java.lang.String);
  public void setAttribute(java.lang.String, java.lang.Object);
  public void setStreams(java.io.InputStream, java.io.OutputStream);
  public com.sun.net.httpserver.HttpPrincipal getPrincipal();
}
```

## `cn.hutool.http.server.HttpServerBase`

```java
public class cn.hutool.http.server.HttpServerBase implements java.io.Closeable {
  public cn.hutool.http.server.HttpServerBase(com.sun.net.httpserver.HttpExchange);
  public com.sun.net.httpserver.HttpExchange getHttpExchange();
  public com.sun.net.httpserver.HttpContext getHttpContext();
  public void close();
}
```

## `cn.hutool.http.server.HttpServerRequest`

```java
public class cn.hutool.http.server.HttpServerRequest extends cn.hutool.http.server.HttpServerBase {
  public cn.hutool.http.server.HttpServerRequest(com.sun.net.httpserver.HttpExchange);
  public java.lang.String getMethod();
  public boolean isGetMethod();
  public boolean isPostMethod();
  public java.net.URI getURI();
  public java.lang.String getPath();
  public java.lang.String getQuery();
  public com.sun.net.httpserver.Headers getHeaders();
  public java.lang.String getHeader(cn.hutool.http.Header);
  public java.lang.String getHeader(java.lang.String);
  public java.lang.String getHeader(java.lang.String, java.nio.charset.Charset);
  public java.lang.String getContentType();
  public java.nio.charset.Charset getCharset();
  public java.lang.String getUserAgentStr();
  public cn.hutool.http.useragent.UserAgent getUserAgent();
  public java.lang.String getCookiesStr();
  public java.util.Collection<java.net.HttpCookie> getCookies();
  public java.util.Map<java.lang.String, java.net.HttpCookie> getCookieMap();
  public java.net.HttpCookie getCookie(java.lang.String);
  public boolean isMultipart();
  public java.lang.String getBody();
  public java.lang.String getBody(java.nio.charset.Charset);
  public byte[] getBodyBytes();
  public java.io.InputStream getBodyStream();
  public java.lang.String getParam(java.lang.String);
  public java.util.List<java.lang.String> getParams(java.lang.String);
  public cn.hutool.core.map.multi.ListValueMap<java.lang.String, java.lang.String> getParams();
  public java.lang.String getClientIP(java.lang.String...);
  public java.lang.String getClientIPByHeader(java.lang.String...);
  public cn.hutool.core.net.multipart.MultipartFormData getMultipart() throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.net.multipart.MultipartFormData parseMultipart(cn.hutool.core.net.multipart.UploadSetting) throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.http.server.HttpServerResponse`

```java
public class cn.hutool.http.server.HttpServerResponse extends cn.hutool.http.server.HttpServerBase {
  public cn.hutool.http.server.HttpServerResponse(com.sun.net.httpserver.HttpExchange);
  public cn.hutool.http.server.HttpServerResponse send(int);
  public cn.hutool.http.server.HttpServerResponse sendOk();
  public cn.hutool.http.server.HttpServerResponse sendOk(int);
  public cn.hutool.http.server.HttpServerResponse send404(java.lang.String);
  public cn.hutool.http.server.HttpServerResponse sendError(int, java.lang.String);
  public cn.hutool.http.server.HttpServerResponse send(int, long);
  public com.sun.net.httpserver.Headers getHeaders();
  public cn.hutool.http.server.HttpServerResponse addHeader(java.lang.String, java.lang.String);
  public cn.hutool.http.server.HttpServerResponse setHeader(cn.hutool.http.Header, java.lang.String);
  public cn.hutool.http.server.HttpServerResponse setHeader(java.lang.String, java.lang.String);
  public cn.hutool.http.server.HttpServerResponse setHeader(java.lang.String, java.util.List<java.lang.String>);
  public cn.hutool.http.server.HttpServerResponse setHeaders(java.util.Map<java.lang.String, java.util.List<java.lang.String>>);
  public cn.hutool.http.server.HttpServerResponse setContentType(java.lang.String);
  public cn.hutool.http.server.HttpServerResponse setContentLength(long);
  public cn.hutool.http.server.HttpServerResponse setCharset(java.nio.charset.Charset);
  public cn.hutool.http.server.HttpServerResponse setAttr(java.lang.String, java.lang.Object);
  public java.io.OutputStream getOut();
  public java.io.PrintWriter getWriter();
  public cn.hutool.http.server.HttpServerResponse write(java.lang.String, java.lang.String);
  public cn.hutool.http.server.HttpServerResponse write(java.lang.String);
  public cn.hutool.http.server.HttpServerResponse write(byte[], java.lang.String);
  public cn.hutool.http.server.HttpServerResponse write(byte[]);
  public cn.hutool.http.server.HttpServerResponse write(java.io.InputStream, java.lang.String);
  public cn.hutool.http.server.HttpServerResponse write(java.io.InputStream, int, java.lang.String);
  public cn.hutool.http.server.HttpServerResponse write(java.io.InputStream);
  public cn.hutool.http.server.HttpServerResponse write(java.io.InputStream, int);
  public cn.hutool.http.server.HttpServerResponse write(java.io.File);
  public cn.hutool.http.server.HttpServerResponse write(java.io.File, java.lang.String);
  public void write(java.io.InputStream, java.lang.String, java.lang.String);
  public cn.hutool.http.server.HttpServerResponse write(java.io.InputStream, int, java.lang.String, java.lang.String);
}
```

## `cn.hutool.http.server.SimpleServer`

```java
public class cn.hutool.http.server.SimpleServer {
  public cn.hutool.http.server.SimpleServer(int);
  public cn.hutool.http.server.SimpleServer(java.lang.String, int);
  public cn.hutool.http.server.SimpleServer(java.net.InetSocketAddress);
  public cn.hutool.http.server.SimpleServer(java.net.InetSocketAddress, com.sun.net.httpserver.HttpsConfigurator);
  public cn.hutool.http.server.SimpleServer addFilter(com.sun.net.httpserver.Filter);
  public cn.hutool.http.server.SimpleServer addFilter(cn.hutool.http.server.filter.HttpFilter);
  public cn.hutool.http.server.SimpleServer addHandler(java.lang.String, com.sun.net.httpserver.HttpHandler);
  public com.sun.net.httpserver.HttpContext createContext(java.lang.String, com.sun.net.httpserver.HttpHandler);
  public cn.hutool.http.server.SimpleServer setRoot(java.lang.String);
  public cn.hutool.http.server.SimpleServer setRoot(java.io.File);
  public cn.hutool.http.server.SimpleServer addAction(java.lang.String, cn.hutool.http.server.action.Action);
  public cn.hutool.http.server.SimpleServer setExecutor(java.util.concurrent.Executor);
  public com.sun.net.httpserver.HttpServer getRawServer();
  public java.net.InetSocketAddress getAddress();
  public void start();
}
```
