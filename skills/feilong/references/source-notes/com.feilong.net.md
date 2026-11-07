# com.feilong.net

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.SSLContextBuilder` | `SSLContext build(String protocol)` | 构造 SSLContext. |
| `com.feilong.net.UriProcessor` | `String process(String uri,boolean isTrimUri)` | 获得 请求的uri地址. 如果uri是null,将返回empty 如果uri中有空格,将会替换成%20 |
