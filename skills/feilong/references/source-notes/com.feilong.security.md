# com.feilong.security

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.security.Base64Util` | `String encodeBase64(String str,Charset charset)` | 【原文待译】Encode base 64. |
| `com.feilong.security.Base64Util` | `String encodeBase64(String str,String charsetName)` | 【原文待译】Encode base 64. |
| `com.feilong.security.Base64Util` | `String encodeBase64(byte[] bytes)` | 【原文待译】Encode base 64. |
| `com.feilong.security.ByteUtil` | `String byteToHexStringLowerCase(byte b)` | 字节转成16进制小写字符串. Example: |
| `com.feilong.security.ByteUtil` | `String bytesToHexStringLowerCase(byte[] b)` | 字节数组,转成小写的16进制字符串. md5加密使用这个. same as: |
| `com.feilong.security.ByteUtil` | `String bytesToHexStringUpperCase(byte[] bytes)` | 字节数组,转成大写的16进制字符串 . 网友gdpglc的思路. |
| `com.feilong.security.ByteUtil` | `byte uniteBytes(byte byte1,byte byte2)` | 将两个ASCII字符合成一个字节,如:"EF"--> 0xEF. |
| `com.feilong.security.ByteUtil` | `byte[] hexBytesToBytes(byte[] bytes)` | 16进制字符串转成字节数组. |
| `com.feilong.security.ByteUtil` | `byte[] hexBytesToBytes2(byte[] bytes)` | 将指定字符串hexString,以每两个字符分割转换为16进制形式. 如:"2B44EFD9" --> byte[] 0x2B, 0x44, 0xEF, 0xD9 . |
| `com.feilong.security.KeyUtil` | `Key generatePrivateKey(String privateKeyString)` | 基于私钥字符串, 生成私钥. |
| `com.feilong.security.KeyUtil` | `Key generatePrivateKey(String privateKeyString,String algorithm)` | 基于私钥字符串, 生成私钥. |
