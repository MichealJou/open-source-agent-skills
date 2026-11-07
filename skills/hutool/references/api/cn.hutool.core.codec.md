# cn.hutool.core.codec

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.codec.BCD`

```java
public class cn.hutool.core.codec.BCD {
  public cn.hutool.core.codec.BCD();
  public static byte[] strToBcd(java.lang.String);
  public static byte[] ascToBcd(byte[]);
  public static byte[] ascToBcd(byte[], int);
  public static java.lang.String bcdToStr(byte[]);
}
```

## `cn.hutool.core.codec.Base16Codec`

```java
public class cn.hutool.core.codec.Base16Codec implements cn.hutool.core.codec.Encoder<byte[], char[]>, cn.hutool.core.codec.Decoder<java.lang.CharSequence, byte[]> {
  public cn.hutool.core.codec.Base16Codec(boolean);
  public char[] encode(byte[]);
  public byte[] decode(java.lang.CharSequence);
  public java.lang.String toUnicodeHex(char);
  public void appendHex(java.lang.StringBuilder, byte);
  public java.lang.Object encode(java.lang.Object);
  public java.lang.Object decode(java.lang.Object);
}
```

## `cn.hutool.core.codec.Base32`

```java
public class cn.hutool.core.codec.Base32 {
  public cn.hutool.core.codec.Base32();
  public static java.lang.String encode(byte[]);
  public static java.lang.String encode(java.lang.String);
  public static java.lang.String encode(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String encodeHex(byte[]);
  public static java.lang.String encodeHex(java.lang.String);
  public static java.lang.String encodeHex(java.lang.String, java.nio.charset.Charset);
  public static byte[] decode(java.lang.String);
  public static java.lang.String decodeStr(java.lang.String);
  public static java.lang.String decodeStr(java.lang.String, java.nio.charset.Charset);
  public static byte[] decodeHex(java.lang.String);
  public static java.lang.String decodeStrHex(java.lang.String);
  public static java.lang.String decodeStrHex(java.lang.String, java.nio.charset.Charset);
}
```

## `cn.hutool.core.codec.Base32Codec`

```java
public class cn.hutool.core.codec.Base32Codec implements cn.hutool.core.codec.Encoder<byte[], java.lang.String>, cn.hutool.core.codec.Decoder<java.lang.CharSequence, byte[]> {
  public cn.hutool.core.codec.Base32Codec();
  public java.lang.String encode(byte[]);
  public java.lang.String encode(byte[], boolean);
  public byte[] decode(java.lang.CharSequence);
  public byte[] decode(java.lang.CharSequence, boolean);
  public java.lang.Object encode(java.lang.Object);
  public java.lang.Object decode(java.lang.Object);
}
```

## `cn.hutool.core.codec.Base32Codec$Base32Decoder`

```java
public class cn.hutool.core.codec.Base32Codec$Base32Decoder implements cn.hutool.core.codec.Decoder<java.lang.CharSequence, byte[]> {
  public cn.hutool.core.codec.Base32Codec$Base32Decoder(java.lang.String);
  public byte[] decode(java.lang.CharSequence);
  public java.lang.Object decode(java.lang.Object);
}
```

## `cn.hutool.core.codec.Base32Codec$Base32Encoder`

```java
public class cn.hutool.core.codec.Base32Codec$Base32Encoder implements cn.hutool.core.codec.Encoder<byte[], java.lang.String> {
  public cn.hutool.core.codec.Base32Codec$Base32Encoder(java.lang.String, java.lang.Character);
  public java.lang.String encode(byte[]);
  public java.lang.Object encode(java.lang.Object);
}
```

## `cn.hutool.core.codec.Base58`

```java
public class cn.hutool.core.codec.Base58 {
  public cn.hutool.core.codec.Base58();
  public static java.lang.String encodeChecked(java.lang.Integer, byte[]);
  public static java.lang.String encode(byte[]);
  public static byte[] decodeChecked(java.lang.CharSequence) throws cn.hutool.core.exceptions.ValidateException;
  public static byte[] decodeChecked(java.lang.CharSequence, boolean) throws cn.hutool.core.exceptions.ValidateException;
  public static byte[] decode(java.lang.CharSequence);
}
```

## `cn.hutool.core.codec.Base58Codec`

```java
public class cn.hutool.core.codec.Base58Codec implements cn.hutool.core.codec.Encoder<byte[], java.lang.String>, cn.hutool.core.codec.Decoder<java.lang.CharSequence, byte[]> {
  public cn.hutool.core.codec.Base58Codec();
  public java.lang.String encode(byte[]);
  public byte[] decode(java.lang.CharSequence) throws java.lang.IllegalArgumentException;
  public java.lang.Object encode(java.lang.Object);
  public java.lang.Object decode(java.lang.Object);
}
```

## `cn.hutool.core.codec.Base58Codec$Base58Decoder`

```java
public class cn.hutool.core.codec.Base58Codec$Base58Decoder implements cn.hutool.core.codec.Decoder<java.lang.CharSequence, byte[]> {
  public cn.hutool.core.codec.Base58Codec$Base58Decoder(java.lang.String);
  public byte[] decode(java.lang.CharSequence);
  public java.lang.Object decode(java.lang.Object);
}
```

## `cn.hutool.core.codec.Base58Codec$Base58Encoder`

```java
public class cn.hutool.core.codec.Base58Codec$Base58Encoder implements cn.hutool.core.codec.Encoder<byte[], java.lang.String> {
  public cn.hutool.core.codec.Base58Codec$Base58Encoder(char[]);
  public java.lang.String encode(byte[]);
  public java.lang.Object encode(java.lang.Object);
}
```

## `cn.hutool.core.codec.Base62`

```java
public class cn.hutool.core.codec.Base62 {
  public cn.hutool.core.codec.Base62();
  public static java.lang.String encode(java.lang.CharSequence);
  public static java.lang.String encode(java.lang.CharSequence, java.nio.charset.Charset);
  public static java.lang.String encode(byte[]);
  public static java.lang.String encode(java.io.InputStream);
  public static java.lang.String encode(java.io.File);
  public static java.lang.String encodeInverted(java.lang.CharSequence);
  public static java.lang.String encodeInverted(java.lang.CharSequence, java.nio.charset.Charset);
  public static java.lang.String encodeInverted(byte[]);
  public static java.lang.String encodeInverted(java.io.InputStream);
  public static java.lang.String encodeInverted(java.io.File);
  public static java.lang.String decodeStrGbk(java.lang.CharSequence);
  public static java.lang.String decodeStr(java.lang.CharSequence);
  public static java.lang.String decodeStr(java.lang.CharSequence, java.nio.charset.Charset);
  public static java.io.File decodeToFile(java.lang.CharSequence, java.io.File);
  public static void decodeToStream(java.lang.CharSequence, java.io.OutputStream, boolean);
  public static byte[] decode(java.lang.CharSequence);
  public static byte[] decode(byte[]);
  public static java.lang.String decodeStrInverted(java.lang.CharSequence);
  public static java.lang.String decodeStrInverted(java.lang.CharSequence, java.nio.charset.Charset);
  public static java.io.File decodeToFileInverted(java.lang.CharSequence, java.io.File);
  public static void decodeToStreamInverted(java.lang.CharSequence, java.io.OutputStream, boolean);
  public static byte[] decodeInverted(java.lang.CharSequence);
  public static byte[] decodeInverted(byte[]);
}
```

## `cn.hutool.core.codec.Base62Codec`

```java
public class cn.hutool.core.codec.Base62Codec implements cn.hutool.core.codec.Encoder<byte[], byte[]>, cn.hutool.core.codec.Decoder<byte[], byte[]>, java.io.Serializable {
  public cn.hutool.core.codec.Base62Codec();
  public byte[] encode(byte[]);
  public byte[] encode(byte[], boolean);
  public byte[] decode(byte[]);
  public byte[] decode(byte[], boolean);
  public java.lang.Object encode(java.lang.Object);
  public java.lang.Object decode(java.lang.Object);
}
```

## `cn.hutool.core.codec.Base62Codec$Base62Decoder`

```java
public class cn.hutool.core.codec.Base62Codec$Base62Decoder implements cn.hutool.core.codec.Decoder<byte[], byte[]> {
  public cn.hutool.core.codec.Base62Codec$Base62Decoder(byte[]);
  public byte[] decode(byte[]);
  public java.lang.Object decode(java.lang.Object);
}
```

## `cn.hutool.core.codec.Base62Codec$Base62Encoder`

```java
public class cn.hutool.core.codec.Base62Codec$Base62Encoder implements cn.hutool.core.codec.Encoder<byte[], byte[]> {
  public cn.hutool.core.codec.Base62Codec$Base62Encoder(byte[]);
  public byte[] encode(byte[]);
  public java.lang.Object encode(java.lang.Object);
}
```

## `cn.hutool.core.codec.Base64`

```java
public class cn.hutool.core.codec.Base64 {
  public cn.hutool.core.codec.Base64();
  public static byte[] encode(byte[], boolean);
  public static byte[] encodeUrlSafe(byte[], boolean);
  public static java.lang.String encode(java.lang.CharSequence);
  public static java.lang.String encodeUrlSafe(java.lang.CharSequence);
  public static java.lang.String encode(java.lang.CharSequence, java.lang.String);
  public static java.lang.String encodeWithoutPadding(java.lang.CharSequence, java.lang.String);
  public static java.lang.String encodeUrlSafe(java.lang.CharSequence, java.lang.String);
  public static java.lang.String encode(java.lang.CharSequence, java.nio.charset.Charset);
  public static java.lang.String encodeUrlSafe(java.lang.CharSequence, java.nio.charset.Charset);
  public static java.lang.String encode(byte[]);
  public static java.lang.String encodeWithoutPadding(byte[]);
  public static java.lang.String encodeUrlSafe(byte[]);
  public static java.lang.String encode(java.io.InputStream);
  public static java.lang.String encodeUrlSafe(java.io.InputStream);
  public static java.lang.String encode(java.io.File);
  public static java.lang.String encodeUrlSafe(java.io.File);
  public static java.lang.String encodeStr(byte[], boolean, boolean);
  public static byte[] encode(byte[], boolean, boolean);
  public static java.lang.String decodeStrGbk(java.lang.CharSequence);
  public static java.lang.String decodeStr(java.lang.CharSequence);
  public static java.lang.String decodeStr(java.lang.CharSequence, java.lang.String);
  public static java.lang.String decodeStr(java.lang.CharSequence, java.nio.charset.Charset);
  public static java.io.File decodeToFile(java.lang.CharSequence, java.io.File);
  public static void decodeToStream(java.lang.CharSequence, java.io.OutputStream, boolean);
  public static byte[] decode(java.lang.CharSequence);
  public static byte[] decode(byte[]);
  public static boolean isBase64(java.lang.CharSequence);
  public static boolean isBase64(byte[]);
}
```

## `cn.hutool.core.codec.Base64Decoder`

```java
public class cn.hutool.core.codec.Base64Decoder {
  public cn.hutool.core.codec.Base64Decoder();
  public static java.lang.String decodeStr(java.lang.CharSequence);
  public static java.lang.String decodeStr(java.lang.CharSequence, java.nio.charset.Charset);
  public static byte[] decode(java.lang.CharSequence);
  public static byte[] decode(byte[]);
  public static byte[] decode(byte[], int, int);
  public static boolean isBase64Code(byte);
}
```

## `cn.hutool.core.codec.Base64Encoder`

```java
public class cn.hutool.core.codec.Base64Encoder {
  public cn.hutool.core.codec.Base64Encoder();
  public static byte[] encode(byte[], boolean);
  public static byte[] encodeUrlSafe(byte[], boolean);
  public static java.lang.String encode(java.lang.CharSequence);
  public static java.lang.String encodeUrlSafe(java.lang.CharSequence);
  public static java.lang.String encode(java.lang.CharSequence, java.nio.charset.Charset);
  public static java.lang.String encodeUrlSafe(java.lang.CharSequence, java.nio.charset.Charset);
  public static java.lang.String encode(byte[]);
  public static java.lang.String encodeUrlSafe(byte[]);
  public static java.lang.String encodeStr(byte[], boolean, boolean);
  public static byte[] encode(byte[], boolean, boolean);
}
```

## `cn.hutool.core.codec.Caesar`

```java
public class cn.hutool.core.codec.Caesar {
  public cn.hutool.core.codec.Caesar();
  public static java.lang.String encode(java.lang.String, int);
  public static java.lang.String decode(java.lang.String, int);
}
```

## `cn.hutool.core.codec.Decoder`

```java
public interface cn.hutool.core.codec.Decoder<T, R> {
  public abstract R decode(T);
}
```

## `cn.hutool.core.codec.Encoder`

```java
public interface cn.hutool.core.codec.Encoder<T, R> {
  public abstract R encode(T);
}
```

## `cn.hutool.core.codec.Hashids`

```java
public class cn.hutool.core.codec.Hashids implements cn.hutool.core.codec.Encoder<long[], java.lang.String>, cn.hutool.core.codec.Decoder<java.lang.String, long[]> {
  public static cn.hutool.core.codec.Hashids create(char[]);
  public static cn.hutool.core.codec.Hashids create(char[], int);
  public static cn.hutool.core.codec.Hashids create(char[], char[], int);
  public cn.hutool.core.codec.Hashids(char[], char[], int);
  public java.lang.String encodeFromHex(java.lang.String);
  public java.lang.String encode(long...);
  public java.lang.String decodeToHex(java.lang.String);
  public long[] decode(java.lang.String);
  public java.lang.Object encode(java.lang.Object);
  public java.lang.Object decode(java.lang.Object);
}
```

## `cn.hutool.core.codec.Morse`

```java
public class cn.hutool.core.codec.Morse {
  public cn.hutool.core.codec.Morse();
  public cn.hutool.core.codec.Morse(char, char, char);
  public java.lang.String encode(java.lang.String);
  public java.lang.String decode(java.lang.String);
}
```

## `cn.hutool.core.codec.PercentCodec`

```java
public class cn.hutool.core.codec.PercentCodec implements java.io.Serializable {
  public static cn.hutool.core.codec.PercentCodec of(cn.hutool.core.codec.PercentCodec);
  public static cn.hutool.core.codec.PercentCodec of(java.lang.CharSequence);
  public cn.hutool.core.codec.PercentCodec();
  public cn.hutool.core.codec.PercentCodec(java.util.BitSet);
  public cn.hutool.core.codec.PercentCodec addSafe(char);
  public cn.hutool.core.codec.PercentCodec removeSafe(char);
  public cn.hutool.core.codec.PercentCodec or(cn.hutool.core.codec.PercentCodec);
  public cn.hutool.core.codec.PercentCodec orNew(cn.hutool.core.codec.PercentCodec);
  public cn.hutool.core.codec.PercentCodec setEncodeSpaceAsPlus(boolean);
  public java.lang.String encode(java.lang.CharSequence, java.nio.charset.Charset, char...);
}
```

## `cn.hutool.core.codec.PunyCode`

```java
public class cn.hutool.core.codec.PunyCode {
  public cn.hutool.core.codec.PunyCode();
  public static java.lang.String encodeDomain(java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.String encode(java.lang.CharSequence) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.String encode(java.lang.CharSequence, boolean) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.String decodeDomain(java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.String decode(java.lang.String) throws cn.hutool.core.exceptions.UtilException;
}
```

## `cn.hutool.core.codec.Rot`

```java
public class cn.hutool.core.codec.Rot {
  public cn.hutool.core.codec.Rot();
  public static java.lang.String encode13(java.lang.String);
  public static java.lang.String encode13(java.lang.String, boolean);
  public static java.lang.String encode(java.lang.String, int, boolean);
  public static java.lang.String decode13(java.lang.String);
  public static java.lang.String decode13(java.lang.String, boolean);
  public static java.lang.String decode(java.lang.String, int, boolean);
}
```
