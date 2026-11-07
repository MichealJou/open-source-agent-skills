# cn.hutool.jwt

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.jwt.Claims`

```java
public class cn.hutool.jwt.Claims implements java.io.Serializable {
  public cn.hutool.jwt.Claims();
  public java.lang.Object getClaim(java.lang.String);
  public cn.hutool.json.JSONObject getClaimsJson();
  public void parse(java.lang.String, java.nio.charset.Charset);
  public java.lang.String toString();
}
```

## `cn.hutool.jwt.JWT`

```java
public class cn.hutool.jwt.JWT implements cn.hutool.jwt.RegisteredPayload<cn.hutool.jwt.JWT> {
  public static cn.hutool.jwt.JWT create();
  public static cn.hutool.jwt.JWT of(java.lang.String);
  public cn.hutool.jwt.JWT();
  public cn.hutool.jwt.JWT(java.lang.String);
  public cn.hutool.jwt.JWT parse(java.lang.String);
  public cn.hutool.jwt.JWT setCharset(java.nio.charset.Charset);
  public cn.hutool.jwt.JWT setKey(byte[]);
  public cn.hutool.jwt.JWT setSigner(java.lang.String, byte[]);
  public cn.hutool.jwt.JWT setSigner(java.lang.String, java.security.Key);
  public cn.hutool.jwt.JWT setSigner(java.lang.String, java.security.KeyPair);
  public cn.hutool.jwt.JWT setSigner(cn.hutool.jwt.signers.JWTSigner);
  public cn.hutool.jwt.signers.JWTSigner getSigner();
  public cn.hutool.json.JSONObject getHeaders();
  public cn.hutool.jwt.JWTHeader getHeader();
  public java.lang.Object getHeader(java.lang.String);
  public java.lang.String getAlgorithm();
  public cn.hutool.jwt.JWT setHeader(java.lang.String, java.lang.Object);
  public cn.hutool.jwt.JWT addHeaders(java.util.Map<java.lang.String, ?>);
  public cn.hutool.json.JSONObject getPayloads();
  public cn.hutool.jwt.JWTPayload getPayload();
  public java.lang.Object getPayload(java.lang.String);
  public cn.hutool.jwt.JWT setPayload(java.lang.String, java.lang.Object);
  public cn.hutool.jwt.JWT addPayloads(java.util.Map<java.lang.String, ?>);
  public java.lang.String sign();
  public java.lang.String sign(boolean);
  public java.lang.String sign(cn.hutool.jwt.signers.JWTSigner);
  public java.lang.String sign(cn.hutool.jwt.signers.JWTSigner, boolean);
  public boolean verify();
  public boolean validate(long);
  public boolean verify(cn.hutool.jwt.signers.JWTSigner);
  public cn.hutool.jwt.RegisteredPayload setPayload(java.lang.String, java.lang.Object);
}
```

## `cn.hutool.jwt.JWTException`

```java
public class cn.hutool.jwt.JWTException extends java.lang.RuntimeException {
  public cn.hutool.jwt.JWTException(java.lang.Throwable);
  public cn.hutool.jwt.JWTException(java.lang.String);
  public cn.hutool.jwt.JWTException(java.lang.String, java.lang.Object...);
  public cn.hutool.jwt.JWTException(java.lang.String, java.lang.Throwable);
  public cn.hutool.jwt.JWTException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.jwt.JWTException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.jwt.JWTHeader`

```java
public class cn.hutool.jwt.JWTHeader extends cn.hutool.jwt.Claims {
  public cn.hutool.jwt.JWTHeader();
  public cn.hutool.jwt.JWTHeader setAlgorithm(java.lang.String);
  public cn.hutool.jwt.JWTHeader setType(java.lang.String);
  public cn.hutool.jwt.JWTHeader setContentType(java.lang.String);
  public cn.hutool.jwt.JWTHeader setKeyId(java.lang.String);
  public cn.hutool.jwt.JWTHeader addHeaders(java.util.Map<java.lang.String, ?>);
}
```

## `cn.hutool.jwt.JWTPayload`

```java
public class cn.hutool.jwt.JWTPayload extends cn.hutool.jwt.Claims implements cn.hutool.jwt.RegisteredPayload<cn.hutool.jwt.JWTPayload> {
  public cn.hutool.jwt.JWTPayload();
  public cn.hutool.jwt.JWTPayload addPayloads(java.util.Map<java.lang.String, ?>);
  public cn.hutool.jwt.JWTPayload setPayload(java.lang.String, java.lang.Object);
  public cn.hutool.jwt.RegisteredPayload setPayload(java.lang.String, java.lang.Object);
}
```

## `cn.hutool.jwt.JWTUtil`

```java
public class cn.hutool.jwt.JWTUtil {
  public cn.hutool.jwt.JWTUtil();
  public static java.lang.String createToken(java.util.Map<java.lang.String, java.lang.Object>, byte[]);
  public static java.lang.String createToken(java.util.Map<java.lang.String, java.lang.Object>, java.util.Map<java.lang.String, java.lang.Object>, byte[]);
  public static java.lang.String createToken(java.util.Map<java.lang.String, java.lang.Object>, cn.hutool.jwt.signers.JWTSigner);
  public static java.lang.String createToken(java.util.Map<java.lang.String, java.lang.Object>, java.util.Map<java.lang.String, java.lang.Object>, cn.hutool.jwt.signers.JWTSigner);
  public static cn.hutool.jwt.JWT parseToken(java.lang.String);
  public static boolean verify(java.lang.String, byte[]);
  public static boolean verify(java.lang.String, cn.hutool.jwt.signers.JWTSigner);
}
```

## `cn.hutool.jwt.JWTValidator`

```java
public class cn.hutool.jwt.JWTValidator {
  public static cn.hutool.jwt.JWTValidator of(java.lang.String);
  public static cn.hutool.jwt.JWTValidator of(cn.hutool.jwt.JWT);
  public cn.hutool.jwt.JWTValidator(cn.hutool.jwt.JWT);
  public cn.hutool.jwt.JWTValidator validateAlgorithm() throws cn.hutool.core.exceptions.ValidateException;
  public cn.hutool.jwt.JWTValidator validateAlgorithm(cn.hutool.jwt.signers.JWTSigner) throws cn.hutool.core.exceptions.ValidateException;
  public cn.hutool.jwt.JWTValidator validateDate() throws cn.hutool.core.exceptions.ValidateException;
  public cn.hutool.jwt.JWTValidator validateDate(java.util.Date) throws cn.hutool.core.exceptions.ValidateException;
  public cn.hutool.jwt.JWTValidator validateDate(java.util.Date, long) throws cn.hutool.core.exceptions.ValidateException;
}
```

## `cn.hutool.jwt.RegisteredPayload`

```java
public interface cn.hutool.jwt.RegisteredPayload<T extends cn.hutool.jwt.RegisteredPayload<T>> {
  public default T setIssuer(java.lang.String);
  public default T setSubject(java.lang.String);
  public default T setAudience(java.lang.String...);
  public default T setExpiresAt(java.util.Date);
  public default T setNotBefore(java.util.Date);
  public default T setIssuedAt(java.util.Date);
  public default T setJWTId(java.lang.String);
  public abstract T setPayload(java.lang.String, java.lang.Object);
}
```
