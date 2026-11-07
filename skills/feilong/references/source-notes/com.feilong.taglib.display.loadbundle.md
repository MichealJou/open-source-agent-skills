# com.feilong.taglib.display.loadbundle

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.taglib.display.loadbundle.LoadBundleBuilder` | `Map<String, String> build(LoadBundleParam loadBundleParam)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.display.loadbundle.LoadBundleParam` | `Locale getLocale()` | 获得 国际化当前语言,如果不传,那么使用默认的 Locale#getDefault(). |
| `com.feilong.taglib.display.loadbundle.LoadBundleParam` | `String getBaseName()` | 获得 配置文件的路径, 用于 ResourceBundleUtil,比如如果在i18n文件下面有 edu-en. |
| `com.feilong.taglib.display.loadbundle.LoadBundleParam` | `boolean equals(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.display.loadbundle.LoadBundleParam` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.display.loadbundle.LoadBundleParam` | `void setBaseName(String baseName)` | 设置 配置文件的路径, 用于 ResourceBundleUtil,比如如果在i18n文件下面有 edu-en. |
| `com.feilong.taglib.display.loadbundle.LoadBundleParam` | `void setLocale(Locale locale)` | 设置 国际化当前语言,如果不传,那么使用默认的 Locale#getDefault(). |
| `com.feilong.taglib.display.loadbundle.LoadBundleTag` | `void setVar(String var)` | 设置 存储在作用于里面的属性名称. |
