# com.feilong.lib.org.apache.http.conn.ssl

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.conn.ssl.AbstractVerifier`

```java
public abstract class com.feilong.lib.org.apache.http.conn.ssl.AbstractVerifier implements com.feilong.lib.org.apache.http.conn.ssl.X509HostnameVerifier {
  public com.feilong.lib.org.apache.http.conn.ssl.AbstractVerifier();
  public final void verify(java.lang.String, javax.net.ssl.SSLSocket) throws java.io.IOException;
  public final boolean verify(java.lang.String, javax.net.ssl.SSLSession);
  public final void verify(java.lang.String, java.security.cert.X509Certificate) throws javax.net.ssl.SSLException;
  public final void verify(java.lang.String, java.lang.String[], java.lang.String[], boolean) throws javax.net.ssl.SSLException;
  public static boolean acceptableCountryWildcard(java.lang.String);
  public static java.lang.String[] getCNs(java.security.cert.X509Certificate);
  public static java.lang.String[] getDNSSubjectAlts(java.security.cert.X509Certificate);
  public static int countDots(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.conn.ssl.AllowAllHostnameVerifier`

```java
public class com.feilong.lib.org.apache.http.conn.ssl.AllowAllHostnameVerifier extends com.feilong.lib.org.apache.http.conn.ssl.AbstractVerifier {
  public com.feilong.lib.org.apache.http.conn.ssl.AllowAllHostnameVerifier();
  public final void verify(java.lang.String, java.lang.String[], java.lang.String[]);
  public final java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.conn.ssl.BrowserCompatHostnameVerifier`

```java
public class com.feilong.lib.org.apache.http.conn.ssl.BrowserCompatHostnameVerifier extends com.feilong.lib.org.apache.http.conn.ssl.AbstractVerifier {
  public com.feilong.lib.org.apache.http.conn.ssl.BrowserCompatHostnameVerifier();
  public final void verify(java.lang.String, java.lang.String[], java.lang.String[]) throws javax.net.ssl.SSLException;
  public final java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.conn.ssl.DefaultHostnameVerifier`

```java
public final class com.feilong.lib.org.apache.http.conn.ssl.DefaultHostnameVerifier implements javax.net.ssl.HostnameVerifier {
  public com.feilong.lib.org.apache.http.conn.ssl.DefaultHostnameVerifier(com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher);
  public com.feilong.lib.org.apache.http.conn.ssl.DefaultHostnameVerifier();
  public boolean verify(java.lang.String, javax.net.ssl.SSLSession);
  public void verify(java.lang.String, java.security.cert.X509Certificate) throws javax.net.ssl.SSLException;
}
```

## `com.feilong.lib.org.apache.http.conn.ssl.NoopHostnameVerifier`

```java
public class com.feilong.lib.org.apache.http.conn.ssl.NoopHostnameVerifier implements javax.net.ssl.HostnameVerifier {
  public com.feilong.lib.org.apache.http.conn.ssl.NoopHostnameVerifier();
  public boolean verify(java.lang.String, javax.net.ssl.SSLSession);
  public final java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.conn.ssl.SSLConnectionSocketFactory`

```java
public class com.feilong.lib.org.apache.http.conn.ssl.SSLConnectionSocketFactory implements com.feilong.lib.org.apache.http.conn.socket.LayeredConnectionSocketFactory {
  public static javax.net.ssl.HostnameVerifier getDefaultHostnameVerifier();
  public static com.feilong.lib.org.apache.http.conn.ssl.SSLConnectionSocketFactory getSocketFactory() throws com.feilong.lib.org.apache.http.conn.ssl.SSLInitializationException;
  public static com.feilong.lib.org.apache.http.conn.ssl.SSLConnectionSocketFactory getSystemSocketFactory() throws com.feilong.lib.org.apache.http.conn.ssl.SSLInitializationException;
  public com.feilong.lib.org.apache.http.conn.ssl.SSLConnectionSocketFactory(javax.net.ssl.SSLContext);
  public com.feilong.lib.org.apache.http.conn.ssl.SSLConnectionSocketFactory(javax.net.ssl.SSLContext, com.feilong.lib.org.apache.http.conn.ssl.X509HostnameVerifier);
  public com.feilong.lib.org.apache.http.conn.ssl.SSLConnectionSocketFactory(javax.net.ssl.SSLContext, java.lang.String[], java.lang.String[], com.feilong.lib.org.apache.http.conn.ssl.X509HostnameVerifier);
  public com.feilong.lib.org.apache.http.conn.ssl.SSLConnectionSocketFactory(javax.net.ssl.SSLSocketFactory, com.feilong.lib.org.apache.http.conn.ssl.X509HostnameVerifier);
  public com.feilong.lib.org.apache.http.conn.ssl.SSLConnectionSocketFactory(javax.net.ssl.SSLSocketFactory, java.lang.String[], java.lang.String[], com.feilong.lib.org.apache.http.conn.ssl.X509HostnameVerifier);
  public com.feilong.lib.org.apache.http.conn.ssl.SSLConnectionSocketFactory(javax.net.ssl.SSLContext, javax.net.ssl.HostnameVerifier);
  public com.feilong.lib.org.apache.http.conn.ssl.SSLConnectionSocketFactory(javax.net.ssl.SSLContext, java.lang.String[], java.lang.String[], javax.net.ssl.HostnameVerifier);
  public com.feilong.lib.org.apache.http.conn.ssl.SSLConnectionSocketFactory(javax.net.ssl.SSLSocketFactory, javax.net.ssl.HostnameVerifier);
  public com.feilong.lib.org.apache.http.conn.ssl.SSLConnectionSocketFactory(javax.net.ssl.SSLSocketFactory, java.lang.String[], java.lang.String[], javax.net.ssl.HostnameVerifier);
  public java.net.Socket createSocket(com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public java.net.Socket connectSocket(int, java.net.Socket, com.feilong.lib.org.apache.http.HttpHost, java.net.InetSocketAddress, java.net.InetSocketAddress, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public java.net.Socket createLayeredSocket(java.net.Socket, java.lang.String, int, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.conn.ssl.SSLInitializationException`

```java
public class com.feilong.lib.org.apache.http.conn.ssl.SSLInitializationException extends java.lang.IllegalStateException {
  public com.feilong.lib.org.apache.http.conn.ssl.SSLInitializationException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.conn.ssl.StrictHostnameVerifier`

```java
public class com.feilong.lib.org.apache.http.conn.ssl.StrictHostnameVerifier extends com.feilong.lib.org.apache.http.conn.ssl.AbstractVerifier {
  public com.feilong.lib.org.apache.http.conn.ssl.StrictHostnameVerifier();
  public final void verify(java.lang.String, java.lang.String[], java.lang.String[]) throws javax.net.ssl.SSLException;
  public final java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.conn.ssl.TrustAllStrategy`

```java
public class com.feilong.lib.org.apache.http.conn.ssl.TrustAllStrategy implements com.feilong.lib.org.apache.http.conn.ssl.TrustStrategy {
  public com.feilong.lib.org.apache.http.conn.ssl.TrustAllStrategy();
  public boolean isTrusted(java.security.cert.X509Certificate[], java.lang.String) throws java.security.cert.CertificateException;
}
```

## `com.feilong.lib.org.apache.http.conn.ssl.TrustSelfSignedStrategy`

```java
public class com.feilong.lib.org.apache.http.conn.ssl.TrustSelfSignedStrategy implements com.feilong.lib.org.apache.http.conn.ssl.TrustStrategy {
  public com.feilong.lib.org.apache.http.conn.ssl.TrustSelfSignedStrategy();
  public boolean isTrusted(java.security.cert.X509Certificate[], java.lang.String) throws java.security.cert.CertificateException;
}
```

## `com.feilong.lib.org.apache.http.conn.ssl.X509HostnameVerifier`

```java
public interface com.feilong.lib.org.apache.http.conn.ssl.X509HostnameVerifier extends javax.net.ssl.HostnameVerifier {
  public abstract void verify(java.lang.String, javax.net.ssl.SSLSocket) throws java.io.IOException;
  public abstract void verify(java.lang.String, java.security.cert.X509Certificate) throws javax.net.ssl.SSLException;
  public abstract void verify(java.lang.String, java.lang.String[], java.lang.String[]) throws javax.net.ssl.SSLException;
}
```
