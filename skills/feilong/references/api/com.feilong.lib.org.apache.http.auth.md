# com.feilong.lib.org.apache.http.auth

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.auth.AuthOption`

```java
public final class com.feilong.lib.org.apache.http.auth.AuthOption {
  public com.feilong.lib.org.apache.http.auth.AuthOption(com.feilong.lib.org.apache.http.auth.AuthScheme, com.feilong.lib.org.apache.http.auth.Credentials);
  public com.feilong.lib.org.apache.http.auth.AuthScheme getAuthScheme();
  public com.feilong.lib.org.apache.http.auth.Credentials getCredentials();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.auth.AuthProtocolState`

```java
public final class com.feilong.lib.org.apache.http.auth.AuthProtocolState extends java.lang.Enum<com.feilong.lib.org.apache.http.auth.AuthProtocolState> {
  public static com.feilong.lib.org.apache.http.auth.AuthProtocolState[] values();
  public static com.feilong.lib.org.apache.http.auth.AuthProtocolState valueOf(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.auth.AuthScheme`

```java
public interface com.feilong.lib.org.apache.http.auth.AuthScheme {
  public abstract void processChallenge(com.feilong.lib.org.apache.http.Header) throws com.feilong.lib.org.apache.http.auth.MalformedChallengeException;
  public abstract java.lang.String getSchemeName();
  public abstract java.lang.String getParameter(java.lang.String);
  public abstract java.lang.String getRealm();
  public abstract boolean isConnectionBased();
  public abstract boolean isComplete();
  public abstract com.feilong.lib.org.apache.http.Header authenticate(com.feilong.lib.org.apache.http.auth.Credentials, com.feilong.lib.org.apache.http.HttpRequest) throws com.feilong.lib.org.apache.http.auth.AuthenticationException;
}
```

## `com.feilong.lib.org.apache.http.auth.AuthSchemeProvider`

```java
public interface com.feilong.lib.org.apache.http.auth.AuthSchemeProvider {
  public abstract com.feilong.lib.org.apache.http.auth.AuthScheme create(com.feilong.lib.org.apache.http.protocol.HttpContext);
}
```

## `com.feilong.lib.org.apache.http.auth.AuthScope`

```java
public class com.feilong.lib.org.apache.http.auth.AuthScope {
  public com.feilong.lib.org.apache.http.auth.AuthScope(java.lang.String, int, java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.auth.AuthScope(com.feilong.lib.org.apache.http.HttpHost, java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.auth.AuthScope(com.feilong.lib.org.apache.http.HttpHost);
  public com.feilong.lib.org.apache.http.auth.AuthScope(java.lang.String, int, java.lang.String);
  public com.feilong.lib.org.apache.http.auth.AuthScope(java.lang.String, int);
  public com.feilong.lib.org.apache.http.auth.AuthScope(com.feilong.lib.org.apache.http.auth.AuthScope);
  public com.feilong.lib.org.apache.http.HttpHost getOrigin();
  public java.lang.String getHost();
  public int getPort();
  public java.lang.String getRealm();
  public java.lang.String getScheme();
  public int match(com.feilong.lib.org.apache.http.auth.AuthScope);
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
  public int hashCode();
}
```

## `com.feilong.lib.org.apache.http.auth.AuthState`

```java
public class com.feilong.lib.org.apache.http.auth.AuthState {
  public com.feilong.lib.org.apache.http.auth.AuthState();
  public void reset();
  public com.feilong.lib.org.apache.http.auth.AuthProtocolState getState();
  public void setState(com.feilong.lib.org.apache.http.auth.AuthProtocolState);
  public com.feilong.lib.org.apache.http.auth.AuthScheme getAuthScheme();
  public com.feilong.lib.org.apache.http.auth.Credentials getCredentials();
  public void update(com.feilong.lib.org.apache.http.auth.AuthScheme, com.feilong.lib.org.apache.http.auth.Credentials);
  public java.util.Queue<com.feilong.lib.org.apache.http.auth.AuthOption> getAuthOptions();
  public boolean hasAuthOptions();
  public boolean isConnectionBased();
  public void update(java.util.Queue<com.feilong.lib.org.apache.http.auth.AuthOption>);
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.auth.AuthenticationException`

```java
public class com.feilong.lib.org.apache.http.auth.AuthenticationException extends com.feilong.lib.org.apache.http.ProtocolException {
  public com.feilong.lib.org.apache.http.auth.AuthenticationException();
  public com.feilong.lib.org.apache.http.auth.AuthenticationException(java.lang.String);
  public com.feilong.lib.org.apache.http.auth.AuthenticationException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.auth.BasicUserPrincipal`

```java
public final class com.feilong.lib.org.apache.http.auth.BasicUserPrincipal implements java.security.Principal,java.io.Serializable {
  public com.feilong.lib.org.apache.http.auth.BasicUserPrincipal(java.lang.String);
  public java.lang.String getName();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.auth.ChallengeState`

```java
public final class com.feilong.lib.org.apache.http.auth.ChallengeState extends java.lang.Enum<com.feilong.lib.org.apache.http.auth.ChallengeState> {
  public static com.feilong.lib.org.apache.http.auth.ChallengeState[] values();
  public static com.feilong.lib.org.apache.http.auth.ChallengeState valueOf(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.auth.ContextAwareAuthScheme`

```java
public interface com.feilong.lib.org.apache.http.auth.ContextAwareAuthScheme extends com.feilong.lib.org.apache.http.auth.AuthScheme {
  public abstract com.feilong.lib.org.apache.http.Header authenticate(com.feilong.lib.org.apache.http.auth.Credentials, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.auth.AuthenticationException;
}
```

## `com.feilong.lib.org.apache.http.auth.Credentials`

```java
public interface com.feilong.lib.org.apache.http.auth.Credentials {
  public abstract java.security.Principal getUserPrincipal();
  public abstract java.lang.String getPassword();
}
```

## `com.feilong.lib.org.apache.http.auth.InvalidCredentialsException`

```java
public class com.feilong.lib.org.apache.http.auth.InvalidCredentialsException extends com.feilong.lib.org.apache.http.auth.AuthenticationException {
  public com.feilong.lib.org.apache.http.auth.InvalidCredentialsException();
  public com.feilong.lib.org.apache.http.auth.InvalidCredentialsException(java.lang.String);
  public com.feilong.lib.org.apache.http.auth.InvalidCredentialsException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.auth.KerberosCredentials`

```java
public class com.feilong.lib.org.apache.http.auth.KerberosCredentials implements com.feilong.lib.org.apache.http.auth.Credentials,java.io.Serializable {
  public com.feilong.lib.org.apache.http.auth.KerberosCredentials(org.ietf.jgss.GSSCredential);
  public org.ietf.jgss.GSSCredential getGSSCredential();
  public java.security.Principal getUserPrincipal();
  public java.lang.String getPassword();
}
```

## `com.feilong.lib.org.apache.http.auth.MalformedChallengeException`

```java
public class com.feilong.lib.org.apache.http.auth.MalformedChallengeException extends com.feilong.lib.org.apache.http.ProtocolException {
  public com.feilong.lib.org.apache.http.auth.MalformedChallengeException();
  public com.feilong.lib.org.apache.http.auth.MalformedChallengeException(java.lang.String);
  public com.feilong.lib.org.apache.http.auth.MalformedChallengeException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.org.apache.http.auth.NTCredentials`

```java
public class com.feilong.lib.org.apache.http.auth.NTCredentials implements com.feilong.lib.org.apache.http.auth.Credentials,java.io.Serializable {
  public com.feilong.lib.org.apache.http.auth.NTCredentials(java.lang.String, java.lang.String, java.lang.String, java.lang.String);
  public java.security.Principal getUserPrincipal();
  public java.lang.String getUserName();
  public java.lang.String getPassword();
  public java.lang.String getDomain();
  public java.lang.String getWorkstation();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.auth.NTUserPrincipal`

```java
public class com.feilong.lib.org.apache.http.auth.NTUserPrincipal implements java.security.Principal,java.io.Serializable {
  public com.feilong.lib.org.apache.http.auth.NTUserPrincipal(java.lang.String, java.lang.String);
  public java.lang.String getName();
  public java.lang.String getDomain();
  public java.lang.String getUsername();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.auth.UsernamePasswordCredentials`

```java
public class com.feilong.lib.org.apache.http.auth.UsernamePasswordCredentials implements com.feilong.lib.org.apache.http.auth.Credentials,java.io.Serializable {
  public com.feilong.lib.org.apache.http.auth.UsernamePasswordCredentials(java.lang.String);
  public com.feilong.lib.org.apache.http.auth.UsernamePasswordCredentials(java.lang.String, java.lang.String);
  public java.security.Principal getUserPrincipal();
  public java.lang.String getUserName();
  public java.lang.String getPassword();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
}
```
