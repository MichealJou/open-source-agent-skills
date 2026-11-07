# cn.hutool.crypto.digest

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.crypto.digest.Argon2`

```java
public class cn.hutool.crypto.digest.Argon2 {
  public cn.hutool.crypto.digest.Argon2();
  public cn.hutool.crypto.digest.Argon2(int);
  public cn.hutool.crypto.digest.Argon2(org.bouncycastle.crypto.params.Argon2Parameters$Builder);
  public cn.hutool.crypto.digest.Argon2 setHashLength(int);
  public cn.hutool.crypto.digest.Argon2 setVersion(int);
  public cn.hutool.crypto.digest.Argon2 setSalt(byte[]);
  public cn.hutool.crypto.digest.Argon2 setSecret(byte[]);
  public cn.hutool.crypto.digest.Argon2 setAdditional(byte[]);
  public cn.hutool.crypto.digest.Argon2 setIterations(int);
  public cn.hutool.crypto.digest.Argon2 setMemoryAsKB(int);
  public cn.hutool.crypto.digest.Argon2 setParallelism(int);
  public byte[] digest(char[]);
}
```

## `cn.hutool.crypto.digest.BCrypt`

```java
public class cn.hutool.crypto.digest.BCrypt {
  public cn.hutool.crypto.digest.BCrypt();
  public byte[] crypt(byte[], byte[], int, int[]);
  public static java.lang.String hashpw(java.lang.String);
  public static java.lang.String hashpw(java.lang.String, java.lang.String);
  public static java.lang.String gensalt(int, java.security.SecureRandom);
  public static java.lang.String gensalt(int);
  public static java.lang.String gensalt();
  public static boolean checkpw(java.lang.String, java.lang.String);
}
```

## `cn.hutool.crypto.digest.DigestAlgorithm`

```java
public final class cn.hutool.crypto.digest.DigestAlgorithm extends java.lang.Enum<cn.hutool.crypto.digest.DigestAlgorithm> {
  public static cn.hutool.crypto.digest.DigestAlgorithm[] values();
  public static cn.hutool.crypto.digest.DigestAlgorithm valueOf(java.lang.String);
  public java.lang.String getValue();
}
```

## `cn.hutool.crypto.digest.DigestUtil`

```java
public class cn.hutool.crypto.digest.DigestUtil {
  public cn.hutool.crypto.digest.DigestUtil();
  public static byte[] md5(byte[]);
  public static byte[] md5(java.lang.String, java.lang.String);
  public static byte[] md5(java.lang.String);
  public static byte[] md5(java.io.InputStream);
  public static byte[] md5(java.io.File);
  public static java.lang.String md5Hex(byte[]);
  public static java.lang.String md5Hex(java.lang.String, java.lang.String);
  public static java.lang.String md5Hex(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String md5Hex(java.lang.String);
  public static java.lang.String md5Hex(java.io.InputStream);
  public static java.lang.String md5Hex(java.io.File);
  public static java.lang.String md5Hex16(byte[]);
  public static java.lang.String md5Hex16(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String md5Hex16(java.lang.String);
  public static java.lang.String md5Hex16(java.io.InputStream);
  public static java.lang.String md5Hex16(java.io.File);
  public static java.lang.String md5HexTo16(java.lang.String);
  public static byte[] sha1(byte[]);
  public static byte[] sha1(java.lang.String, java.lang.String);
  public static byte[] sha1(java.lang.String);
  public static byte[] sha1(java.io.InputStream);
  public static byte[] sha1(java.io.File);
  public static java.lang.String sha1Hex(byte[]);
  public static java.lang.String sha1Hex(java.lang.String, java.lang.String);
  public static java.lang.String sha1Hex(java.lang.String);
  public static java.lang.String sha1Hex(java.io.InputStream);
  public static java.lang.String sha1Hex(java.io.File);
  public static byte[] sha256(byte[]);
  public static byte[] sha256(java.lang.String, java.lang.String);
  public static byte[] sha256(java.lang.String);
  public static byte[] sha256(java.io.InputStream);
  public static byte[] sha256(java.io.File);
  public static java.lang.String sha256Hex(byte[]);
  public static java.lang.String sha256Hex(java.lang.String, java.lang.String);
  public static java.lang.String sha256Hex(java.lang.String);
  public static java.lang.String sha256Hex(java.io.InputStream);
  public static java.lang.String sha256Hex(java.io.File);
  public static cn.hutool.crypto.digest.HMac hmac(cn.hutool.crypto.digest.HmacAlgorithm, byte[]);
  public static cn.hutool.crypto.digest.HMac hmac(cn.hutool.crypto.digest.HmacAlgorithm, javax.crypto.SecretKey);
  public static cn.hutool.crypto.digest.Digester digester(cn.hutool.crypto.digest.DigestAlgorithm);
  public static cn.hutool.crypto.digest.Digester digester(java.lang.String);
  public static java.lang.String bcrypt(java.lang.String);
  public static boolean bcryptCheck(java.lang.String, java.lang.String);
  public static byte[] sha512(byte[]);
  public static byte[] sha512(java.lang.String, java.lang.String);
  public static byte[] sha512(java.lang.String);
  public static byte[] sha512(java.io.InputStream);
  public static byte[] sha512(java.io.File);
  public static java.lang.String sha512Hex(byte[]);
  public static java.lang.String sha512Hex(java.lang.String, java.lang.String);
  public static java.lang.String sha512Hex(java.lang.String);
  public static java.lang.String sha512Hex(java.io.InputStream);
  public static java.lang.String sha512Hex(java.io.File);
}
```

## `cn.hutool.crypto.digest.Digester`

```java
public class cn.hutool.crypto.digest.Digester implements java.io.Serializable {
  public cn.hutool.crypto.digest.Digester(cn.hutool.crypto.digest.DigestAlgorithm);
  public cn.hutool.crypto.digest.Digester(java.lang.String);
  public cn.hutool.crypto.digest.Digester(cn.hutool.crypto.digest.DigestAlgorithm, java.security.Provider);
  public cn.hutool.crypto.digest.Digester(java.lang.String, java.security.Provider);
  public cn.hutool.crypto.digest.Digester(java.security.MessageDigest);
  public cn.hutool.crypto.digest.Digester init(java.lang.String, java.security.Provider);
  public cn.hutool.crypto.digest.Digester setSalt(byte[]);
  public cn.hutool.crypto.digest.Digester setSaltPosition(int);
  public cn.hutool.crypto.digest.Digester setDigestCount(int);
  public cn.hutool.crypto.digest.Digester reset();
  public byte[] digest(java.lang.String, java.lang.String);
  public byte[] digest(java.lang.String, java.nio.charset.Charset);
  public byte[] digest(java.lang.String);
  public java.lang.String digestHex(java.lang.String, java.lang.String);
  public java.lang.String digestHex(java.lang.String, java.nio.charset.Charset);
  public java.lang.String digestHex(java.lang.String);
  public byte[] digest(java.io.File) throws cn.hutool.crypto.CryptoException;
  public java.lang.String digestHex(java.io.File);
  public byte[] digest(byte[]);
  public java.lang.String digestHex(byte[]);
  public byte[] digest(java.io.InputStream);
  public java.lang.String digestHex(java.io.InputStream);
  public byte[] digest(java.io.InputStream, int) throws cn.hutool.core.io.IORuntimeException;
  public java.lang.String digestHex(java.io.InputStream, int);
  public java.security.MessageDigest getDigest();
  public int getDigestLength();
}
```

## `cn.hutool.crypto.digest.DigesterFactory`

```java
public class cn.hutool.crypto.digest.DigesterFactory {
  public static cn.hutool.crypto.digest.DigesterFactory ofJdk(java.lang.String);
  public static cn.hutool.crypto.digest.DigesterFactory of(java.lang.String);
  public static cn.hutool.crypto.digest.DigesterFactory of(java.security.MessageDigest);
  public cn.hutool.crypto.digest.Digester createDigester();
  public java.security.MessageDigest createMessageDigester();
}
```

## `cn.hutool.crypto.digest.HMac`

```java
public class cn.hutool.crypto.digest.HMac extends cn.hutool.crypto.digest.mac.Mac {
  public cn.hutool.crypto.digest.HMac(cn.hutool.crypto.digest.HmacAlgorithm);
  public cn.hutool.crypto.digest.HMac(cn.hutool.crypto.digest.HmacAlgorithm, byte[]);
  public cn.hutool.crypto.digest.HMac(cn.hutool.crypto.digest.HmacAlgorithm, java.security.Key);
  public cn.hutool.crypto.digest.HMac(java.lang.String, byte[]);
  public cn.hutool.crypto.digest.HMac(java.lang.String, java.security.Key);
  public cn.hutool.crypto.digest.HMac(java.lang.String, java.security.Key, java.security.spec.AlgorithmParameterSpec);
  public cn.hutool.crypto.digest.HMac(cn.hutool.crypto.digest.mac.MacEngine);
}
```

## `cn.hutool.crypto.digest.HmacAlgorithm`

```java
public final class cn.hutool.crypto.digest.HmacAlgorithm extends java.lang.Enum<cn.hutool.crypto.digest.HmacAlgorithm> {
  public static cn.hutool.crypto.digest.HmacAlgorithm[] values();
  public static cn.hutool.crypto.digest.HmacAlgorithm valueOf(java.lang.String);
  public java.lang.String getValue();
}
```

## `cn.hutool.crypto.digest.MD5`

```java
public class cn.hutool.crypto.digest.MD5 extends cn.hutool.crypto.digest.Digester {
  public static cn.hutool.crypto.digest.MD5 create();
  public cn.hutool.crypto.digest.MD5();
  public cn.hutool.crypto.digest.MD5(byte[]);
  public cn.hutool.crypto.digest.MD5(byte[], int);
  public cn.hutool.crypto.digest.MD5(byte[], int, int);
  public java.lang.String digestHex16(java.lang.String, java.nio.charset.Charset);
  public java.lang.String digestHex16(java.lang.String);
  public java.lang.String digestHex16(java.io.InputStream);
  public java.lang.String digestHex16(java.io.File);
  public java.lang.String digestHex16(byte[]);
}
```

## `cn.hutool.crypto.digest.SM3`

```java
public class cn.hutool.crypto.digest.SM3 extends cn.hutool.crypto.digest.Digester {
  public static cn.hutool.crypto.digest.SM3 create();
  public cn.hutool.crypto.digest.SM3();
  public cn.hutool.crypto.digest.SM3(byte[]);
  public cn.hutool.crypto.digest.SM3(byte[], int);
  public cn.hutool.crypto.digest.SM3(byte[], int, int);
}
```
