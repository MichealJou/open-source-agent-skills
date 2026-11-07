# cn.hutool.extra.servlet

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.servlet.JakartaServletUtil`

```java
public class cn.hutool.extra.servlet.JakartaServletUtil {
  public cn.hutool.extra.servlet.JakartaServletUtil();
  public static java.util.Map<java.lang.String, java.lang.String[]> getParams(jakarta.servlet.ServletRequest);
  public static java.util.Map<java.lang.String, java.lang.String> getParamMap(jakarta.servlet.ServletRequest);
  public static java.lang.String getBody(jakarta.servlet.ServletRequest);
  public static byte[] getBodyBytes(jakarta.servlet.ServletRequest);
  public static <T> T fillBean(jakarta.servlet.ServletRequest, T, cn.hutool.core.bean.copier.CopyOptions);
  public static <T> T fillBean(jakarta.servlet.ServletRequest, T, boolean);
  public static <T> T toBean(jakarta.servlet.ServletRequest, java.lang.Class<T>, boolean);
  public static java.lang.String getClientIP(jakarta.servlet.http.HttpServletRequest, java.lang.String...);
  public static java.lang.String getClientIPByHeader(jakarta.servlet.http.HttpServletRequest, java.lang.String...);
  public static cn.hutool.core.net.multipart.MultipartFormData getMultipart(jakarta.servlet.ServletRequest) throws cn.hutool.core.io.IORuntimeException;
  public static cn.hutool.core.net.multipart.MultipartFormData getMultipart(jakarta.servlet.ServletRequest, cn.hutool.core.net.multipart.UploadSetting) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.Map<java.lang.String, java.lang.String> getHeaderMap(jakarta.servlet.http.HttpServletRequest);
  public static java.util.Map<java.lang.String, java.util.List<java.lang.String>> getHeadersMap(jakarta.servlet.http.HttpServletRequest);
  public static java.util.Map<java.lang.String, java.util.Collection<java.lang.String>> getHeadersMap(jakarta.servlet.http.HttpServletResponse);
  public static java.lang.String getHeaderIgnoreCase(jakarta.servlet.http.HttpServletRequest, java.lang.String);
  public static java.lang.String getHeader(jakarta.servlet.http.HttpServletRequest, java.lang.String, java.lang.String);
  public static java.lang.String getHeader(jakarta.servlet.http.HttpServletRequest, java.lang.String, java.nio.charset.Charset);
  public static boolean isIE(jakarta.servlet.http.HttpServletRequest);
  public static boolean isGetMethod(jakarta.servlet.http.HttpServletRequest);
  public static boolean isPostMethod(jakarta.servlet.http.HttpServletRequest);
  public static boolean isMultipart(jakarta.servlet.http.HttpServletRequest);
  public static jakarta.servlet.http.Cookie getCookie(jakarta.servlet.http.HttpServletRequest, java.lang.String);
  public static java.util.Map<java.lang.String, jakarta.servlet.http.Cookie> readCookieMap(jakarta.servlet.http.HttpServletRequest);
  public static void addCookie(jakarta.servlet.http.HttpServletResponse, jakarta.servlet.http.Cookie);
  public static void addCookie(jakarta.servlet.http.HttpServletResponse, java.lang.String, java.lang.String);
  public static void addCookie(jakarta.servlet.http.HttpServletResponse, java.lang.String, java.lang.String, int, java.lang.String, java.lang.String);
  public static void addCookie(jakarta.servlet.http.HttpServletResponse, java.lang.String, java.lang.String, int);
  public static java.io.PrintWriter getWriter(jakarta.servlet.http.HttpServletResponse) throws cn.hutool.core.io.IORuntimeException;
  public static void write(jakarta.servlet.http.HttpServletResponse, java.lang.String, java.lang.String);
  public static void write(jakarta.servlet.http.HttpServletResponse, java.io.File);
  public static void write(jakarta.servlet.http.HttpServletResponse, java.io.InputStream, java.lang.String, java.lang.String);
  public static void write(jakarta.servlet.http.HttpServletResponse, java.io.InputStream, java.lang.String);
  public static void write(jakarta.servlet.http.HttpServletResponse, java.io.InputStream);
  public static void write(jakarta.servlet.http.HttpServletResponse, java.io.InputStream, int);
  public static void setHeader(jakarta.servlet.http.HttpServletResponse, java.lang.String, java.lang.Object);
}
```

## `cn.hutool.extra.servlet.ServletUtil`

```java
public class cn.hutool.extra.servlet.ServletUtil {
  public cn.hutool.extra.servlet.ServletUtil();
  public static java.util.Map<java.lang.String, java.lang.String[]> getParams(javax.servlet.ServletRequest);
  public static java.util.Map<java.lang.String, java.lang.String> getParamMap(javax.servlet.ServletRequest);
  public static java.lang.String getBody(javax.servlet.ServletRequest);
  public static byte[] getBodyBytes(javax.servlet.ServletRequest);
  public static <T> T fillBean(javax.servlet.ServletRequest, T, cn.hutool.core.bean.copier.CopyOptions);
  public static <T> T fillBean(javax.servlet.ServletRequest, T, boolean);
  public static <T> T toBean(javax.servlet.ServletRequest, java.lang.Class<T>, boolean);
  public static java.lang.String getClientIP(javax.servlet.http.HttpServletRequest, java.lang.String...);
  public static java.lang.String getClientIPByHeader(javax.servlet.http.HttpServletRequest, java.lang.String...);
  public static cn.hutool.core.net.multipart.MultipartFormData getMultipart(javax.servlet.ServletRequest) throws cn.hutool.core.io.IORuntimeException;
  public static cn.hutool.core.net.multipart.MultipartFormData getMultipart(javax.servlet.ServletRequest, cn.hutool.core.net.multipart.UploadSetting) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.Map<java.lang.String, java.lang.String> getHeaderMap(javax.servlet.http.HttpServletRequest);
  public static java.util.Map<java.lang.String, java.util.List<java.lang.String>> getHeadersMap(javax.servlet.http.HttpServletRequest);
  public static java.util.Map<java.lang.String, java.util.Collection<java.lang.String>> getHeadersMap(javax.servlet.http.HttpServletResponse);
  public static java.lang.String getHeaderIgnoreCase(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static java.lang.String getHeader(javax.servlet.http.HttpServletRequest, java.lang.String, java.lang.String);
  public static java.lang.String getHeader(javax.servlet.http.HttpServletRequest, java.lang.String, java.nio.charset.Charset);
  public static boolean isIE(javax.servlet.http.HttpServletRequest);
  public static boolean isGetMethod(javax.servlet.http.HttpServletRequest);
  public static boolean isPostMethod(javax.servlet.http.HttpServletRequest);
  public static boolean isMultipart(javax.servlet.http.HttpServletRequest);
  public static javax.servlet.http.Cookie getCookie(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static java.util.Map<java.lang.String, javax.servlet.http.Cookie> readCookieMap(javax.servlet.http.HttpServletRequest);
  public static void addCookie(javax.servlet.http.HttpServletResponse, javax.servlet.http.Cookie);
  public static void addCookie(javax.servlet.http.HttpServletResponse, java.lang.String, java.lang.String);
  public static void addCookie(javax.servlet.http.HttpServletResponse, java.lang.String, java.lang.String, int, java.lang.String, java.lang.String);
  public static void addCookie(javax.servlet.http.HttpServletResponse, java.lang.String, java.lang.String, int);
  public static java.io.PrintWriter getWriter(javax.servlet.http.HttpServletResponse) throws cn.hutool.core.io.IORuntimeException;
  public static void write(javax.servlet.http.HttpServletResponse, java.lang.String, java.lang.String);
  public static void write(javax.servlet.http.HttpServletResponse, java.io.File);
  public static void write(javax.servlet.http.HttpServletResponse, java.io.InputStream, java.lang.String, java.lang.String);
  public static void write(javax.servlet.http.HttpServletResponse, java.io.InputStream, java.lang.String);
  public static void write(javax.servlet.http.HttpServletResponse, java.io.InputStream);
  public static void write(javax.servlet.http.HttpServletResponse, java.io.InputStream, int);
  public static void setHeader(javax.servlet.http.HttpServletResponse, java.lang.String, java.lang.Object);
}
```
