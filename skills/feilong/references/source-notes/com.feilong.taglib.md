# com.feilong.taglib

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.taglib.AbstractConditionalTag` | `int doStartTag()` | 标签开始. |
| `com.feilong.taglib.AbstractEndWriteContentTag` | `int doEndTag()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.AbstractEndWriteContentTag` | `int doStartTag()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.AbstractLocaleSupportTag` | `void setBaseName(String baseName)` | 配置文件的路径, 用于 ResourceBundleUtil,比如如果在i18n文件下面有 edu-en.properties那么baseName就是去掉后缀,并且去掉语言的值:i18n/edu . |
| `com.feilong.taglib.AbstractLocaleSupportTag` | `void setLocale(Object locale)` | 设置Locale 环境, 支持 java.util.Locale 或 String 类型的实例 ,如果是null,将默认使用 request.getLocale() . |
| `com.feilong.taglib.AbstractStartWriteContentTag` | `int doStartTag()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.BaseTag` | `void doCatch(Throwable t)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.BaseTag` | `void doFinally()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.CacheTag` | `String buildCacheTagKey()` | 【原文待译】Builds the cache tag key. |
| `com.feilong.taglib.LocaleSupport` | `void setLocale(Object locale)` | 设置Locale 环境, 支持 java.util.Locale 或 String 类型的实例 ,如果是null,将默认使用 request.getLocale() . |
| `com.feilong.taglib.SimpleTagStringCacheManager` | `Object get(String key)` | 【原文待译】Builds the options. |
| `com.feilong.taglib.SimpleTagStringCacheManager` | `void put(String cacheParam,Object content)` | 设置. |
| `com.feilong.taglib.TagUtils` | `T findAttributeValue(PageContext pageContext,String attributeName,String scope)` | 【原文待译】Find attribute value. |
| `com.feilong.taglib.TagUtils` | `int getScope(String scope)` | 【原文待译】Determines the scope for a given input String. If the String does not match 'request', 'session', 'page' or 'application', the method will return PageContext#PAGE_SCOPE. |
