# com.feilong.taglib.display.httpconcat.command

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `Boolean getHttpConcatSupport()` | 获得 是否支持 HTTP_CONCAT (全局参数). |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `Integer getAutoPartitionSize()` | 自动分片大小. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `String getDomain()` | 获得 全局的域名. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `String getTemplateCss()` | 获得 the template css. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `String getTemplateJs()` | 获得 the template js. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `String getVersionAutoRefreshValue()` | 当version 值是指定value的时候, 每次自动变. httpconcat.version.autoRefresh.value |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `String getVersionEncode()` | version值的加密格式,值可以是 md5 或者sha1 (忽视大小写). # 如果没有配置, 那么显示原样内容 # 如果需要这个功能, 需要依赖 feilong-security jar httpconcat.version.encode= |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `String getVersionNameInScope()` | httpconcat version 作用域里面变量名字. # 如果没有配置或者是空,那么不会去作用域中查找 httpconcat.version.nameInScope=httpconcatVersion |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `String getVersionSearchScope()` | version 名字在哪个作用域. # 如果没有值那么会依次从系列作用域中去找值 page request session application httpconcat.version.search.scope= |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `boolean getDefaultCacheEnable()` | 获得 default cache enable. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `int getDefaultCacheSizeLimit()` | cache size 限制,仅当 #defaultCacheEnable开启生效, 当cache数达到 #defaultCacheEnable,将不会再缓存结果 经过测试 300000 size cache占用 内存 :87.43KB(非精准) 304850 size cache占用 内存 :87.43KB(非精准) 400000 size cache占用 内存 :8.36MB(非精准) 对于一个正式项目而言,http concat的cache, size极限大小会是 |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `void setAutoPartitionSize(Integer autoPartitionSize)` | 自动分片大小. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `void setDefaultCacheEnable(boolean defaultCacheEnable)` | 设置 default cache enable. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `void setDefaultCacheSizeLimit(int defaultCacheSizeLimit)` | cache size 限制,仅当 #defaultCacheEnable开启生效, 当cache数达到 #defaultCacheEnable,将不会再缓存结果 经过测试 300000 size cache占用 内存 :87.43KB(非精准) 304850 size cache占用 内存 :87.43KB(非精准) 400000 size cache占用 内存 :8.36MB(非精准) 对于一个正式项目而言,http concat的cache, size极限大小会是 |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `void setDomain(String domain)` | 设置 全局的域名. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `void setHttpConcatSupport(Boolean httpConcatSupport)` | 设置 是否支持 HTTP_CONCAT (全局参数). |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `void setTemplateCss(String templateCss)` | 设置 the template css. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `void setTemplateJs(String templateJs)` | 设置 the template js. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `void setVersionAutoRefreshValue(String versionAutoRefreshValue)` | 当version 值是指定value的时候, 每次自动变. httpconcat.version.autoRefresh.value |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `void setVersionEncode(String versionEncode)` | version值的加密格式,值可以是 md5 或者sha1 (忽视大小写). # 如果没有配置, 那么显示原样内容 # 如果需要这个功能, 需要依赖 feilong-security jar httpconcat.version.encode= |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `void setVersionNameInScope(String versionNameInScope)` | httpconcat version 作用域里面变量名字. # 如果没有配置或者是空,那么不会去作用域中查找 httpconcat.version.nameInScope=httpconcatVersion |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatGlobalConfig` | `void setVersionSearchScope(String versionSearchScope)` | version 名字在哪个作用域. # 如果没有值那么会依次从系列作用域中去找值 page request session application httpconcat.version.search.scope= |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatParam` | `Boolean getHttpConcatSupport()` | 获得 是否支持 http concat(如果设置这个参数,本次渲染,将会覆盖全局变量). |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatParam` | `String getContent()` | 获得 内容(原样内容,内部解析). |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatParam` | `String getDomain()` | 获得 the domain. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatParam` | `String getRoot()` | 根目录. 如果设置root为'/script' 会拼成http://staging.feilongstore.com.cn/script/??jquery/jquery-1.4.2.min.js?2013022801 |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatParam` | `String getType()` | 获得 类型css/js. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatParam` | `String getVersion()` | 获得 版本号. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatParam` | `boolean equals(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatParam` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatParam` | `void setContent(String content)` | 设置 内容(原样内容,内部解析). |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatParam` | `void setDomain(String domain)` | 设置 the domain. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatParam` | `void setHttpConcatSupport(Boolean httpConcatSupport)` | 设置 是否支持 http concat(如果设置这个参数,本次渲染,将会覆盖全局变量). |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatParam` | `void setRoot(String root)` | 根目录. 如果设置root为'/script' 会拼成http://staging.feilongstore.com.cn/script/??jquery/jquery-1.4.2.min.js?2013022801 |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatParam` | `void setType(String type)` | 设置 类型css/js. |
| `com.feilong.taglib.display.httpconcat.command.HttpConcatParam` | `void setVersion(String version)` | 设置 版本号. |
