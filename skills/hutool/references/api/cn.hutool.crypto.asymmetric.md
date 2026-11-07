# cn.hutool.crypto.asymmetric

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.crypto.asymmetric.AbstractAsymmetricCrypto`

```java
public abstract class cn.hutool.crypto.asymmetric.AbstractAsymmetricCrypto<T extends cn.hutool.crypto.asymmetric.AbstractAsymmetricCrypto<T>> extends cn.hutool.crypto.asymmetric.BaseAsymmetric<T> implements cn.hutool.crypto.asymmetric.AsymmetricEncryptor, cn.hutool.crypto.asymmetric.AsymmetricDecryptor {
  public cn.hutool.crypto.asymmetric.AbstractAsymmetricCrypto(java.lang.String, java.security.PrivateKey, java.security.PublicKey);
}
```

## `cn.hutool.crypto.asymmetric.AsymmetricAlgorithm`

```java
public final class cn.hutool.crypto.asymmetric.AsymmetricAlgorithm extends java.lang.Enum<cn.hutool.crypto.asymmetric.AsymmetricAlgorithm> {
  public static cn.hutool.crypto.asymmetric.AsymmetricAlgorithm[] values();
  public static cn.hutool.crypto.asymmetric.AsymmetricAlgorithm valueOf(java.lang.String);
  public java.lang.String getValue();
}
```

## `cn.hutool.crypto.asymmetric.AsymmetricCrypto`

```java
public class cn.hutool.crypto.asymmetric.AsymmetricCrypto extends cn.hutool.crypto.asymmetric.AbstractAsymmetricCrypto<cn.hutool.crypto.asymmetric.AsymmetricCrypto> {
  public cn.hutool.crypto.asymmetric.AsymmetricCrypto(cn.hutool.crypto.asymmetric.AsymmetricAlgorithm);
  public cn.hutool.crypto.asymmetric.AsymmetricCrypto(java.lang.String);
  public cn.hutool.crypto.asymmetric.AsymmetricCrypto(cn.hutool.crypto.asymmetric.AsymmetricAlgorithm, java.lang.String, java.lang.String);
  public cn.hutool.crypto.asymmetric.AsymmetricCrypto(cn.hutool.crypto.asymmetric.AsymmetricAlgorithm, byte[], byte[]);
  public cn.hutool.crypto.asymmetric.AsymmetricCrypto(cn.hutool.crypto.asymmetric.AsymmetricAlgorithm, java.security.PrivateKey, java.security.PublicKey);
  public cn.hutool.crypto.asymmetric.AsymmetricCrypto(java.lang.String, java.lang.String, java.lang.String);
  public cn.hutool.crypto.asymmetric.AsymmetricCrypto(java.lang.String, byte[], byte[]);
  public cn.hutool.crypto.asymmetric.AsymmetricCrypto(java.lang.String, java.security.PrivateKey, java.security.PublicKey);
  public int getEncryptBlockSize();
  public void setEncryptBlockSize(int);
  public int getDecryptBlockSize();
  public void setDecryptBlockSize(int);
  public java.security.spec.AlgorithmParameterSpec getAlgorithmParameterSpec();
  public void setAlgorithmParameterSpec(java.security.spec.AlgorithmParameterSpec);
  public cn.hutool.crypto.asymmetric.AsymmetricCrypto setRandom(java.security.SecureRandom);
  public cn.hutool.crypto.asymmetric.AsymmetricCrypto init(java.lang.String, java.security.PrivateKey, java.security.PublicKey);
  public byte[] encrypt(byte[], cn.hutool.crypto.asymmetric.KeyType);
  public byte[] decrypt(byte[], cn.hutool.crypto.asymmetric.KeyType);
  public javax.crypto.Cipher getCipher();
  public cn.hutool.crypto.asymmetric.BaseAsymmetric init(java.lang.String, java.security.PrivateKey, java.security.PublicKey);
}
```

## `cn.hutool.crypto.asymmetric.AsymmetricDecryptor`

```java
public interface cn.hutool.crypto.asymmetric.AsymmetricDecryptor {
  public abstract byte[] decrypt(byte[], cn.hutool.crypto.asymmetric.KeyType);
  public default byte[] decrypt(java.io.InputStream, cn.hutool.crypto.asymmetric.KeyType) throws cn.hutool.core.io.IORuntimeException;
  public default byte[] decrypt(java.lang.String, cn.hutool.crypto.asymmetric.KeyType);
  public default java.lang.String decryptStr(java.lang.String, cn.hutool.crypto.asymmetric.KeyType, java.nio.charset.Charset);
  public default java.lang.String decryptStr(java.lang.String, cn.hutool.crypto.asymmetric.KeyType);
  public default byte[] decryptFromBcd(java.lang.String, cn.hutool.crypto.asymmetric.KeyType);
  public default byte[] decryptFromBcd(java.lang.String, cn.hutool.crypto.asymmetric.KeyType, java.nio.charset.Charset);
  public default java.lang.String decryptStrFromBcd(java.lang.String, cn.hutool.crypto.asymmetric.KeyType, java.nio.charset.Charset);
  public default java.lang.String decryptStrFromBcd(java.lang.String, cn.hutool.crypto.asymmetric.KeyType);
}
```

## `cn.hutool.crypto.asymmetric.AsymmetricEncryptor`

```java
public interface cn.hutool.crypto.asymmetric.AsymmetricEncryptor {
  public abstract byte[] encrypt(byte[], cn.hutool.crypto.asymmetric.KeyType);
  public default java.lang.String encryptHex(byte[], cn.hutool.crypto.asymmetric.KeyType);
  public default java.lang.String encryptBase64(byte[], cn.hutool.crypto.asymmetric.KeyType);
  public default byte[] encrypt(java.lang.String, java.lang.String, cn.hutool.crypto.asymmetric.KeyType);
  public default byte[] encrypt(java.lang.String, java.nio.charset.Charset, cn.hutool.crypto.asymmetric.KeyType);
  public default byte[] encrypt(java.lang.String, cn.hutool.crypto.asymmetric.KeyType);
  public default java.lang.String encryptHex(java.lang.String, cn.hutool.crypto.asymmetric.KeyType);
  public default java.lang.String encryptHex(java.lang.String, java.nio.charset.Charset, cn.hutool.crypto.asymmetric.KeyType);
  public default java.lang.String encryptBase64(java.lang.String, cn.hutool.crypto.asymmetric.KeyType);
  public default java.lang.String encryptBase64(java.lang.String, java.nio.charset.Charset, cn.hutool.crypto.asymmetric.KeyType);
  public default byte[] encrypt(java.io.InputStream, cn.hutool.crypto.asymmetric.KeyType) throws cn.hutool.core.io.IORuntimeException;
  public default java.lang.String encryptHex(java.io.InputStream, cn.hutool.crypto.asymmetric.KeyType);
  public default java.lang.String encryptBase64(java.io.InputStream, cn.hutool.crypto.asymmetric.KeyType);
  public default java.lang.String encryptBcd(java.lang.String, cn.hutool.crypto.asymmetric.KeyType);
  public default java.lang.String encryptBcd(java.lang.String, cn.hutool.crypto.asymmetric.KeyType, java.nio.charset.Charset);
}
```

## `cn.hutool.crypto.asymmetric.BaseAsymmetric`

```java
public class cn.hutool.crypto.asymmetric.BaseAsymmetric<T extends cn.hutool.crypto.asymmetric.BaseAsymmetric<T>> implements java.io.Serializable {
  public cn.hutool.crypto.asymmetric.BaseAsymmetric(java.lang.String, java.security.PrivateKey, java.security.PublicKey);
  public T initKeys();
  public java.security.PublicKey getPublicKey();
  public java.lang.String getPublicKeyBase64();
  public T setPublicKey(java.security.PublicKey);
  public java.security.PrivateKey getPrivateKey();
  public java.lang.String getPrivateKeyBase64();
  public T setPrivateKey(java.security.PrivateKey);
  public T setKey(java.security.Key);
}
```

## `cn.hutool.crypto.asymmetric.ECIES`

```java
public class cn.hutool.crypto.asymmetric.ECIES extends cn.hutool.crypto.asymmetric.AsymmetricCrypto {
  public cn.hutool.crypto.asymmetric.ECIES();
  public cn.hutool.crypto.asymmetric.ECIES(java.lang.String);
  public cn.hutool.crypto.asymmetric.ECIES(java.lang.String, java.lang.String);
  public cn.hutool.crypto.asymmetric.ECIES(java.lang.String, java.lang.String, java.lang.String);
  public cn.hutool.crypto.asymmetric.ECIES(byte[], byte[]);
  public cn.hutool.crypto.asymmetric.ECIES(java.security.PrivateKey, java.security.PublicKey);
  public cn.hutool.crypto.asymmetric.ECIES(java.lang.String, java.security.PrivateKey, java.security.PublicKey);
}
```

## `cn.hutool.crypto.asymmetric.KeyType`

```java
public final class cn.hutool.crypto.asymmetric.KeyType extends java.lang.Enum<cn.hutool.crypto.asymmetric.KeyType> {
  public static cn.hutool.crypto.asymmetric.KeyType[] values();
  public static cn.hutool.crypto.asymmetric.KeyType valueOf(java.lang.String);
  public int getValue();
}
```

## `cn.hutool.crypto.asymmetric.RSA`

```java
public class cn.hutool.crypto.asymmetric.RSA extends cn.hutool.crypto.asymmetric.AsymmetricCrypto {
  public static java.security.PrivateKey generatePrivateKey(java.math.BigInteger, java.math.BigInteger);
  public static java.security.PublicKey generatePublicKey(java.math.BigInteger, java.math.BigInteger);
  public cn.hutool.crypto.asymmetric.RSA();
  public cn.hutool.crypto.asymmetric.RSA(java.lang.String);
  public cn.hutool.crypto.asymmetric.RSA(java.lang.String, java.lang.String);
  public cn.hutool.crypto.asymmetric.RSA(java.lang.String, java.lang.String, java.lang.String);
  public cn.hutool.crypto.asymmetric.RSA(byte[], byte[]);
  public cn.hutool.crypto.asymmetric.RSA(java.math.BigInteger, java.math.BigInteger, java.math.BigInteger);
  public cn.hutool.crypto.asymmetric.RSA(java.security.PrivateKey, java.security.PublicKey);
  public cn.hutool.crypto.asymmetric.RSA(java.lang.String, java.security.PrivateKey, java.security.PublicKey);
  public byte[] encrypt(byte[], cn.hutool.crypto.asymmetric.KeyType);
  public byte[] decrypt(byte[], cn.hutool.crypto.asymmetric.KeyType);
}
```

## `cn.hutool.crypto.asymmetric.SM2`

```java
public class cn.hutool.crypto.asymmetric.SM2 extends cn.hutool.crypto.asymmetric.AbstractAsymmetricCrypto<cn.hutool.crypto.asymmetric.SM2> {
  public cn.hutool.crypto.asymmetric.SM2();
  public cn.hutool.crypto.asymmetric.SM2(java.lang.String, java.lang.String);
  public cn.hutool.crypto.asymmetric.SM2(byte[], byte[]);
  public cn.hutool.crypto.asymmetric.SM2(java.security.PrivateKey, java.security.PublicKey);
  public cn.hutool.crypto.asymmetric.SM2(java.lang.String, java.lang.String, java.lang.String);
  public cn.hutool.crypto.asymmetric.SM2(byte[], byte[], byte[]);
  public cn.hutool.crypto.asymmetric.SM2(org.bouncycastle.crypto.params.ECPrivateKeyParameters, org.bouncycastle.crypto.params.ECPublicKeyParameters);
  public cn.hutool.crypto.asymmetric.SM2 init();
  public cn.hutool.crypto.asymmetric.SM2 initKeys();
  public byte[] encrypt(byte[]) throws cn.hutool.crypto.CryptoException;
  public byte[] encrypt(byte[], cn.hutool.crypto.asymmetric.KeyType) throws cn.hutool.crypto.CryptoException;
  public byte[] encrypt(byte[], org.bouncycastle.crypto.CipherParameters) throws cn.hutool.crypto.CryptoException;
  public byte[] decrypt(byte[]) throws cn.hutool.crypto.CryptoException;
  public byte[] decrypt(byte[], cn.hutool.crypto.asymmetric.KeyType) throws cn.hutool.crypto.CryptoException;
  public byte[] decrypt(byte[], org.bouncycastle.crypto.CipherParameters) throws cn.hutool.crypto.CryptoException;
  public java.lang.String signHexFromHex(java.lang.String);
  public java.lang.String signHex(java.lang.String);
  public java.lang.String signHexFromHex(java.lang.String, java.lang.String);
  public java.lang.String signHex(java.lang.String, java.lang.String);
  public byte[] sign(byte[]);
  public byte[] sign(byte[], byte[]);
  public boolean verifyHex(java.lang.String, java.lang.String);
  public boolean verify(byte[], byte[]);
  public boolean verifyHex(java.lang.String, java.lang.String, java.lang.String);
  public boolean verify(byte[], byte[], byte[]);
  public cn.hutool.crypto.asymmetric.SM2 setPrivateKey(java.security.PrivateKey);
  public cn.hutool.crypto.asymmetric.SM2 setPrivateKeyParams(org.bouncycastle.crypto.params.ECPrivateKeyParameters);
  public cn.hutool.crypto.asymmetric.SM2 setPublicKey(java.security.PublicKey);
  public cn.hutool.crypto.asymmetric.SM2 setPublicKeyParams(org.bouncycastle.crypto.params.ECPublicKeyParameters);
  public cn.hutool.crypto.asymmetric.SM2 usePlainEncoding();
  public cn.hutool.crypto.asymmetric.SM2 setEncoding(org.bouncycastle.crypto.signers.DSAEncoding);
  public cn.hutool.crypto.asymmetric.SM2 setDigest(org.bouncycastle.crypto.Digest);
  public cn.hutool.crypto.asymmetric.SM2 setMode(org.bouncycastle.crypto.engines.SM2Engine$Mode);
  public byte[] getD();
  public java.lang.String getDHex();
  public java.math.BigInteger getDBigInteger();
  public byte[] getQ(boolean);
  public cn.hutool.crypto.asymmetric.BaseAsymmetric setPrivateKey(java.security.PrivateKey);
  public cn.hutool.crypto.asymmetric.BaseAsymmetric setPublicKey(java.security.PublicKey);
  public cn.hutool.crypto.asymmetric.BaseAsymmetric initKeys();
}
```

## `cn.hutool.crypto.asymmetric.Sign`

```java
public class cn.hutool.crypto.asymmetric.Sign extends cn.hutool.crypto.asymmetric.BaseAsymmetric<cn.hutool.crypto.asymmetric.Sign> {
  public cn.hutool.crypto.asymmetric.Sign(cn.hutool.crypto.asymmetric.SignAlgorithm);
  public cn.hutool.crypto.asymmetric.Sign(java.lang.String);
  public cn.hutool.crypto.asymmetric.Sign(cn.hutool.crypto.asymmetric.SignAlgorithm, java.lang.String, java.lang.String);
  public cn.hutool.crypto.asymmetric.Sign(cn.hutool.crypto.asymmetric.SignAlgorithm, byte[], byte[]);
  public cn.hutool.crypto.asymmetric.Sign(cn.hutool.crypto.asymmetric.SignAlgorithm, java.security.KeyPair);
  public cn.hutool.crypto.asymmetric.Sign(cn.hutool.crypto.asymmetric.SignAlgorithm, java.security.PrivateKey, java.security.PublicKey);
  public cn.hutool.crypto.asymmetric.Sign(java.lang.String, java.lang.String, java.lang.String);
  public cn.hutool.crypto.asymmetric.Sign(java.lang.String, byte[], byte[]);
  public cn.hutool.crypto.asymmetric.Sign(java.lang.String, java.security.KeyPair);
  public cn.hutool.crypto.asymmetric.Sign(java.lang.String, java.security.PrivateKey, java.security.PublicKey);
  public cn.hutool.crypto.asymmetric.Sign init(java.lang.String, java.security.PrivateKey, java.security.PublicKey);
  public cn.hutool.crypto.asymmetric.Sign setParameter(java.security.spec.AlgorithmParameterSpec);
  public byte[] sign(java.lang.String, java.nio.charset.Charset);
  public byte[] sign(java.lang.String);
  public java.lang.String signHex(java.lang.String, java.nio.charset.Charset);
  public java.lang.String signHex(java.lang.String);
  public byte[] sign(byte[]);
  public java.lang.String signHex(byte[]);
  public java.lang.String signHex(java.io.InputStream);
  public byte[] sign(java.io.InputStream);
  public java.lang.String digestHex(java.io.InputStream, int);
  public byte[] sign(java.io.InputStream, int);
  public boolean verify(byte[], byte[]);
  public java.security.Signature getSignature();
  public cn.hutool.crypto.asymmetric.Sign setSignature(java.security.Signature);
  public cn.hutool.crypto.asymmetric.Sign setCertificate(java.security.cert.Certificate);
  public cn.hutool.crypto.asymmetric.BaseAsymmetric init(java.lang.String, java.security.PrivateKey, java.security.PublicKey);
}
```

## `cn.hutool.crypto.asymmetric.SignAlgorithm`

```java
public final class cn.hutool.crypto.asymmetric.SignAlgorithm extends java.lang.Enum<cn.hutool.crypto.asymmetric.SignAlgorithm> {
  public static cn.hutool.crypto.asymmetric.SignAlgorithm[] values();
  public static cn.hutool.crypto.asymmetric.SignAlgorithm valueOf(java.lang.String);
  public java.lang.String getValue();
}
```
