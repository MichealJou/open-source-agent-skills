# com.feilong.security.oneway

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.security.oneway.MD5Util` | `String encode(String origin)` | 使用md5算法 单向加密字符串(小写格式). 加密之后的转成 小写的 16进制,长度32位的字符串 如果你要大写的值,请调用 #encodeUpperCase(String) |
| `com.feilong.security.oneway.MD5Util` | `String encode(String origin,String charsetName)` | 使用md5算法 单向加密字符串. 加密之后的转成 小写的 16进制,长度32位的字符串 |
| `com.feilong.security.oneway.MD5Util` | `String encode(byte[] inputBytes)` | 使用md5算法 单向加密 inputBytes. 加密之后的转成 小写的 16进制,长度32位的字符串 |
| `com.feilong.security.oneway.MD5Util` | `String encodeFile(String location)` | 计算文件的单向加密值. |
| `com.feilong.security.oneway.MD5Util` | `String encodeUpperCase(String origin)` | 使用md5算法 单向加密字符串返回大写格式. 加密之后的转成 大写的 16进制,长度32位的字符串; 如果你要小写的值,请调用 #encode(String) |
| `com.feilong.security.oneway.OnewayEncryption` | `String encode(OnewayType onewayType,String origin)` | 使用算法 单向加密字符串. |
| `com.feilong.security.oneway.OnewayEncryption` | `String encode(OnewayType onewayType,String origin,String charsetName)` | 使用算法 单向加密字符串. |
| `com.feilong.security.oneway.OnewayEncryption` | `String encode(OnewayType onewayType,byte[] inputBytes)` | 使用算法 单向加密byte[],返回的值是小写的16进制字符串 |
| `com.feilong.security.oneway.OnewayEncryption` | `String encodeFile(OnewayType onewayType,String location)` | 计算文件的加密值. |
| `com.feilong.security.oneway.OnewayEncryption` | `String encodeUpperCase(OnewayType onewayType,String origin)` | 使用算法单向加密字符串,返回大写格式. |
| `com.feilong.security.oneway.OnewayType` | `String getAlgorithm()` | Gets the 算法. |
| `com.feilong.security.oneway.SHA1Util` | `String encode(String origin)` | 使用sha1算法 单向加密字符串. 加密之后的转成 小写的 16进制字符串 |
| `com.feilong.security.oneway.SHA1Util` | `String encode(String origin,String charsetName)` | 使用sha1算法 单向加密字符串. 加密之后的转成 小写的 16进制字符串 |
| `com.feilong.security.oneway.SHA1Util` | `String encode(byte[] inputBytes)` | 使用sha1算法 单向加密 inputBytes. 加密之后的转成 小写的 16进制,长度32位的字符串 |
| `com.feilong.security.oneway.SHA1Util` | `String encodeFile(String location)` | 计算文件的单向加密值. |
| `com.feilong.security.oneway.SHA1Util` | `String encodeUpperCase(String origin)` | 使用sha1算法 单向加密字符串(大写). 加密之后的转成 大写的 16进制字符串 |
| `com.feilong.security.oneway.SHA256Util` | `String encode(String origin)` | 使用sha256算法 单向加密字符串(小写). 加密之后的转成 小写的 16进制字符串 |
| `com.feilong.security.oneway.SHA256Util` | `String encode(String origin,String charsetName)` | 使用sha256算法 单向加密字符串. 加密之后的转成 小写的 16进制字符串 |
| `com.feilong.security.oneway.SHA256Util` | `String encode(byte[] inputBytes)` | 使用sha256算法 单向加密 inputBytes. 加密之后的转成 小写的 16进制,长度32位的字符串 |
| `com.feilong.security.oneway.SHA256Util` | `String encodeFile(String location)` | 计算文件的单向加密值. |
| `com.feilong.security.oneway.SHA256Util` | `String encodeUpperCase(String origin)` | 使用sha256算法 单向加密字符串(大写). 加密之后的转成 大写的 16进制字符串 |
| `com.feilong.security.oneway.SHA384Util` | `String encode(String origin)` | 使用sha384算法 单向加密字符串(小写). 加密之后的转成 小写的 16进制字符串 |
| `com.feilong.security.oneway.SHA384Util` | `String encode(String origin,String charsetName)` | 使用sha384算法 单向加密字符串. 加密之后的转成 小写的 16进制字符串 |
| `com.feilong.security.oneway.SHA384Util` | `String encode(byte[] inputBytes)` | 使用sha384算法 单向加密 inputBytes. 加密之后的转成 小写的 16进制,长度32位的字符串 |
| `com.feilong.security.oneway.SHA384Util` | `String encodeFile(String location)` | 计算文件的单向加密值. |
| `com.feilong.security.oneway.SHA384Util` | `String encodeUpperCase(String origin)` | 使用sha384算法 单向加密字符串(大写). 加密之后的转成 大写的 16进制字符串 |
| `com.feilong.security.oneway.SHA512Util` | `String encode(String origin)` | 使用sha512算法 单向加密字符串(小写). 加密之后的转成 小写的 16进制字符串 |
| `com.feilong.security.oneway.SHA512Util` | `String encode(String origin,String charsetName)` | 使用sha512算法 单向加密字符串(小写). 加密之后的转成 小写的 16进制字符串 |
| `com.feilong.security.oneway.SHA512Util` | `String encode(byte[] inputBytes)` | 使用sha512算法 单向加密 inputBytes. 加密之后的转成 小写的 16进制,长度32位的字符串 |
| `com.feilong.security.oneway.SHA512Util` | `String encodeFile(String location)` | 计算文件的单向加密值. |
| `com.feilong.security.oneway.SHA512Util` | `String encodeUpperCase(String origin)` | 使用sha512算法 单向加密字符串(大写). 加密之后的转成 大写的 16进制字符串 |
| `com.feilong.security.oneway.Sm3Util` | `String encode(String origin)` | 使用Sm3算法 单向加密字符串. 加密之后的转成 小写的 16进制字符串 |
| `com.feilong.security.oneway.Sm3Util` | `String encode(String origin,String charsetName)` | 使用Sm3算法 单向加密字符串. 加密之后的转成 小写的 16进制字符串 |
| `com.feilong.security.oneway.Sm3Util` | `String encode(byte[] inputBytes)` | 使用Sm3算法 单向加密 inputBytes. 加密之后的转成 小写的 16进制,长度32位的字符串 |
| `com.feilong.security.oneway.Sm3Util` | `String encodeFile(String location)` | 计算文件的单向加密值. |
| `com.feilong.security.oneway.Sm3Util` | `String encodeUpperCase(String origin)` | 使用Sm3算法 单向加密字符串(大写). 加密之后的转成 大写的 16进制字符串 |
