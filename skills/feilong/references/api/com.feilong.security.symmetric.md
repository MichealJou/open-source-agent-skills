# com.feilong.security.symmetric

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.security.symmetric.AesUtil`

```java
public class com.feilong.security.symmetric.AesUtil extends com.feilong.security.symmetric.SymmetricEncryption {
  public com.feilong.security.symmetric.AesUtil();
  public com.feilong.security.symmetric.AesUtil(java.lang.String);
  public com.feilong.security.symmetric.AesUtil(java.lang.String, com.feilong.security.symmetric.builder.KeyBuilder);
  public com.feilong.security.symmetric.AesUtil(java.lang.String, com.feilong.security.symmetric.CipherMode, com.feilong.security.symmetric.CipherPadding);
  public com.feilong.security.symmetric.AesUtil(java.lang.String, com.feilong.security.symmetric.builder.KeyBuilder, com.feilong.security.symmetric.CipherMode, com.feilong.security.symmetric.CipherPadding);
  public void setSymmetricType(com.feilong.security.symmetric.SymmetricType);
}
```

## `com.feilong.security.symmetric.CipherMode`

```java
public final class com.feilong.security.symmetric.CipherMode extends java.lang.Enum<com.feilong.security.symmetric.CipherMode> {
  public static com.feilong.security.symmetric.CipherMode[] values();
  public static com.feilong.security.symmetric.CipherMode valueOf(java.lang.String);
}
```

## `com.feilong.security.symmetric.CipherPadding`

```java
public final class com.feilong.security.symmetric.CipherPadding extends java.lang.Enum<com.feilong.security.symmetric.CipherPadding> {
  public static com.feilong.security.symmetric.CipherPadding[] values();
  public static com.feilong.security.symmetric.CipherPadding valueOf(java.lang.String);
}
```

## `com.feilong.security.symmetric.CipherUtil`

```java
public class com.feilong.security.symmetric.CipherUtil {
  public static byte[] encrypt(byte[], java.lang.String, java.security.Key);
  public static byte[] decrypt(byte[], java.lang.String, java.security.Key);
}
```

## `com.feilong.security.symmetric.LogBuilder`

```java
public class com.feilong.security.symmetric.LogBuilder {
  public static java.lang.String hided(java.lang.String);
}
```

## `com.feilong.security.symmetric.SymmetricEncryption`

```java
public class com.feilong.security.symmetric.SymmetricEncryption {
  public com.feilong.security.symmetric.SymmetricEncryption();
  public com.feilong.security.symmetric.SymmetricEncryption(com.feilong.security.symmetric.SymmetricType);
  public com.feilong.security.symmetric.SymmetricEncryption(com.feilong.security.symmetric.SymmetricType, java.lang.String);
  public com.feilong.security.symmetric.SymmetricEncryption(com.feilong.security.symmetric.SymmetricType, java.lang.String, com.feilong.security.symmetric.builder.KeyBuilder);
  public com.feilong.security.symmetric.SymmetricEncryption(com.feilong.security.symmetric.SymmetricType, java.lang.String, com.feilong.security.symmetric.CipherMode, com.feilong.security.symmetric.CipherPadding);
  public com.feilong.security.symmetric.SymmetricEncryption(com.feilong.security.symmetric.SymmetricType, java.lang.String, com.feilong.security.symmetric.builder.KeyBuilder, com.feilong.security.symmetric.CipherMode, com.feilong.security.symmetric.CipherPadding);
  public java.lang.String encryptBase64(java.lang.String);
  public java.lang.String encryptBase64(java.lang.String, java.lang.String);
  public java.lang.String decryptBase64(java.lang.String);
  public java.lang.String decryptBase64(java.lang.String, java.lang.String);
  public java.lang.String encryptHex(java.lang.String);
  public java.lang.String encryptHex(java.lang.String, java.lang.String);
  public java.lang.String decryptHex(java.lang.String);
  public java.lang.String decryptHex(java.lang.String, java.lang.String);
  public void setKeyString(java.lang.String);
  public void setKeyBuilder(com.feilong.security.symmetric.builder.KeyBuilder);
  public void setCipherMode(com.feilong.security.symmetric.CipherMode);
  public void setCipherPadding(com.feilong.security.symmetric.CipherPadding);
  public void setSymmetricType(com.feilong.security.symmetric.SymmetricType);
}
```

## `com.feilong.security.symmetric.SymmetricType`

```java
public final class com.feilong.security.symmetric.SymmetricType extends java.lang.Enum<com.feilong.security.symmetric.SymmetricType> {
  public static com.feilong.security.symmetric.SymmetricType[] values();
  public static com.feilong.security.symmetric.SymmetricType valueOf(java.lang.String);
  public java.lang.String getAlgorithm();
}
```
