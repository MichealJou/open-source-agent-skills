# cn.hutool.crypto.symmetric

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.crypto.symmetric.PBKDF2` | `String encryptHex(char[] password,byte[] salt)` | 加密 |
| `cn.hutool.crypto.symmetric.PBKDF2` | `byte[] encrypt(char[] password,byte[] salt)` | 加密 |
| `cn.hutool.crypto.symmetric.RC4` | `String decrypt(String message)` | 解密Hex（16进制）或Base64表示的字符串，使用默认编码UTF-8 |
| `cn.hutool.crypto.symmetric.RC4` | `String decrypt(String message,Charset charset)` | 解密Hex（16进制）或Base64表示的字符串 |
| `cn.hutool.crypto.symmetric.RC4` | `String decrypt(byte[] message)` | 解密，使用默认编码UTF-8 |
| `cn.hutool.crypto.symmetric.RC4` | `String decrypt(byte[] message,Charset charset)` | 解密 |
| `cn.hutool.crypto.symmetric.RC4` | `String encryptBase64(String data)` | 加密，使用UTF-8编码 |
| `cn.hutool.crypto.symmetric.RC4` | `String encryptBase64(String data,Charset charset)` | 加密 |
| `cn.hutool.crypto.symmetric.RC4` | `String encryptBase64(byte[] data)` | 加密 |
| `cn.hutool.crypto.symmetric.RC4` | `String encryptHex(String data)` | 加密，使用UTF-8编码 |
| `cn.hutool.crypto.symmetric.RC4` | `String encryptHex(String data,Charset charset)` | 加密 |
| `cn.hutool.crypto.symmetric.RC4` | `String encryptHex(byte[] data)` | 加密 |
| `cn.hutool.crypto.symmetric.RC4` | `byte[] crypt(final byte[] msg)` | 加密或解密指定值，调用此方法前需初始化密钥 |
| `cn.hutool.crypto.symmetric.RC4` | `byte[] encrypt(String message)` | 加密，使用默认编码：UTF-8 |
| `cn.hutool.crypto.symmetric.RC4` | `byte[] encrypt(String message,Charset charset)` | 加密 |
| `cn.hutool.crypto.symmetric.RC4` | `void setKey(String key)` | 设置密钥 |
| `cn.hutool.crypto.symmetric.SymmetricAlgorithm` | `String getValue()` | 获得算法的字符串表示形式 |
| `cn.hutool.crypto.symmetric.SymmetricCrypto` | `Cipher getCipher()` | 获得加密或解密器 |
| `cn.hutool.crypto.symmetric.SymmetricCrypto` | `SecretKey getSecretKey()` | 获得对称密钥 |
| `cn.hutool.crypto.symmetric.SymmetricCrypto` | `String updateHex(byte[] data)` | 更新数据，分组加密中间结果可以当作随机数 第一次更新数据前需要调用#setMode(CipherMode)初始化加密或解密模式，然后每次更新数据都是累加模式 |
| `cn.hutool.crypto.symmetric.SymmetricCrypto` | `SymmetricCrypto init(String algorithm,SecretKey key)` | 初始化 |
| `cn.hutool.crypto.symmetric.SymmetricCrypto` | `SymmetricCrypto setIv(IvParameterSpec iv)` | 设置偏移向量 |
| `cn.hutool.crypto.symmetric.SymmetricCrypto` | `SymmetricCrypto setIv(byte[] iv)` | 设置偏移向量 |
| `cn.hutool.crypto.symmetric.SymmetricCrypto` | `SymmetricCrypto setMode(CipherMode mode)` | 初始化模式并清空数据 |
| `cn.hutool.crypto.symmetric.SymmetricCrypto` | `SymmetricCrypto setParams(AlgorithmParameterSpec params)` | 设置 AlgorithmParameterSpec，通常用于加盐或偏移向量 |
| `cn.hutool.crypto.symmetric.SymmetricCrypto` | `SymmetricCrypto setRandom(SecureRandom random)` | 设置随机数生成器，可自定义随机数种子 |
| `cn.hutool.crypto.symmetric.SymmetricCrypto` | `byte[] decrypt(byte[] bytes)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.symmetric.SymmetricCrypto` | `byte[] encrypt(byte[] data)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.symmetric.SymmetricCrypto` | `byte[] update(byte[] data)` | 更新数据，分组加密中间结果可以当作随机数 第一次更新数据前需要调用#setMode(CipherMode)初始化加密或解密模式，然后每次更新数据都是累加模式 |
| `cn.hutool.crypto.symmetric.SymmetricCrypto` | `void decrypt(InputStream data,OutputStream out,boolean isClose)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.symmetric.SymmetricCrypto` | `void encrypt(InputStream data,OutputStream out,boolean isClose)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.symmetric.SymmetricDecryptor` | `String decryptStr(InputStream data)` | 解密 |
| `cn.hutool.crypto.symmetric.SymmetricDecryptor` | `String decryptStr(InputStream data,Charset charset)` | 解密，不会关闭流 |
| `cn.hutool.crypto.symmetric.SymmetricDecryptor` | `String decryptStr(String data)` | 解密Hex（16进制）或Base64表示的字符串，默认UTF-8编码 |
| `cn.hutool.crypto.symmetric.SymmetricDecryptor` | `String decryptStr(String data,Charset charset)` | 解密Hex（16进制）或Base64表示的字符串 |
| `cn.hutool.crypto.symmetric.SymmetricDecryptor` | `String decryptStr(byte[] bytes)` | 解密为字符串，默认UTF-8编码 |
| `cn.hutool.crypto.symmetric.SymmetricDecryptor` | `String decryptStr(byte[] bytes,Charset charset)` | 解密为字符串 |
| `cn.hutool.crypto.symmetric.SymmetricDecryptor` | `byte[] decrypt(InputStream data)` | 解密，会关闭流 |
| `cn.hutool.crypto.symmetric.SymmetricDecryptor` | `byte[] decrypt(String data)` | 解密Hex（16进制）或Base64表示的字符串 |
| `cn.hutool.crypto.symmetric.SymmetricDecryptor` | `byte[] decrypt(byte[] bytes)` | 解密 |
| `cn.hutool.crypto.symmetric.SymmetricDecryptor` | `void decrypt(InputStream data,OutputStream out,boolean isClose)` | 解密，针对大数据量，结束后不关闭流 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `String encryptBase64(InputStream data)` | 加密 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `String encryptBase64(String data)` | 加密，使用UTF-8编码 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `String encryptBase64(String data,Charset charset)` | 加密 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `String encryptBase64(String data,String charset)` | 加密 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `String encryptBase64(byte[] data)` | 加密 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `String encryptHex(InputStream data)` | 加密 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `String encryptHex(String data)` | 加密，使用UTF-8编码 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `String encryptHex(String data,Charset charset)` | 加密 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `String encryptHex(String data,String charset)` | 加密 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `String encryptHex(byte[] data)` | 加密 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `byte[] encrypt(InputStream data)` | 加密，加密后关闭流 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `byte[] encrypt(String data)` | 加密，使用UTF-8编码 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `byte[] encrypt(String data,Charset charset)` | 加密 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `byte[] encrypt(String data,String charset)` | 加密 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `byte[] encrypt(byte[] data)` | 加密 |
| `cn.hutool.crypto.symmetric.SymmetricEncryptor` | `void encrypt(InputStream data,OutputStream out,boolean isClose)` | 加密，针对大数据量，可选结束后是否关闭流 |
| `cn.hutool.crypto.symmetric.Vigenere` | `String decrypt(CharSequence data,CharSequence cipherKey)` | 解密 |
| `cn.hutool.crypto.symmetric.Vigenere` | `String encrypt(CharSequence data,CharSequence cipherKey)` | 加密 |
| `cn.hutool.crypto.symmetric.XXTEA` | `byte[] decrypt(byte[] data)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.symmetric.XXTEA` | `byte[] encrypt(byte[] data)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.symmetric.XXTEA` | `void decrypt(InputStream data,OutputStream out,boolean isClose)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.symmetric.XXTEA` | `void encrypt(InputStream data,OutputStream out,boolean isClose)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.symmetric.ZUC` | `byte[] generateKey(ZUCAlgorithm algorithm)` | 生成ZUC算法密钥 |
| `cn.hutool.crypto.symmetric.ZUC$ZUCAlgorithm` | `String getValue()` | 获得算法的字符串表示形式 |
