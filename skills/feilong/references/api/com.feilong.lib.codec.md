# com.feilong.lib.codec

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.codec.BinaryDecoder`

```java
public interface com.feilong.lib.codec.BinaryDecoder extends com.feilong.lib.codec.Decoder {
  public abstract byte[] decode(byte[]) throws com.feilong.lib.codec.DecoderException;
}
```

## `com.feilong.lib.codec.BinaryEncoder`

```java
public interface com.feilong.lib.codec.BinaryEncoder extends com.feilong.lib.codec.Encoder {
  public abstract byte[] encode(byte[]) throws com.feilong.lib.codec.EncoderException;
}
```

## `com.feilong.lib.codec.Decoder`

```java
public interface com.feilong.lib.codec.Decoder {
  public abstract java.lang.Object decode(java.lang.Object) throws com.feilong.lib.codec.DecoderException;
}
```

## `com.feilong.lib.codec.DecoderException`

```java
public class com.feilong.lib.codec.DecoderException extends java.lang.Exception {
  public com.feilong.lib.codec.DecoderException(java.lang.String);
  public com.feilong.lib.codec.DecoderException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.codec.Encoder`

```java
public interface com.feilong.lib.codec.Encoder {
  public abstract java.lang.Object encode(java.lang.Object) throws com.feilong.lib.codec.EncoderException;
}
```

## `com.feilong.lib.codec.EncoderException`

```java
public class com.feilong.lib.codec.EncoderException extends java.lang.Exception {
  public com.feilong.lib.codec.EncoderException();
  public com.feilong.lib.codec.EncoderException(java.lang.String);
  public com.feilong.lib.codec.EncoderException(java.lang.String, java.lang.Throwable);
  public com.feilong.lib.codec.EncoderException(java.lang.Throwable);
}
```
