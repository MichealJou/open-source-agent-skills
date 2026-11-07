# cn.hutool.jwt.signers

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.jwt.signers.AlgorithmUtil`

```java
public class cn.hutool.jwt.signers.AlgorithmUtil {
  public cn.hutool.jwt.signers.AlgorithmUtil();
  public static java.lang.String getAlgorithm(java.lang.String);
  public static java.lang.String getId(java.lang.String);
}
```

## `cn.hutool.jwt.signers.AsymmetricJWTSigner`

```java
public class cn.hutool.jwt.signers.AsymmetricJWTSigner implements cn.hutool.jwt.signers.JWTSigner {
  public cn.hutool.jwt.signers.AsymmetricJWTSigner(java.lang.String, java.security.Key);
  public cn.hutool.jwt.signers.AsymmetricJWTSigner(java.lang.String, java.security.KeyPair);
  public cn.hutool.jwt.signers.AsymmetricJWTSigner setCharset(java.nio.charset.Charset);
  public java.lang.String sign(java.lang.String, java.lang.String);
  public boolean verify(java.lang.String, java.lang.String, java.lang.String);
  public java.lang.String getAlgorithm();
}
```

## `cn.hutool.jwt.signers.EllipticCurveJWTSigner`

```java
public class cn.hutool.jwt.signers.EllipticCurveJWTSigner extends cn.hutool.jwt.signers.AsymmetricJWTSigner {
  public cn.hutool.jwt.signers.EllipticCurveJWTSigner(java.lang.String, java.security.Key);
  public cn.hutool.jwt.signers.EllipticCurveJWTSigner(java.lang.String, java.security.KeyPair);
}
```

## `cn.hutool.jwt.signers.HMacJWTSigner`

```java
public class cn.hutool.jwt.signers.HMacJWTSigner implements cn.hutool.jwt.signers.JWTSigner {
  public cn.hutool.jwt.signers.HMacJWTSigner(java.lang.String, byte[]);
  public cn.hutool.jwt.signers.HMacJWTSigner(java.lang.String, java.security.Key);
  public cn.hutool.jwt.signers.HMacJWTSigner setCharset(java.nio.charset.Charset);
  public java.lang.String sign(java.lang.String, java.lang.String);
  public boolean verify(java.lang.String, java.lang.String, java.lang.String);
  public java.lang.String getAlgorithm();
}
```

## `cn.hutool.jwt.signers.JWTSigner`

```java
public interface cn.hutool.jwt.signers.JWTSigner {
  public abstract java.lang.String sign(java.lang.String, java.lang.String);
  public abstract boolean verify(java.lang.String, java.lang.String, java.lang.String);
  public abstract java.lang.String getAlgorithm();
  public default java.lang.String getAlgorithmId();
}
```

## `cn.hutool.jwt.signers.JWTSignerUtil`

```java
public class cn.hutool.jwt.signers.JWTSignerUtil {
  public cn.hutool.jwt.signers.JWTSignerUtil();
  public static cn.hutool.jwt.signers.JWTSigner none();
  public static cn.hutool.jwt.signers.JWTSigner hs256(byte[]);
  public static cn.hutool.jwt.signers.JWTSigner hs384(byte[]);
  public static cn.hutool.jwt.signers.JWTSigner hs512(byte[]);
  public static cn.hutool.jwt.signers.JWTSigner rs256(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner rs384(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner rs512(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner es256(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner es384(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner es512(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner hmd5(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner hsha1(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner sm4cmac(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner rmd2(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner rmd5(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner rsha1(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner dnone(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner dsha1(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner enone(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner esha1(java.security.Key);
  public static cn.hutool.jwt.signers.JWTSigner createSigner(java.lang.String, byte[]);
  public static cn.hutool.jwt.signers.JWTSigner createSigner(java.lang.String, java.security.KeyPair);
  public static cn.hutool.jwt.signers.JWTSigner createSigner(java.lang.String, java.security.Key);
}
```

## `cn.hutool.jwt.signers.NoneJWTSigner`

```java
public class cn.hutool.jwt.signers.NoneJWTSigner implements cn.hutool.jwt.signers.JWTSigner {
  public cn.hutool.jwt.signers.NoneJWTSigner();
  public static boolean isNone(java.lang.String);
  public java.lang.String sign(java.lang.String, java.lang.String);
  public boolean verify(java.lang.String, java.lang.String, java.lang.String);
  public java.lang.String getAlgorithm();
}
```
