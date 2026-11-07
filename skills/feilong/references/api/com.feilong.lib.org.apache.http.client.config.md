# com.feilong.lib.org.apache.http.client.config

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.client.config.RequestConfig`

```java
public class com.feilong.lib.org.apache.http.client.config.RequestConfig implements java.lang.Cloneable {
  public boolean isExpectContinueEnabled();
  public com.feilong.lib.org.apache.http.HttpHost getProxy();
  public java.net.InetAddress getLocalAddress();
  public boolean isStaleConnectionCheckEnabled();
  public java.lang.String getCookieSpec();
  public boolean isRedirectsEnabled();
  public boolean isRelativeRedirectsAllowed();
  public boolean isCircularRedirectsAllowed();
  public int getMaxRedirects();
  public boolean isAuthenticationEnabled();
  public java.util.Collection<java.lang.String> getTargetPreferredAuthSchemes();
  public java.util.Collection<java.lang.String> getProxyPreferredAuthSchemes();
  public int getConnectionRequestTimeout();
  public int getConnectTimeout();
  public int getSocketTimeout();
  public boolean isDecompressionEnabled();
  public boolean isContentCompressionEnabled();
  public boolean isNormalizeUri();
  public java.lang.String toString();
  public static com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder custom();
  public static com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder copy(com.feilong.lib.org.apache.http.client.config.RequestConfig);
}
```

## `com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder`

```java
public class com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder {
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setExpectContinueEnabled(boolean);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setProxy(com.feilong.lib.org.apache.http.HttpHost);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setLocalAddress(java.net.InetAddress);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setStaleConnectionCheckEnabled(boolean);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setCookieSpec(java.lang.String);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setRedirectsEnabled(boolean);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setRelativeRedirectsAllowed(boolean);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setCircularRedirectsAllowed(boolean);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setMaxRedirects(int);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setAuthenticationEnabled(boolean);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setTargetPreferredAuthSchemes(java.util.Collection<java.lang.String>);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setProxyPreferredAuthSchemes(java.util.Collection<java.lang.String>);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setConnectionRequestTimeout(int);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setConnectTimeout(int);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setSocketTimeout(int);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setDecompressionEnabled(boolean);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setContentCompressionEnabled(boolean);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig$Builder setNormalizeUri(boolean);
  public com.feilong.lib.org.apache.http.client.config.RequestConfig build();
}
```
