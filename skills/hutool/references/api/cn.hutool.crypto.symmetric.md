# cn.hutool.crypto.symmetric

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.crypto.symmetric.AES`

```java
public class cn.hutool.crypto.symmetric.AES extends cn.hutool.crypto.symmetric.SymmetricCrypto {
  public cn.hutool.crypto.symmetric.AES();
  public cn.hutool.crypto.symmetric.AES(byte[]);
  public cn.hutool.crypto.symmetric.AES(javax.crypto.SecretKey);
  public cn.hutool.crypto.symmetric.AES(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding);
  public cn.hutool.crypto.symmetric.AES(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, byte[]);
  public cn.hutool.crypto.symmetric.AES(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, byte[], byte[]);
  public cn.hutool.crypto.symmetric.AES(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, javax.crypto.SecretKey);
  public cn.hutool.crypto.symmetric.AES(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, javax.crypto.SecretKey, byte[]);
  public cn.hutool.crypto.symmetric.AES(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, javax.crypto.SecretKey, java.security.spec.AlgorithmParameterSpec);
  public cn.hutool.crypto.symmetric.AES(java.lang.String, java.lang.String);
  public cn.hutool.crypto.symmetric.AES(java.lang.String, java.lang.String, byte[]);
  public cn.hutool.crypto.symmetric.AES(java.lang.String, java.lang.String, byte[], byte[]);
  public cn.hutool.crypto.symmetric.AES(java.lang.String, java.lang.String, javax.crypto.SecretKey);
  public cn.hutool.crypto.symmetric.AES(java.lang.String, java.lang.String, javax.crypto.SecretKey, java.security.spec.AlgorithmParameterSpec);
}
```

## `cn.hutool.crypto.symmetric.ChaCha20`

```java
public class cn.hutool.crypto.symmetric.ChaCha20 extends cn.hutool.crypto.symmetric.SymmetricCrypto {
  public cn.hutool.crypto.symmetric.ChaCha20(byte[], byte[]);
}
```

## `cn.hutool.crypto.symmetric.DES`

```java
public class cn.hutool.crypto.symmetric.DES extends cn.hutool.crypto.symmetric.SymmetricCrypto {
  public cn.hutool.crypto.symmetric.DES();
  public cn.hutool.crypto.symmetric.DES(byte[]);
  public cn.hutool.crypto.symmetric.DES(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding);
  public cn.hutool.crypto.symmetric.DES(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, byte[]);
  public cn.hutool.crypto.symmetric.DES(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, byte[], byte[]);
  public cn.hutool.crypto.symmetric.DES(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, javax.crypto.SecretKey);
  public cn.hutool.crypto.symmetric.DES(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, javax.crypto.SecretKey, javax.crypto.spec.IvParameterSpec);
  public cn.hutool.crypto.symmetric.DES(java.lang.String, java.lang.String);
  public cn.hutool.crypto.symmetric.DES(java.lang.String, java.lang.String, byte[]);
  public cn.hutool.crypto.symmetric.DES(java.lang.String, java.lang.String, byte[], byte[]);
  public cn.hutool.crypto.symmetric.DES(java.lang.String, java.lang.String, javax.crypto.SecretKey);
  public cn.hutool.crypto.symmetric.DES(java.lang.String, java.lang.String, javax.crypto.SecretKey, javax.crypto.spec.IvParameterSpec);
}
```

## `cn.hutool.crypto.symmetric.DESede`

```java
public class cn.hutool.crypto.symmetric.DESede extends cn.hutool.crypto.symmetric.SymmetricCrypto {
  public cn.hutool.crypto.symmetric.DESede();
  public cn.hutool.crypto.symmetric.DESede(byte[]);
  public cn.hutool.crypto.symmetric.DESede(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding);
  public cn.hutool.crypto.symmetric.DESede(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, byte[]);
  public cn.hutool.crypto.symmetric.DESede(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, byte[], byte[]);
  public cn.hutool.crypto.symmetric.DESede(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, javax.crypto.SecretKey);
  public cn.hutool.crypto.symmetric.DESede(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, javax.crypto.SecretKey, javax.crypto.spec.IvParameterSpec);
  public cn.hutool.crypto.symmetric.DESede(java.lang.String, java.lang.String);
  public cn.hutool.crypto.symmetric.DESede(java.lang.String, java.lang.String, byte[]);
  public cn.hutool.crypto.symmetric.DESede(java.lang.String, java.lang.String, byte[], byte[]);
  public cn.hutool.crypto.symmetric.DESede(java.lang.String, java.lang.String, javax.crypto.SecretKey);
  public cn.hutool.crypto.symmetric.DESede(java.lang.String, java.lang.String, javax.crypto.SecretKey, javax.crypto.spec.IvParameterSpec);
}
```

## `cn.hutool.crypto.symmetric.PBKDF2`

```java
public class cn.hutool.crypto.symmetric.PBKDF2 {
  public cn.hutool.crypto.symmetric.PBKDF2();
  public cn.hutool.crypto.symmetric.PBKDF2(java.lang.String, int, int);
  public byte[] encrypt(char[], byte[]);
  public java.lang.String encryptHex(char[], byte[]);
}
```

## `cn.hutool.crypto.symmetric.RC4`

```java
public class cn.hutool.crypto.symmetric.RC4 implements java.io.Serializable {
  public cn.hutool.crypto.symmetric.RC4(java.lang.String) throws cn.hutool.crypto.CryptoException;
  public byte[] encrypt(java.lang.String, java.nio.charset.Charset) throws cn.hutool.crypto.CryptoException;
  public byte[] encrypt(java.lang.String) throws cn.hutool.crypto.CryptoException;
  public java.lang.String encryptHex(byte[]);
  public java.lang.String encryptBase64(byte[]);
  public java.lang.String encryptHex(java.lang.String, java.nio.charset.Charset);
  public java.lang.String encryptHex(java.lang.String);
  public java.lang.String encryptBase64(java.lang.String, java.nio.charset.Charset);
  public java.lang.String encryptBase64(java.lang.String);
  public java.lang.String decrypt(byte[], java.nio.charset.Charset) throws cn.hutool.crypto.CryptoException;
  public java.lang.String decrypt(byte[]) throws cn.hutool.crypto.CryptoException;
  public java.lang.String decrypt(java.lang.String);
  public java.lang.String decrypt(java.lang.String, java.nio.charset.Charset);
  public byte[] crypt(byte[]);
  public void setKey(java.lang.String) throws cn.hutool.crypto.CryptoException;
}
```

## `cn.hutool.crypto.symmetric.SM4`

```java
public class cn.hutool.crypto.symmetric.SM4 extends cn.hutool.crypto.symmetric.SymmetricCrypto {
  public cn.hutool.crypto.symmetric.SM4();
  public cn.hutool.crypto.symmetric.SM4(byte[]);
  public cn.hutool.crypto.symmetric.SM4(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding);
  public cn.hutool.crypto.symmetric.SM4(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, byte[]);
  public cn.hutool.crypto.symmetric.SM4(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, byte[], byte[]);
  public cn.hutool.crypto.symmetric.SM4(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, javax.crypto.SecretKey);
  public cn.hutool.crypto.symmetric.SM4(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, javax.crypto.SecretKey, byte[]);
  public cn.hutool.crypto.symmetric.SM4(cn.hutool.crypto.Mode, cn.hutool.crypto.Padding, javax.crypto.SecretKey, javax.crypto.spec.IvParameterSpec);
  public cn.hutool.crypto.symmetric.SM4(java.lang.String, java.lang.String);
  public cn.hutool.crypto.symmetric.SM4(java.lang.String, java.lang.String, byte[]);
  public cn.hutool.crypto.symmetric.SM4(java.lang.String, java.lang.String, byte[], byte[]);
  public cn.hutool.crypto.symmetric.SM4(java.lang.String, java.lang.String, javax.crypto.SecretKey);
  public cn.hutool.crypto.symmetric.SM4(java.lang.String, java.lang.String, javax.crypto.SecretKey, javax.crypto.spec.IvParameterSpec);
}
```

## `cn.hutool.crypto.symmetric.SymmetricAlgorithm`

```java
public final class cn.hutool.crypto.symmetric.SymmetricAlgorithm extends java.lang.Enum<cn.hutool.crypto.symmetric.SymmetricAlgorithm> {
  public static cn.hutool.crypto.symmetric.SymmetricAlgorithm[] values();
  public static cn.hutool.crypto.symmetric.SymmetricAlgorithm valueOf(java.lang.String);
  public java.lang.String getValue();
}
```

## `cn.hutool.crypto.symmetric.SymmetricCrypto`

```java
public class cn.hutool.crypto.symmetric.SymmetricCrypto implements cn.hutool.crypto.symmetric.SymmetricEncryptor,cn.hutool.crypto.symmetric.SymmetricDecryptor,java.io.Serializable {
  public cn.hutool.crypto.symmetric.SymmetricCrypto(cn.hutool.crypto.symmetric.SymmetricAlgorithm);
  public cn.hutool.crypto.symmetric.SymmetricCrypto(java.lang.String);
  public cn.hutool.crypto.symmetric.SymmetricCrypto(cn.hutool.crypto.symmetric.SymmetricAlgorithm, byte[]);
  public cn.hutool.crypto.symmetric.SymmetricCrypto(cn.hutool.crypto.symmetric.SymmetricAlgorithm, javax.crypto.SecretKey);
  public cn.hutool.crypto.symmetric.SymmetricCrypto(java.lang.String, byte[]);
  public cn.hutool.crypto.symmetric.SymmetricCrypto(java.lang.String, javax.crypto.SecretKey);
  public cn.hutool.crypto.symmetric.SymmetricCrypto(java.lang.String, javax.crypto.SecretKey, java.security.spec.AlgorithmParameterSpec);
  public cn.hutool.crypto.symmetric.SymmetricCrypto init(java.lang.String, javax.crypto.SecretKey);
  public javax.crypto.SecretKey getSecretKey();
  public javax.crypto.Cipher getCipher();
  public cn.hutool.crypto.symmetric.SymmetricCrypto setIv(byte[]);
  public cn.hutool.crypto.symmetric.SymmetricCrypto setIv(javax.crypto.spec.IvParameterSpec);
  public cn.hutool.crypto.symmetric.SymmetricCrypto setParams(java.security.spec.AlgorithmParameterSpec);
  public cn.hutool.crypto.symmetric.SymmetricCrypto setRandom(java.security.SecureRandom);
  public cn.hutool.crypto.symmetric.SymmetricCrypto setMode(cn.hutool.crypto.CipherMode);
  public byte[] update(byte[]);
  public java.lang.String updateHex(byte[]);
  public byte[] encrypt(byte[]);
  public void encrypt(java.io.InputStream, java.io.OutputStream, boolean) throws cn.hutool.core.io.IORuntimeException;
  public byte[] decrypt(byte[]);
  public void decrypt(java.io.InputStream, java.io.OutputStream, boolean) throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.crypto.symmetric.SymmetricDecryptor`

```java
public interface cn.hutool.crypto.symmetric.SymmetricDecryptor {
  public abstract byte[] decrypt(byte[]);
  public abstract void decrypt(java.io.InputStream, java.io.OutputStream, boolean);
  public default java.lang.String decryptStr(byte[], java.nio.charset.Charset);
  public default java.lang.String decryptStr(byte[]);
  public default byte[] decrypt(java.lang.String);
  public default java.lang.String decryptStr(java.lang.String, java.nio.charset.Charset);
  public default java.lang.String decryptStr(java.lang.String);
  public default byte[] decrypt(java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public default java.lang.String decryptStr(java.io.InputStream, java.nio.charset.Charset);
  public default java.lang.String decryptStr(java.io.InputStream);
}
```

## `cn.hutool.crypto.symmetric.SymmetricEncryptor`

```java
public interface cn.hutool.crypto.symmetric.SymmetricEncryptor {
  public abstract byte[] encrypt(byte[]);
  public abstract void encrypt(java.io.InputStream, java.io.OutputStream, boolean);
  public default java.lang.String encryptHex(byte[]);
  public default java.lang.String encryptBase64(byte[]);
  public default byte[] encrypt(java.lang.String, java.lang.String);
  public default byte[] encrypt(java.lang.String, java.nio.charset.Charset);
  public default java.lang.String encryptHex(java.lang.String, java.lang.String);
  public default java.lang.String encryptHex(java.lang.String, java.nio.charset.Charset);
  public default java.lang.String encryptBase64(java.lang.String, java.lang.String);
  public default java.lang.String encryptBase64(java.lang.String, java.nio.charset.Charset);
  public default byte[] encrypt(java.lang.String);
  public default java.lang.String encryptHex(java.lang.String);
  public default java.lang.String encryptBase64(java.lang.String);
  public default byte[] encrypt(java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public default java.lang.String encryptHex(java.io.InputStream);
  public default java.lang.String encryptBase64(java.io.InputStream);
}
```

## `cn.hutool.crypto.symmetric.Vigenere`

```java
public class cn.hutool.crypto.symmetric.Vigenere {
  public cn.hutool.crypto.symmetric.Vigenere();
  public static java.lang.String encrypt(java.lang.CharSequence, java.lang.CharSequence);
  public static java.lang.String decrypt(java.lang.CharSequence, java.lang.CharSequence);
}
```

## `cn.hutool.crypto.symmetric.XXTEA`

```java
public class cn.hutool.crypto.symmetric.XXTEA implements cn.hutool.crypto.symmetric.SymmetricEncryptor,cn.hutool.crypto.symmetric.SymmetricDecryptor,java.io.Serializable {
  public cn.hutool.crypto.symmetric.XXTEA(byte[]);
  public byte[] encrypt(byte[]);
  public void encrypt(java.io.InputStream, java.io.OutputStream, boolean);
  public byte[] decrypt(byte[]);
  public void decrypt(java.io.InputStream, java.io.OutputStream, boolean);
}
```

## `cn.hutool.crypto.symmetric.ZUC`

```java
public class cn.hutool.crypto.symmetric.ZUC extends cn.hutool.crypto.symmetric.SymmetricCrypto {
  public static byte[] generateKey(cn.hutool.crypto.symmetric.ZUC$ZUCAlgorithm);
  public cn.hutool.crypto.symmetric.ZUC(cn.hutool.crypto.symmetric.ZUC$ZUCAlgorithm, byte[], byte[]);
}
```

## `cn.hutool.crypto.symmetric.ZUC$ZUCAlgorithm`

```java
public final class cn.hutool.crypto.symmetric.ZUC$ZUCAlgorithm extends java.lang.Enum<cn.hutool.crypto.symmetric.ZUC$ZUCAlgorithm> {
  public static cn.hutool.crypto.symmetric.ZUC$ZUCAlgorithm[] values();
  public static cn.hutool.crypto.symmetric.ZUC$ZUCAlgorithm valueOf(java.lang.String);
  public java.lang.String getValue();
}
```
