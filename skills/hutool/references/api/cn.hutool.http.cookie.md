# cn.hutool.http.cookie

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.http.cookie.GlobalCookieManager`

```java
public class cn.hutool.http.cookie.GlobalCookieManager {
  public cn.hutool.http.cookie.GlobalCookieManager();
  public static void setCookieManager(java.net.CookieManager);
  public static java.net.CookieManager getCookieManager();
  public static java.util.List<java.net.HttpCookie> getCookies(cn.hutool.http.HttpConnection);
  public static void add(cn.hutool.http.HttpConnection);
  public static void store(cn.hutool.http.HttpConnection);
}
```

## `cn.hutool.http.cookie.ThreadLocalCookieStore`

```java
public class cn.hutool.http.cookie.ThreadLocalCookieStore implements java.net.CookieStore {
  public cn.hutool.http.cookie.ThreadLocalCookieStore();
  public java.net.CookieStore getCookieStore();
  public cn.hutool.http.cookie.ThreadLocalCookieStore removeCurrent();
  public void add(java.net.URI, java.net.HttpCookie);
  public java.util.List<java.net.HttpCookie> get(java.net.URI);
  public java.util.List<java.net.HttpCookie> getCookies();
  public java.util.List<java.net.URI> getURIs();
  public boolean remove(java.net.URI, java.net.HttpCookie);
  public boolean removeAll();
}
```
