# cn.hutool.crypto.digest.mac

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.crypto.digest.mac.BCHMacEngine` | `BCHMacEngine init(Digest digest,CipherParameters params)` | 初始化 |
| `cn.hutool.crypto.digest.mac.BCMacEngine` | `BCMacEngine init(Mac mac,CipherParameters params)` | 初始化 |
| `cn.hutool.crypto.digest.mac.BCMacEngine` | `Mac getMac()` | 获得 Mac |
| `cn.hutool.crypto.digest.mac.BCMacEngine` | `String getAlgorithm()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.digest.mac.BCMacEngine` | `byte[] doFinal()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.digest.mac.BCMacEngine` | `int getMacLength()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.digest.mac.BCMacEngine` | `void reset()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.digest.mac.BCMacEngine` | `void update(byte[] in,int inOff,int len)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.digest.mac.CBCBlockCipherMacEngine` | `CBCBlockCipherMacEngine init(BlockCipher cipher,CipherParameters params)` | 初始化 |
| `cn.hutool.crypto.digest.mac.DefaultHMacEngine` | `DefaultHMacEngine init(String algorithm,Key key)` | 初始化 |
| `cn.hutool.crypto.digest.mac.DefaultHMacEngine` | `DefaultHMacEngine init(String algorithm,Key key,AlgorithmParameterSpec spec)` | 初始化 |
| `cn.hutool.crypto.digest.mac.DefaultHMacEngine` | `DefaultHMacEngine init(String algorithm,byte[] key)` | 初始化 |
| `cn.hutool.crypto.digest.mac.DefaultHMacEngine` | `Mac getMac()` | 获得 Mac |
| `cn.hutool.crypto.digest.mac.DefaultHMacEngine` | `String getAlgorithm()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.digest.mac.DefaultHMacEngine` | `byte[] doFinal()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.digest.mac.DefaultHMacEngine` | `int getMacLength()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.digest.mac.DefaultHMacEngine` | `void reset()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.digest.mac.DefaultHMacEngine` | `void update(byte[] in)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.digest.mac.DefaultHMacEngine` | `void update(byte[] in,int inOff,int len)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.crypto.digest.mac.Mac` | `MacEngine getEngine()` | 获得MAC算法引擎 |
| `cn.hutool.crypto.digest.mac.Mac` | `String digestBase64(String data,Charset charset,boolean isUrlSafe)` | 生成文件摘要，并转为Base64 |
| `cn.hutool.crypto.digest.mac.Mac` | `String digestBase64(String data,boolean isUrlSafe)` | 生成文件摘要，并转为Base64 |
| `cn.hutool.crypto.digest.mac.Mac` | `String digestHex(File file)` | 生成文件摘要，并转为16进制字符串 使用默认缓存大小，见 IoUtil#DEFAULT_BUFFER_SIZE |
| `cn.hutool.crypto.digest.mac.Mac` | `String digestHex(InputStream data)` | 生成摘要，并转为16进制字符串 使用默认缓存大小，见 IoUtil#DEFAULT_BUFFER_SIZE |
| `cn.hutool.crypto.digest.mac.Mac` | `String digestHex(InputStream data,int bufferLength)` | 生成摘要，并转为16进制字符串 使用默认缓存大小，见 IoUtil#DEFAULT_BUFFER_SIZE |
| `cn.hutool.crypto.digest.mac.Mac` | `String digestHex(String data)` | 生成文件摘要 |
| `cn.hutool.crypto.digest.mac.Mac` | `String digestHex(String data,Charset charset)` | 生成文件摘要，并转为16进制字符串 |
| `cn.hutool.crypto.digest.mac.Mac` | `String digestHex(byte[] data)` | 生成摘要，并转为16进制字符串 |
| `cn.hutool.crypto.digest.mac.Mac` | `String getAlgorithm()` | 获取算法 |
| `cn.hutool.crypto.digest.mac.Mac` | `boolean verify(byte[] digest,byte[] digestToCompare)` | 验证生成的摘要与给定的摘要比较是否一致 简单比较每个byte位是否相同 |
| `cn.hutool.crypto.digest.mac.Mac` | `byte[] digest(File file)` | 生成文件摘要 使用默认缓存大小，见 IoUtil#DEFAULT_BUFFER_SIZE |
| `cn.hutool.crypto.digest.mac.Mac` | `byte[] digest(InputStream data)` | 生成摘要，使用默认缓存大小，见 IoUtil#DEFAULT_BUFFER_SIZE |
| `cn.hutool.crypto.digest.mac.Mac` | `byte[] digest(InputStream data,int bufferLength)` | 生成摘要 |
| `cn.hutool.crypto.digest.mac.Mac` | `byte[] digest(String data)` | 生成文件摘要 |
| `cn.hutool.crypto.digest.mac.Mac` | `byte[] digest(String data,Charset charset)` | 生成文件摘要 |
| `cn.hutool.crypto.digest.mac.Mac` | `byte[] digest(byte[] data)` | 生成摘要 |
| `cn.hutool.crypto.digest.mac.Mac` | `int getMacLength()` | 获取MAC算法块长度 |
| `cn.hutool.crypto.digest.mac.MacEngine` | `String getAlgorithm()` | 获取当前算法 |
| `cn.hutool.crypto.digest.mac.MacEngine` | `byte[] digest(InputStream data,int bufferLength)` | 生成摘要 |
| `cn.hutool.crypto.digest.mac.MacEngine` | `byte[] doFinal()` | 结束并生成摘要 |
| `cn.hutool.crypto.digest.mac.MacEngine` | `int getMacLength()` | 获取MAC算法块大小 |
| `cn.hutool.crypto.digest.mac.MacEngine` | `void reset()` | 重置 |
| `cn.hutool.crypto.digest.mac.MacEngine` | `void update(byte[] in)` | 加入需要被摘要的内容 |
| `cn.hutool.crypto.digest.mac.MacEngine` | `void update(byte[] in,int inOff,int len)` | 加入需要被摘要的内容 |
| `cn.hutool.crypto.digest.mac.MacEngineFactory` | `MacEngine createEngine(String algorithm,Key key)` | 根据给定算法和密钥生成对应的MacEngine |
| `cn.hutool.crypto.digest.mac.MacEngineFactory` | `MacEngine createEngine(String algorithm,Key key,AlgorithmParameterSpec spec)` | 根据给定算法和密钥生成对应的MacEngine |
