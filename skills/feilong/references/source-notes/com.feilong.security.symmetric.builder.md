# com.feilong.security.symmetric.builder

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.security.symmetric.builder.AbstractSecretKeySpecBuilder` | `Key build(String algorithm,String keyString)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.security.symmetric.builder.KeyBuilder` | `Key build(String algorithm,String keyString)` | 【原文待译】Builds the. |
| `com.feilong.security.symmetric.builder.KeyGeneratorKeyBuilder` | `void setKeyGeneratorKeysize(int keyGeneratorKeysize)` | 设置 用于构造 KeyGenerator. |
| `com.feilong.security.symmetric.builder.KeyGeneratorKeyBuilder` | `void setSecureRandomAlgorithm(String secureRandomAlgorithm)` | 设置 用于构造 SecureRandom. |
| `com.feilong.security.symmetric.builder.TransformationBuilder` | `String build(String algorithm,CipherMode cipherMode,CipherPadding cipherPadding)` | 转换的名称,例如 DES/CBC/PKCS5Padding. 有关标准转换名称的信息,请参见 Java Cryptography Architecture Reference Guide 的附录 A. |
