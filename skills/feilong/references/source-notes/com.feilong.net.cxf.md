# com.feilong.net.cxf

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.cxf.ClientUtil` | `void wrap(Client client)` | 封装 TLSClientParameters. |
| `com.feilong.net.cxf.JaxWsDynamicClientUtil` | `T call(String wsdlUrl,String operationName,Object... params)` | 调用webservice. |
| `com.feilong.net.cxf.JaxWsDynamicClientUtil` | `void setDefaultHostnameVerifierTrue()` | 如果没有这段代码, 对于 https://203.94.12.226:58443/***_official_ws/OfficialWebservice?wsdl 这么一段 ip+https 的wsdl 的调用, 将会出现 以下异常信息 |
