# cn.hutool.crypto

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.crypto.ASN1Util`

```java
public class cn.hutool.crypto.ASN1Util {
  public cn.hutool.crypto.ASN1Util();
  public static byte[] encodeDer(org.bouncycastle.asn1.ASN1Encodable...);
  public static byte[] encode(java.lang.String, org.bouncycastle.asn1.ASN1Encodable...);
  public static void encodeTo(java.lang.String, java.io.OutputStream, org.bouncycastle.asn1.ASN1Encodable...);
  public static org.bouncycastle.asn1.ASN1Object decode(java.io.InputStream);
  public static java.lang.String getDumpStr(java.io.InputStream);
}
```

## `cn.hutool.crypto.BCUtil`

```java
public class cn.hutool.crypto.BCUtil {
  public cn.hutool.crypto.BCUtil();
  public static byte[] encodeECPrivateKey(java.security.PrivateKey);
  public static java.security.PrivateKey decodeECPrivateKey(byte[], java.lang.String);
  public static byte[] encodeECPublicKey(java.security.PublicKey);
  public static byte[] encodeECPublicKey(java.security.PublicKey, boolean);
  public static java.security.PublicKey decodeECPoint(java.lang.String, java.lang.String);
  public static java.security.PublicKey decodeECPoint(byte[], java.lang.String);
  public static org.bouncycastle.crypto.params.ECDomainParameters toDomainParams(org.bouncycastle.jce.spec.ECParameterSpec);
  public static org.bouncycastle.crypto.params.ECDomainParameters toDomainParams(java.lang.String);
  public static org.bouncycastle.crypto.params.ECDomainParameters toDomainParams(org.bouncycastle.asn1.x9.X9ECParameters);
  public static org.bouncycastle.crypto.params.AsymmetricKeyParameter toParams(java.security.Key);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters toSm2Params(java.lang.String);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters toParams(java.lang.String, org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters toSm2Params(byte[]);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters toParams(byte[], org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters toSm2Params(java.math.BigInteger);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters toParams(java.math.BigInteger, org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toParams(java.math.BigInteger, java.math.BigInteger, org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toSm2Params(java.lang.String, java.lang.String);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toParams(java.lang.String, java.lang.String, org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toSm2Params(byte[], byte[]);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toParams(byte[], byte[], org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toParams(java.security.PublicKey);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters toParams(java.security.PrivateKey);
  public static java.security.PrivateKey readPemPrivateKey(java.io.InputStream);
  public static java.security.PublicKey readPemPublicKey(java.io.InputStream);
  public static byte[] toPkcs1(java.security.PrivateKey);
  public static byte[] toPkcs1(java.security.PublicKey);
}
```

## `cn.hutool.crypto.CipherMode`

```java
public final class cn.hutool.crypto.CipherMode extends java.lang.Enum<cn.hutool.crypto.CipherMode> {
  public static cn.hutool.crypto.CipherMode[] values();
  public static cn.hutool.crypto.CipherMode valueOf(java.lang.String);
  public int getValue();
}
```

## `cn.hutool.crypto.CipherWrapper`

```java
public class cn.hutool.crypto.CipherWrapper {
  public cn.hutool.crypto.CipherWrapper(java.lang.String);
  public cn.hutool.crypto.CipherWrapper(javax.crypto.Cipher);
  public java.security.spec.AlgorithmParameterSpec getParams();
  public cn.hutool.crypto.CipherWrapper setParams(java.security.spec.AlgorithmParameterSpec);
  public cn.hutool.crypto.CipherWrapper setRandom(java.security.SecureRandom);
  public javax.crypto.Cipher getCipher();
  public cn.hutool.crypto.CipherWrapper initMode(int, java.security.Key) throws java.security.InvalidKeyException, java.security.InvalidAlgorithmParameterException;
}
```

## `cn.hutool.crypto.CryptoException`

```java
public class cn.hutool.crypto.CryptoException extends java.lang.RuntimeException {
  public cn.hutool.crypto.CryptoException(java.lang.Throwable);
  public cn.hutool.crypto.CryptoException(java.lang.String);
  public cn.hutool.crypto.CryptoException(java.lang.String, java.lang.Object...);
  public cn.hutool.crypto.CryptoException(java.lang.String, java.lang.Throwable);
  public cn.hutool.crypto.CryptoException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.crypto.CryptoException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.crypto.ECKeyUtil`

```java
public class cn.hutool.crypto.ECKeyUtil {
  public cn.hutool.crypto.ECKeyUtil();
  public static org.bouncycastle.crypto.params.AsymmetricKeyParameter toParams(java.security.Key);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters getPublicParams(org.bouncycastle.crypto.params.ECPrivateKeyParameters);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toSm2PublicParams(byte[]);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toSm2PublicParams(java.lang.String);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toSm2PublicParams(java.lang.String, java.lang.String);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toSm2PublicParams(byte[], byte[]);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toPublicParams(java.lang.String, java.lang.String, org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toPublicParams(byte[], byte[], org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toPublicParams(java.math.BigInteger, java.math.BigInteger, org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toPublicParams(java.lang.String, org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toPublicParams(byte[], org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toPublicParams(org.bouncycastle.math.ec.ECPoint, org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters toPublicParams(java.security.PublicKey);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters toSm2PrivateParams(java.lang.String);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters toSm2PrivateParams(byte[]);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters toSm2PrivateParams(java.math.BigInteger);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters toPrivateParams(java.lang.String, org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters toPrivateParams(byte[], org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters toPrivateParams(java.math.BigInteger, org.bouncycastle.crypto.params.ECDomainParameters);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters toPrivateParams(java.security.PrivateKey);
  public static java.security.PrivateKey toSm2PrivateKey(org.bouncycastle.asn1.sec.ECPrivateKey);
  public static java.security.spec.KeySpec createOpenSSHPrivateKeySpec(byte[]);
  public static java.security.spec.KeySpec createOpenSSHPublicKeySpec(byte[]);
  public static org.bouncycastle.crypto.params.ECPrivateKeyParameters decodePrivateKeyParams(byte[]);
  public static org.bouncycastle.crypto.params.ECPublicKeyParameters decodePublicKeyParams(byte[]);
}
```

## `cn.hutool.crypto.GlobalBouncyCastleProvider`

```java
public final class cn.hutool.crypto.GlobalBouncyCastleProvider extends java.lang.Enum<cn.hutool.crypto.GlobalBouncyCastleProvider> {
  public static cn.hutool.crypto.GlobalBouncyCastleProvider[] values();
  public static cn.hutool.crypto.GlobalBouncyCastleProvider valueOf(java.lang.String);
  public java.security.Provider getProvider();
  public static void setUseBouncyCastle(boolean);
}
```

## `cn.hutool.crypto.KeyUtil`

```java
public class cn.hutool.crypto.KeyUtil {
  public cn.hutool.crypto.KeyUtil();
  public static javax.crypto.SecretKey generateKey(java.lang.String);
  public static javax.crypto.SecretKey generateKey(java.lang.String, int);
  public static javax.crypto.SecretKey generateKey(java.lang.String, int, java.security.SecureRandom);
  public static javax.crypto.SecretKey generateKey(java.lang.String, byte[]);
  public static javax.crypto.SecretKey generateDESKey(java.lang.String, byte[]);
  public static javax.crypto.SecretKey generatePBEKey(java.lang.String, char[]);
  public static javax.crypto.SecretKey generateKey(java.lang.String, java.security.spec.KeySpec);
  public static java.security.PrivateKey generateRSAPrivateKey(java.lang.String);
  public static java.security.PrivateKey generateRSAPrivateKey(byte[]);
  public static java.security.PrivateKey generateRSAPrivateKey(java.security.spec.KeySpec);
  public static java.security.PrivateKey generatePrivateKey(java.lang.String, byte[]);
  public static java.security.PrivateKey generatePrivateKey(java.lang.String, java.security.spec.KeySpec);
  public static java.security.PrivateKey generatePrivateKey(java.security.KeyStore, java.lang.String, char[]);
  public static java.security.PublicKey generateRSAPublicKey(byte[]);
  public static java.security.PublicKey generatePublicKey(java.lang.String, byte[]);
  public static java.security.PublicKey generatePublicKey(java.lang.String, java.security.spec.KeySpec);
  public static java.security.KeyPair generateKeyPair(java.lang.String);
  public static java.security.KeyPair generateKeyPair(java.lang.String, int);
  public static java.security.KeyPair generateKeyPair(java.lang.String, int, byte[]);
  public static java.security.KeyPair generateKeyPair(java.lang.String, java.security.spec.AlgorithmParameterSpec);
  public static java.security.KeyPair generateKeyPair(java.lang.String, byte[], java.security.spec.AlgorithmParameterSpec);
  public static java.security.KeyPair generateKeyPair(java.lang.String, int, byte[], java.security.spec.AlgorithmParameterSpec...);
  public static java.security.KeyPair generateKeyPair(java.lang.String, int, java.security.SecureRandom, java.security.spec.AlgorithmParameterSpec...);
  public static java.security.KeyPairGenerator getKeyPairGenerator(java.lang.String);
  public static java.security.KeyFactory getKeyFactory(java.lang.String);
  public static javax.crypto.SecretKeyFactory getSecretKeyFactory(java.lang.String);
  public static javax.crypto.KeyGenerator getKeyGenerator(java.lang.String);
  public static java.lang.String getMainAlgorithm(java.lang.String);
  public static java.lang.String getAlgorithmAfterWith(java.lang.String);
  public static java.security.KeyStore readJKSKeyStore(java.io.File, char[]);
  public static java.security.KeyStore readJKSKeyStore(java.io.InputStream, char[]);
  public static java.security.KeyStore readPKCS12KeyStore(java.io.File, char[]);
  public static java.security.KeyStore readPKCS12KeyStore(java.io.InputStream, char[]);
  public static java.security.KeyStore readKeyStore(java.lang.String, java.io.File, char[]);
  public static java.security.KeyStore readKeyStore(java.lang.String, java.io.InputStream, char[]);
  public static java.security.KeyStore getKeyStore(java.lang.String);
  public static java.security.KeyPair getKeyPair(java.lang.String, java.io.InputStream, char[], java.lang.String);
  public static java.security.KeyPair getKeyPair(java.security.KeyStore, char[], java.lang.String);
  public static java.security.cert.Certificate readX509Certificate(java.io.InputStream, char[], java.lang.String);
  public static java.security.PublicKey readPublicKeyFromCert(java.io.InputStream);
  public static java.security.cert.Certificate readX509Certificate(java.io.InputStream);
  public static java.security.cert.Certificate readCertificate(java.lang.String, java.io.InputStream, char[], java.lang.String);
  public static java.security.cert.Certificate readCertificate(java.lang.String, java.io.InputStream);
  public static java.security.cert.Certificate getCertificate(java.security.KeyStore, java.lang.String);
  public static java.security.cert.CertificateFactory getCertificateFactory(java.lang.String);
  public static byte[] encodeECPublicKey(java.security.PublicKey);
  public static java.security.PublicKey decodeECPoint(java.lang.String, java.lang.String);
  public static java.security.PublicKey decodeECPoint(byte[], java.lang.String);
  public static java.security.PublicKey getRSAPublicKey(java.security.PrivateKey);
  public static java.security.PublicKey getRSAPublicKey(java.lang.String, java.lang.String);
  public static java.security.PublicKey getRSAPublicKey(java.math.BigInteger, java.math.BigInteger);
  public static java.lang.String toBase64(java.security.Key);
}
```

## `cn.hutool.crypto.Mode`

```java
public final class cn.hutool.crypto.Mode extends java.lang.Enum<cn.hutool.crypto.Mode> {
  public static cn.hutool.crypto.Mode[] values();
  public static cn.hutool.crypto.Mode valueOf(java.lang.String);
}
```

## `cn.hutool.crypto.OpensslKeyUtil`

```java
public class cn.hutool.crypto.OpensslKeyUtil {
  public cn.hutool.crypto.OpensslKeyUtil();
  public static java.security.PrivateKey getPrivateKey(org.bouncycastle.asn1.pkcs.PrivateKeyInfo) throws cn.hutool.crypto.CryptoException;
  public static java.security.PublicKey getPublicKey(org.bouncycastle.asn1.x509.SubjectPublicKeyInfo) throws cn.hutool.crypto.CryptoException;
  public static java.security.KeyPair getKeyPair(org.bouncycastle.openssl.PEMKeyPair) throws cn.hutool.crypto.CryptoException;
  public static java.security.Key readPemKey(java.io.InputStream, char[]);
  public static org.bouncycastle.asn1.pkcs.PrivateKeyInfo decrypt(org.bouncycastle.pkcs.PKCS8EncryptedPrivateKeyInfo, char[]) throws cn.hutool.crypto.CryptoException;
  public static org.bouncycastle.openssl.PEMKeyPair decrypt(org.bouncycastle.openssl.PEMEncryptedKeyPair, char[]) throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.crypto.Padding`

```java
public final class cn.hutool.crypto.Padding extends java.lang.Enum<cn.hutool.crypto.Padding> {
  public static cn.hutool.crypto.Padding[] values();
  public static cn.hutool.crypto.Padding valueOf(java.lang.String);
}
```

## `cn.hutool.crypto.PemUtil`

```java
public class cn.hutool.crypto.PemUtil {
  public cn.hutool.crypto.PemUtil();
  public static java.security.PrivateKey readPemPrivateKey(java.io.InputStream);
  public static java.security.PublicKey readPemPublicKey(java.io.InputStream);
  public static java.security.Key readPemKey(java.io.InputStream);
  public static byte[] readPem(java.io.InputStream);
  public static org.bouncycastle.util.io.pem.PemObject readPemObject(java.io.InputStream);
  public static org.bouncycastle.util.io.pem.PemObject readPemObject(java.io.Reader);
  public static java.security.PrivateKey readSm2PemPrivateKey(java.io.InputStream);
  public static java.lang.String toPem(java.lang.String, byte[]);
  public static void writePemObject(java.lang.String, byte[], java.io.OutputStream);
  public static void writePemObject(java.lang.String, byte[], java.io.Writer);
  public static void writePemObject(org.bouncycastle.util.io.pem.PemObjectGenerator, java.io.OutputStream);
  public static void writePemObject(org.bouncycastle.util.io.pem.PemObjectGenerator, java.io.Writer);
}
```

## `cn.hutool.crypto.ProviderFactory`

```java
public class cn.hutool.crypto.ProviderFactory {
  public static java.security.Provider createBouncyCastleProvider();
}
```

## `cn.hutool.crypto.SecureUtil`

```java
public class cn.hutool.crypto.SecureUtil {
  public cn.hutool.crypto.SecureUtil();
  public static javax.crypto.SecretKey generateKey(java.lang.String);
  public static javax.crypto.SecretKey generateKey(java.lang.String, int);
  public static javax.crypto.SecretKey generateKey(java.lang.String, byte[]);
  public static javax.crypto.SecretKey generateDESKey(java.lang.String, byte[]);
  public static javax.crypto.SecretKey generatePBEKey(java.lang.String, char[]);
  public static javax.crypto.SecretKey generateKey(java.lang.String, java.security.spec.KeySpec);
  public static java.security.PrivateKey generatePrivateKey(java.lang.String, byte[]);
  public static java.security.PrivateKey generatePrivateKey(java.lang.String, java.security.spec.KeySpec);
  public static java.security.PrivateKey generatePrivateKey(java.security.KeyStore, java.lang.String, char[]);
  public static java.security.PublicKey generatePublicKey(java.lang.String, byte[]);
  public static java.security.PublicKey generatePublicKey(java.lang.String, java.security.spec.KeySpec);
  public static java.security.KeyPair generateKeyPair(java.lang.String);
  public static java.security.KeyPair generateKeyPair(java.lang.String, int);
  public static java.security.KeyPair generateKeyPair(java.lang.String, int, byte[]);
  public static java.security.KeyPair generateKeyPair(java.lang.String, java.security.spec.AlgorithmParameterSpec);
  public static java.security.KeyPair generateKeyPair(java.lang.String, byte[], java.security.spec.AlgorithmParameterSpec);
  public static java.lang.String getAlgorithmAfterWith(java.lang.String);
  public static java.lang.String generateAlgorithm(cn.hutool.crypto.asymmetric.AsymmetricAlgorithm, cn.hutool.crypto.digest.DigestAlgorithm);
  public static java.security.Signature generateSignature(cn.hutool.crypto.asymmetric.AsymmetricAlgorithm, cn.hutool.crypto.digest.DigestAlgorithm);
  public static java.security.KeyStore readJKSKeyStore(java.io.InputStream, char[]);
  public static java.security.KeyStore readKeyStore(java.lang.String, java.io.InputStream, char[]);
  public static java.security.cert.Certificate readX509Certificate(java.io.InputStream, char[], java.lang.String);
  public static java.security.cert.Certificate readX509Certificate(java.io.InputStream);
  public static java.security.cert.Certificate readCertificate(java.lang.String, java.io.InputStream, char[], java.lang.String);
  public static java.security.cert.Certificate readCertificate(java.lang.String, java.io.InputStream);
  public static java.security.cert.Certificate getCertificate(java.security.KeyStore, java.lang.String);
  public static cn.hutool.crypto.symmetric.AES aes();
  public static cn.hutool.crypto.symmetric.AES aes(byte[]);
  public static cn.hutool.crypto.symmetric.DES des();
  public static cn.hutool.crypto.symmetric.DES des(byte[]);
  public static cn.hutool.crypto.symmetric.DESede desede();
  public static cn.hutool.crypto.symmetric.DESede desede(byte[]);
  public static cn.hutool.crypto.digest.MD5 md5();
  public static java.lang.String md5(java.lang.String);
  public static java.lang.String md5(java.io.InputStream);
  public static java.lang.String md5(java.io.File);
  public static cn.hutool.crypto.digest.Digester sha1();
  public static java.lang.String sha1(java.lang.String);
  public static java.lang.String sha1(java.io.InputStream);
  public static java.lang.String sha1(java.io.File);
  public static cn.hutool.crypto.digest.Digester sha256();
  public static java.lang.String sha256(java.lang.String);
  public static java.lang.String sha256(java.io.InputStream);
  public static java.lang.String sha256(java.io.File);
  public static cn.hutool.crypto.digest.HMac hmac(cn.hutool.crypto.digest.HmacAlgorithm, java.lang.String);
  public static cn.hutool.crypto.digest.HMac hmac(cn.hutool.crypto.digest.HmacAlgorithm, byte[]);
  public static cn.hutool.crypto.digest.HMac hmac(cn.hutool.crypto.digest.HmacAlgorithm, javax.crypto.SecretKey);
  public static cn.hutool.crypto.digest.HMac hmacMd5(java.lang.String);
  public static cn.hutool.crypto.digest.HMac hmacMd5(byte[]);
  public static cn.hutool.crypto.digest.HMac hmacMd5();
  public static cn.hutool.crypto.digest.HMac hmacSha1(java.lang.String);
  public static cn.hutool.crypto.digest.HMac hmacSha1(byte[]);
  public static cn.hutool.crypto.digest.HMac hmacSha1();
  public static cn.hutool.crypto.digest.HMac hmacSha256(java.lang.String);
  public static cn.hutool.crypto.digest.HMac hmacSha256(byte[]);
  public static cn.hutool.crypto.digest.HMac hmacSha256();
  public static cn.hutool.crypto.asymmetric.RSA rsa();
  public static cn.hutool.crypto.asymmetric.RSA rsa(java.lang.String, java.lang.String);
  public static cn.hutool.crypto.asymmetric.RSA rsa(byte[], byte[]);
  public static cn.hutool.crypto.asymmetric.Sign sign(cn.hutool.crypto.asymmetric.SignAlgorithm);
  public static cn.hutool.crypto.asymmetric.Sign sign(cn.hutool.crypto.asymmetric.SignAlgorithm, java.lang.String, java.lang.String);
  public static cn.hutool.crypto.asymmetric.Sign sign(cn.hutool.crypto.asymmetric.SignAlgorithm, byte[], byte[]);
  public static java.lang.String signParams(cn.hutool.crypto.symmetric.SymmetricCrypto, java.util.Map<?, ?>, java.lang.String...);
  public static java.lang.String signParams(cn.hutool.crypto.symmetric.SymmetricCrypto, java.util.Map<?, ?>, java.lang.String, java.lang.String, boolean, java.lang.String...);
  public static java.lang.String signParamsMd5(java.util.Map<?, ?>, java.lang.String...);
  public static java.lang.String signParamsSha1(java.util.Map<?, ?>, java.lang.String...);
  public static java.lang.String signParamsSha256(java.util.Map<?, ?>, java.lang.String...);
  public static java.lang.String signParams(cn.hutool.crypto.digest.DigestAlgorithm, java.util.Map<?, ?>, java.lang.String...);
  public static java.lang.String signParams(cn.hutool.crypto.digest.DigestAlgorithm, java.util.Map<?, ?>, java.lang.String, java.lang.String, boolean, java.lang.String...);
  public static void addProvider(java.security.Provider);
  public static byte[] decode(java.lang.String);
  public static javax.crypto.Cipher createCipher(java.lang.String);
  public static java.security.MessageDigest createMessageDigest(java.lang.String);
  public static java.security.MessageDigest createJdkMessageDigest(java.lang.String);
  public static javax.crypto.Mac createMac(java.lang.String);
  public static java.security.Signature createSignature(java.lang.String);
  public static cn.hutool.crypto.symmetric.RC4 rc4(java.lang.String);
  public static void disableBouncyCastle();
  public static java.lang.String pbkdf2(char[], byte[]);
  public static cn.hutool.crypto.symmetric.fpe.FPE fpe(cn.hutool.crypto.symmetric.fpe.FPE$FPEMode, byte[], org.bouncycastle.crypto.AlphabetMapper, byte[]);
  public static cn.hutool.crypto.symmetric.ZUC zuc128(byte[], byte[]);
  public static cn.hutool.crypto.symmetric.ZUC zuc256(byte[], byte[]);
}
```

## `cn.hutool.crypto.SignUtil`

```java
public class cn.hutool.crypto.SignUtil {
  public cn.hutool.crypto.SignUtil();
  public static cn.hutool.crypto.asymmetric.Sign sign(cn.hutool.crypto.asymmetric.SignAlgorithm);
  public static cn.hutool.crypto.asymmetric.Sign sign(cn.hutool.crypto.asymmetric.SignAlgorithm, java.lang.String, java.lang.String);
  public static cn.hutool.crypto.asymmetric.Sign sign(cn.hutool.crypto.asymmetric.SignAlgorithm, byte[], byte[]);
  public static java.lang.String signParams(cn.hutool.crypto.symmetric.SymmetricCrypto, java.util.Map<?, ?>, java.lang.String...);
  public static java.lang.String signParams(cn.hutool.crypto.symmetric.SymmetricCrypto, java.util.Map<?, ?>, java.lang.String, java.lang.String, boolean, java.lang.String...);
  public static java.lang.String signParamsMd5(java.util.Map<?, ?>, java.lang.String...);
  public static java.lang.String signParamsSha1(java.util.Map<?, ?>, java.lang.String...);
  public static java.lang.String signParamsSha256(java.util.Map<?, ?>, java.lang.String...);
  public static java.lang.String signParams(cn.hutool.crypto.digest.DigestAlgorithm, java.util.Map<?, ?>, java.lang.String...);
  public static java.lang.String signParams(cn.hutool.crypto.digest.DigestAlgorithm, java.util.Map<?, ?>, java.lang.String, java.lang.String, boolean, java.lang.String...);
}
```

## `cn.hutool.crypto.SmUtil`

```java
public class cn.hutool.crypto.SmUtil {
  public cn.hutool.crypto.SmUtil();
  public static cn.hutool.crypto.asymmetric.SM2 sm2();
  public static cn.hutool.crypto.asymmetric.SM2 sm2(java.lang.String, java.lang.String);
  public static cn.hutool.crypto.asymmetric.SM2 sm2(byte[], byte[]);
  public static cn.hutool.crypto.asymmetric.SM2 sm2(java.security.PrivateKey, java.security.PublicKey);
  public static cn.hutool.crypto.asymmetric.SM2 sm2(org.bouncycastle.crypto.params.ECPrivateKeyParameters, org.bouncycastle.crypto.params.ECPublicKeyParameters);
  public static cn.hutool.crypto.digest.SM3 sm3();
  public static cn.hutool.crypto.digest.SM3 sm3WithSalt(byte[]);
  public static java.lang.String sm3(java.lang.String);
  public static java.lang.String sm3(java.io.InputStream);
  public static java.lang.String sm3(java.io.File);
  public static cn.hutool.crypto.symmetric.SM4 sm4();
  public static cn.hutool.crypto.symmetric.SM4 sm4(byte[]);
  public static byte[] changeC1C2C3ToC1C3C2(byte[], org.bouncycastle.crypto.params.ECDomainParameters);
  public static byte[] changeC1C3C2ToC1C2C3(byte[], org.bouncycastle.crypto.params.ECDomainParameters);
  public static byte[] rsAsn1ToPlain(byte[]);
  public static byte[] rsPlainToAsn1(byte[]);
  public static cn.hutool.crypto.digest.mac.MacEngine createHmacSm3Engine(byte[]);
  public static cn.hutool.crypto.digest.HMac hmacSm3(byte[]);
}
```

## `cn.hutool.crypto.SpecUtil`

```java
public class cn.hutool.crypto.SpecUtil {
  public cn.hutool.crypto.SpecUtil();
  public static java.security.spec.KeySpec createKeySpec(java.lang.String, byte[]);
  public static javax.crypto.spec.PBEKeySpec createPBEKeySpec(char[]);
  public static javax.crypto.spec.PBEParameterSpec createPBEParameterSpec(byte[], int);
  public static java.security.spec.RSAPrivateCrtKeySpec xmlToRSAPrivateCrtKeySpec(java.lang.String);
}
```
