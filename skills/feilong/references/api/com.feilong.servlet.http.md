# com.feilong.servlet.http

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.servlet.http.CookieUtil`

```java
public final class com.feilong.servlet.http.CookieUtil {
  public static java.lang.String getCookieValue(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static java.lang.Integer getCookieIntegerValue(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static java.lang.Long getCookieLongValue(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static javax.servlet.http.Cookie getCookie(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static java.util.Map<java.lang.String, java.lang.String> getCookieMap(javax.servlet.http.HttpServletRequest);
  public static void deleteCookie(java.lang.String, javax.servlet.http.HttpServletResponse);
  public static void deleteCookie(com.feilong.servlet.http.entity.CookieEntity, javax.servlet.http.HttpServletResponse);
  public static void addCookie(java.lang.String, java.lang.String, javax.servlet.http.HttpServletResponse);
  public static void addCookie(java.lang.String, java.lang.String, int, javax.servlet.http.HttpServletResponse);
  public static void addCookie(com.feilong.servlet.http.entity.CookieEntity, javax.servlet.http.HttpServletResponse);
}
```

## `com.feilong.servlet.http.RequestException`

```java
public final class com.feilong.servlet.http.RequestException extends com.feilong.core.DefaultRuntimeException {
  public com.feilong.servlet.http.RequestException(java.lang.String, java.lang.Throwable);
  public com.feilong.servlet.http.RequestException(java.lang.Throwable);
}
```

## `com.feilong.servlet.http.RequestUtil`

```java
public final class com.feilong.servlet.http.RequestUtil {
  public static boolean isStaticResource(java.lang.String);
  public static boolean isSupportMethod(java.lang.String[], java.lang.String);
  public static boolean containsParam(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static java.util.Map<java.lang.String, java.lang.String[]> getParameterMap(javax.servlet.http.HttpServletRequest);
  public static java.util.Map<java.lang.String, java.lang.String> getParameterSingleValueMap(javax.servlet.http.HttpServletRequest);
  public static java.util.Map<java.lang.String, java.lang.Object> getRequestInfoMapForLog(javax.servlet.http.HttpServletRequest);
  public static java.util.Map<java.lang.String, java.lang.Object> getRequestInfoFullMapForLog(javax.servlet.http.HttpServletRequest);
  public static java.util.Map<java.lang.String, java.lang.Object> getRequestInfoMapForLog(javax.servlet.http.HttpServletRequest, com.feilong.servlet.http.entity.RequestLogSwitch);
  public static <T> T getAttribute(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static <T> T getAttribute(javax.servlet.http.HttpServletRequest, java.lang.String, T);
  public static <T> T getAttribute(javax.servlet.http.HttpServletRequest, java.lang.String, java.lang.Class<T>);
  public static <T> T getAttribute(javax.servlet.http.HttpServletRequest, java.lang.String, java.lang.Class<T>, T);
  public static java.lang.String getRequestURL(javax.servlet.http.HttpServletRequest);
  public static java.lang.String getOriginatingServletPath(javax.servlet.http.HttpServletRequest);
  public static java.lang.String getRequestFullURL(javax.servlet.http.HttpServletRequest);
  public static java.lang.String getRequestFullURL(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static java.lang.String parseParamsToQueryString(javax.servlet.http.HttpServletRequest);
  public static java.lang.String decodeISO88591String(java.lang.String, java.lang.String);
  public static java.lang.String getServerRootWithContextPath(javax.servlet.http.HttpServletRequest);
  public static void forward(java.lang.String, javax.servlet.http.HttpServletRequest, javax.servlet.http.HttpServletResponse);
  public static void include(java.lang.String, javax.servlet.http.HttpServletRequest, javax.servlet.http.HttpServletResponse);
  public static java.lang.String getHeader(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static java.lang.Integer getHeaderIntegerValue(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static java.lang.Long getHeaderLongValue(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static java.lang.String getClientIp(javax.servlet.http.HttpServletRequest);
  public static java.lang.String getHeaderUserAgent(javax.servlet.http.HttpServletRequest);
  public static java.lang.String getHeaderReferer(javax.servlet.http.HttpServletRequest);
  public static java.lang.String getHeaderOrigin(javax.servlet.http.HttpServletRequest);
  public static java.util.Map<java.lang.String, java.lang.String> getHeaderMap(javax.servlet.http.HttpServletRequest);
  public static boolean isGetMethod(javax.servlet.http.HttpServletRequest);
  public static boolean isPostMethod(javax.servlet.http.HttpServletRequest);
  public static boolean isWechatRequest(javax.servlet.http.HttpServletRequest);
  public static boolean isNotWechatRequest(javax.servlet.http.HttpServletRequest);
  public static boolean isWechatMiniProgramRequest(javax.servlet.http.HttpServletRequest);
  public static boolean isNotWechatMiniProgramRequest(javax.servlet.http.HttpServletRequest);
  public static boolean isAjaxRequest(javax.servlet.http.HttpServletRequest);
  public static boolean isNotAjaxRequest(javax.servlet.http.HttpServletRequest);
  public static java.util.Map<java.lang.String, java.lang.Object> getAttributeMap(javax.servlet.http.HttpServletRequest);
  public static java.lang.String getParameter(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static java.lang.String getParameterDefaultValue(javax.servlet.http.HttpServletRequest, java.lang.String, java.lang.String);
  public static <T> T getParameterDefaultValue(javax.servlet.http.HttpServletRequest, java.lang.String, java.lang.Class<T>, T);
  public static java.lang.Integer getParameterPageNo(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static java.lang.Integer getParameterPageSize(javax.servlet.http.HttpServletRequest, java.lang.String, java.lang.Integer);
  public static java.lang.String getRequestBody(javax.servlet.http.HttpServletRequest);
}
```

## `com.feilong.servlet.http.ResponseDownloadUtil`

```java
public final class com.feilong.servlet.http.ResponseDownloadUtil {
  public static void download(java.lang.String, javax.servlet.http.HttpServletRequest, javax.servlet.http.HttpServletResponse);
  public static void download(java.io.File, javax.servlet.http.HttpServletRequest, javax.servlet.http.HttpServletResponse);
  public static void download(java.lang.String, java.io.InputStream, java.lang.Number, javax.servlet.http.HttpServletRequest, javax.servlet.http.HttpServletResponse);
  public static void download(java.lang.String, java.io.InputStream, java.lang.Number, java.lang.String, java.lang.String, javax.servlet.http.HttpServletRequest, javax.servlet.http.HttpServletResponse);
}
```

## `com.feilong.servlet.http.ResponseUtil`

```java
public final class com.feilong.servlet.http.ResponseUtil {
  public static void sendRedirect(javax.servlet.http.HttpServletResponse, java.lang.String);
  public static void sendError(javax.servlet.http.HttpServletResponse, int);
  public static void sendError(javax.servlet.http.HttpServletResponse, int, java.lang.String);
  public static void setNoCacheHeader(javax.servlet.http.HttpServletResponse);
  public static void setCacheHeader(javax.servlet.http.HttpServletResponse, int);
  public static void writeText(javax.servlet.http.HttpServletResponse, java.lang.Object);
  public static void writeText(javax.servlet.http.HttpServletResponse, java.lang.Object, java.lang.String);
  public static void writeJson(javax.servlet.http.HttpServletResponse, java.lang.Object);
  public static void writeJson(javax.servlet.http.HttpServletResponse, java.lang.Object, java.lang.String);
  public static void write(javax.servlet.http.HttpServletResponse, java.lang.Object);
  public static void write(javax.servlet.http.HttpServletResponse, java.lang.Object, java.lang.String, java.lang.String);
  public static java.util.Map<java.lang.String, java.lang.Object> getResponseInfoMapForLog(javax.servlet.http.HttpServletResponse);
}
```

## `com.feilong.servlet.http.SessionUtil`

```java
public final class com.feilong.servlet.http.SessionUtil {
  public static java.lang.String getSessionId(javax.servlet.http.HttpServletRequest);
  public static <T> T getAttribute(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static <T> T getRequiredAttribute(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static void setAttribute(javax.servlet.http.HttpServletRequest, java.lang.String, java.io.Serializable);
  public static void removeAttribute(javax.servlet.http.HttpServletRequest, java.lang.String);
  public static java.util.Map<java.lang.String, java.lang.Object> getSessionInfoMapForLog(javax.servlet.http.HttpSession);
  public static java.util.Map<java.lang.String, java.io.Serializable> getAttributeMap(javax.servlet.http.HttpSession);
  public static javax.servlet.http.HttpSession replaceSession(javax.servlet.http.HttpServletRequest);
}
```
