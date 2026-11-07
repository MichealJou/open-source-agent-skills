# cn.hutool.crypto

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.crypto.ASN1Util` | `ASN1Object decode(InputStream in)` | 读取ASN.1数据流为ASN1Object |
| `cn.hutool.crypto.ASN1Util` | `String getDumpStr(InputStream in)` | 获取ASN1格式的导出格式，一般用于调试 |
| `cn.hutool.crypto.ASN1Util` | `byte[] encode(String asn1Encoding,ASN1Encodable... elements)` | 编码为指定ASN1格式 |
| `cn.hutool.crypto.ASN1Util` | `byte[] encodeDer(ASN1Encodable... elements)` | 编码为DER格式 |
| `cn.hutool.crypto.ASN1Util` | `void encodeTo(String asn1Encoding,OutputStream out,ASN1Encodable... elements)` | 编码为指定ASN1格式 |
| `cn.hutool.crypto.BCUtil` | `AsymmetricKeyParameter toParams(Key key)` | 密钥转换为AsymmetricKeyParameter |
| `cn.hutool.crypto.BCUtil` | `ECDomainParameters toDomainParams(ECParameterSpec parameterSpec)` | 构建ECDomainParameters对象 |
| `cn.hutool.crypto.BCUtil` | `ECDomainParameters toDomainParams(String curveName)` | 构建ECDomainParameters对象 |
| `cn.hutool.crypto.BCUtil` | `ECDomainParameters toDomainParams(X9ECParameters x9ECParameters)` | 构建ECDomainParameters对象 |
| `cn.hutool.crypto.BCUtil` | `ECPrivateKeyParameters toParams(BigInteger d,ECDomainParameters domainParameters)` | 转换为 ECPrivateKeyParameters |
| `cn.hutool.crypto.BCUtil` | `ECPrivateKeyParameters toParams(PrivateKey privateKey)` | 私钥转换为 ECPrivateKeyParameters |
| `cn.hutool.crypto.BCUtil` | `ECPrivateKeyParameters toParams(String dHex,ECDomainParameters domainParameters)` | 转换为 ECPrivateKeyParameters |
| `cn.hutool.crypto.BCUtil` | `ECPrivateKeyParameters toParams(byte[] d,ECDomainParameters domainParameters)` | 转换为 ECPrivateKeyParameters |
| `cn.hutool.crypto.BCUtil` | `ECPrivateKeyParameters toSm2Params(BigInteger d)` | 转换为 ECPrivateKeyParameters |
| `cn.hutool.crypto.BCUtil` | `ECPrivateKeyParameters toSm2Params(String d)` | 转换为 ECPrivateKeyParameters |
| `cn.hutool.crypto.BCUtil` | `ECPrivateKeyParameters toSm2Params(byte[] d)` | 转换为 ECPrivateKeyParameters |
| `cn.hutool.crypto.BCUtil` | `ECPublicKeyParameters toParams(BigInteger x,BigInteger y,ECDomainParameters domainParameters)` | 转换为ECPublicKeyParameters |
| `cn.hutool.crypto.BCUtil` | `ECPublicKeyParameters toParams(PublicKey publicKey)` | 公钥转换为 ECPublicKeyParameters |
| `cn.hutool.crypto.BCUtil` | `ECPublicKeyParameters toParams(String xHex,String yHex,ECDomainParameters domainParameters)` | 转换为ECPublicKeyParameters |
| `cn.hutool.crypto.BCUtil` | `ECPublicKeyParameters toParams(byte[] xBytes,byte[] yBytes,ECDomainParameters domainParameters)` | 转换为ECPublicKeyParameters |
| `cn.hutool.crypto.BCUtil` | `ECPublicKeyParameters toSm2Params(String xHex,String yHex)` | 转换为SM2的ECPublicKeyParameters |
| `cn.hutool.crypto.BCUtil` | `ECPublicKeyParameters toSm2Params(byte[] xBytes,byte[] yBytes)` | 转换为SM2的ECPublicKeyParameters |
| `cn.hutool.crypto.BCUtil` | `PrivateKey decodeECPrivateKey(final byte[] d,final String curveName)` | 解码恢复EC私钥,支持Base64和Hex编码,（基于BouncyCastle） |
| `cn.hutool.crypto.BCUtil` | `PrivateKey readPemPrivateKey(InputStream pemStream)` | 读取PEM格式的私钥 |
| `cn.hutool.crypto.BCUtil` | `PublicKey decodeECPoint(String encode,String curveName)` | 解码恢复EC压缩公钥,支持Base64和Hex编码,（基于BouncyCastle） 见：https://www.cnblogs.com/xinzhao/p/8963724.html |
| `cn.hutool.crypto.BCUtil` | `PublicKey decodeECPoint(byte[] encodeByte,String curveName)` | 解码恢复EC压缩公钥,支持Base64和Hex编码,（基于BouncyCastle） |
| `cn.hutool.crypto.BCUtil` | `PublicKey readPemPublicKey(InputStream pemStream)` | 读取PEM格式的公钥 |
| `cn.hutool.crypto.BCUtil` | `byte[] encodeECPrivateKey(PrivateKey privateKey)` | 只获取私钥里的d，32字节 |
| `cn.hutool.crypto.BCUtil` | `byte[] encodeECPublicKey(PublicKey publicKey)` | 编码压缩EC公钥（基于BouncyCastle），即Q值 见：https://www.cnblogs.com/xinzhao/p/8963724.html |
| `cn.hutool.crypto.BCUtil` | `byte[] encodeECPublicKey(PublicKey publicKey,boolean isCompressed)` | 编码压缩EC公钥（基于BouncyCastle），即Q值 见：https://www.cnblogs.com/xinzhao/p/8963724.html |
| `cn.hutool.crypto.BCUtil` | `byte[] toPkcs1(PrivateKey privateKey)` | Java中的PKCS#8格式私钥转换为OpenSSL支持的PKCS#1格式 |
| `cn.hutool.crypto.BCUtil` | `byte[] toPkcs1(PublicKey publicKey)` | Java中的X.509格式公钥转换为OpenSSL支持的PKCS#1格式 |
| `cn.hutool.crypto.CipherMode` | `int getValue()` | 获取枚举值对应的int表示 |
| `cn.hutool.crypto.CipherWrapper` | `AlgorithmParameterSpec getParams()` | 获取AlgorithmParameterSpec 在某些算法中，需要特别的参数，例如在ECIES中，此处为IESParameterSpec |
| `cn.hutool.crypto.CipherWrapper` | `Cipher getCipher()` | 获取被包装的Cipher |
| `cn.hutool.crypto.CipherWrapper` | `CipherWrapper initMode(int mode,Key key)` | 初始化Cipher为加密或者解密模式 |
| `cn.hutool.crypto.CipherWrapper` | `CipherWrapper setParams(AlgorithmParameterSpec params)` | 设置 AlgorithmParameterSpec，通常用于加盐或偏移向量 |
| `cn.hutool.crypto.CipherWrapper` | `CipherWrapper setRandom(SecureRandom random)` | 设置随机数生成器，可自定义随机数种子 |
| `cn.hutool.crypto.ECKeyUtil` | `AsymmetricKeyParameter toParams(Key key)` | 密钥转换为AsymmetricKeyParameter |
| `cn.hutool.crypto.ECKeyUtil` | `ECPrivateKeyParameters decodePrivateKeyParams(byte[] privateKeyBytes)` | 尝试解析转换各种类型私钥为ECPrivateKeyParameters，支持包括： D值 PKCS#8 PKCS#1 |
| `cn.hutool.crypto.ECKeyUtil` | `ECPrivateKeyParameters toPrivateParams(BigInteger d,ECDomainParameters domainParameters)` | 转换为 ECPrivateKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPrivateKeyParameters toPrivateParams(PrivateKey privateKey)` | 私钥转换为 ECPrivateKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPrivateKeyParameters toPrivateParams(String d,ECDomainParameters domainParameters)` | 转换为 ECPrivateKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPrivateKeyParameters toPrivateParams(byte[] d,ECDomainParameters domainParameters)` | 转换为 ECPrivateKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPrivateKeyParameters toSm2PrivateParams(BigInteger d)` | 转换为 ECPrivateKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPrivateKeyParameters toSm2PrivateParams(String d)` | 转换为 ECPrivateKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPrivateKeyParameters toSm2PrivateParams(byte[] d)` | 转换为 ECPrivateKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPublicKeyParameters decodePublicKeyParams(byte[] publicKeyBytes)` | 尝试解析转换各种类型公钥为ECPublicKeyParameters，支持包括： Q值 X.509 PKCS#1 |
| `cn.hutool.crypto.ECKeyUtil` | `ECPublicKeyParameters getPublicParams(ECPrivateKeyParameters privateKeyParameters)` | 根据私钥参数获取公钥参数 |
| `cn.hutool.crypto.ECKeyUtil` | `ECPublicKeyParameters toPublicParams(BigInteger x,BigInteger y,ECDomainParameters domainParameters)` | 转换为ECPublicKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPublicKeyParameters toPublicParams(PublicKey publicKey)` | 公钥转换为 ECPublicKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPublicKeyParameters toPublicParams(String pointEncoded,ECDomainParameters domainParameters)` | 转换为ECPublicKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPublicKeyParameters toPublicParams(String x,String y,ECDomainParameters domainParameters)` | 转换为ECPublicKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPublicKeyParameters toPublicParams(byte[] pointEncoded,ECDomainParameters domainParameters)` | 转换为ECPublicKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPublicKeyParameters toPublicParams(byte[] xBytes,byte[] yBytes,ECDomainParameters domainParameters)` | 转换为ECPublicKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPublicKeyParameters toPublicParams(org.bouncycastle.math.ec.ECPoint point,ECDomainParameters domainParameters)` | 转换为ECPublicKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPublicKeyParameters toSm2PublicParams(String q)` | 转换为 ECPublicKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPublicKeyParameters toSm2PublicParams(String x,String y)` | 转换为SM2的ECPublicKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPublicKeyParameters toSm2PublicParams(byte[] q)` | 转换为 ECPublicKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `ECPublicKeyParameters toSm2PublicParams(byte[] xBytes,byte[] yBytes)` | 转换为SM2的ECPublicKeyParameters |
| `cn.hutool.crypto.ECKeyUtil` | `KeySpec createOpenSSHPrivateKeySpec(byte[] key)` | 创建OpenSSHPrivateKeySpec |
| `cn.hutool.crypto.ECKeyUtil` | `KeySpec createOpenSSHPublicKeySpec(byte[] key)` | 创建OpenSSHPublicKeySpec |
| `cn.hutool.crypto.ECKeyUtil` | `PrivateKey toSm2PrivateKey(ECPrivateKey privateKey)` | 将SM2算法的ECPrivateKey 转换为 PrivateKey |
| `cn.hutool.crypto.GlobalBouncyCastleProvider` | `Provider getProvider()` | 获取Provider |
| `cn.hutool.crypto.GlobalBouncyCastleProvider` | `void setUseBouncyCastle(boolean isUseBouncyCastle)` | 设置是否使用Bouncy Castle库 如果设置为false，表示强制关闭Bouncy Castle而使用JDK |
| `cn.hutool.crypto.KeyUtil` | `Certificate getCertificate(KeyStore keyStore,String alias)` | 获得 Certification |
| `cn.hutool.crypto.KeyUtil` | `Certificate readCertificate(String type,InputStream in)` | 读取Certification文件 Certification为证书文件 see: http://snowolf.iteye.com/blog/391931 |
| `cn.hutool.crypto.KeyUtil` | `Certificate readCertificate(String type,InputStream in,char[] password,String alias)` | 读取Certification文件 Certification为证书文件 see: http://snowolf.iteye.com/blog/391931 |
| `cn.hutool.crypto.KeyUtil` | `Certificate readX509Certificate(InputStream in)` | 读取X.509 Certification文件 Certification为证书文件 see: http://snowolf.iteye.com/blog/391931 |
| `cn.hutool.crypto.KeyUtil` | `Certificate readX509Certificate(InputStream in,char[] password,String alias)` | 读取X.509 Certification文件 Certification为证书文件 see: http://snowolf.iteye.com/blog/391931 |
| `cn.hutool.crypto.KeyUtil` | `CertificateFactory getCertificateFactory(String type)` | 获取CertificateFactory |
| `cn.hutool.crypto.KeyUtil` | `KeyFactory getKeyFactory(String algorithm)` | 获取KeyFactory |
| `cn.hutool.crypto.KeyUtil` | `KeyGenerator getKeyGenerator(String algorithm)` | 获取KeyGenerator |
| `cn.hutool.crypto.KeyUtil` | `KeyPair generateKeyPair(String algorithm)` | 生成用于非对称加密的公钥和私钥，仅用于非对称加密 密钥对生成算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyPairGenerator |
| `cn.hutool.crypto.KeyUtil` | `KeyPair generateKeyPair(String algorithm,AlgorithmParameterSpec params)` | 生成用于非对称加密的公钥和私钥 密钥对生成算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyPairGenerator |
| `cn.hutool.crypto.KeyUtil` | `KeyPair generateKeyPair(String algorithm,byte[] seed,AlgorithmParameterSpec param)` | 生成用于非对称加密的公钥和私钥 密钥对生成算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyPairGenerator |
| `cn.hutool.crypto.KeyUtil` | `KeyPair generateKeyPair(String algorithm,int keySize)` | 生成用于非对称加密的公钥和私钥 密钥对生成算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyPairGenerator |
| `cn.hutool.crypto.KeyUtil` | `KeyPair generateKeyPair(String algorithm,int keySize,SecureRandom random,AlgorithmParameterSpec... params)` | 生成用于非对称加密的公钥和私钥 密钥对生成算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyPairGenerator 对于非对称加密算法，密钥长度有严格限制，具体如下： RSA： |
| `cn.hutool.crypto.KeyUtil` | `KeyPair generateKeyPair(String algorithm,int keySize,byte[] seed)` | 生成用于非对称加密的公钥和私钥 密钥对生成算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyPairGenerator |
| `cn.hutool.crypto.KeyUtil` | `KeyPair generateKeyPair(String algorithm,int keySize,byte[] seed,AlgorithmParameterSpec... params)` | 生成用于非对称加密的公钥和私钥 密钥对生成算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyPairGenerator 对于非对称加密算法，密钥长度有严格限制，具体如下： RSA： |
| `cn.hutool.crypto.KeyUtil` | `KeyPair getKeyPair(KeyStore keyStore,char[] password,String alias)` | 从KeyStore中获取私钥公钥 |
| `cn.hutool.crypto.KeyUtil` | `KeyPair getKeyPair(String type,InputStream in,char[] password,String alias)` | 从KeyStore中获取私钥公钥 |
| `cn.hutool.crypto.KeyUtil` | `KeyPairGenerator getKeyPairGenerator(String algorithm)` | 获取KeyPairGenerator |
| `cn.hutool.crypto.KeyUtil` | `KeyStore getKeyStore(final String type)` | 获取KeyStore对象 |
| `cn.hutool.crypto.KeyUtil` | `KeyStore readJKSKeyStore(File keyFile,char[] password)` | 读取密钥库(Java Key Store，JKS) KeyStore文件 KeyStore文件用于数字证书的密钥对保存 see: http://snowolf.iteye.com/blog/391931 |
| `cn.hutool.crypto.KeyUtil` | `KeyStore readJKSKeyStore(InputStream in,char[] password)` | 读取密钥库(Java Key Store，JKS) KeyStore文件 KeyStore文件用于数字证书的密钥对保存 see: http://snowolf.iteye.com/blog/391931 |
| `cn.hutool.crypto.KeyUtil` | `KeyStore readKeyStore(String type,File keyFile,char[] password)` | 读取KeyStore文件 KeyStore文件用于数字证书的密钥对保存 see: http://snowolf.iteye.com/blog/391931 |
| `cn.hutool.crypto.KeyUtil` | `KeyStore readKeyStore(String type,InputStream in,char[] password)` | 读取KeyStore文件 KeyStore文件用于数字证书的密钥对保存 see: http://snowolf.iteye.com/blog/391931 |
| `cn.hutool.crypto.KeyUtil` | `KeyStore readPKCS12KeyStore(File keyFile,char[] password)` | 读取PKCS12 KeyStore文件 KeyStore文件用于数字证书的密钥对保存 |
| `cn.hutool.crypto.KeyUtil` | `KeyStore readPKCS12KeyStore(InputStream in,char[] password)` | 读取PKCS12 KeyStore文件 KeyStore文件用于数字证书的密钥对保存 |
| `cn.hutool.crypto.KeyUtil` | `PrivateKey generatePrivateKey(KeyStore keyStore,String alias,char[] password)` | 生成私钥，仅用于非对称加密 |
| `cn.hutool.crypto.KeyUtil` | `PrivateKey generatePrivateKey(String algorithm,KeySpec keySpec)` | 生成私钥，仅用于非对称加密 算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyFactory |
| `cn.hutool.crypto.KeyUtil` | `PrivateKey generatePrivateKey(String algorithm,byte[] key)` | 生成私钥，仅用于非对称加密 采用PKCS#8规范，此规范定义了私钥信息语法和加密私钥语法 算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyFactory |
| `cn.hutool.crypto.KeyUtil` | `PrivateKey generateRSAPrivateKey(String key)` | 生成RSA私钥，仅用于非对称加密 算法见： ... |
| `cn.hutool.crypto.KeyUtil` | `PrivateKey generateRSAPrivateKey(byte[] key)` | 生成RSA私钥，仅用于非对称加密 采用PKCS#8规范，此规范定义了私钥信息语法和加密私钥语法 算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyFactory |
| `cn.hutool.crypto.KeyUtil` | `PrivateKey generateRSAPrivateKey(final KeySpec keySpec)` | 生成RSA私钥，仅用于非对称加密 算法见： ... |
| `cn.hutool.crypto.KeyUtil` | `PublicKey decodeECPoint(String encode,String curveName)` | 解码恢复EC压缩公钥,支持Base64和Hex编码,（基于BouncyCastle） 见：https://www.cnblogs.com/xinzhao/p/8963724.html |
| `cn.hutool.crypto.KeyUtil` | `PublicKey decodeECPoint(byte[] encodeByte,String curveName)` | 解码恢复EC压缩公钥,支持Base64和Hex编码,（基于BouncyCastle） 见：https://www.cnblogs.com/xinzhao/p/8963724.html |
| `cn.hutool.crypto.KeyUtil` | `PublicKey generatePublicKey(String algorithm,KeySpec keySpec)` | 生成公钥，仅用于非对称加密 算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyFactory |
| `cn.hutool.crypto.KeyUtil` | `PublicKey generatePublicKey(String algorithm,byte[] key)` | 生成公钥，仅用于非对称加密 采用X509证书规范 算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyFactory |
| `cn.hutool.crypto.KeyUtil` | `PublicKey generateRSAPublicKey(byte[] key)` | 生成RSA公钥，仅用于非对称加密 采用X509证书规范 算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyFactory |
| `cn.hutool.crypto.KeyUtil` | `PublicKey getRSAPublicKey(BigInteger modulus,BigInteger publicExponent)` | 获得RSA公钥对象 |
| `cn.hutool.crypto.KeyUtil` | `PublicKey getRSAPublicKey(PrivateKey privateKey)` | 通过RSA私钥生成RSA公钥 |
| `cn.hutool.crypto.KeyUtil` | `PublicKey getRSAPublicKey(String modulus,String publicExponent)` | 获得RSA公钥对象 |
| `cn.hutool.crypto.KeyUtil` | `PublicKey readPublicKeyFromCert(InputStream in)` | 读取X.509 Certification文件中的公钥 Certification为证书文件 see: https://www.cnblogs.com/yinliang/p/10115519.html |
| `cn.hutool.crypto.KeyUtil` | `SecretKey generateDESKey(String algorithm,byte[] key)` | 生成 SecretKey |
| `cn.hutool.crypto.KeyUtil` | `SecretKey generateKey(String algorithm)` | 生成 SecretKey，仅用于对称加密和摘要算法密钥生成 |
| `cn.hutool.crypto.KeyUtil` | `SecretKey generateKey(String algorithm,KeySpec keySpec)` | 生成 SecretKey，仅用于对称加密和摘要算法 |
| `cn.hutool.crypto.KeyUtil` | `SecretKey generateKey(String algorithm,byte[] key)` | 生成 SecretKey，仅用于对称加密和摘要算法密钥生成 |
| `cn.hutool.crypto.KeyUtil` | `SecretKey generateKey(String algorithm,int keySize)` | 生成 SecretKey，仅用于对称加密和摘要算法密钥生成 当指定keySize<0时，AES默认长度为128，其它算法不指定。 |
| `cn.hutool.crypto.KeyUtil` | `SecretKey generateKey(String algorithm,int keySize,SecureRandom random)` | 生成 SecretKey，仅用于对称加密和摘要算法密钥生成 当指定keySize<0时，AES默认长度为128，其它算法不指定。 |
| `cn.hutool.crypto.KeyUtil` | `SecretKey generatePBEKey(String algorithm,char[] key)` | 生成PBE SecretKey |
| `cn.hutool.crypto.KeyUtil` | `SecretKeyFactory getSecretKeyFactory(String algorithm)` | 获取SecretKeyFactory |
| `cn.hutool.crypto.KeyUtil` | `String getAlgorithmAfterWith(String algorithm)` | 获取用于密钥生成的算法 获取XXXwithXXX算法的后半部分算法，如果为ECDSA或SM2，返回算法为EC |
| `cn.hutool.crypto.KeyUtil` | `String getMainAlgorithm(String algorithm)` | 获取主体算法名，例如RSA/ECB/PKCS1Padding的主体算法是RSA |
| `cn.hutool.crypto.KeyUtil` | `String toBase64(Key key)` | 将密钥编码为Base64格式 |
| `cn.hutool.crypto.KeyUtil` | `byte[] encodeECPublicKey(PublicKey publicKey)` | 编码压缩EC公钥（基于BouncyCastle） 见：https://www.cnblogs.com/xinzhao/p/8963724.html |
| `cn.hutool.crypto.OpensslKeyUtil` | `Key readPemKey(final InputStream keyStream,final char[] password)` | 从pem文件中读取公钥或私钥 根据类型返回 PublicKey 或者 PrivateKey |
| `cn.hutool.crypto.OpensslKeyUtil` | `KeyPair getKeyPair(final PEMKeyPair keyPair)` | 转换PEMKeyPair为KeyPair |
| `cn.hutool.crypto.OpensslKeyUtil` | `PEMKeyPair decrypt(final PEMEncryptedKeyPair pemEncryptedKeyPair,final char[] password)` | 解密PEMEncryptedKeyPair为PEMKeyPair |
| `cn.hutool.crypto.OpensslKeyUtil` | `PrivateKey getPrivateKey(final PrivateKeyInfo privateKeyInfo)` | 转换PrivateKeyInfo为PrivateKey |
| `cn.hutool.crypto.OpensslKeyUtil` | `PrivateKeyInfo decrypt(final PKCS8EncryptedPrivateKeyInfo pkcs8Info,final char[] password)` | 解密PKCS8EncryptedPrivateKeyInfo为PrivateKeyInfo |
| `cn.hutool.crypto.OpensslKeyUtil` | `PublicKey getPublicKey(final SubjectPublicKeyInfo publicKeyInfo)` | 转换SubjectPublicKeyInfo为PublicKey |
| `cn.hutool.crypto.PemUtil` | `Key readPemKey(InputStream keyStream)` | 从pem文件中读取公钥或私钥 根据类型返回 PublicKey 或者 PrivateKey |
| `cn.hutool.crypto.PemUtil` | `PemObject readPemObject(InputStream keyStream)` | 读取pem文件中的信息，包括类型、头信息和密钥内容 |
| `cn.hutool.crypto.PemUtil` | `PemObject readPemObject(Reader reader)` | 读取pem文件中的信息，包括类型、头信息和密钥内容 |
| `cn.hutool.crypto.PemUtil` | `PrivateKey readPemPrivateKey(InputStream pemStream)` | 读取PEM格式的私钥，支持PKCS#8和PKCS#1的ECC格式 |
| `cn.hutool.crypto.PemUtil` | `PrivateKey readSm2PemPrivateKey(InputStream keyStream)` | 读取OpenSSL生成的ANS1格式的Pem私钥文件，必须为PKCS#1格式 |
| `cn.hutool.crypto.PemUtil` | `PublicKey readPemPublicKey(InputStream pemStream)` | 读取PEM格式的公钥 |
| `cn.hutool.crypto.PemUtil` | `String toPem(String type,byte[] content)` | 将私钥或公钥转换为PEM格式的字符串 |
| `cn.hutool.crypto.PemUtil` | `byte[] readPem(InputStream keyStream)` | 从pem流中读取公钥或私钥 |
| `cn.hutool.crypto.PemUtil` | `void writePemObject(PemObjectGenerator pemObject,OutputStream keyStream)` | 写出pem密钥（私钥、公钥、证书） |
| `cn.hutool.crypto.PemUtil` | `void writePemObject(PemObjectGenerator pemObject,Writer writer)` | 写出pem密钥（私钥、公钥、证书） |
| `cn.hutool.crypto.PemUtil` | `void writePemObject(String type,byte[] content,OutputStream keyStream)` | 写出pem密钥（私钥、公钥、证书） |
| `cn.hutool.crypto.PemUtil` | `void writePemObject(String type,byte[] content,Writer writer)` | 写出pem密钥（私钥、公钥、证书） |
| `cn.hutool.crypto.ProviderFactory` | `Provider createBouncyCastleProvider()` | 创建Bouncy Castle 提供者 如果用户未引入bouncycastle库，则此方法抛出NoClassDefFoundError 异常 |
| `cn.hutool.crypto.SecureUtil` | `AES aes()` | AES加密，生成随机KEY。注意解密时必须使用相同 AES对象或者使用相同KEY 例： |
| `cn.hutool.crypto.SecureUtil` | `AES aes(byte[] key)` | AES加密 例： |
| `cn.hutool.crypto.SecureUtil` | `Certificate getCertificate(KeyStore keyStore,String alias)` | 获得 Certification |
| `cn.hutool.crypto.SecureUtil` | `Certificate readCertificate(String type,InputStream in)` | 读取Certification文件 Certification为证书文件 see: http://snowolf.iteye.com/blog/391931 |
| `cn.hutool.crypto.SecureUtil` | `Certificate readCertificate(String type,InputStream in,char[] password,String alias)` | 读取Certification文件 Certification为证书文件 see: http://snowolf.iteye.com/blog/391931 |
| `cn.hutool.crypto.SecureUtil` | `Certificate readX509Certificate(InputStream in)` | 读取X.509 Certification文件 Certification为证书文件 see: http://snowolf.iteye.com/blog/391931 |
| `cn.hutool.crypto.SecureUtil` | `Certificate readX509Certificate(InputStream in,char[] password,String alias)` | 读取X.509 Certification文件 Certification为证书文件 see: http://snowolf.iteye.com/blog/391931 |
| `cn.hutool.crypto.SecureUtil` | `Cipher createCipher(String algorithm)` | 创建Cipher |
| `cn.hutool.crypto.SecureUtil` | `DES des()` | DES加密，生成随机KEY。注意解密时必须使用相同 DES对象或者使用相同KEY 例： |
| `cn.hutool.crypto.SecureUtil` | `DES des(byte[] key)` | DES加密 例： |
| `cn.hutool.crypto.SecureUtil` | `DESede desede()` | DESede加密（又名3DES、TripleDES），生成随机KEY。注意解密时必须使用相同 DESede对象或者使用相同KEY Java中默认实现为：DESede/ECB/PKCS5Padding 例： |
| `cn.hutool.crypto.SecureUtil` | `DESede desede(byte[] key)` | DESede加密（又名3DES、TripleDES） Java中默认实现为：DESede/ECB/PKCS5Padding 例： |
| `cn.hutool.crypto.SecureUtil` | `Digester sha1()` | SHA1加密 例： SHA1加密：sha1().digest(data) SHA1加密并转为16进制字符串：sha1().digestHex(data) |
| `cn.hutool.crypto.SecureUtil` | `Digester sha256()` | SHA256加密 例： SHA256加密：sha256().digest(data) SHA256加密并转为16进制字符串：sha256().digestHex(data) |
| `cn.hutool.crypto.SecureUtil` | `FPE fpe(FPE.FPEMode mode,byte[] key,AlphabetMapper mapper,byte[] tweak)` | FPE(Format Preserving Encryption)实现，支持FF1和FF3-1模式。 |
| `cn.hutool.crypto.SecureUtil` | `HMac hmac(HmacAlgorithm algorithm,SecretKey key)` | 创建HMac对象，调用digest方法可获得hmac值 |
| `cn.hutool.crypto.SecureUtil` | `HMac hmac(HmacAlgorithm algorithm,String key)` | 创建HMac对象，调用digest方法可获得hmac值 |
| `cn.hutool.crypto.SecureUtil` | `HMac hmac(HmacAlgorithm algorithm,byte[] key)` | 创建HMac对象，调用digest方法可获得hmac值 |
| `cn.hutool.crypto.SecureUtil` | `HMac hmacMd5()` | HmacMD5加密器，生成随机KEY 例： HmacMD5加密：hmacMd5().digest(data) HmacMD5加密并转为16进制字符串：hmacMd5().digestHex(data) |
| `cn.hutool.crypto.SecureUtil` | `HMac hmacMd5(String key)` | HmacMD5加密器 例： HmacMD5加密：hmacMd5(key).digest(data) HmacMD5加密并转为16进制字符串：hmacMd5(key).digestHex(data) |
| `cn.hutool.crypto.SecureUtil` | `HMac hmacMd5(byte[] key)` | HmacMD5加密器 例： HmacMD5加密：hmacMd5(key).digest(data) HmacMD5加密并转为16进制字符串：hmacMd5(key).digestHex(data) |
| `cn.hutool.crypto.SecureUtil` | `HMac hmacSha1()` | HmacSHA1加密器，生成随机KEY 例： HmacSHA1加密：hmacSha1().digest(data) HmacSHA1加密并转为16进制字符串：hmacSha1().digestHex(data) |
| `cn.hutool.crypto.SecureUtil` | `HMac hmacSha1(String key)` | HmacSHA1加密器 例： HmacSHA1加密：hmacSha1(key).digest(data) HmacSHA1加密并转为16进制字符串：hmacSha1(key).digestHex(data) |
| `cn.hutool.crypto.SecureUtil` | `HMac hmacSha1(byte[] key)` | HmacSHA1加密器 例： HmacSHA1加密：hmacSha1(key).digest(data) HmacSHA1加密并转为16进制字符串：hmacSha1(key).digestHex(data) |
| `cn.hutool.crypto.SecureUtil` | `HMac hmacSha256()` | HmacSHA256加密器，生成随机KEY 例： HmacSHA256加密：hmacSha256().digest(data) HmacSHA256加密并转为16进制字符串：hmacSha256().digestHex(data) |
| `cn.hutool.crypto.SecureUtil` | `HMac hmacSha256(String key)` | HmacSHA256加密器 例： HmacSHA256加密：hmacSha256(key).digest(data) HmacSHA256加密并转为16进制字符串：hmacSha256(key).digestHex(data) |
| `cn.hutool.crypto.SecureUtil` | `HMac hmacSha256(byte[] key)` | HmacSHA256加密器 例： HmacSHA256加密：hmacSha256(key).digest(data) HmacSHA256加密并转为16进制字符串：hmacSha256(key).digestHex(data) |
| `cn.hutool.crypto.SecureUtil` | `KeyPair generateKeyPair(String algorithm)` | 生成用于非对称加密的公钥和私钥，仅用于非对称加密 密钥对生成算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyPairGenerator |
| `cn.hutool.crypto.SecureUtil` | `KeyPair generateKeyPair(String algorithm,AlgorithmParameterSpec params)` | 生成用于非对称加密的公钥和私钥 密钥对生成算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyPairGenerator |
| `cn.hutool.crypto.SecureUtil` | `KeyPair generateKeyPair(String algorithm,byte[] seed,AlgorithmParameterSpec params)` | 生成用于非对称加密的公钥和私钥 密钥对生成算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyPairGenerator |
| `cn.hutool.crypto.SecureUtil` | `KeyPair generateKeyPair(String algorithm,int keySize)` | 生成用于非对称加密的公钥和私钥 密钥对生成算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyPairGenerator |
| `cn.hutool.crypto.SecureUtil` | `KeyPair generateKeyPair(String algorithm,int keySize,byte[] seed)` | 生成用于非对称加密的公钥和私钥 密钥对生成算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyPairGenerator |
| `cn.hutool.crypto.SecureUtil` | `KeyStore readJKSKeyStore(InputStream in,char[] password)` | 读取密钥库(Java Key Store，JKS) KeyStore文件 KeyStore文件用于数字证书的密钥对保存 see: http://snowolf.iteye.com/blog/391931 |
| `cn.hutool.crypto.SecureUtil` | `KeyStore readKeyStore(String type,InputStream in,char[] password)` | 读取KeyStore文件 KeyStore文件用于数字证书的密钥对保存 see: http://snowolf.iteye.com/blog/391931 |
| `cn.hutool.crypto.SecureUtil` | `MD5 md5()` | MD5加密 例： |
| `cn.hutool.crypto.SecureUtil` | `Mac createMac(String algorithm)` | 创建Mac |
| `cn.hutool.crypto.SecureUtil` | `MessageDigest createJdkMessageDigest(final String algorithm)` | 创建MessageDigest，使用JDK默认的Provider |
| `cn.hutool.crypto.SecureUtil` | `MessageDigest createMessageDigest(String algorithm)` | 创建MessageDigest |
| `cn.hutool.crypto.SecureUtil` | `PrivateKey generatePrivateKey(KeyStore keyStore,String alias,char[] password)` | 生成私钥，仅用于非对称加密 |
| `cn.hutool.crypto.SecureUtil` | `PrivateKey generatePrivateKey(String algorithm,KeySpec keySpec)` | 生成私钥，仅用于非对称加密 算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyFactory |
| `cn.hutool.crypto.SecureUtil` | `PrivateKey generatePrivateKey(String algorithm,byte[] key)` | 生成私钥，仅用于非对称加密 算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyFactory |
| `cn.hutool.crypto.SecureUtil` | `PublicKey generatePublicKey(String algorithm,KeySpec keySpec)` | 生成公钥，仅用于非对称加密 算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyFactory |
| `cn.hutool.crypto.SecureUtil` | `PublicKey generatePublicKey(String algorithm,byte[] key)` | 生成公钥，仅用于非对称加密 算法见：https://docs.oracle.com/javase/7/docs/technotes/guides/security/StandardNames.html#KeyFactory |
| `cn.hutool.crypto.SecureUtil` | `RC4 rc4(String key)` | RC4算法 |
| `cn.hutool.crypto.SecureUtil` | `RSA rsa()` | 创建RSA算法对象 生成新的私钥公钥对 |
| `cn.hutool.crypto.SecureUtil` | `RSA rsa(String privateKeyBase64,String publicKeyBase64)` | 创建RSA算法对象 私钥和公钥同时为空时生成一对新的私钥和公钥 私钥和公钥可以单独传入一个，如此则只能使用此钥匙来做加密或者解密 |
| `cn.hutool.crypto.SecureUtil` | `RSA rsa(byte[] privateKey,byte[] publicKey)` | 创建RSA算法对象 私钥和公钥同时为空时生成一对新的私钥和公钥 私钥和公钥可以单独传入一个，如此则只能使用此钥匙来做加密或者解密 |
| `cn.hutool.crypto.SecureUtil` | `SecretKey generateDESKey(String algorithm,byte[] key)` | 生成 SecretKey |
| `cn.hutool.crypto.SecureUtil` | `SecretKey generateKey(String algorithm)` | 生成 SecretKey，仅用于对称加密和摘要算法密钥生成 |
| `cn.hutool.crypto.SecureUtil` | `SecretKey generateKey(String algorithm,KeySpec keySpec)` | 生成 SecretKey，仅用于对称加密和摘要算法 |
| `cn.hutool.crypto.SecureUtil` | `SecretKey generateKey(String algorithm,byte[] key)` | 生成 SecretKey，仅用于对称加密和摘要算法密钥生成 |
| `cn.hutool.crypto.SecureUtil` | `SecretKey generateKey(String algorithm,int keySize)` | 生成 SecretKey，仅用于对称加密和摘要算法密钥生成 |
| `cn.hutool.crypto.SecureUtil` | `SecretKey generatePBEKey(String algorithm,char[] key)` | 生成PBE SecretKey |
| `cn.hutool.crypto.SecureUtil` | `Sign sign(SignAlgorithm algorithm)` | 创建签名算法对象 生成新的私钥公钥对 |
| `cn.hutool.crypto.SecureUtil` | `Sign sign(SignAlgorithm algorithm,String privateKeyBase64,String publicKeyBase64)` | 创建签名算法对象 私钥和公钥同时为空时生成一对新的私钥和公钥 私钥和公钥可以单独传入一个，如此则只能使用此钥匙来做签名或验证 |
| `cn.hutool.crypto.SecureUtil` | `Sign sign(SignAlgorithm algorithm,byte[] privateKey,byte[] publicKey)` | 创建Sign算法对象 私钥和公钥同时为空时生成一对新的私钥和公钥 私钥和公钥可以单独传入一个，如此则只能使用此钥匙来做签名或验证 |
| `cn.hutool.crypto.SecureUtil` | `Signature createSignature(String algorithm)` | 创建Signature |
| `cn.hutool.crypto.SecureUtil` | `Signature generateSignature(AsymmetricAlgorithm asymmetricAlgorithm,DigestAlgorithm digestAlgorithm)` | 生成签名对象，仅用于非对称加密 |
| `cn.hutool.crypto.SecureUtil` | `String generateAlgorithm(AsymmetricAlgorithm asymmetricAlgorithm,DigestAlgorithm digestAlgorithm)` | 生成算法，格式为XXXwithXXX |
| `cn.hutool.crypto.SecureUtil` | `String getAlgorithmAfterWith(String algorithm)` | 获取用于密钥生成的算法 获取XXXwithXXX算法的后半部分算法，如果为ECDSA或SM2，返回算法为EC |
| `cn.hutool.crypto.SecureUtil` | `String md5(File dataFile)` | MD5加密文件，生成16进制MD5字符串 |
| `cn.hutool.crypto.SecureUtil` | `String md5(InputStream data)` | MD5加密，生成16进制MD5字符串 |
| `cn.hutool.crypto.SecureUtil` | `String md5(String data)` | MD5加密，生成16进制MD5字符串 |
| `cn.hutool.crypto.SecureUtil` | `String pbkdf2(char[] password,byte[] salt)` | PBKDF2加密密码 |
| `cn.hutool.crypto.SecureUtil` | `String sha1(File dataFile)` | SHA1加密文件，生成16进制SHA1字符串 |
| `cn.hutool.crypto.SecureUtil` | `String sha1(InputStream data)` | SHA1加密，生成16进制SHA1字符串 |
| `cn.hutool.crypto.SecureUtil` | `String sha1(String data)` | SHA1加密，生成16进制SHA1字符串 |
| `cn.hutool.crypto.SecureUtil` | `String sha256(File dataFile)` | SHA256加密文件，生成16进制SHA256字符串 |
| `cn.hutool.crypto.SecureUtil` | `String sha256(InputStream data)` | SHA256加密，生成16进制SHA256字符串 |
| `cn.hutool.crypto.SecureUtil` | `String sha256(String data)` | SHA256加密，生成16进制SHA256字符串 |
| `cn.hutool.crypto.SecureUtil` | `String signParams(DigestAlgorithm digestAlgorithm,Map<?, ?> params,String separator,String keyValueSeparator,boolean isIgnoreNull,String... otherParams)` | 对参数做签名 参数签名为对Map参数按照key的顺序排序后拼接为字符串，然后根据提供的签名算法生成签名字符串 |
| `cn.hutool.crypto.SecureUtil` | `String signParams(DigestAlgorithm digestAlgorithm,Map<?, ?> params,String... otherParams)` | 对参数做签名 参数签名为对Map参数按照key的顺序排序后拼接为字符串，然后根据提供的签名算法生成签名字符串 拼接后的字符串键值对之间无符号，键值对之间无符号，忽略null值 |
| `cn.hutool.crypto.SecureUtil` | `String signParams(SymmetricCrypto crypto,Map<?, ?> params,String separator,String keyValueSeparator,boolean isIgnoreNull,String... otherParams)` | 对参数做签名 参数签名为对Map参数按照key的顺序排序后拼接为字符串，然后根据提供的签名算法生成签名字符串 |
| `cn.hutool.crypto.SecureUtil` | `String signParams(SymmetricCrypto crypto,Map<?, ?> params,String... otherParams)` | 对参数做签名 参数签名为对Map参数按照key的顺序排序后拼接为字符串，然后根据提供的签名算法生成签名字符串 拼接后的字符串键值对之间无符号，键值对之间无符号，忽略null值 |
| `cn.hutool.crypto.SecureUtil` | `String signParamsMd5(Map<?, ?> params,String... otherParams)` | 对参数做md5签名 参数签名为对Map参数按照key的顺序排序后拼接为字符串，然后根据提供的签名算法生成签名字符串 拼接后的字符串键值对之间无符号，键值对之间无符号，忽略null值 |
| `cn.hutool.crypto.SecureUtil` | `String signParamsSha1(Map<?, ?> params,String... otherParams)` | 对参数做Sha1签名 参数签名为对Map参数按照key的顺序排序后拼接为字符串，然后根据提供的签名算法生成签名字符串 拼接后的字符串键值对之间无符号，键值对之间无符号，忽略null值 |
| `cn.hutool.crypto.SecureUtil` | `String signParamsSha256(Map<?, ?> params,String... otherParams)` | 对参数做Sha256签名 参数签名为对Map参数按照key的顺序排序后拼接为字符串，然后根据提供的签名算法生成签名字符串 拼接后的字符串键值对之间无符号，键值对之间无符号，忽略null值 |
| `cn.hutool.crypto.SecureUtil` | `ZUC zuc128(byte[] key,byte[] iv)` | 祖冲之算法集（ZUC-128算法）实现，基于BouncyCastle实现。 |
| `cn.hutool.crypto.SecureUtil` | `ZUC zuc256(byte[] key,byte[] iv)` | 祖冲之算法集（ZUC-256算法）实现，基于BouncyCastle实现。 |
| `cn.hutool.crypto.SecureUtil` | `byte[] decode(String key)` | 解码字符串密钥，可支持的编码如下： |
| `cn.hutool.crypto.SecureUtil` | `void addProvider(Provider provider)` | 增加加密解密的算法提供者，默认优先使用，例如： |
| `cn.hutool.crypto.SecureUtil` | `void disableBouncyCastle()` | 强制关闭Bouncy Castle库的使用，全局有效 |
| `cn.hutool.crypto.SignUtil` | `Sign sign(SignAlgorithm algorithm)` | 创建签名算法对象 生成新的私钥公钥对 |
| `cn.hutool.crypto.SignUtil` | `Sign sign(SignAlgorithm algorithm,String privateKeyBase64,String publicKeyBase64)` | 创建签名算法对象 私钥和公钥同时为空时生成一对新的私钥和公钥 私钥和公钥可以单独传入一个，如此则只能使用此钥匙来做签名或验证 |
| `cn.hutool.crypto.SignUtil` | `Sign sign(SignAlgorithm algorithm,byte[] privateKey,byte[] publicKey)` | 创建Sign算法对象 私钥和公钥同时为空时生成一对新的私钥和公钥 私钥和公钥可以单独传入一个，如此则只能使用此钥匙来做签名或验证 |
| `cn.hutool.crypto.SignUtil` | `String signParams(DigestAlgorithm digestAlgorithm,Map<?, ?> params,String separator,String keyValueSeparator,boolean isIgnoreNull,String... otherParams)` | 对参数做签名 参数签名为对Map参数按照key的顺序排序后拼接为字符串，然后根据提供的签名算法生成签名字符串 |
| `cn.hutool.crypto.SignUtil` | `String signParams(DigestAlgorithm digestAlgorithm,Map<?, ?> params,String... otherParams)` | 对参数做签名 参数签名为对Map参数按照key的顺序排序后拼接为字符串，然后根据提供的签名算法生成签名字符串 拼接后的字符串键值对之间无符号，键值对之间无符号，忽略null值 |
| `cn.hutool.crypto.SignUtil` | `String signParams(SymmetricCrypto crypto,Map<?, ?> params,String separator,String keyValueSeparator,boolean isIgnoreNull,String... otherParams)` | 对参数做签名 参数签名为对Map参数按照key的顺序排序后拼接为字符串，然后根据提供的签名算法生成签名字符串 |
| `cn.hutool.crypto.SignUtil` | `String signParams(SymmetricCrypto crypto,Map<?, ?> params,String... otherParams)` | 对参数做签名 参数签名为对Map参数按照key的顺序排序后拼接为字符串，然后根据提供的签名算法生成签名字符串 拼接后的字符串键值对之间无符号，键值对之间无符号，忽略null值 |
| `cn.hutool.crypto.SignUtil` | `String signParamsMd5(Map<?, ?> params,String... otherParams)` | 对参数做md5签名 参数签名为对Map参数按照key的顺序排序后拼接为字符串，然后根据提供的签名算法生成签名字符串 拼接后的字符串键值对之间无符号，键值对之间无符号，忽略null值 |
| `cn.hutool.crypto.SignUtil` | `String signParamsSha1(Map<?, ?> params,String... otherParams)` | 对参数做Sha1签名 参数签名为对Map参数按照key的顺序排序后拼接为字符串，然后根据提供的签名算法生成签名字符串 拼接后的字符串键值对之间无符号，键值对之间无符号，忽略null值 |
| `cn.hutool.crypto.SignUtil` | `String signParamsSha256(Map<?, ?> params,String... otherParams)` | 对参数做Sha256签名 参数签名为对Map参数按照key的顺序排序后拼接为字符串，然后根据提供的签名算法生成签名字符串 拼接后的字符串键值对之间无符号，键值对之间无符号，忽略null值 |
| `cn.hutool.crypto.SmUtil` | `HMac hmacSm3(byte[] key)` | HmacSM3算法实现 |
| `cn.hutool.crypto.SmUtil` | `MacEngine createHmacSm3Engine(byte[] key)` | 创建HmacSM3算法的MacEngine |
| `cn.hutool.crypto.SmUtil` | `SM2 sm2()` | 创建SM2算法对象 生成新的私钥公钥对 |
| `cn.hutool.crypto.SmUtil` | `SM2 sm2(ECPrivateKeyParameters privateKeyParams,ECPublicKeyParameters publicKeyParams)` | 创建SM2算法对象 私钥和公钥同时为空时生成一对新的私钥和公钥 私钥和公钥可以单独传入一个，如此则只能使用此钥匙来做加密或者解密 |
| `cn.hutool.crypto.SmUtil` | `SM2 sm2(PrivateKey privateKey,PublicKey publicKey)` | 创建SM2算法对象 私钥和公钥同时为空时生成一对新的私钥和公钥 私钥和公钥可以单独传入一个，如此则只能使用此钥匙来做加密或者解密 |
| `cn.hutool.crypto.SmUtil` | `SM2 sm2(String privateKeyStr,String publicKeyStr)` | 创建SM2算法对象 私钥和公钥同时为空时生成一对新的私钥和公钥 私钥和公钥可以单独传入一个，如此则只能使用此钥匙来做加密或者解密 |
| `cn.hutool.crypto.SmUtil` | `SM2 sm2(byte[] privateKey,byte[] publicKey)` | 创建SM2算法对象 私钥和公钥同时为空时生成一对新的私钥和公钥 私钥和公钥可以单独传入一个，如此则只能使用此钥匙来做加密或者解密 |
| `cn.hutool.crypto.SmUtil` | `SM3 sm3()` | SM3加密 例： SM3加密：sm3().digest(data) SM3加密并转为16进制字符串：sm3().digestHex(data) |
| `cn.hutool.crypto.SmUtil` | `SM3 sm3WithSalt(byte[] salt)` | SM3加密，可以传入盐 |
| `cn.hutool.crypto.SmUtil` | `SM4 sm4()` | SM4加密，生成随机KEY。注意解密时必须使用相同 SymmetricCrypto对象或者使用相同KEY 例： |
| `cn.hutool.crypto.SmUtil` | `SM4 sm4(byte[] key)` | SM4加密 例： |
| `cn.hutool.crypto.SmUtil` | `String sm3(File dataFile)` | SM3加密文件，生成16进制SM3字符串 |
| `cn.hutool.crypto.SmUtil` | `String sm3(InputStream data)` | SM3加密，生成16进制SM3字符串 |
| `cn.hutool.crypto.SmUtil` | `String sm3(String data)` | SM3加密，生成16进制SM3字符串 |
| `cn.hutool.crypto.SmUtil` | `byte[] changeC1C2C3ToC1C3C2(byte[] c1c2c3,ECDomainParameters ecDomainParameters)` | bc加解密使用旧标c1\|\|c2\|\|c3，此方法在加密后调用，将结果转化为c1\|\|c3\|\|c2 |
| `cn.hutool.crypto.SmUtil` | `byte[] changeC1C3C2ToC1C2C3(byte[] c1c3c2,ECDomainParameters ecDomainParameters)` | bc加解密使用旧标c1\|\|c3\|\|c2，此方法在解密前调用，将密文转化为c1\|\|c2\|\|c3再去解密 |
| `cn.hutool.crypto.SmUtil` | `byte[] rsAsn1ToPlain(byte[] rsDer)` | BC的SM3withSM2签名得到的结果的rs是asn1格式的，这个方法转化成直接拼接r\|\|s |
| `cn.hutool.crypto.SmUtil` | `byte[] rsPlainToAsn1(byte[] sign)` | BC的SM3withSM2验签需要的rs是asn1格式的，这个方法将直接拼接r\|\|s的字节数组转化成asn1格式 |
| `cn.hutool.crypto.SpecUtil` | `KeySpec createKeySpec(final String algorithm,byte[] key)` | 根据算法创建KeySpec DESede: DESedeKeySpec DES : DESedeKeySpec 其它 : SecretKeySpec |
| `cn.hutool.crypto.SpecUtil` | `PBEKeySpec createPBEKeySpec(char[] password)` | 创建PBEKeySpec PBE算法没有密钥的概念，密钥在其它对称加密算法中是经过算法计算得出来的，PBE算法则是使用口令替代了密钥。 |
| `cn.hutool.crypto.SpecUtil` | `PBEParameterSpec createPBEParameterSpec(final byte[] salt,final int iterationCount)` | 创建PBEParameterSpec |
| `cn.hutool.crypto.SpecUtil` | `RSAPrivateCrtKeySpec xmlToRSAPrivateCrtKeySpec(final String xml)` | 将XML格式的密钥参数转化为RSAPrivateCrtKeySpec，XML为C#生成格式，类似于： |
