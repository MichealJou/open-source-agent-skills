# cn.hutool.crypto.asymmetric

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.crypto.asymmetric.AsymmetricAlgorithm` | `String getValue()` | 获取算法字符串表示，区分大小写 |
| `cn.hutool.crypto.asymmetric.AsymmetricCrypto` | `AlgorithmParameterSpec getAlgorithmParameterSpec()` | 获取AlgorithmParameterSpec 在某些算法中，需要特别的参数，例如在ECIES中，此处为IESParameterSpec |
| `cn.hutool.crypto.asymmetric.AsymmetricCrypto` | `AsymmetricCrypto init(String algorithm,PrivateKey privateKey,PublicKey publicKey)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.asymmetric.AsymmetricCrypto` | `AsymmetricCrypto setRandom(SecureRandom random)` | 设置随机数生成器，可自定义随机数种子 |
| `cn.hutool.crypto.asymmetric.AsymmetricCrypto` | `Cipher getCipher()` | 获得加密或解密器 |
| `cn.hutool.crypto.asymmetric.AsymmetricCrypto` | `byte[] decrypt(byte[] data,KeyType keyType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.asymmetric.AsymmetricCrypto` | `byte[] encrypt(byte[] data,KeyType keyType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.asymmetric.AsymmetricCrypto` | `int getDecryptBlockSize()` | 获取解密块大小 |
| `cn.hutool.crypto.asymmetric.AsymmetricCrypto` | `int getEncryptBlockSize()` | 获取加密块大小 |
| `cn.hutool.crypto.asymmetric.AsymmetricCrypto` | `void setAlgorithmParameterSpec(AlgorithmParameterSpec algorithmParameterSpec)` | 设置AlgorithmParameterSpec 在某些算法中，需要特别的参数，例如在ECIES中，此处为IESParameterSpec |
| `cn.hutool.crypto.asymmetric.AsymmetricCrypto` | `void setDecryptBlockSize(int decryptBlockSize)` | 设置解密块大小 |
| `cn.hutool.crypto.asymmetric.AsymmetricCrypto` | `void setEncryptBlockSize(int encryptBlockSize)` | 设置加密块大小 |
| `cn.hutool.crypto.asymmetric.AsymmetricDecryptor` | `String decryptStr(String data,KeyType keyType)` | 解密为字符串，密文需为Hex（16进制）或Base64字符串 |
| `cn.hutool.crypto.asymmetric.AsymmetricDecryptor` | `String decryptStr(String data,KeyType keyType,Charset charset)` | 解密为字符串，密文需为Hex（16进制）或Base64字符串 |
| `cn.hutool.crypto.asymmetric.AsymmetricDecryptor` | `String decryptStrFromBcd(String data,KeyType keyType)` | 解密为字符串，密文需为BCD格式，编码为UTF-8格式 |
| `cn.hutool.crypto.asymmetric.AsymmetricDecryptor` | `String decryptStrFromBcd(String data,KeyType keyType,Charset charset)` | 解密为字符串，密文需为BCD格式 |
| `cn.hutool.crypto.asymmetric.AsymmetricDecryptor` | `byte[] decrypt(InputStream data,KeyType keyType)` | 解密 |
| `cn.hutool.crypto.asymmetric.AsymmetricDecryptor` | `byte[] decrypt(String data,KeyType keyType)` | 从Hex或Base64字符串解密，编码为UTF-8格式 |
| `cn.hutool.crypto.asymmetric.AsymmetricDecryptor` | `byte[] decrypt(byte[] bytes,KeyType keyType)` | 解密 |
| `cn.hutool.crypto.asymmetric.AsymmetricDecryptor` | `byte[] decryptFromBcd(String data,KeyType keyType)` | 解密BCD |
| `cn.hutool.crypto.asymmetric.AsymmetricDecryptor` | `byte[] decryptFromBcd(String data,KeyType keyType,Charset charset)` | 分组解密 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `String encryptBase64(InputStream data,KeyType keyType)` | 编码为Base64字符串 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `String encryptBase64(String data,Charset charset,KeyType keyType)` | 编码为Base64字符串 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `String encryptBase64(String data,KeyType keyType)` | 编码为Base64字符串，使用UTF-8编码 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `String encryptBase64(byte[] data,KeyType keyType)` | 编码为Base64字符串 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `String encryptBcd(String data,KeyType keyType)` | 分组加密 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `String encryptBcd(String data,KeyType keyType,Charset charset)` | 分组加密 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `String encryptHex(InputStream data,KeyType keyType)` | 编码为Hex字符串 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `String encryptHex(String data,Charset charset,KeyType keyType)` | 编码为Hex字符串 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `String encryptHex(String data,KeyType keyType)` | 编码为Hex字符串 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `String encryptHex(byte[] data,KeyType keyType)` | 编码为Hex字符串 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `byte[] encrypt(InputStream data,KeyType keyType)` | 加密 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `byte[] encrypt(String data,Charset charset,KeyType keyType)` | 加密 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `byte[] encrypt(String data,KeyType keyType)` | 加密，使用UTF-8编码 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `byte[] encrypt(String data,String charset,KeyType keyType)` | 加密 |
| `cn.hutool.crypto.asymmetric.AsymmetricEncryptor` | `byte[] encrypt(byte[] data,KeyType keyType)` | 加密 |
| `cn.hutool.crypto.asymmetric.BaseAsymmetric` | `PrivateKey getPrivateKey()` | 获得私钥 |
| `cn.hutool.crypto.asymmetric.BaseAsymmetric` | `PublicKey getPublicKey()` | 获得公钥 |
| `cn.hutool.crypto.asymmetric.BaseAsymmetric` | `String getPrivateKeyBase64()` | 获得私钥 |
| `cn.hutool.crypto.asymmetric.BaseAsymmetric` | `String getPublicKeyBase64()` | 获得公钥 |
| `cn.hutool.crypto.asymmetric.BaseAsymmetric` | `T initKeys()` | 生成公钥和私钥 |
| `cn.hutool.crypto.asymmetric.BaseAsymmetric` | `T setKey(Key key)` | 设置密钥，可以是公钥PublicKey或者私钥PrivateKey |
| `cn.hutool.crypto.asymmetric.BaseAsymmetric` | `T setPrivateKey(PrivateKey privateKey)` | 设置私钥 |
| `cn.hutool.crypto.asymmetric.BaseAsymmetric` | `T setPublicKey(PublicKey publicKey)` | 设置公钥 |
| `cn.hutool.crypto.asymmetric.KeyType` | `int getValue()` | 获取枚举值对应的int表示 |
| `cn.hutool.crypto.asymmetric.RSA` | `PrivateKey generatePrivateKey(BigInteger modulus,BigInteger privateExponent)` | 生成RSA私钥 |
| `cn.hutool.crypto.asymmetric.RSA` | `PublicKey generatePublicKey(BigInteger modulus,BigInteger publicExponent)` | 生成RSA公钥 |
| `cn.hutool.crypto.asymmetric.RSA` | `byte[] decrypt(byte[] bytes,KeyType keyType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.asymmetric.RSA` | `byte[] encrypt(byte[] data,KeyType keyType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.asymmetric.SM2` | `BigInteger getDBigInteger()` | 获得私钥D值 |
| `cn.hutool.crypto.asymmetric.SM2` | `SM2 init()` | 初始化 私钥和公钥同时为空时生成一对新的私钥和公钥 私钥和公钥可以单独传入一个，如此则只能使用此钥匙来做加密（签名）或者解密（校验） |
| `cn.hutool.crypto.asymmetric.SM2` | `SM2 initKeys()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.asymmetric.SM2` | `SM2 setDigest(Digest digest)` | 设置Hash算法 |
| `cn.hutool.crypto.asymmetric.SM2` | `SM2 setEncoding(DSAEncoding encoding)` | 设置DSA signatures的编码 |
| `cn.hutool.crypto.asymmetric.SM2` | `SM2 setMode(SM2Engine.Mode mode)` | 设置SM2模式，旧版是C1C2C3，新版本是C1C3C2 |
| `cn.hutool.crypto.asymmetric.SM2` | `SM2 setPrivateKey(PrivateKey privateKey)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.asymmetric.SM2` | `SM2 setPrivateKeyParams(ECPrivateKeyParameters privateKeyParams)` | 设置私钥参数 |
| `cn.hutool.crypto.asymmetric.SM2` | `SM2 setPublicKey(PublicKey publicKey)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.asymmetric.SM2` | `SM2 setPublicKeyParams(ECPublicKeyParameters publicKeyParams)` | 设置公钥参数 |
| `cn.hutool.crypto.asymmetric.SM2` | `SM2 usePlainEncoding()` | 设置DSA signatures的编码为PlainDSAEncoding |
| `cn.hutool.crypto.asymmetric.SM2` | `String getDHex()` | 获得私钥D值（编码后的私钥） |
| `cn.hutool.crypto.asymmetric.SM2` | `String signHex(String dataHex)` | 用私钥对信息生成数字签名 |
| `cn.hutool.crypto.asymmetric.SM2` | `String signHex(String dataHex,String idHex)` | 用私钥对信息生成数字签名 |
| `cn.hutool.crypto.asymmetric.SM2` | `String signHexFromHex(String dataHex)` | 用私钥对信息生成数字签名 |
| `cn.hutool.crypto.asymmetric.SM2` | `String signHexFromHex(String dataHex,String idHex)` | 用私钥对信息生成数字签名 |
| `cn.hutool.crypto.asymmetric.SM2` | `boolean verify(byte[] data,byte[] sign)` | 用公钥检验数字签名的合法性 |
| `cn.hutool.crypto.asymmetric.SM2` | `boolean verify(byte[] data,byte[] sign,byte[] id)` | 用公钥检验数字签名的合法性 |
| `cn.hutool.crypto.asymmetric.SM2` | `boolean verifyHex(String dataHex,String signHex)` | 用公钥检验数字签名的合法性 |
| `cn.hutool.crypto.asymmetric.SM2` | `boolean verifyHex(String dataHex,String signHex,String idHex)` | 用公钥检验数字签名的合法性 |
| `cn.hutool.crypto.asymmetric.SM2` | `byte[] decrypt(byte[] data)` | 使用私钥解密 |
| `cn.hutool.crypto.asymmetric.SM2` | `byte[] decrypt(byte[] data,CipherParameters privateKeyParameters)` | 解密 |
| `cn.hutool.crypto.asymmetric.SM2` | `byte[] decrypt(byte[] data,KeyType keyType)` | 解密 |
| `cn.hutool.crypto.asymmetric.SM2` | `byte[] encrypt(byte[] data)` | 使用公钥加密，SM2非对称加密的结果由C1,C3,C2三部分组成，其中： |
| `cn.hutool.crypto.asymmetric.SM2` | `byte[] encrypt(byte[] data,CipherParameters pubKeyParameters)` | 加密，SM2非对称加密的结果由C1,C2,C3三部分组成，其中： |
| `cn.hutool.crypto.asymmetric.SM2` | `byte[] encrypt(byte[] data,KeyType keyType)` | 加密，SM2非对称加密的结果由C1,C3,C2三部分组成，其中： |
| `cn.hutool.crypto.asymmetric.SM2` | `byte[] getD()` | 获得私钥D值（编码后的私钥） |
| `cn.hutool.crypto.asymmetric.SM2` | `byte[] getQ(boolean isCompressed)` | 获得公钥Q值（编码后的公钥） |
| `cn.hutool.crypto.asymmetric.SM2` | `byte[] sign(byte[] data)` | 用私钥对信息生成数字签名，签名格式为ASN1 * 在硬件签名中，返回结果为R+S，可以通过调用cn.hutool.crypto.SmUtil#rsAsn1ToPlain(byte[])方法转换之。 |
| `cn.hutool.crypto.asymmetric.SM2` | `byte[] sign(byte[] data,byte[] id)` | 用私钥对信息生成数字签名，签名格式为ASN1 在硬件签名中，返回结果为R+S，可以通过调用cn.hutool.crypto.SmUtil#rsAsn1ToPlain(byte[])方法转换之。 |
| `cn.hutool.crypto.asymmetric.Sign` | `Sign init(String algorithm,PrivateKey privateKey,PublicKey publicKey)` | 初始化 |
| `cn.hutool.crypto.asymmetric.Sign` | `Sign setCertificate(Certificate certificate)` | 设置Certificate 为PublicKey 如果Certificate是X509Certificate，我们需要检查是否有密钥扩展 |
| `cn.hutool.crypto.asymmetric.Sign` | `Sign setParameter(AlgorithmParameterSpec params)` | 设置签名的参数 |
| `cn.hutool.crypto.asymmetric.Sign` | `Sign setSignature(Signature signature)` | 设置签名 |
| `cn.hutool.crypto.asymmetric.Sign` | `Signature getSignature()` | 获得签名对象 |
| `cn.hutool.crypto.asymmetric.Sign` | `String digestHex(InputStream data,int bufferLength)` | 生成签名，并转为16进制字符串 使用默认缓存大小，见 IoUtil#DEFAULT_BUFFER_SIZE |
| `cn.hutool.crypto.asymmetric.Sign` | `String signHex(InputStream data)` | 生成签名，并转为16进制字符串 使用默认缓存大小，见 IoUtil#DEFAULT_BUFFER_SIZE |
| `cn.hutool.crypto.asymmetric.Sign` | `String signHex(String data)` | 生成文件签名 |
| `cn.hutool.crypto.asymmetric.Sign` | `String signHex(String data,Charset charset)` | 生成文件签名，并转为16进制字符串 |
| `cn.hutool.crypto.asymmetric.Sign` | `String signHex(byte[] data)` | 生成签名，并转为16进制字符串 |
| `cn.hutool.crypto.asymmetric.Sign` | `boolean verify(byte[] data,byte[] sign)` | 用公钥检验数字签名的合法性 |
| `cn.hutool.crypto.asymmetric.Sign` | `byte[] sign(InputStream data)` | 生成签名，使用默认缓存大小，见 IoUtil#DEFAULT_BUFFER_SIZE |
| `cn.hutool.crypto.asymmetric.Sign` | `byte[] sign(InputStream data,int bufferLength)` | 生成签名 |
| `cn.hutool.crypto.asymmetric.Sign` | `byte[] sign(String data)` | 生成文件签名 |
| `cn.hutool.crypto.asymmetric.Sign` | `byte[] sign(String data,Charset charset)` | 生成文件签名 |
| `cn.hutool.crypto.asymmetric.Sign` | `byte[] sign(byte[] data)` | 用私钥对信息生成数字签名 |
| `cn.hutool.crypto.asymmetric.SignAlgorithm` | `String getValue()` | 获取算法字符串表示，区分大小写 |
