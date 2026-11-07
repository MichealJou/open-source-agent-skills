# com.feilong.core.net

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.core.net.ParamUtil` | `Map<String, String> toSingleValueMap(String queryString,String charsetType)` | 将a=1&b=2这样格式的 queryString 数据转换成map. |
| `com.feilong.core.net.ParamUtil` | `String addParameter(String uriString,String paramName,String paramValue,String charsetType)` | 给指定的 uriString 添加指定的参数 paramName 和值 paramValue . |
| `com.feilong.core.net.ParamUtil` | `String addParameterArrayValueMap(String uriString,Map<String, String[]> arrayValueMap,String charsetType)` | 给指定的 uriString 添加参数 arrayValueMap ,如果uri包含指定的参数名字,那么会被新的值替换. |
| `com.feilong.core.net.ParamUtil` | `String addParameterSingleValueMap(String uriString,Map<String, String> singleValueMap,String charsetType)` | 给指定的 uriString 添加指定的参数 singleValueMap . |
| `com.feilong.core.net.ParamUtil` | `String joinValuesOrderByIncludeKeys(Map<K, String> singleValueMap,K... includeKeys)` | 在 singleValueMap 中取到指定 includeKeys key的 value ,连接起来( 不使用任何连接符 ). |
| `com.feilong.core.net.ParamUtil` | `String toNaturalOrderingJoinValue(Map<String, String> singleValueMap)` | 将 singleValueMap 转成 自然排序 , 然后仅将value直接拼接成字符串( 不使用 = 和& 分隔 ). 已知,适用于 银联大华捷通 |
| `com.feilong.core.net.ParamUtil` | `String toNaturalOrderingKeyJoinValue(Map<String, String> singleValueMap)` | 将 singleValueMap 转成 自然排序 , 然后将key和value直接拼接成字符串( 不使用 = 和& 分隔 ). 已知,适用于 网易易盾验证码 |
| `com.feilong.core.net.ParamUtil` | `String toNaturalOrderingQueryString(Map<String, String> singleValueMap)` | 将 singleValueMap 转成 自然排序 的 queryString 字符串. |
| `com.feilong.core.net.ParamUtil` | `String toQueryStringUseArrayValueMap(Map<String, String[]> arrayValueMap)` | 只是简单的将map的key value 连接起来,最终格式类似于 url 的queryString. |
| `com.feilong.core.net.ParamUtil` | `String toQueryStringUseSingleValueMap(Map<String, String> singleValueMap)` | 将 singleValueMap 转成 queryString. |
| `com.feilong.core.net.URIUtil` | `String decode(String value)` | 使用默认的 utf-8 来解码一个 application/x-www-form-urlencoded 格式的字符串 . |
| `com.feilong.core.net.URIUtil` | `String decode(String value,String charsetType)` | 使用指定的编码格式 charsetType 来解码一个 application/x-www-form-urlencoded 格式的字符串 . |
| `com.feilong.core.net.URIUtil` | `String decodeIfExceptionDefault(String value,String charsetType,String defaultValue)` | 使用指定的编码格式 charsetType 来解码一个 application/x-www-form-urlencoded 格式的字符串,如果有异常,返回默认值 defaultValue . . |
| `com.feilong.core.net.URIUtil` | `String decodeIfExceptionDefault(String value,String defaultValue)` | 使用默认的 utf-8 来解码一个 application/x-www-form-urlencoded 格式的字符串,如果有异常,返回默认值 defaultValue . |
| `com.feilong.core.net.URIUtil` | `String encode(String value)` | 使用 utf-8 ,将普通的字符串转成 application/x-www-form-urlencoded 格式的字符串. |
| `com.feilong.core.net.URIUtil` | `String encode(String value,String charsetType)` | 使用指定的编码 charsetType ,将普通的字符串转成 application/x-www-form-urlencoded 格式的字符串. |
| `com.feilong.core.net.URIUtil` | `String encodeUri(String uriString,String charsetType)` | 基于 uriString 和 charsetType 创建 URI. |
| `com.feilong.core.net.URIUtil` | `URI create(String uri)` | 直接调用 java.net.URI#create(String) 创造一个URI,异常信息更丰富. |
| `com.feilong.core.net.URIUtil` | `URI create(String uriString,String charsetType)` | 基于 uri字符串和charset创建 URI. |
| `com.feilong.core.net.URLUtil` | `InputStream openStream(URL url)` | 打开当前 url 的连接,并且读取返回 InputStream . 这个方法是以下方法的简写 |
| `com.feilong.core.net.URLUtil` | `String getUnionUrl(String context,String spec)` | 获取联合url,通过在指定的上下文中对给定的 spec 进行解析创建 URL,新的 URL 从给定的上下文 URL 和 spec 参数创建. 网站地址拼接,请使用这个method, 如果文件上传到OSS, OSS返回了两段, 1段是domain,另一段是后面的部分 |
| `com.feilong.core.net.URLUtil` | `String getUnionUrl(URL context,String spec)` | 获取联合url,通过在指定的上下文中对给定的 spec 进行解析创建 URL,新的 URL 从给定的上下文 URL 和 spec 参数创建. 网站地址拼接,请使用这个method |
| `com.feilong.core.net.URLUtil` | `String ifNoHttpOrHttpsProtocolPrependPre(String url,String perfix)` | 判断给定的url地址, 如果没有指定的(http:// 或者 https://)协议前缀(忽视大小写),拼接前缀 perfix |
| `com.feilong.core.net.URLUtil` | `String ifNoProtocolPrependPre(String url,String[] protocolPres,String perfix)` | 判断给定的url地址, 如果没有指定的协议前缀(比如http:// 或者 https://)(忽视大小写),拼接前缀 perfix 通常可以直接使用 #ifNoHttpOrHttpsProtocolPrependPre(String, String)方法 |
| `com.feilong.core.net.URLUtil` | `String transformHttpToHttps(String url)` | 将url http协议转成https协议. 场景: 自己的资源 https:/http: 都支持,默认返回的是 http: , 当合作方需要获取 https: 路径时候,做一次转换. |
| `com.feilong.core.net.URLUtil` | `String transformHttpsToHttp(String url)` | 将url https协议转成http协议. 场景: 自己的资源 https:/http: 都支持,默认返回的是 https: , 当合作方需要获取 http: 路径时候,做一次转换. |
| `com.feilong.core.net.URLUtil` | `String transformProtocol(String url,String oldProtocol,String newProtocol)` | 转换协议. 场景: 自己的资源 oldProtocol/newProtocol 都支持,默认返回的是 oldProtocol , 当合作方需要获取 newProtocol 路径时候,做一次转换. |
| `com.feilong.core.net.URLUtil` | `URI toURI(URL url)` | 将 URL转成 URI. |
| `com.feilong.core.net.URLUtil` | `URL toURL(String spec)` | 将字符串 spec 转成 URL. |
