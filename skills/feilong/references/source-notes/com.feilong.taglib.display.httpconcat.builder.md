# com.feilong.taglib.display.httpconcat.builder

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.taglib.display.httpconcat.builder.DomainRebuilder` | `String rebuild(String domain,HttpServletRequest request)` | 如果domain 是null或者 empty 那么会使用 javax.servlet.http.HttpServletRequest#getContextPath(). |
| `com.feilong.taglib.display.httpconcat.builder.HttpConcatParamBuilder` | `HttpConcatParam build(String blockContent,String type,String domain,String root,String version,Boolean httpConcatSupport)` | 【原文待译】Builds the. |
| `com.feilong.taglib.display.httpconcat.builder.HttpConcatParamBuilder` | `HttpConcatParam standardHttpConcatParam(List<String> itemSrcList,HttpConcatParam httpConcatParam)` | 标准化 httpConcatParam,比如标准化domain等等. |
| `com.feilong.taglib.display.httpconcat.builder.ResultBuilder` | `String build(List<String> itemSrcList,HttpConcatParam httpConcatParam)` | 构造content. |
| `com.feilong.taglib.display.httpconcat.builder.TemplateFactory` | `String getTemplate(String type)` | 不同的type不同的模板. |
| `com.feilong.taglib.display.httpconcat.builder.VersionRebuilder` | `String rebuild(String version,PageContext pageContext)` | 【原文待译】Rebuild version. |
