# cn.hutool.jwt.signers

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.jwt.signers.AlgorithmUtil` | `String getAlgorithm(String idOrAlgorithm)` | 获取算法，用户传入算法ID返回算法名，传入算法名返回本身 |
| `cn.hutool.jwt.signers.AlgorithmUtil` | `String getId(String idOrAlgorithm)` | 获取算法ID，用户传入算法名返回ID，传入算法ID返回本身 |
| `cn.hutool.jwt.signers.AsymmetricJWTSigner` | `AsymmetricJWTSigner setCharset(Charset charset)` | 设置编码 |
| `cn.hutool.jwt.signers.AsymmetricJWTSigner` | `String getAlgorithm()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.jwt.signers.AsymmetricJWTSigner` | `String sign(String headerBase64,String payloadBase64)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.jwt.signers.AsymmetricJWTSigner` | `boolean verify(String headerBase64,String payloadBase64,String signBase64)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.jwt.signers.HMacJWTSigner` | `HMacJWTSigner setCharset(Charset charset)` | 设置编码 |
| `cn.hutool.jwt.signers.HMacJWTSigner` | `String getAlgorithm()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.jwt.signers.HMacJWTSigner` | `String sign(String headerBase64,String payloadBase64)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.jwt.signers.HMacJWTSigner` | `boolean verify(String headerBase64,String payloadBase64,String signBase64)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.jwt.signers.JWTSigner` | `String getAlgorithm()` | 获取算法 |
| `cn.hutool.jwt.signers.JWTSigner` | `String getAlgorithmId()` | 获取算法ID，即算法的简写形式，如HS256 |
| `cn.hutool.jwt.signers.JWTSigner` | `String sign(String headerBase64,String payloadBase64)` | 签名 |
| `cn.hutool.jwt.signers.JWTSigner` | `boolean verify(String headerBase64,String payloadBase64,String signBase64)` | 验签 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner createSigner(String algorithmId,Key key)` | 创建签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner createSigner(String algorithmId,KeyPair keyPair)` | 创建签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner createSigner(String algorithmId,byte[] key)` | 创建签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner dnone(Key key)` | DNONE(NONEwithDSA)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner dsha1(Key key)` | DSHA1(SHA1withDSA)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner enone(Key key)` | ENONE(NONEwithECDSA)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner es256(Key key)` | ES256(SHA256withECDSA)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner es384(Key key)` | ES384(SHA383withECDSA)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner es512(Key key)` | ES512(SHA512withECDSA)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner esha1(Key key)` | ESHA1(SHA1withECDSA)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner hmd5(Key key)` | HMD5(HmacMD5)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner hs256(byte[] key)` | HS256(HmacSHA256)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner hs384(byte[] key)` | HS384(HmacSHA384)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner hs512(byte[] key)` | HS512(HmacSHA512)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner hsha1(Key key)` | HSHA1(HmacSHA1)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner none()` | 无签名 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner rmd2(Key key)` | RMD2(MD2withRSA)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner rmd5(Key key)` | RMD5(MD5withRSA)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner rs256(Key key)` | RS256(SHA256withRSA)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner rs384(Key key)` | RS384(SHA384withRSA)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner rs512(Key key)` | RS512(SHA512withRSA)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner rsha1(Key key)` | RSHA1(SHA1withRSA)签名器 |
| `cn.hutool.jwt.signers.JWTSignerUtil` | `JWTSigner sm4cmac(Key key)` | SM4CMAC(SM4CMAC)签名器 |
| `cn.hutool.jwt.signers.NoneJWTSigner` | `String getAlgorithm()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.jwt.signers.NoneJWTSigner` | `String sign(String headerBase64,String payloadBase64)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.jwt.signers.NoneJWTSigner` | `boolean isNone(final String alg)` | 判断给定的算法是否为无签名的算法 |
| `cn.hutool.jwt.signers.NoneJWTSigner` | `boolean verify(String headerBase64,String payloadBase64,String signBase64)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
