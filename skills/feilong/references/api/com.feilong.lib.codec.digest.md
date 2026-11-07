# com.feilong.lib.codec.digest

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.codec.digest.DigestUtils`

```java
public class com.feilong.lib.codec.digest.DigestUtils {
  public static byte[] digest(java.security.MessageDigest, byte[]);
  public static byte[] digest(java.security.MessageDigest, java.nio.ByteBuffer);
  public static byte[] digest(java.security.MessageDigest, java.io.File) throws java.io.IOException;
  public static byte[] digest(java.security.MessageDigest, java.io.InputStream) throws java.io.IOException;
  public static byte[] digest(java.security.MessageDigest, java.nio.file.Path, java.nio.file.OpenOption...) throws java.io.IOException;
  public static byte[] digest(java.security.MessageDigest, java.io.RandomAccessFile) throws java.io.IOException;
  public static java.security.MessageDigest getDigest(java.lang.String);
  public static java.security.MessageDigest getDigest(java.lang.String, java.security.MessageDigest);
  public static java.security.MessageDigest getMd2Digest();
  public static java.security.MessageDigest getMd5Digest();
  public static java.security.MessageDigest getSha1Digest();
  public static java.security.MessageDigest getSha256Digest();
  public static java.security.MessageDigest getSha3_224Digest();
  public static java.security.MessageDigest getSha3_256Digest();
  public static java.security.MessageDigest getSha3_384Digest();
  public static java.security.MessageDigest getSha3_512Digest();
  public static java.security.MessageDigest getSha384Digest();
  public static java.security.MessageDigest getSha512_224Digest();
  public static java.security.MessageDigest getSha512_256Digest();
  public static java.security.MessageDigest getSha512Digest();
  public static boolean isAvailable(java.lang.String);
  public static byte[] md2(byte[]);
  public static byte[] md2(java.io.InputStream) throws java.io.IOException;
  public static byte[] md2(java.lang.String);
  public static java.lang.String md2Hex(byte[]);
  public static java.lang.String md2Hex(java.io.InputStream) throws java.io.IOException;
  public static java.lang.String md2Hex(java.lang.String);
  public static byte[] md5(byte[]);
  public static byte[] md5(java.io.InputStream) throws java.io.IOException;
  public static byte[] md5(java.lang.String);
  public static java.lang.String md5Hex(byte[]);
  public static java.lang.String md5Hex(java.io.InputStream) throws java.io.IOException;
  public static java.lang.String md5Hex(java.lang.String);
  public static byte[] sha1(byte[]);
  public static byte[] sha1(java.io.InputStream) throws java.io.IOException;
  public static byte[] sha1(java.lang.String);
  public static java.lang.String sha1Hex(byte[]);
  public static java.lang.String sha1Hex(java.io.InputStream) throws java.io.IOException;
  public static java.lang.String sha1Hex(java.lang.String);
  public static byte[] sha256(byte[]);
  public static byte[] sha256(java.io.InputStream) throws java.io.IOException;
  public static byte[] sha256(java.lang.String);
  public static java.lang.String sha256Hex(byte[]);
  public static java.lang.String sha256Hex(java.io.InputStream) throws java.io.IOException;
  public static java.lang.String sha256Hex(java.lang.String);
  public static byte[] sha3_224(byte[]);
  public static byte[] sha3_224(java.io.InputStream) throws java.io.IOException;
  public static byte[] sha3_224(java.lang.String);
  public static java.lang.String sha3_224Hex(byte[]);
  public static java.lang.String sha3_224Hex(java.io.InputStream) throws java.io.IOException;
  public static java.lang.String sha3_224Hex(java.lang.String);
  public static byte[] sha3_256(byte[]);
  public static byte[] sha3_256(java.io.InputStream) throws java.io.IOException;
  public static byte[] sha3_256(java.lang.String);
  public static java.lang.String sha3_256Hex(byte[]);
  public static java.lang.String sha3_256Hex(java.io.InputStream) throws java.io.IOException;
  public static java.lang.String sha3_256Hex(java.lang.String);
  public static byte[] sha3_384(byte[]);
  public static byte[] sha3_384(java.io.InputStream) throws java.io.IOException;
  public static byte[] sha3_384(java.lang.String);
  public static java.lang.String sha3_384Hex(byte[]);
  public static java.lang.String sha3_384Hex(java.io.InputStream) throws java.io.IOException;
  public static java.lang.String sha3_384Hex(java.lang.String);
  public static byte[] sha3_512(byte[]);
  public static byte[] sha3_512(java.io.InputStream) throws java.io.IOException;
  public static byte[] sha3_512(java.lang.String);
  public static java.lang.String sha3_512Hex(byte[]);
  public static java.lang.String sha3_512Hex(java.io.InputStream) throws java.io.IOException;
  public static java.lang.String sha3_512Hex(java.lang.String);
  public static byte[] sha384(byte[]);
  public static byte[] sha384(java.io.InputStream) throws java.io.IOException;
  public static byte[] sha384(java.lang.String);
  public static java.lang.String sha384Hex(byte[]);
  public static java.lang.String sha384Hex(java.io.InputStream) throws java.io.IOException;
  public static java.lang.String sha384Hex(java.lang.String);
  public static byte[] sha512(byte[]);
  public static byte[] sha512(java.io.InputStream) throws java.io.IOException;
  public static byte[] sha512(java.lang.String);
  public static byte[] sha512_224(byte[]);
  public static byte[] sha512_224(java.io.InputStream) throws java.io.IOException;
  public static byte[] sha512_224(java.lang.String);
  public static java.lang.String sha512_224Hex(byte[]);
  public static java.lang.String sha512_224Hex(java.io.InputStream) throws java.io.IOException;
  public static java.lang.String sha512_224Hex(java.lang.String);
  public static byte[] sha512_256(byte[]);
  public static byte[] sha512_256(java.io.InputStream) throws java.io.IOException;
  public static byte[] sha512_256(java.lang.String);
  public static java.lang.String sha512_256Hex(byte[]);
  public static java.lang.String sha512_256Hex(java.io.InputStream) throws java.io.IOException;
  public static java.lang.String sha512_256Hex(java.lang.String);
  public static java.lang.String sha512Hex(byte[]);
  public static java.lang.String sha512Hex(java.io.InputStream) throws java.io.IOException;
  public static java.lang.String sha512Hex(java.lang.String);
  public static java.security.MessageDigest updateDigest(java.security.MessageDigest, byte[]);
  public static java.security.MessageDigest updateDigest(java.security.MessageDigest, java.nio.ByteBuffer);
  public static java.security.MessageDigest updateDigest(java.security.MessageDigest, java.io.File) throws java.io.IOException;
  public static java.security.MessageDigest updateDigest(java.security.MessageDigest, java.io.InputStream) throws java.io.IOException;
  public static java.security.MessageDigest updateDigest(java.security.MessageDigest, java.nio.file.Path, java.nio.file.OpenOption...) throws java.io.IOException;
  public static java.security.MessageDigest updateDigest(java.security.MessageDigest, java.io.RandomAccessFile) throws java.io.IOException;
  public static java.security.MessageDigest updateDigest(java.security.MessageDigest, java.lang.String);
  public com.feilong.lib.codec.digest.DigestUtils(java.security.MessageDigest);
  public com.feilong.lib.codec.digest.DigestUtils(java.lang.String);
  public byte[] digest(byte[]);
  public byte[] digest(java.nio.ByteBuffer);
  public byte[] digest(java.io.File) throws java.io.IOException;
  public byte[] digest(java.io.InputStream) throws java.io.IOException;
  public byte[] digest(java.nio.file.Path, java.nio.file.OpenOption...) throws java.io.IOException;
  public byte[] digest(java.lang.String);
  public java.lang.String digestAsHex(byte[]);
  public java.lang.String digestAsHex(java.nio.ByteBuffer);
  public java.lang.String digestAsHex(java.io.File) throws java.io.IOException;
  public java.lang.String digestAsHex(java.io.InputStream) throws java.io.IOException;
  public java.lang.String digestAsHex(java.nio.file.Path, java.nio.file.OpenOption...) throws java.io.IOException;
  public java.lang.String digestAsHex(java.lang.String);
  public java.security.MessageDigest getMessageDigest();
}
```

## `com.feilong.lib.codec.digest.HmacAlgorithms`

```java
public final class com.feilong.lib.codec.digest.HmacAlgorithms extends java.lang.Enum<com.feilong.lib.codec.digest.HmacAlgorithms> {
  public static com.feilong.lib.codec.digest.HmacAlgorithms[] values();
  public static com.feilong.lib.codec.digest.HmacAlgorithms valueOf(java.lang.String);
  public java.lang.String getName();
  public java.lang.String toString();
}
```

## `com.feilong.lib.codec.digest.HmacUtils`

```java
public final class com.feilong.lib.codec.digest.HmacUtils {
  public static boolean isAvailable(java.lang.String);
  public static boolean isAvailable(com.feilong.lib.codec.digest.HmacAlgorithms);
  public static javax.crypto.Mac getHmacMd5(byte[]);
  public static javax.crypto.Mac getHmacSha1(byte[]);
  public static javax.crypto.Mac getHmacSha256(byte[]);
  public static javax.crypto.Mac getHmacSha384(byte[]);
  public static javax.crypto.Mac getHmacSha512(byte[]);
  public static javax.crypto.Mac getInitializedMac(com.feilong.lib.codec.digest.HmacAlgorithms, byte[]);
  public static javax.crypto.Mac getInitializedMac(java.lang.String, byte[]);
  public static byte[] hmacMd5(byte[], byte[]);
  public static byte[] hmacMd5(byte[], java.io.InputStream) throws java.io.IOException;
  public static byte[] hmacMd5(java.lang.String, java.lang.String);
  public static java.lang.String hmacMd5Hex(byte[], byte[]);
  public static java.lang.String hmacMd5Hex(byte[], java.io.InputStream) throws java.io.IOException;
  public static java.lang.String hmacMd5Hex(java.lang.String, java.lang.String);
  public static byte[] hmacSha1(byte[], byte[]);
  public static byte[] hmacSha1(byte[], java.io.InputStream) throws java.io.IOException;
  public static byte[] hmacSha1(java.lang.String, java.lang.String);
  public static java.lang.String hmacSha1Hex(byte[], byte[]);
  public static java.lang.String hmacSha1Hex(byte[], java.io.InputStream) throws java.io.IOException;
  public static java.lang.String hmacSha1Hex(java.lang.String, java.lang.String);
  public static byte[] hmacSha256(byte[], byte[]);
  public static byte[] hmacSha256(byte[], java.io.InputStream) throws java.io.IOException;
  public static byte[] hmacSha256(java.lang.String, java.lang.String);
  public static java.lang.String hmacSha256Hex(byte[], byte[]);
  public static java.lang.String hmacSha256Hex(byte[], java.io.InputStream) throws java.io.IOException;
  public static java.lang.String hmacSha256Hex(java.lang.String, java.lang.String);
  public static byte[] hmacSha384(byte[], byte[]);
  public static byte[] hmacSha384(byte[], java.io.InputStream) throws java.io.IOException;
  public static byte[] hmacSha384(java.lang.String, java.lang.String);
  public static java.lang.String hmacSha384Hex(byte[], byte[]);
  public static java.lang.String hmacSha384Hex(byte[], java.io.InputStream) throws java.io.IOException;
  public static java.lang.String hmacSha384Hex(java.lang.String, java.lang.String);
  public static byte[] hmacSha512(byte[], byte[]);
  public static byte[] hmacSha512(byte[], java.io.InputStream) throws java.io.IOException;
  public static byte[] hmacSha512(java.lang.String, java.lang.String);
  public static java.lang.String hmacSha512Hex(byte[], byte[]);
  public static java.lang.String hmacSha512Hex(byte[], java.io.InputStream) throws java.io.IOException;
  public static java.lang.String hmacSha512Hex(java.lang.String, java.lang.String);
  public static javax.crypto.Mac updateHmac(javax.crypto.Mac, byte[]);
  public static javax.crypto.Mac updateHmac(javax.crypto.Mac, java.io.InputStream) throws java.io.IOException;
  public static javax.crypto.Mac updateHmac(javax.crypto.Mac, java.lang.String);
  public com.feilong.lib.codec.digest.HmacUtils();
  public com.feilong.lib.codec.digest.HmacUtils(java.lang.String, byte[]);
  public com.feilong.lib.codec.digest.HmacUtils(java.lang.String, java.lang.String);
  public com.feilong.lib.codec.digest.HmacUtils(com.feilong.lib.codec.digest.HmacAlgorithms, java.lang.String);
  public com.feilong.lib.codec.digest.HmacUtils(com.feilong.lib.codec.digest.HmacAlgorithms, byte[]);
  public byte[] hmac(byte[]);
  public java.lang.String hmacHex(byte[]);
  public byte[] hmac(java.lang.String);
  public java.lang.String hmacHex(java.lang.String);
  public byte[] hmac(java.nio.ByteBuffer);
  public java.lang.String hmacHex(java.nio.ByteBuffer);
  public byte[] hmac(java.io.InputStream) throws java.io.IOException;
  public java.lang.String hmacHex(java.io.InputStream) throws java.io.IOException;
  public byte[] hmac(java.io.File) throws java.io.IOException;
  public java.lang.String hmacHex(java.io.File) throws java.io.IOException;
}
```
