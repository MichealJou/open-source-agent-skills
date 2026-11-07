# cn.hutool.crypto.digest

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.crypto.digest.Argon2` | `Argon2 setAdditional(byte[] additional)` | @param additional 附加数据 |
| `cn.hutool.crypto.digest.Argon2` | `Argon2 setHashLength(int hashLength)` | 设置hash长度 |
| `cn.hutool.crypto.digest.Argon2` | `Argon2 setIterations(int iterations)` | 设置迭代次数 迭代次数越多，生成哈希的时间就越长，破解哈希就越困难 |
| `cn.hutool.crypto.digest.Argon2` | `Argon2 setMemoryAsKB(int memoryAsKB)` | 设置内存，单位KB 内存越大，生成哈希的时间就越长，破解哈希就越困难 |
| `cn.hutool.crypto.digest.Argon2` | `Argon2 setParallelism(int parallelism)` | 设置并行度，即同时使用的核心数 值越高，生成哈希的时间就越长，破解哈希就越困难 |
| `cn.hutool.crypto.digest.Argon2` | `Argon2 setSalt(byte[] salt)` | 设置盐 |
| `cn.hutool.crypto.digest.Argon2` | `Argon2 setSecret(byte[] secret)` | 设置可选的密钥数据，用于增加哈希的复杂性 |
| `cn.hutool.crypto.digest.Argon2` | `Argon2 setVersion(int version)` | 设置版本 |
| `cn.hutool.crypto.digest.Argon2` | `byte[] digest(char[] password)` | 生成hash值 |
| `cn.hutool.crypto.digest.BCrypt` | `String gensalt()` | 生成盐 |
| `cn.hutool.crypto.digest.BCrypt` | `String gensalt(int log_rounds)` | 生成盐 |
| `cn.hutool.crypto.digest.BCrypt` | `String gensalt(int log_rounds,SecureRandom random)` | 生成盐 |
| `cn.hutool.crypto.digest.BCrypt` | `String hashpw(String password)` | 生成密文，使用长度为10的加盐方式 |
| `cn.hutool.crypto.digest.BCrypt` | `String hashpw(String password,String salt)` | 生成密文 |
| `cn.hutool.crypto.digest.BCrypt` | `boolean checkpw(String plaintext,String hashed)` | 检查明文密码文本是否匹配加密后的文本 |
| `cn.hutool.crypto.digest.BCrypt` | `byte[] crypt(byte[] password,byte[] salt,int log_rounds,int[] cdata)` | 加密密文 |
| `cn.hutool.crypto.digest.DigestAlgorithm` | `String getValue()` | 获取算法字符串表示 |
| `cn.hutool.crypto.digest.DigestUtil` | `Digester digester(DigestAlgorithm algorithm)` | 新建摘要器 |
| `cn.hutool.crypto.digest.DigestUtil` | `Digester digester(String algorithm)` | 新建摘要器 |
| `cn.hutool.crypto.digest.DigestUtil` | `HMac hmac(HmacAlgorithm algorithm,SecretKey key)` | 创建HMac对象，调用digest方法可获得hmac值 |
| `cn.hutool.crypto.digest.DigestUtil` | `HMac hmac(HmacAlgorithm algorithm,byte[] key)` | 创建HMac对象，调用digest方法可获得hmac值 |
| `cn.hutool.crypto.digest.DigestUtil` | `String bcrypt(String password)` | 生成Bcrypt加密后的密文 |
| `cn.hutool.crypto.digest.DigestUtil` | `String md5Hex(File file)` | 计算32位MD5摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String md5Hex(InputStream data)` | 计算32位MD5摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String md5Hex(String data)` | 计算32位MD5摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String md5Hex(String data,Charset charset)` | 计算32位MD5摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String md5Hex(String data,String charset)` | 计算32位MD5摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String md5Hex(byte[] data)` | 计算32位MD5摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String md5Hex16(File file)` | 计算16位MD5摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String md5Hex16(InputStream data)` | 计算16位MD5摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String md5Hex16(String data)` | 计算16位MD5摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String md5Hex16(String data,Charset charset)` | 计算16位MD5摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String md5Hex16(byte[] data)` | 计算16位MD5摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String md5HexTo16(String md5Hex)` | 32位MD5转16位MD5 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha1Hex(File file)` | 计算SHA-1摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha1Hex(InputStream data)` | 计算SHA-1摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha1Hex(String data)` | 计算SHA-1摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha1Hex(String data,String charset)` | 计算SHA-1摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha1Hex(byte[] data)` | 计算SHA-1摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha256Hex(File file)` | 计算SHA-256摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha256Hex(InputStream data)` | 计算SHA-256摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha256Hex(String data)` | 计算SHA-256摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha256Hex(String data,String charset)` | 计算SHA-256摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha256Hex(byte[] data)` | 计算SHA-1摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha512Hex(final File file)` | 计算SHA-512摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha512Hex(final InputStream data)` | 计算SHA-512摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha512Hex(final String data)` | 计算SHA-512摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha512Hex(final String data,final String charset)` | 计算SHA-512摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `String sha512Hex(final byte[] data)` | 计算SHA-1摘要值，并转为16进制字符串 |
| `cn.hutool.crypto.digest.DigestUtil` | `boolean bcryptCheck(String password,String hashed)` | 验证密码是否与Bcrypt加密后的密文匹配 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] md5(File file)` | 计算32位MD5摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] md5(InputStream data)` | 计算32位MD5摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] md5(String data)` | 计算32位MD5摘要值，使用UTF-8编码 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] md5(String data,String charset)` | 计算32位MD5摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] md5(byte[] data)` | 计算32位MD5摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha1(File file)` | 计算SHA-1摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha1(InputStream data)` | 计算SHA-1摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha1(String data)` | 计算sha1摘要值，使用UTF-8编码 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha1(String data,String charset)` | 计算SHA-1摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha1(byte[] data)` | 计算SHA-1摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha256(File file)` | 计算SHA-256摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha256(InputStream data)` | 计算SHA-256摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha256(String data)` | 计算sha256摘要值，使用UTF-8编码 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha256(String data,String charset)` | 计算SHA-256摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha256(byte[] data)` | 计算SHA-256摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha512(final File file)` | 计算SHA-512摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha512(final InputStream data)` | 计算SHA-512摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha512(final String data)` | 计算sha512摘要值，使用UTF-8编码 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha512(final String data,final String charset)` | 计算SHA-512摘要值 |
| `cn.hutool.crypto.digest.DigestUtil` | `byte[] sha512(final byte[] data)` | 计算SHA-512摘要值 |
| `cn.hutool.crypto.digest.Digester` | `Digester init(String algorithm,Provider provider)` | 初始化 |
| `cn.hutool.crypto.digest.Digester` | `Digester reset()` | 重置MessageDigest |
| `cn.hutool.crypto.digest.Digester` | `Digester setDigestCount(int digestCount)` | 设置重复计算摘要值次数 |
| `cn.hutool.crypto.digest.Digester` | `Digester setSalt(byte[] salt)` | 设置加盐内容 |
| `cn.hutool.crypto.digest.Digester` | `Digester setSaltPosition(int saltPosition)` | 设置加盐的位置，只有盐值存在时有效 加盐的位置指盐位于数据byte数组中的位置，例如： |
| `cn.hutool.crypto.digest.Digester` | `MessageDigest getDigest()` | 获得 MessageDigest |
| `cn.hutool.crypto.digest.Digester` | `String digestHex(File file)` | 生成文件摘要，并转为16进制字符串 使用默认缓存大小，见 IoUtil#DEFAULT_BUFFER_SIZE |
| `cn.hutool.crypto.digest.Digester` | `String digestHex(InputStream data)` | 生成摘要，并转为16进制字符串 使用默认缓存大小，见 IoUtil#DEFAULT_BUFFER_SIZE |
| `cn.hutool.crypto.digest.Digester` | `String digestHex(InputStream data,int bufferLength)` | 生成摘要，并转为16进制字符串 使用默认缓存大小，见 IoUtil#DEFAULT_BUFFER_SIZE |
| `cn.hutool.crypto.digest.Digester` | `String digestHex(String data)` | 生成文件摘要 |
| `cn.hutool.crypto.digest.Digester` | `String digestHex(String data,Charset charset)` | 生成文件摘要，并转为16进制字符串 |
| `cn.hutool.crypto.digest.Digester` | `String digestHex(String data,String charsetName)` | 生成文件摘要，并转为16进制字符串 |
| `cn.hutool.crypto.digest.Digester` | `String digestHex(byte[] data)` | 生成摘要，并转为16进制字符串 |
| `cn.hutool.crypto.digest.Digester` | `byte[] digest(File file)` | 生成文件摘要 使用默认缓存大小，见 IoUtil#DEFAULT_BUFFER_SIZE |
| `cn.hutool.crypto.digest.Digester` | `byte[] digest(InputStream data)` | 生成摘要，使用默认缓存大小，见 IoUtil#DEFAULT_BUFFER_SIZE |
| `cn.hutool.crypto.digest.Digester` | `byte[] digest(InputStream data,int bufferLength)` | 生成摘要 |
| `cn.hutool.crypto.digest.Digester` | `byte[] digest(String data)` | 生成文件摘要 |
| `cn.hutool.crypto.digest.Digester` | `byte[] digest(String data,Charset charset)` | 生成文件摘要 |
| `cn.hutool.crypto.digest.Digester` | `byte[] digest(String data,String charsetName)` | 生成文件摘要 |
| `cn.hutool.crypto.digest.Digester` | `byte[] digest(byte[] data)` | 生成摘要，考虑加盐和重复摘要次数 |
| `cn.hutool.crypto.digest.Digester` | `int getDigestLength()` | 获取散列长度，0表示不支持此方法 |
| `cn.hutool.crypto.digest.DigesterFactory` | `Digester createDigester()` | 创建Digester |
| `cn.hutool.crypto.digest.DigesterFactory` | `DigesterFactory of(final MessageDigest messageDigest)` | 创建工厂 |
| `cn.hutool.crypto.digest.DigesterFactory` | `DigesterFactory of(final String algorithm)` | 创建工厂，使用GlobalBouncyCastleProvider找到的提供方。 |
| `cn.hutool.crypto.digest.DigesterFactory` | `DigesterFactory ofJdk(final String algorithm)` | 创建工厂 |
| `cn.hutool.crypto.digest.DigesterFactory` | `MessageDigest createMessageDigester()` | 创建MessageDigest |
| `cn.hutool.crypto.digest.HmacAlgorithm` | `String getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.digest.MD5` | `MD5 create()` | 创建MD5实例 |
| `cn.hutool.crypto.digest.MD5` | `String digestHex16(File data)` | 生成16位MD5摘要 |
| `cn.hutool.crypto.digest.MD5` | `String digestHex16(InputStream data)` | 生成16位MD5摘要 |
| `cn.hutool.crypto.digest.MD5` | `String digestHex16(String data)` | 生成16位MD5摘要 |
| `cn.hutool.crypto.digest.MD5` | `String digestHex16(String data,Charset charset)` | 生成16位MD5摘要 |
| `cn.hutool.crypto.digest.MD5` | `String digestHex16(byte[] data)` | 生成16位MD5摘要 |
| `cn.hutool.crypto.digest.SM3` | `SM3 create()` | 创建SM3实例 |
