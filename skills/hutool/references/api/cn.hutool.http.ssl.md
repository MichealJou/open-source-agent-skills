# cn.hutool.http.ssl

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.http.ssl.AndroidSupportSSLFactory`

```java
public class cn.hutool.http.ssl.AndroidSupportSSLFactory extends cn.hutool.http.ssl.CustomProtocolsSSLFactory {
  public cn.hutool.http.ssl.AndroidSupportSSLFactory() throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.http.ssl.CustomProtocolsSSLFactory`

```java
public class cn.hutool.http.ssl.CustomProtocolsSSLFactory extends javax.net.ssl.SSLSocketFactory {
  public cn.hutool.http.ssl.CustomProtocolsSSLFactory(java.lang.String...) throws cn.hutool.core.io.IORuntimeException;
  public java.lang.String[] getDefaultCipherSuites();
  public java.lang.String[] getSupportedCipherSuites();
  public java.net.Socket createSocket() throws java.io.IOException;
  public javax.net.ssl.SSLSocket createSocket(java.net.Socket, java.lang.String, int, boolean) throws java.io.IOException;
  public java.net.Socket createSocket(java.lang.String, int) throws java.io.IOException;
  public java.net.Socket createSocket(java.lang.String, int, java.net.InetAddress, int) throws java.io.IOException;
  public java.net.Socket createSocket(java.net.InetAddress, int) throws java.io.IOException;
  public java.net.Socket createSocket(java.net.InetAddress, int, java.net.InetAddress, int) throws java.io.IOException;
  public java.net.Socket createSocket(java.net.Socket, java.lang.String, int, boolean) throws java.io.IOException;
}
```

## `cn.hutool.http.ssl.DefaultSSLFactory`

```java
public class cn.hutool.http.ssl.DefaultSSLFactory extends cn.hutool.http.ssl.CustomProtocolsSSLFactory {
  public cn.hutool.http.ssl.DefaultSSLFactory();
}
```

## `cn.hutool.http.ssl.DefaultSSLInfo`

```java
public class cn.hutool.http.ssl.DefaultSSLInfo {
  public cn.hutool.http.ssl.DefaultSSLInfo();
}
```

## `cn.hutool.http.ssl.SSLSocketFactoryBuilder`

```java
public class cn.hutool.http.ssl.SSLSocketFactoryBuilder implements cn.hutool.core.net.SSLProtocols {
  public cn.hutool.http.ssl.SSLSocketFactoryBuilder();
  public static cn.hutool.http.ssl.SSLSocketFactoryBuilder create();
  public cn.hutool.http.ssl.SSLSocketFactoryBuilder setProtocol(java.lang.String);
  public cn.hutool.http.ssl.SSLSocketFactoryBuilder setTrustManagers(javax.net.ssl.TrustManager...);
  public cn.hutool.http.ssl.SSLSocketFactoryBuilder setKeyManagers(javax.net.ssl.KeyManager...);
  public cn.hutool.http.ssl.SSLSocketFactoryBuilder setSecureRandom(java.security.SecureRandom);
  public javax.net.ssl.SSLSocketFactory build() throws java.security.NoSuchAlgorithmException, java.security.KeyManagementException;
}
```

## `cn.hutool.http.ssl.TrustAnyHostnameVerifier`

```java
public class cn.hutool.http.ssl.TrustAnyHostnameVerifier implements javax.net.ssl.HostnameVerifier {
  public cn.hutool.http.ssl.TrustAnyHostnameVerifier();
  public boolean verify(java.lang.String, javax.net.ssl.SSLSession);
}
```
