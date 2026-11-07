# com.feilong.lib.net.util

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.net.util.Base64`

```java
public class com.feilong.lib.net.util.Base64 {
  public com.feilong.lib.net.util.Base64();
  public com.feilong.lib.net.util.Base64(boolean);
  public com.feilong.lib.net.util.Base64(int);
  public com.feilong.lib.net.util.Base64(int, byte[]);
  public com.feilong.lib.net.util.Base64(int, byte[], boolean);
  public boolean isUrlSafe();
  public static boolean isBase64(byte);
  public static boolean isArrayByteBase64(byte[]);
  public static byte[] encodeBase64(byte[]);
  public static java.lang.String encodeBase64String(byte[]);
  public static java.lang.String encodeBase64StringUnChunked(byte[]);
  public static java.lang.String encodeBase64String(byte[], boolean);
  public static byte[] encodeBase64URLSafe(byte[]);
  public static java.lang.String encodeBase64URLSafeString(byte[]);
  public static byte[] encodeBase64Chunked(byte[]);
  public byte[] decode(java.lang.String);
  public byte[] decode(byte[]);
  public static byte[] encodeBase64(byte[], boolean);
  public static byte[] encodeBase64(byte[], boolean, boolean);
  public static byte[] encodeBase64(byte[], boolean, boolean, int);
  public static byte[] decodeBase64(java.lang.String);
  public static byte[] decodeBase64(byte[]);
  public java.lang.String encodeToString(byte[]);
  public byte[] encode(byte[]);
  public static java.math.BigInteger decodeInteger(byte[]);
  public static byte[] encodeInteger(java.math.BigInteger);
}
```

## `com.feilong.lib.net.util.Charsets`

```java
public class com.feilong.lib.net.util.Charsets {
  public com.feilong.lib.net.util.Charsets();
  public static java.nio.charset.Charset toCharset(java.lang.String);
}
```

## `com.feilong.lib.net.util.KeyManagerUtils`

```java
public final class com.feilong.lib.net.util.KeyManagerUtils {
  public static javax.net.ssl.KeyManager createClientKeyManager(java.security.KeyStore, java.lang.String, java.lang.String) throws java.security.GeneralSecurityException;
  public static javax.net.ssl.KeyManager createClientKeyManager(java.lang.String, java.io.File, java.lang.String, java.lang.String, java.lang.String) throws java.io.IOException, java.security.GeneralSecurityException;
  public static javax.net.ssl.KeyManager createClientKeyManager(java.io.File, java.lang.String, java.lang.String) throws java.io.IOException, java.security.GeneralSecurityException;
  public static javax.net.ssl.KeyManager createClientKeyManager(java.io.File, java.lang.String) throws java.io.IOException, java.security.GeneralSecurityException;
}
```

## `com.feilong.lib.net.util.ListenerList`

```java
public class com.feilong.lib.net.util.ListenerList implements java.io.Serializable, java.lang.Iterable<java.util.EventListener> {
  public com.feilong.lib.net.util.ListenerList();
  public void addListener(java.util.EventListener);
  public void removeListener(java.util.EventListener);
  public int getListenerCount();
  public java.util.Iterator<java.util.EventListener> iterator();
}
```

## `com.feilong.lib.net.util.SSLContextUtils`

```java
public class com.feilong.lib.net.util.SSLContextUtils {
  public static javax.net.ssl.SSLContext createSSLContext(java.lang.String, javax.net.ssl.KeyManager, javax.net.ssl.TrustManager) throws java.io.IOException;
  public static javax.net.ssl.SSLContext createSSLContext(java.lang.String, javax.net.ssl.KeyManager[], javax.net.ssl.TrustManager[]) throws java.io.IOException;
}
```

## `com.feilong.lib.net.util.SSLSocketUtils`

```java
public class com.feilong.lib.net.util.SSLSocketUtils {
  public static boolean enableEndpointNameVerification(javax.net.ssl.SSLSocket);
}
```

## `com.feilong.lib.net.util.TrustManagerUtils`

```java
public final class com.feilong.lib.net.util.TrustManagerUtils {
  public com.feilong.lib.net.util.TrustManagerUtils();
  public static javax.net.ssl.X509TrustManager getAcceptAllTrustManager();
  public static javax.net.ssl.X509TrustManager getValidateServerCertificateTrustManager();
  public static javax.net.ssl.X509TrustManager getDefaultTrustManager(java.security.KeyStore) throws java.security.GeneralSecurityException;
}
```
