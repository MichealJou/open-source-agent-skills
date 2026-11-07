# com.feilong.taglib.display.httpconcat.handler

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.taglib.display.httpconcat.handler.ConcatLinkResolver` | `String resolver(List<String> itemSrcList,HttpConcatParam standardHttpConcatParam)` | 获得合并的链接. 去重,删空等操作,已经在 ItemSrcListResolver 做过了 |
| `com.feilong.taglib.display.httpconcat.handler.ConcatLinkResolver` | `String resolverNoConcatLink(String itemSrc,HttpConcatParam standardHttpConcatParam)` | 获得不需要 Concat 的连接. |
| `com.feilong.taglib.display.httpconcat.handler.DomainFormatter` | `String format(String domain)` | 格式化 domain 成 http://www.feilong.com/ 形式. |
| `com.feilong.taglib.display.httpconcat.handler.ItemSrcListResolver` | `List<String> resolve(String blockContent,String domain)` | 【原文待译】Resolve. |
| `com.feilong.taglib.display.httpconcat.handler.RootFormatter` | `String format(String root)` | 格式化 root 成 xxxx/xxx/ 形式,. |
| `com.feilong.taglib.display.httpconcat.handler.TypeFormatter` | `String format(String type,List<String> itemSrcList)` | 【原文待译】Builds the type. |
| `com.feilong.taglib.display.httpconcat.handler.VersionFormatter` | `String format(String version)` | 【原文待译】Format. |
