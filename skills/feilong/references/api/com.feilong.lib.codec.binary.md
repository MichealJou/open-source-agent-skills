# com.feilong.lib.codec.binary

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.codec.binary.Base64`

```java
public class com.feilong.lib.codec.binary.Base64 extends com.feilong.lib.codec.binary.BaseNCodec {
  public com.feilong.lib.codec.binary.Base64();
  public com.feilong.lib.codec.binary.Base64(boolean);
  public com.feilong.lib.codec.binary.Base64(int);
  public com.feilong.lib.codec.binary.Base64(int, byte[]);
  public com.feilong.lib.codec.binary.Base64(int, byte[], boolean);
  public boolean isUrlSafe();
  public static boolean isBase64(byte);
  public static boolean isBase64(java.lang.String);
  public static boolean isBase64(byte[]);
  public static byte[] encodeBase64(byte[]);
  public static java.lang.String encodeBase64String(byte[]);
  public static byte[] encodeBase64URLSafe(byte[]);
  public static java.lang.String encodeBase64URLSafeString(byte[]);
  public static byte[] encodeBase64Chunked(byte[]);
  public static byte[] encodeBase64(byte[], boolean);
  public static byte[] encodeBase64(byte[], boolean, boolean);
  public static byte[] encodeBase64(byte[], boolean, boolean, int);
  public static byte[] decodeBase64(java.lang.String);
  public static byte[] decodeBase64(byte[]);
  public static java.math.BigInteger decodeInteger(byte[]);
  public static byte[] encodeInteger(java.math.BigInteger);
}
```

## `com.feilong.lib.codec.binary.BaseNCodec`

```java
public abstract class com.feilong.lib.codec.binary.BaseNCodec implements com.feilong.lib.codec.BinaryEncoder,com.feilong.lib.codec.BinaryDecoder {
  public java.lang.Object encode(java.lang.Object) throws com.feilong.lib.codec.EncoderException;
  public java.lang.String encodeToString(byte[]);
  public java.lang.String encodeAsString(byte[]);
  public java.lang.Object decode(java.lang.Object) throws com.feilong.lib.codec.DecoderException;
  public byte[] decode(java.lang.String);
  public byte[] decode(byte[]);
  public byte[] encode(byte[]);
  public byte[] encode(byte[], int, int);
  public boolean isInAlphabet(byte[], boolean);
  public boolean isInAlphabet(java.lang.String);
  public long getEncodedLength(byte[]);
}
```

## `com.feilong.lib.codec.binary.Hex`

```java
public class com.feilong.lib.codec.binary.Hex implements com.feilong.lib.codec.BinaryEncoder,com.feilong.lib.codec.BinaryDecoder {
  public static byte[] decodeHex(java.lang.String) throws com.feilong.lib.codec.DecoderException;
  public static byte[] decodeHex(char[]) throws com.feilong.lib.codec.DecoderException;
  public static char[] encodeHex(byte[]);
  public static char[] encodeHex(java.nio.ByteBuffer);
  public static char[] encodeHex(byte[], boolean);
  public static char[] encodeHex(java.nio.ByteBuffer, boolean);
  public static java.lang.String encodeHexString(byte[]);
  public static java.lang.String encodeHexString(byte[], boolean);
  public static java.lang.String encodeHexString(java.nio.ByteBuffer);
  public static java.lang.String encodeHexString(java.nio.ByteBuffer, boolean);
  public com.feilong.lib.codec.binary.Hex();
  public com.feilong.lib.codec.binary.Hex(java.nio.charset.Charset);
  public com.feilong.lib.codec.binary.Hex(java.lang.String);
  public byte[] decode(byte[]) throws com.feilong.lib.codec.DecoderException;
  public byte[] decode(java.nio.ByteBuffer) throws com.feilong.lib.codec.DecoderException;
  public java.lang.Object decode(java.lang.Object) throws com.feilong.lib.codec.DecoderException;
  public byte[] encode(byte[]);
  public byte[] encode(java.nio.ByteBuffer);
  public java.lang.Object encode(java.lang.Object) throws com.feilong.lib.codec.EncoderException;
  public java.nio.charset.Charset getCharset();
  public java.lang.String getCharsetName();
  public java.lang.String toString();
}
```

## `com.feilong.lib.codec.binary.StringUtils`

```java
public class com.feilong.lib.codec.binary.StringUtils {
  public com.feilong.lib.codec.binary.StringUtils();
  public static byte[] getBytesUnchecked(java.lang.String, java.lang.String);
  public static byte[] getBytesUtf8(java.lang.String);
  public static java.lang.String newStringUsAscii(byte[]);
  public static java.lang.String newStringUtf8(byte[]);
}
```
