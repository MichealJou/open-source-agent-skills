# com.feilong.lib.org.apache.http.impl.auth

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.impl.auth.AuthSchemeBase`

```java
public abstract class com.feilong.lib.org.apache.http.impl.auth.AuthSchemeBase implements com.feilong.lib.org.apache.http.auth.ContextAwareAuthScheme {
  public com.feilong.lib.org.apache.http.impl.auth.AuthSchemeBase();
  public void processChallenge(com.feilong.lib.org.apache.http.Header) throws com.feilong.lib.org.apache.http.auth.MalformedChallengeException;
  public com.feilong.lib.org.apache.http.Header authenticate(com.feilong.lib.org.apache.http.auth.Credentials, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.auth.AuthenticationException;
  public boolean isProxy();
  public com.feilong.lib.org.apache.http.auth.ChallengeState getChallengeState();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.auth.BasicScheme`

```java
public class com.feilong.lib.org.apache.http.impl.auth.BasicScheme extends com.feilong.lib.org.apache.http.impl.auth.RFC2617Scheme {
  public com.feilong.lib.org.apache.http.impl.auth.BasicScheme(java.nio.charset.Charset);
  public com.feilong.lib.org.apache.http.impl.auth.BasicScheme();
  public java.lang.String getSchemeName();
  public void processChallenge(com.feilong.lib.org.apache.http.Header) throws com.feilong.lib.org.apache.http.auth.MalformedChallengeException;
  public boolean isComplete();
  public boolean isConnectionBased();
  public com.feilong.lib.org.apache.http.Header authenticate(com.feilong.lib.org.apache.http.auth.Credentials, com.feilong.lib.org.apache.http.HttpRequest) throws com.feilong.lib.org.apache.http.auth.AuthenticationException;
  public com.feilong.lib.org.apache.http.Header authenticate(com.feilong.lib.org.apache.http.auth.Credentials, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.auth.AuthenticationException;
  public static com.feilong.lib.org.apache.http.Header authenticate(com.feilong.lib.org.apache.http.auth.Credentials, java.lang.String, boolean);
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.auth.BasicSchemeFactory`

```java
public class com.feilong.lib.org.apache.http.impl.auth.BasicSchemeFactory implements com.feilong.lib.org.apache.http.auth.AuthSchemeProvider {
  public com.feilong.lib.org.apache.http.impl.auth.BasicSchemeFactory(java.nio.charset.Charset);
  public com.feilong.lib.org.apache.http.impl.auth.BasicSchemeFactory();
  public com.feilong.lib.org.apache.http.auth.AuthScheme create(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.auth.DigestScheme`

```java
public class com.feilong.lib.org.apache.http.impl.auth.DigestScheme extends com.feilong.lib.org.apache.http.impl.auth.RFC2617Scheme {
  public com.feilong.lib.org.apache.http.impl.auth.DigestScheme(java.nio.charset.Charset);
  public com.feilong.lib.org.apache.http.impl.auth.DigestScheme();
  public void processChallenge(com.feilong.lib.org.apache.http.Header) throws com.feilong.lib.org.apache.http.auth.MalformedChallengeException;
  public boolean isComplete();
  public java.lang.String getSchemeName();
  public boolean isConnectionBased();
  public void overrideParamter(java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.Header authenticate(com.feilong.lib.org.apache.http.auth.Credentials, com.feilong.lib.org.apache.http.HttpRequest) throws com.feilong.lib.org.apache.http.auth.AuthenticationException;
  public com.feilong.lib.org.apache.http.Header authenticate(com.feilong.lib.org.apache.http.auth.Credentials, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.auth.AuthenticationException;
  public static java.lang.String createCnonce();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.impl.auth.DigestSchemeFactory`

```java
public class com.feilong.lib.org.apache.http.impl.auth.DigestSchemeFactory implements com.feilong.lib.org.apache.http.auth.AuthSchemeProvider {
  public com.feilong.lib.org.apache.http.impl.auth.DigestSchemeFactory(java.nio.charset.Charset);
  public com.feilong.lib.org.apache.http.impl.auth.DigestSchemeFactory();
  public com.feilong.lib.org.apache.http.auth.AuthScheme create(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.auth.GGSSchemeBase`

```java
public abstract class com.feilong.lib.org.apache.http.impl.auth.GGSSchemeBase extends com.feilong.lib.org.apache.http.impl.auth.AuthSchemeBase {
  public boolean isComplete();
  public com.feilong.lib.org.apache.http.Header authenticate(com.feilong.lib.org.apache.http.auth.Credentials, com.feilong.lib.org.apache.http.HttpRequest) throws com.feilong.lib.org.apache.http.auth.AuthenticationException;
  public com.feilong.lib.org.apache.http.Header authenticate(com.feilong.lib.org.apache.http.auth.Credentials, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.auth.AuthenticationException;
}
```

## `com.feilong.lib.org.apache.http.impl.auth.HttpAuthenticator`

```java
public class com.feilong.lib.org.apache.http.impl.auth.HttpAuthenticator {
  public com.feilong.lib.org.apache.http.impl.auth.HttpAuthenticator();
  public boolean isAuthenticationRequested(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.client.AuthenticationStrategy, com.feilong.lib.org.apache.http.auth.AuthState, com.feilong.lib.org.apache.http.protocol.HttpContext);
  public boolean handleAuthChallenge(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpResponse, com.feilong.lib.org.apache.http.client.AuthenticationStrategy, com.feilong.lib.org.apache.http.auth.AuthState, com.feilong.lib.org.apache.http.protocol.HttpContext);
  public void generateAuthResponse(com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.auth.AuthState, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException, java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.auth.KerberosScheme`

```java
public class com.feilong.lib.org.apache.http.impl.auth.KerberosScheme extends com.feilong.lib.org.apache.http.impl.auth.GGSSchemeBase {
  public com.feilong.lib.org.apache.http.impl.auth.KerberosScheme(boolean, boolean);
  public com.feilong.lib.org.apache.http.impl.auth.KerberosScheme(boolean);
  public com.feilong.lib.org.apache.http.impl.auth.KerberosScheme();
  public java.lang.String getSchemeName();
  public com.feilong.lib.org.apache.http.Header authenticate(com.feilong.lib.org.apache.http.auth.Credentials, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.auth.AuthenticationException;
  public java.lang.String getParameter(java.lang.String);
  public java.lang.String getRealm();
  public boolean isConnectionBased();
}
```

## `com.feilong.lib.org.apache.http.impl.auth.KerberosSchemeFactory`

```java
public class com.feilong.lib.org.apache.http.impl.auth.KerberosSchemeFactory implements com.feilong.lib.org.apache.http.auth.AuthSchemeProvider {
  public com.feilong.lib.org.apache.http.impl.auth.KerberosSchemeFactory(boolean, boolean);
  public com.feilong.lib.org.apache.http.impl.auth.KerberosSchemeFactory(boolean);
  public com.feilong.lib.org.apache.http.impl.auth.KerberosSchemeFactory();
  public boolean isStripPort();
  public boolean isUseCanonicalHostname();
  public com.feilong.lib.org.apache.http.auth.AuthScheme create(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.auth.NTLMEngine`

```java
public interface com.feilong.lib.org.apache.http.impl.auth.NTLMEngine {
  public abstract java.lang.String generateType1Msg(java.lang.String, java.lang.String) throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public abstract java.lang.String generateType3Msg(java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String) throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
}
```

## `com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException`

```java
public class com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException extends com.feilong.lib.org.apache.http.auth.AuthenticationException {
  public com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException();
  public com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException(java.lang.String);
  public com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.impl.auth.NTLMEngineImpl$CipherGen`

```java
public class com.feilong.lib.org.apache.http.impl.auth.NTLMEngineImpl$CipherGen {
  public com.feilong.lib.org.apache.http.impl.auth.NTLMEngineImpl$CipherGen(java.lang.String, java.lang.String, java.lang.String, byte[], java.lang.String, byte[], byte[], byte[], byte[], byte[]);
  public com.feilong.lib.org.apache.http.impl.auth.NTLMEngineImpl$CipherGen(java.util.Random, long, java.lang.String, java.lang.String, java.lang.String, byte[], java.lang.String, byte[], byte[], byte[], byte[], byte[]);
  public com.feilong.lib.org.apache.http.impl.auth.NTLMEngineImpl$CipherGen(java.lang.String, java.lang.String, java.lang.String, byte[], java.lang.String, byte[]);
  public com.feilong.lib.org.apache.http.impl.auth.NTLMEngineImpl$CipherGen(java.util.Random, long, java.lang.String, java.lang.String, java.lang.String, byte[], java.lang.String, byte[]);
  public byte[] getClientChallenge() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getClientChallenge2() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getSecondaryKey() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getLMHash() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getLMResponse() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getNTLMHash() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getNTLMResponse() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getLMv2Hash() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getNTLMv2Hash() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getTimestamp();
  public byte[] getNTLMv2Blob() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getNTLMv2Response() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getLMv2Response() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getNTLM2SessionResponse() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getLM2SessionResponse() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getLMUserSessionKey() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getNTLMUserSessionKey() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getNTLMv2UserSessionKey() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getNTLM2SessionResponseUserSessionKey() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
  public byte[] getLanManagerSessionKey() throws com.feilong.lib.org.apache.http.impl.auth.NTLMEngineException;
}
```

## `com.feilong.lib.org.apache.http.impl.auth.NTLMScheme`

```java
public class com.feilong.lib.org.apache.http.impl.auth.NTLMScheme extends com.feilong.lib.org.apache.http.impl.auth.AuthSchemeBase {
  public com.feilong.lib.org.apache.http.impl.auth.NTLMScheme(com.feilong.lib.org.apache.http.impl.auth.NTLMEngine);
  public com.feilong.lib.org.apache.http.impl.auth.NTLMScheme();
  public java.lang.String getSchemeName();
  public java.lang.String getParameter(java.lang.String);
  public java.lang.String getRealm();
  public boolean isConnectionBased();
  public com.feilong.lib.org.apache.http.Header authenticate(com.feilong.lib.org.apache.http.auth.Credentials, com.feilong.lib.org.apache.http.HttpRequest) throws com.feilong.lib.org.apache.http.auth.AuthenticationException;
  public boolean isComplete();
}
```

## `com.feilong.lib.org.apache.http.impl.auth.NTLMSchemeFactory`

```java
public class com.feilong.lib.org.apache.http.impl.auth.NTLMSchemeFactory implements com.feilong.lib.org.apache.http.auth.AuthSchemeProvider {
  public com.feilong.lib.org.apache.http.impl.auth.NTLMSchemeFactory();
  public com.feilong.lib.org.apache.http.auth.AuthScheme create(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.auth.RFC2617Scheme`

```java
public abstract class com.feilong.lib.org.apache.http.impl.auth.RFC2617Scheme extends com.feilong.lib.org.apache.http.impl.auth.AuthSchemeBase implements java.io.Serializable {
  public com.feilong.lib.org.apache.http.impl.auth.RFC2617Scheme(java.nio.charset.Charset);
  public com.feilong.lib.org.apache.http.impl.auth.RFC2617Scheme();
  public java.nio.charset.Charset getCredentialsCharset();
  public java.lang.String getParameter(java.lang.String);
  public java.lang.String getRealm();
}
```

## `com.feilong.lib.org.apache.http.impl.auth.SPNegoScheme`

```java
public class com.feilong.lib.org.apache.http.impl.auth.SPNegoScheme extends com.feilong.lib.org.apache.http.impl.auth.GGSSchemeBase {
  public com.feilong.lib.org.apache.http.impl.auth.SPNegoScheme(boolean, boolean);
  public com.feilong.lib.org.apache.http.impl.auth.SPNegoScheme(boolean);
  public com.feilong.lib.org.apache.http.impl.auth.SPNegoScheme();
  public java.lang.String getSchemeName();
  public com.feilong.lib.org.apache.http.Header authenticate(com.feilong.lib.org.apache.http.auth.Credentials, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.auth.AuthenticationException;
  public java.lang.String getParameter(java.lang.String);
  public java.lang.String getRealm();
  public boolean isConnectionBased();
}
```

## `com.feilong.lib.org.apache.http.impl.auth.SPNegoSchemeFactory`

```java
public class com.feilong.lib.org.apache.http.impl.auth.SPNegoSchemeFactory implements com.feilong.lib.org.apache.http.auth.AuthSchemeProvider {
  public com.feilong.lib.org.apache.http.impl.auth.SPNegoSchemeFactory(boolean, boolean);
  public com.feilong.lib.org.apache.http.impl.auth.SPNegoSchemeFactory(boolean);
  public com.feilong.lib.org.apache.http.impl.auth.SPNegoSchemeFactory();
  public boolean isStripPort();
  public boolean isUseCanonicalHostname();
  public com.feilong.lib.org.apache.http.auth.AuthScheme create(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.impl.auth.UnsupportedDigestAlgorithmException`

```java
public class com.feilong.lib.org.apache.http.impl.auth.UnsupportedDigestAlgorithmException extends java.lang.RuntimeException {
  public com.feilong.lib.org.apache.http.impl.auth.UnsupportedDigestAlgorithmException();
  public com.feilong.lib.org.apache.http.impl.auth.UnsupportedDigestAlgorithmException(java.lang.String);
  public com.feilong.lib.org.apache.http.impl.auth.UnsupportedDigestAlgorithmException(java.lang.String, java.lang.Throwable);
}
```
