# com.feilong.lib.org.apache.http.ssl

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.ssl.PrivateKeyDetails`

```java
public final class com.feilong.lib.org.apache.http.ssl.PrivateKeyDetails {
  public com.feilong.lib.org.apache.http.ssl.PrivateKeyDetails(java.lang.String, java.security.cert.X509Certificate[]);
  public java.lang.String getType();
  public java.security.cert.X509Certificate[] getCertChain();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.ssl.PrivateKeyStrategy`

```java
public interface com.feilong.lib.org.apache.http.ssl.PrivateKeyStrategy {
  public abstract java.lang.String chooseAlias(java.util.Map<java.lang.String, com.feilong.lib.org.apache.http.ssl.PrivateKeyDetails>, java.net.Socket);
}
```

## `com.feilong.lib.org.apache.http.ssl.SSLContextBuilder`

```java
public class com.feilong.lib.org.apache.http.ssl.SSLContextBuilder {
  public static com.feilong.lib.org.apache.http.ssl.SSLContextBuilder create();
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder();
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder useProtocol(java.lang.String);
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder setProtocol(java.lang.String);
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder setSecureRandom(java.security.SecureRandom);
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder setProvider(java.security.Provider);
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder setProvider(java.lang.String);
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder setKeyStoreType(java.lang.String);
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder setKeyManagerFactoryAlgorithm(java.lang.String);
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder setTrustManagerFactoryAlgorithm(java.lang.String);
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder loadTrustMaterial(java.security.KeyStore, com.feilong.lib.org.apache.http.ssl.TrustStrategy) throws java.security.NoSuchAlgorithmException, java.security.KeyStoreException;
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder loadTrustMaterial(com.feilong.lib.org.apache.http.ssl.TrustStrategy) throws java.security.NoSuchAlgorithmException, java.security.KeyStoreException;
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder loadTrustMaterial(java.io.File, char[], com.feilong.lib.org.apache.http.ssl.TrustStrategy) throws java.security.NoSuchAlgorithmException, java.security.KeyStoreException, java.security.cert.CertificateException, java.io.IOException;
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder loadTrustMaterial(java.io.File, char[]) throws java.security.NoSuchAlgorithmException, java.security.KeyStoreException, java.security.cert.CertificateException, java.io.IOException;
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder loadTrustMaterial(java.io.File) throws java.security.NoSuchAlgorithmException, java.security.KeyStoreException, java.security.cert.CertificateException, java.io.IOException;
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder loadTrustMaterial(java.net.URL, char[], com.feilong.lib.org.apache.http.ssl.TrustStrategy) throws java.security.NoSuchAlgorithmException, java.security.KeyStoreException, java.security.cert.CertificateException, java.io.IOException;
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder loadTrustMaterial(java.net.URL, char[]) throws java.security.NoSuchAlgorithmException, java.security.KeyStoreException, java.security.cert.CertificateException, java.io.IOException;
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder loadKeyMaterial(java.security.KeyStore, char[], com.feilong.lib.org.apache.http.ssl.PrivateKeyStrategy) throws java.security.NoSuchAlgorithmException, java.security.KeyStoreException, java.security.UnrecoverableKeyException;
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder loadKeyMaterial(java.security.KeyStore, char[]) throws java.security.NoSuchAlgorithmException, java.security.KeyStoreException, java.security.UnrecoverableKeyException;
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder loadKeyMaterial(java.io.File, char[], char[], com.feilong.lib.org.apache.http.ssl.PrivateKeyStrategy) throws java.security.NoSuchAlgorithmException, java.security.KeyStoreException, java.security.UnrecoverableKeyException, java.security.cert.CertificateException, java.io.IOException;
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder loadKeyMaterial(java.io.File, char[], char[]) throws java.security.NoSuchAlgorithmException, java.security.KeyStoreException, java.security.UnrecoverableKeyException, java.security.cert.CertificateException, java.io.IOException;
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder loadKeyMaterial(java.net.URL, char[], char[], com.feilong.lib.org.apache.http.ssl.PrivateKeyStrategy) throws java.security.NoSuchAlgorithmException, java.security.KeyStoreException, java.security.UnrecoverableKeyException, java.security.cert.CertificateException, java.io.IOException;
  public com.feilong.lib.org.apache.http.ssl.SSLContextBuilder loadKeyMaterial(java.net.URL, char[], char[]) throws java.security.NoSuchAlgorithmException, java.security.KeyStoreException, java.security.UnrecoverableKeyException, java.security.cert.CertificateException, java.io.IOException;
  public javax.net.ssl.SSLContext build() throws java.security.NoSuchAlgorithmException, java.security.KeyManagementException;
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.ssl.SSLContexts`

```java
public class com.feilong.lib.org.apache.http.ssl.SSLContexts {
  public com.feilong.lib.org.apache.http.ssl.SSLContexts();
  public static javax.net.ssl.SSLContext createDefault() throws com.feilong.lib.org.apache.http.ssl.SSLInitializationException;
  public static javax.net.ssl.SSLContext createSystemDefault() throws com.feilong.lib.org.apache.http.ssl.SSLInitializationException;
  public static com.feilong.lib.org.apache.http.ssl.SSLContextBuilder custom();
}
```

## `com.feilong.lib.org.apache.http.ssl.SSLInitializationException`

```java
public class com.feilong.lib.org.apache.http.ssl.SSLInitializationException extends java.lang.IllegalStateException {
  public com.feilong.lib.org.apache.http.ssl.SSLInitializationException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.ssl.TrustStrategy`

```java
public interface com.feilong.lib.org.apache.http.ssl.TrustStrategy {
  public abstract boolean isTrusted(java.security.cert.X509Certificate[], java.lang.String) throws java.security.cert.CertificateException;
}
```
