# cn.hutool.crypto.digest.mac

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.crypto.digest.mac.BCHMacEngine`

```java
public class cn.hutool.crypto.digest.mac.BCHMacEngine extends cn.hutool.crypto.digest.mac.BCMacEngine {
  public cn.hutool.crypto.digest.mac.BCHMacEngine(org.bouncycastle.crypto.Digest, byte[], byte[]);
  public cn.hutool.crypto.digest.mac.BCHMacEngine(org.bouncycastle.crypto.Digest, byte[]);
  public cn.hutool.crypto.digest.mac.BCHMacEngine(org.bouncycastle.crypto.Digest, org.bouncycastle.crypto.CipherParameters);
  public cn.hutool.crypto.digest.mac.BCHMacEngine(org.bouncycastle.crypto.macs.HMac, org.bouncycastle.crypto.CipherParameters);
  public cn.hutool.crypto.digest.mac.BCHMacEngine init(org.bouncycastle.crypto.Digest, org.bouncycastle.crypto.CipherParameters);
}
```

## `cn.hutool.crypto.digest.mac.BCMacEngine`

```java
public class cn.hutool.crypto.digest.mac.BCMacEngine implements cn.hutool.crypto.digest.mac.MacEngine {
  public cn.hutool.crypto.digest.mac.BCMacEngine(org.bouncycastle.crypto.Mac, org.bouncycastle.crypto.CipherParameters);
  public cn.hutool.crypto.digest.mac.BCMacEngine init(org.bouncycastle.crypto.Mac, org.bouncycastle.crypto.CipherParameters);
  public org.bouncycastle.crypto.Mac getMac();
  public void update(byte[], int, int);
  public byte[] doFinal();
  public void reset();
  public int getMacLength();
  public java.lang.String getAlgorithm();
}
```

## `cn.hutool.crypto.digest.mac.CBCBlockCipherMacEngine`

```java
public class cn.hutool.crypto.digest.mac.CBCBlockCipherMacEngine extends cn.hutool.crypto.digest.mac.BCMacEngine {
  public cn.hutool.crypto.digest.mac.CBCBlockCipherMacEngine(org.bouncycastle.crypto.BlockCipher, int, java.security.Key, byte[]);
  public cn.hutool.crypto.digest.mac.CBCBlockCipherMacEngine(org.bouncycastle.crypto.BlockCipher, int, byte[], byte[]);
  public cn.hutool.crypto.digest.mac.CBCBlockCipherMacEngine(org.bouncycastle.crypto.BlockCipher, int, java.security.Key);
  public cn.hutool.crypto.digest.mac.CBCBlockCipherMacEngine(org.bouncycastle.crypto.BlockCipher, int, byte[]);
  public cn.hutool.crypto.digest.mac.CBCBlockCipherMacEngine(org.bouncycastle.crypto.BlockCipher, int, org.bouncycastle.crypto.CipherParameters);
  public cn.hutool.crypto.digest.mac.CBCBlockCipherMacEngine(org.bouncycastle.crypto.macs.CBCBlockCipherMac, org.bouncycastle.crypto.CipherParameters);
  public cn.hutool.crypto.digest.mac.CBCBlockCipherMacEngine init(org.bouncycastle.crypto.BlockCipher, org.bouncycastle.crypto.CipherParameters);
}
```

## `cn.hutool.crypto.digest.mac.DefaultHMacEngine`

```java
public class cn.hutool.crypto.digest.mac.DefaultHMacEngine implements cn.hutool.crypto.digest.mac.MacEngine {
  public cn.hutool.crypto.digest.mac.DefaultHMacEngine(java.lang.String, byte[]);
  public cn.hutool.crypto.digest.mac.DefaultHMacEngine(java.lang.String, java.security.Key);
  public cn.hutool.crypto.digest.mac.DefaultHMacEngine(java.lang.String, java.security.Key, java.security.spec.AlgorithmParameterSpec);
  public cn.hutool.crypto.digest.mac.DefaultHMacEngine init(java.lang.String, byte[]);
  public cn.hutool.crypto.digest.mac.DefaultHMacEngine init(java.lang.String, java.security.Key);
  public cn.hutool.crypto.digest.mac.DefaultHMacEngine init(java.lang.String, java.security.Key, java.security.spec.AlgorithmParameterSpec);
  public javax.crypto.Mac getMac();
  public void update(byte[]);
  public void update(byte[], int, int);
  public byte[] doFinal();
  public void reset();
  public int getMacLength();
  public java.lang.String getAlgorithm();
}
```

## `cn.hutool.crypto.digest.mac.Mac`

```java
public class cn.hutool.crypto.digest.mac.Mac implements java.io.Serializable {
  public cn.hutool.crypto.digest.mac.Mac(cn.hutool.crypto.digest.mac.MacEngine);
  public cn.hutool.crypto.digest.mac.MacEngine getEngine();
  public byte[] digest(java.lang.String, java.nio.charset.Charset);
  public byte[] digest(java.lang.String);
  public java.lang.String digestBase64(java.lang.String, boolean);
  public java.lang.String digestBase64(java.lang.String, java.nio.charset.Charset, boolean);
  public java.lang.String digestHex(java.lang.String, java.nio.charset.Charset);
  public java.lang.String digestHex(java.lang.String);
  public byte[] digest(java.io.File) throws cn.hutool.crypto.CryptoException;
  public java.lang.String digestHex(java.io.File);
  public byte[] digest(byte[]);
  public java.lang.String digestHex(byte[]);
  public byte[] digest(java.io.InputStream);
  public java.lang.String digestHex(java.io.InputStream);
  public byte[] digest(java.io.InputStream, int);
  public java.lang.String digestHex(java.io.InputStream, int);
  public boolean verify(byte[], byte[]);
  public int getMacLength();
  public java.lang.String getAlgorithm();
}
```

## `cn.hutool.crypto.digest.mac.MacEngine`

```java
public interface cn.hutool.crypto.digest.mac.MacEngine {
  public default void update(byte[]);
  public abstract void update(byte[], int, int);
  public abstract byte[] doFinal();
  public abstract void reset();
  public default byte[] digest(java.io.InputStream, int);
  public abstract int getMacLength();
  public abstract java.lang.String getAlgorithm();
}
```

## `cn.hutool.crypto.digest.mac.MacEngineFactory`

```java
public class cn.hutool.crypto.digest.mac.MacEngineFactory {
  public cn.hutool.crypto.digest.mac.MacEngineFactory();
  public static cn.hutool.crypto.digest.mac.MacEngine createEngine(java.lang.String, java.security.Key);
  public static cn.hutool.crypto.digest.mac.MacEngine createEngine(java.lang.String, java.security.Key, java.security.spec.AlgorithmParameterSpec);
}
```

## `cn.hutool.crypto.digest.mac.SM4MacEngine`

```java
public class cn.hutool.crypto.digest.mac.SM4MacEngine extends cn.hutool.crypto.digest.mac.CBCBlockCipherMacEngine {
  public cn.hutool.crypto.digest.mac.SM4MacEngine(org.bouncycastle.crypto.CipherParameters);
}
```
