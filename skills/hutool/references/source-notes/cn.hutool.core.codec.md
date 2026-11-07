# cn.hutool.core.codec

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.codec.BCD` | `String bcdToStr(byte[] bytes)` | BCD转ASCII字符串 |
| `cn.hutool.core.codec.BCD` | `byte[] ascToBcd(byte[] ascii)` | ASCII转BCD |
| `cn.hutool.core.codec.BCD` | `byte[] ascToBcd(byte[] ascii,int ascLength)` | ASCII转BCD |
| `cn.hutool.core.codec.BCD` | `byte[] strToBcd(String asc)` | 字符串转BCD码 |
| `cn.hutool.core.codec.Base16Codec` | `String toUnicodeHex(char ch)` | 将指定char值转换为Unicode字符串形式，常用于特殊字符（例如汉字）转Unicode形式 转换的字符串如果u后不足4位，则前面用0填充，例如： |
| `cn.hutool.core.codec.Base16Codec` | `byte[] decode(CharSequence encoded)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.codec.Base16Codec` | `char[] encode(byte[] data)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.codec.Base16Codec` | `void appendHex(StringBuilder builder,byte b)` | 将byte值转为16进制并添加到StringBuilder中 |
| `cn.hutool.core.codec.Base32` | `String decodeStr(String source)` | base32解码 |
| `cn.hutool.core.codec.Base32` | `String decodeStr(String source,Charset charset)` | base32解码 |
| `cn.hutool.core.codec.Base32` | `String decodeStrHex(String source)` | base32解码 |
| `cn.hutool.core.codec.Base32` | `String decodeStrHex(String source,Charset charset)` | base32解码 |
| `cn.hutool.core.codec.Base32` | `String encode(String source)` | base32编码 |
| `cn.hutool.core.codec.Base32` | `String encode(String source,Charset charset)` | base32编码 |
| `cn.hutool.core.codec.Base32` | `String encode(final byte[] bytes)` | 编码 |
| `cn.hutool.core.codec.Base32` | `String encodeHex(String source)` | base32编码（Hex模式） |
| `cn.hutool.core.codec.Base32` | `String encodeHex(String source,Charset charset)` | base32编码（Hex模式） |
| `cn.hutool.core.codec.Base32` | `String encodeHex(final byte[] bytes)` | 编码 |
| `cn.hutool.core.codec.Base32` | `byte[] decode(String base32)` | 解码 |
| `cn.hutool.core.codec.Base32` | `byte[] decodeHex(String base32)` | 解码 |
| `cn.hutool.core.codec.Base32Codec` | `String encode(byte[] data)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.codec.Base32Codec` | `String encode(byte[] data,boolean useHex)` | 编码数据 |
| `cn.hutool.core.codec.Base32Codec` | `byte[] decode(CharSequence encoded)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.codec.Base32Codec` | `byte[] decode(CharSequence encoded,boolean useHex)` | 解码数据 |
| `cn.hutool.core.codec.Base32Codec$Base32Decoder` | `byte[] decode(CharSequence encoded)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.codec.Base32Codec$Base32Encoder` | `String encode(byte[] data)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.codec.Base58` | `String encode(byte[] data)` | Base58编码 |
| `cn.hutool.core.codec.Base58` | `String encodeChecked(Integer version,byte[] data)` | Base58编码 包含版本位和校验位 |
| `cn.hutool.core.codec.Base58` | `byte[] decode(CharSequence encoded)` | Base58解码 |
| `cn.hutool.core.codec.Base58` | `byte[] decodeChecked(CharSequence encoded)` | Base58解码 解码包含标志位验证和版本呢位去除 |
| `cn.hutool.core.codec.Base58` | `byte[] decodeChecked(CharSequence encoded,boolean withVersion)` | Base58解码 解码包含标志位验证和版本呢位去除 |
| `cn.hutool.core.codec.Base58Codec` | `String encode(byte[] data)` | Base58编码 |
| `cn.hutool.core.codec.Base58Codec` | `byte[] decode(CharSequence encoded)` | 解码给定的Base58字符串 |
| `cn.hutool.core.codec.Base58Codec$Base58Decoder` | `byte[] decode(CharSequence encoded)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.codec.Base58Codec$Base58Encoder` | `String encode(byte[] data)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.codec.Base62` | `File decodeToFile(CharSequence Base62,File destFile)` | Base62解码 |
| `cn.hutool.core.codec.Base62` | `File decodeToFileInverted(CharSequence Base62,File destFile)` | Base62解码（反转字母表模式） |
| `cn.hutool.core.codec.Base62` | `String decodeStr(CharSequence source)` | Base62解码 |
| `cn.hutool.core.codec.Base62` | `String decodeStr(CharSequence source,Charset charset)` | Base62解码 |
| `cn.hutool.core.codec.Base62` | `String decodeStrGbk(CharSequence source)` | Base62解码 |
| `cn.hutool.core.codec.Base62` | `String decodeStrInverted(CharSequence source)` | Base62解码（反转字母表模式） |
| `cn.hutool.core.codec.Base62` | `String decodeStrInverted(CharSequence source,Charset charset)` | Base62解码（反转字母表模式） |
| `cn.hutool.core.codec.Base62` | `String encode(CharSequence source)` | Base62编码 |
| `cn.hutool.core.codec.Base62` | `String encode(CharSequence source,Charset charset)` | Base62编码 |
| `cn.hutool.core.codec.Base62` | `String encode(File file)` | Base62编码 |
| `cn.hutool.core.codec.Base62` | `String encode(InputStream in)` | Base62编码 |
| `cn.hutool.core.codec.Base62` | `String encode(byte[] source)` | Base62编码 |
| `cn.hutool.core.codec.Base62` | `String encodeInverted(CharSequence source)` | Base62编码（反转字母表模式） |
| `cn.hutool.core.codec.Base62` | `String encodeInverted(CharSequence source,Charset charset)` | Base62编码（反转字母表模式） |
| `cn.hutool.core.codec.Base62` | `String encodeInverted(File file)` | Base62编码（反转字母表模式） |
| `cn.hutool.core.codec.Base62` | `String encodeInverted(InputStream in)` | Base62编码 |
| `cn.hutool.core.codec.Base62` | `String encodeInverted(byte[] source)` | Base62编码（反转字母表模式） |
| `cn.hutool.core.codec.Base62` | `byte[] decode(CharSequence base62Str)` | Base62解码 |
| `cn.hutool.core.codec.Base62` | `byte[] decode(byte[] base62bytes)` | 解码Base62 |
| `cn.hutool.core.codec.Base62` | `byte[] decodeInverted(CharSequence base62Str)` | Base62解码（反转字母表模式） |
| `cn.hutool.core.codec.Base62` | `byte[] decodeInverted(byte[] base62bytes)` | 解码Base62（反转字母表模式） |
| `cn.hutool.core.codec.Base62` | `void decodeToStream(CharSequence base62Str,OutputStream out,boolean isCloseOut)` | Base62解码 |
| `cn.hutool.core.codec.Base62` | `void decodeToStreamInverted(CharSequence base62Str,OutputStream out,boolean isCloseOut)` | Base62解码（反转字母表模式） |
| `cn.hutool.core.codec.Base62Codec` | `byte[] decode(byte[] encoded)` | 解码Base62消息 |
| `cn.hutool.core.codec.Base62Codec` | `byte[] decode(byte[] encoded,boolean useInverted)` | 解码Base62消息 |
| `cn.hutool.core.codec.Base62Codec` | `byte[] encode(byte[] data)` | 编码指定消息bytes为Base62格式的bytes |
| `cn.hutool.core.codec.Base62Codec` | `byte[] encode(byte[] data,boolean useInverted)` | 编码指定消息bytes为Base62格式的bytes |
| `cn.hutool.core.codec.Base62Codec$Base62Decoder` | `byte[] decode(byte[] encoded)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.codec.Base62Codec$Base62Encoder` | `byte[] encode(byte[] data)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.codec.Base64` | `File decodeToFile(CharSequence base64,File destFile)` | base64解码 |
| `cn.hutool.core.codec.Base64` | `String decodeStr(CharSequence source)` | base64解码 |
| `cn.hutool.core.codec.Base64` | `String decodeStr(CharSequence source,Charset charset)` | base64解码 |
| `cn.hutool.core.codec.Base64` | `String decodeStr(CharSequence source,String charset)` | base64解码 |
| `cn.hutool.core.codec.Base64` | `String decodeStrGbk(CharSequence source)` | base64解码 |
| `cn.hutool.core.codec.Base64` | `String encode(CharSequence source)` | base64编码 |
| `cn.hutool.core.codec.Base64` | `String encode(CharSequence source,Charset charset)` | base64编码 |
| `cn.hutool.core.codec.Base64` | `String encode(CharSequence source,String charset)` | base64编码 |
| `cn.hutool.core.codec.Base64` | `String encode(File file)` | base64编码 |
| `cn.hutool.core.codec.Base64` | `String encode(InputStream in)` | base64编码 |
| `cn.hutool.core.codec.Base64` | `String encode(byte[] source)` | base64编码 |
| `cn.hutool.core.codec.Base64` | `String encodeStr(byte[] arr,boolean isMultiLine,boolean isUrlSafe)` | 编码为Base64字符串 如果isMultiLine为true，则每76个字符一个换行符，否则在一行显示 |
| `cn.hutool.core.codec.Base64` | `String encodeUrlSafe(CharSequence source)` | base64编码，URL安全 |
| `cn.hutool.core.codec.Base64` | `String encodeUrlSafe(CharSequence source,Charset charset)` | base64编码，URL安全的 |
| `cn.hutool.core.codec.Base64` | `String encodeUrlSafe(CharSequence source,String charset)` | base64编码,URL安全 |
| `cn.hutool.core.codec.Base64` | `String encodeUrlSafe(File file)` | base64编码,URL安全的 |
| `cn.hutool.core.codec.Base64` | `String encodeUrlSafe(InputStream in)` | base64编码,URL安全的 |
| `cn.hutool.core.codec.Base64` | `String encodeUrlSafe(byte[] source)` | base64编码,URL安全的 |
| `cn.hutool.core.codec.Base64` | `String encodeWithoutPadding(CharSequence source,String charset)` | base64编码，不进行padding(末尾不会填充'=') |
| `cn.hutool.core.codec.Base64` | `String encodeWithoutPadding(byte[] source)` | base64编码，不进行padding(末尾不会填充'=') |
| `cn.hutool.core.codec.Base64` | `boolean isBase64(CharSequence base64)` | 检查是否为Base64 |
| `cn.hutool.core.codec.Base64` | `boolean isBase64(byte[] base64Bytes)` | 检查是否为Base64 |
| `cn.hutool.core.codec.Base64` | `byte[] decode(CharSequence base64)` | base64解码 |
| `cn.hutool.core.codec.Base64` | `byte[] decode(byte[] in)` | 解码Base64 |
| `cn.hutool.core.codec.Base64` | `byte[] encode(byte[] arr,boolean isMultiLine,boolean isUrlSafe)` | 编码为Base64 如果isMultiLine为true，则每76个字符一个换行符，否则在一行显示 |
| `cn.hutool.core.codec.Base64` | `byte[] encode(byte[] arr,boolean lineSep)` | 编码为Base64，非URL安全的 |
| `cn.hutool.core.codec.Base64` | `byte[] encodeUrlSafe(byte[] arr,boolean lineSep)` | 编码为Base64，URL安全的 |
| `cn.hutool.core.codec.Base64` | `void decodeToStream(CharSequence base64,OutputStream out,boolean isCloseOut)` | base64解码 |
| `cn.hutool.core.codec.Base64Decoder` | `String decodeStr(CharSequence source)` | base64解码 |
| `cn.hutool.core.codec.Base64Decoder` | `String decodeStr(CharSequence source,Charset charset)` | base64解码 |
| `cn.hutool.core.codec.Base64Decoder` | `boolean isBase64Code(byte octet)` | 给定的字符是否为Base64字符 |
| `cn.hutool.core.codec.Base64Decoder` | `byte[] decode(CharSequence source)` | base64解码 |
| `cn.hutool.core.codec.Base64Decoder` | `byte[] decode(byte[] in)` | 解码Base64 |
| `cn.hutool.core.codec.Base64Decoder` | `byte[] decode(byte[] in,int pos,int length)` | 解码Base64 |
| `cn.hutool.core.codec.Base64Encoder` | `String encode(CharSequence source)` | base64编码 |
| `cn.hutool.core.codec.Base64Encoder` | `String encode(CharSequence source,Charset charset)` | base64编码 |
| `cn.hutool.core.codec.Base64Encoder` | `String encode(byte[] source)` | base64编码 |
| `cn.hutool.core.codec.Base64Encoder` | `String encodeStr(byte[] arr,boolean isMultiLine,boolean isUrlSafe)` | 编码为Base64字符串 如果isMultiLine为true，则每76个字符一个换行符，否则在一行显示 |
| `cn.hutool.core.codec.Base64Encoder` | `String encodeUrlSafe(CharSequence source)` | base64编码，URL安全 |
| `cn.hutool.core.codec.Base64Encoder` | `String encodeUrlSafe(CharSequence source,Charset charset)` | base64编码，URL安全的 |
| `cn.hutool.core.codec.Base64Encoder` | `String encodeUrlSafe(byte[] source)` | base64编码,URL安全的 |
| `cn.hutool.core.codec.Base64Encoder` | `byte[] encode(byte[] arr,boolean isMultiLine,boolean isUrlSafe)` | 编码为Base64 如果isMultiLine为true，则每76个字符一个换行符，否则在一行显示 |
| `cn.hutool.core.codec.Base64Encoder` | `byte[] encode(byte[] arr,boolean lineSep)` | 编码为Base64，非URL安全的 |
| `cn.hutool.core.codec.Base64Encoder` | `byte[] encodeUrlSafe(byte[] arr,boolean lineSep)` | 编码为Base64，URL安全的 |
| `cn.hutool.core.codec.Caesar` | `String decode(String cipherText,int offset)` | 传入明文解密到密文 |
| `cn.hutool.core.codec.Caesar` | `String encode(String message,int offset)` | 传入明文，加密得到密文 |
| `cn.hutool.core.codec.Decoder` | `R decode(T encoded)` | 执行解码 |
| `cn.hutool.core.codec.Encoder` | `R encode(T data)` | 执行编码 |
| `cn.hutool.core.codec.Hashids` | `Hashids create(final char[] salt)` | 根据参数值，创建Hashids，使用默认#DEFAULT_ALPHABET作为字母表，不限制最小长度 |
| `cn.hutool.core.codec.Hashids` | `Hashids create(final char[] salt,final char[] alphabet,final int minLength)` | 根据参数值，创建Hashids |
| `cn.hutool.core.codec.Hashids` | `Hashids create(final char[] salt,final int minLength)` | 根据参数值，创建Hashids，使用默认#DEFAULT_ALPHABET作为字母表 |
| `cn.hutool.core.codec.Hashids` | `String decodeToHex(final String hash)` | 解码Hash值为16进制数字 |
| `cn.hutool.core.codec.Hashids` | `String encode(final long... numbers)` | 编码给定的数字数组 |
| `cn.hutool.core.codec.Hashids` | `String encodeFromHex(final String hexNumbers)` | 编码给定的16进制数字 |
| `cn.hutool.core.codec.Hashids` | `long[] decode(final String hash)` | 解码Hash值为数字数组 |
| `cn.hutool.core.codec.Morse` | `String decode(String morse)` | 解码 |
| `cn.hutool.core.codec.Morse` | `String encode(String text)` | 编码 |
| `cn.hutool.core.codec.PercentCodec` | `PercentCodec addSafe(char c)` | 增加安全字符 安全字符不被编码 |
| `cn.hutool.core.codec.PercentCodec` | `PercentCodec of(CharSequence chars)` | 创建PercentCodec，使用指定字符串中的字符作为安全字符 |
| `cn.hutool.core.codec.PercentCodec` | `PercentCodec of(PercentCodec codec)` | 从已知PercentCodec创建PercentCodec，会复制给定PercentCodec的安全字符 |
| `cn.hutool.core.codec.PercentCodec` | `PercentCodec or(PercentCodec codec)` | 增加安全字符到挡墙的PercentCodec |
| `cn.hutool.core.codec.PercentCodec` | `PercentCodec orNew(PercentCodec codec)` | 组合当前PercentCodec和指定PercentCodec为一个新的PercentCodec，安全字符为并集 |
| `cn.hutool.core.codec.PercentCodec` | `PercentCodec removeSafe(char c)` | 移除安全字符 安全字符不被编码 |
| `cn.hutool.core.codec.PercentCodec` | `PercentCodec setEncodeSpaceAsPlus(boolean encodeSpaceAsPlus)` | 是否将空格编码为+ 如果为true，则将空格编码为"+"，此项只在"application/x-www-form-urlencoded"中使用 如果为false，则空格编码为"%20",此项一般用于URL的Query部分（RFC3986规范） |
| `cn.hutool.core.codec.PercentCodec` | `String encode(CharSequence path,Charset charset,char... customSafeChar)` | 将URL中的字符串编码为%形式 |
| `cn.hutool.core.codec.PunyCode` | `String decode(String input)` | 解码 PunyCode为字符串 |
| `cn.hutool.core.codec.PunyCode` | `String decodeDomain(String domain)` | 解码punycode域名 |
| `cn.hutool.core.codec.PunyCode` | `String encode(CharSequence input)` | 将内容编码为PunyCode |
| `cn.hutool.core.codec.PunyCode` | `String encode(CharSequence input,boolean withPrefix)` | 将内容编码为PunyCode |
| `cn.hutool.core.codec.PunyCode` | `String encodeDomain(String domain)` | punycode转码域名 |
| `cn.hutool.core.codec.Rot` | `String decode(String rot,int offset,boolean isDecodeNumber)` | RotN解码 |
| `cn.hutool.core.codec.Rot` | `String decode13(String rot)` | Rot-13解码，同时解码数字 |
| `cn.hutool.core.codec.Rot` | `String decode13(String rot,boolean isDecodeNumber)` | Rot-13解码 |
| `cn.hutool.core.codec.Rot` | `String encode(String message,int offset,boolean isEncodeNumber)` | RotN编码 |
| `cn.hutool.core.codec.Rot` | `String encode13(String message)` | Rot-13编码，同时编码数字 |
| `cn.hutool.core.codec.Rot` | `String encode13(String message,boolean isEncodeNumber)` | Rot-13编码 |
