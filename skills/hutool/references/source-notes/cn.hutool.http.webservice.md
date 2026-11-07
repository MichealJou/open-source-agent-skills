# cn.hutool.http.webservice

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.http.webservice.JakartaSoapClient` | `HttpResponse sendForResponse()` | 发送请求，获取异步响应 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient charset(Charset charset)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient create(String url)` | 创建SOAP客户端，默认使用soap1.1版本协议 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient create(String url,SoapProtocol protocol)` | 创建SOAP客户端 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient create(String url,SoapProtocol protocol,String namespaceURI)` | 创建SOAP客户端 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient init(SoapProtocol protocol)` | 初始化 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient reset()` | 重置SOAP客户端，用于客户端复用 重置后需调用serMethod方法重新指定请求方法，并调用setParam方法重新定义参数 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient setCharset(Charset charset)` | 设置编码 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient setConnectionTimeout(int milliseconds)` | 设置连接超时，单位：毫秒 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient setMethod(Name name,Map<String, Object> params,boolean useMethodPrefix)` | 设置请求方法 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient setMethod(QName name)` | 设置请求方法 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient setMethod(QName name,Map<String, Object> params,boolean useMethodPrefix)` | 设置请求方法 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient setMethod(String methodName)` | 设置请求方法 方法名自动识别前缀，前缀和方法名使用“:”分隔 当识别到前缀后，自动添加xmlns属性，关联到默认的namespaceURI |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient setMethod(String methodName,String namespaceURI)` | 设置请求方法 方法名自动识别前缀，前缀和方法名使用“:”分隔 当识别到前缀后，自动添加xmlns属性，关联到传入的namespaceURI |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient setParam(String name,Object value)` | 设置方法参数，使用方法的前缀 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient setParam(String name,Object value,boolean useMethodPrefix)` | 设置方法参数 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient setParams(Map<String, Object> params)` | 批量设置参数，使用方法的前缀 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient setParams(Map<String, Object> params,boolean useMethodPrefix)` | 批量设置参数 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient setReadTimeout(int milliseconds)` | 设置连接超时，单位：毫秒 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient setUrl(String url)` | 设置Webservice请求地址 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient timeout(int milliseconds)` | 设置超时，单位：毫秒 超时包括： |
| `cn.hutool.http.webservice.JakartaSoapClient` | `JakartaSoapClient write(OutputStream out)` | 将SOAP消息的XML内容输出到流 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `SOAPBodyElement getMethodEle()` | 获取方法节点 用于创建子节点等操作 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `SOAPHeaderElement addSOAPHeader(QName name)` | 增加SOAP头信息，方法返回SOAPHeaderElement可以设置具体属性和子节点 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `SOAPHeaderElement addSOAPHeader(QName name,String actorURI,String roleUri,Boolean mustUnderstand,Boolean relay)` | 增加SOAP头信息，方法返回SOAPHeaderElement可以设置具体属性和子节点 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `SOAPHeaderElement addSOAPHeader(String localName)` | 增加SOAP头信息，方法返回SOAPHeaderElement可以设置具体属性和子节点 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `SOAPHeaderElement addSOAPHeader(String localName,String value)` | 增加SOAP头信息，方法返回SOAPHeaderElement可以设置具体属性和子节点 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `SOAPMessage getMessage()` | 获取SOAP消息对象 SOAPMessage |
| `cn.hutool.http.webservice.JakartaSoapClient` | `SOAPMessage sendForMessage()` | 执行Webservice请求，即发送SOAP内容 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `String getMsgStr(boolean pretty)` | 获取SOAP请求消息 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `String send()` | 执行Webservice请求，即发送SOAP内容 |
| `cn.hutool.http.webservice.JakartaSoapClient` | `String send(boolean pretty)` | 执行Webservice请求，即发送SOAP内容 |
| `cn.hutool.http.webservice.JakartaSoapProtocol` | `String getValue()` | 获取版本值信息 |
| `cn.hutool.http.webservice.JakartaSoapUtil` | `SoapClient createClient(String url)` | 创建SOAP客户端，默认使用soap1.1版本协议 |
| `cn.hutool.http.webservice.JakartaSoapUtil` | `SoapClient createClient(String url,SoapProtocol protocol)` | 创建SOAP客户端 |
| `cn.hutool.http.webservice.JakartaSoapUtil` | `SoapClient createClient(String url,SoapProtocol protocol,String namespaceURI)` | 创建SOAP客户端 |
| `cn.hutool.http.webservice.JakartaSoapUtil` | `String toString(SOAPMessage message,boolean pretty)` | SOAPMessage 转为字符串 |
| `cn.hutool.http.webservice.JakartaSoapUtil` | `String toString(SOAPMessage message,boolean pretty,Charset charset)` | SOAPMessage 转为字符串 |
| `cn.hutool.http.webservice.SoapClient` | `HttpResponse sendForResponse()` | 发送请求，获取异步响应 |
| `cn.hutool.http.webservice.SoapClient` | `SOAPBodyElement getMethodEle()` | 获取方法节点 用于创建子节点等操作 |
| `cn.hutool.http.webservice.SoapClient` | `SOAPHeaderElement addSOAPHeader(QName name)` | 增加SOAP头信息，方法返回SOAPHeaderElement可以设置具体属性和子节点 |
| `cn.hutool.http.webservice.SoapClient` | `SOAPHeaderElement addSOAPHeader(QName name,String actorURI,String roleUri,Boolean mustUnderstand,Boolean relay)` | 增加SOAP头信息，方法返回SOAPHeaderElement可以设置具体属性和子节点 |
| `cn.hutool.http.webservice.SoapClient` | `SOAPHeaderElement addSOAPHeader(String localName)` | 增加SOAP头信息，方法返回SOAPHeaderElement可以设置具体属性和子节点 |
| `cn.hutool.http.webservice.SoapClient` | `SOAPHeaderElement addSOAPHeader(String localName,String value)` | 增加SOAP头信息，方法返回SOAPHeaderElement可以设置具体属性和子节点 |
| `cn.hutool.http.webservice.SoapClient` | `SOAPMessage getMessage()` | 获取SOAP消息对象 SOAPMessage |
| `cn.hutool.http.webservice.SoapClient` | `SOAPMessage sendForMessage()` | 执行Webservice请求，即发送SOAP内容 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient charset(Charset charset)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient create(String url)` | 创建SOAP客户端，默认使用soap1.1版本协议 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient create(String url,SoapProtocol protocol)` | 创建SOAP客户端 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient create(String url,SoapProtocol protocol,String namespaceURI)` | 创建SOAP客户端 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient init(SoapProtocol protocol)` | 初始化 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient reset()` | 重置SOAP客户端，用于客户端复用 重置后需调用serMethod方法重新指定请求方法，并调用setParam方法重新定义参数 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient setCharset(Charset charset)` | 设置编码 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient setConnectionTimeout(int milliseconds)` | 设置连接超时，单位：毫秒 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient setMethod(Name name,Map<String, Object> params,boolean useMethodPrefix)` | 设置请求方法 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient setMethod(QName name)` | 设置请求方法 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient setMethod(QName name,Map<String, Object> params,boolean useMethodPrefix)` | 设置请求方法 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient setMethod(String methodName)` | 设置请求方法 方法名自动识别前缀，前缀和方法名使用“:”分隔 当识别到前缀后，自动添加xmlns属性，关联到默认的namespaceURI |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient setMethod(String methodName,String namespaceURI)` | 设置请求方法 方法名自动识别前缀，前缀和方法名使用“:”分隔 当识别到前缀后，自动添加xmlns属性，关联到传入的namespaceURI |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient setParam(String name,Object value)` | 设置方法参数，使用方法的前缀 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient setParam(String name,Object value,boolean useMethodPrefix)` | 设置方法参数 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient setParams(Map<String, Object> params)` | 批量设置参数，使用方法的前缀 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient setParams(Map<String, Object> params,boolean useMethodPrefix)` | 批量设置参数 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient setReadTimeout(int milliseconds)` | 设置连接超时，单位：毫秒 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient setUrl(String url)` | 设置Webservice请求地址 |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient timeout(int milliseconds)` | 设置超时，单位：毫秒 超时包括： |
| `cn.hutool.http.webservice.SoapClient` | `SoapClient write(OutputStream out)` | 将SOAP消息的XML内容输出到流 |
| `cn.hutool.http.webservice.SoapClient` | `String getMsgStr(boolean pretty)` | 获取SOAP请求消息 |
| `cn.hutool.http.webservice.SoapClient` | `String send()` | 执行Webservice请求，即发送SOAP内容 |
| `cn.hutool.http.webservice.SoapClient` | `String send(boolean pretty)` | 执行Webservice请求，即发送SOAP内容 |
| `cn.hutool.http.webservice.SoapProtocol` | `String getValue()` | 获取版本值信息 |
| `cn.hutool.http.webservice.SoapUtil` | `SoapClient createClient(String url)` | 创建SOAP客户端，默认使用soap1.1版本协议 |
| `cn.hutool.http.webservice.SoapUtil` | `SoapClient createClient(String url,SoapProtocol protocol)` | 创建SOAP客户端 |
| `cn.hutool.http.webservice.SoapUtil` | `SoapClient createClient(String url,SoapProtocol protocol,String namespaceURI)` | 创建SOAP客户端 |
| `cn.hutool.http.webservice.SoapUtil` | `String toString(SOAPMessage message,boolean pretty)` | SOAPMessage 转为字符串 |
| `cn.hutool.http.webservice.SoapUtil` | `String toString(SOAPMessage message,boolean pretty,Charset charset)` | SOAPMessage 转为字符串 |
