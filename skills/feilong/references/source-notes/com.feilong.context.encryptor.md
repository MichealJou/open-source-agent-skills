# com.feilong.context.encryptor

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.context.encryptor.Encryptor` | `String encrypt(T bean)` | 加密. |
| `com.feilong.context.encryptor.Encryptor` | `T decrypt(String encryptData,Class<T> klass)` | 解密. |
| `com.feilong.context.encryptor.SymmetricJsonHexEncryptor` | `String encrypt(T bean)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.encryptor.SymmetricJsonHexEncryptor` | `T decrypt(String encryptPayResultType,Class<T> klass)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.encryptor.SymmetricJsonHexEncryptor` | `void setCharsetName(String charsetName)` | 设置 编码格式,默认 CharsetType#UTF8. |
| `com.feilong.context.encryptor.SymmetricJsonHexEncryptor` | `void setKey(String key)` | 设置 key. |
| `com.feilong.context.encryptor.SymmetricJsonHexEncryptor` | `void setSymmetricType(SymmetricType symmetricType)` | 设置 对称加密的类型. |
