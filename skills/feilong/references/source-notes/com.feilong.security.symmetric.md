# com.feilong.security.symmetric

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.security.symmetric.AesUtil` | `void setSymmetricType(SymmetricType symmetricType)` | 【原文待译】Sets the symmetric type. |
| `com.feilong.security.symmetric.CipherUtil` | `byte[] decrypt(byte[] bytes,String transformation,Key key)` | 解密. |
| `com.feilong.security.symmetric.CipherUtil` | `byte[] encrypt(byte[] bytes,String transformation,Key key)` | 加密. |
| `com.feilong.security.symmetric.LogBuilder` | `String hided(String keyString)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.security.symmetric.SymmetricEncryption` | `String decryptBase64(String base64String)` | des Base64解密. |
| `com.feilong.security.symmetric.SymmetricEncryption` | `String decryptBase64(String base64String,String charsetName)` | des Base64解密. |
| `com.feilong.security.symmetric.SymmetricEncryption` | `String decryptHex(String hexString)` | 16进制 des 解密,解密 以String密文输入,String明文输出. |
| `com.feilong.security.symmetric.SymmetricEncryption` | `String decryptHex(String hexString,String charsetName)` | 16进制 des 解密,解密 以String密文输入,String明文输出. |
| `com.feilong.security.symmetric.SymmetricEncryption` | `String encryptBase64(String original)` | 将加密之后的字节码,使用 Base64封装返回. |
| `com.feilong.security.symmetric.SymmetricEncryption` | `String encryptBase64(String original,String charsetName)` | 将加密之后的字节码,使用 Base64封装返回. |
| `com.feilong.security.symmetric.SymmetricEncryption` | `String encryptHex(String original)` | 将加密之后的字节码,使用大写的 Hex形式封装返回. |
| `com.feilong.security.symmetric.SymmetricEncryption` | `String encryptHex(String original,String charsetName)` | 将加密之后的字节码,使用大写的 Hex形式封装返回. |
| `com.feilong.security.symmetric.SymmetricEncryption` | `void setCipherMode(CipherMode cipherMode)` | 设置 cipher mode. |
| `com.feilong.security.symmetric.SymmetricEncryption` | `void setCipherPadding(CipherPadding cipherPadding)` | 设置 cipher padding. |
| `com.feilong.security.symmetric.SymmetricEncryption` | `void setKeyBuilder(KeyBuilder keyBuilder)` | 支持设置特殊的 java.security.Key , 默认使用 com.feilong.security.symmetric.builder.DefaultKeyBuilder,. |
| `com.feilong.security.symmetric.SymmetricEncryption` | `void setKeyString(String keyString)` | 设置 key string. |
| `com.feilong.security.symmetric.SymmetricEncryption` | `void setSymmetricType(SymmetricType symmetricType)` | 【原文待译】Sets the symmetric type. |
| `com.feilong.security.symmetric.SymmetricType` | `String getAlgorithm()` | Gets the 算法. |
