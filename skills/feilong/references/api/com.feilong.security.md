# com.feilong.security

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.security.Base64Util`

```java
public class com.feilong.security.Base64Util {
  public com.feilong.security.Base64Util();
  public static java.lang.String encodeBase64(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String encodeBase64(java.lang.String, java.lang.String);
  public static java.lang.String encodeBase64(byte[]);
}
```

## `com.feilong.security.ByteUtil`

```java
public final class com.feilong.security.ByteUtil {
  public static java.lang.String bytesToHexStringLowerCase(byte[]);
  public static java.lang.String bytesToHexStringUpperCase(byte[]);
  public static java.lang.String byteToHexStringLowerCase(byte);
  public static byte[] hexBytesToBytes(byte[]);
  public static byte[] hexBytesToBytes2(byte[]);
  public static byte uniteBytes(byte, byte);
}
```

## `com.feilong.security.EncryptionException`

```java
public class com.feilong.security.EncryptionException extends com.feilong.core.DefaultRuntimeException {
  public com.feilong.security.EncryptionException(java.lang.String, java.lang.Throwable);
  public com.feilong.security.EncryptionException(java.lang.Throwable);
}
```

## `com.feilong.security.KeyUtil`

```java
public class com.feilong.security.KeyUtil {
  public com.feilong.security.KeyUtil();
  public static java.security.Key generatePrivateKey(java.lang.String);
  public static java.security.Key generatePrivateKey(java.lang.String, java.lang.String);
}
```
