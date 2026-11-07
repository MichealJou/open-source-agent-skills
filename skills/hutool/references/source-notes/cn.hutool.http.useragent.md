# cn.hutool.http.useragent

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.http.useragent.Browser` | `String getVersion(String userAgentString)` | 获取浏览器版本 |
| `cn.hutool.http.useragent.Browser` | `boolean isMobile()` | 是否移动浏览器 |
| `cn.hutool.http.useragent.Browser` | `void addCustomBrowser(String name,String regex,String versionRegex)` | 添加自定义的浏览器类型 |
| `cn.hutool.http.useragent.Engine` | `String getVersion(String userAgentString)` | 获取引擎版本 |
| `cn.hutool.http.useragent.OS` | `String getVersion(String userAgentString)` | 获取浏览器版本 |
| `cn.hutool.http.useragent.OS` | `boolean isMacOS()` | 是否为MacOS |
| `cn.hutool.http.useragent.OS` | `void addCustomOs(String name,String regex,String versionRegex)` | 添加自定义的系统类型 |
| `cn.hutool.http.useragent.Platform` | `boolean isAndroid()` | 是否为Android平台，包括Android和Google TV |
| `cn.hutool.http.useragent.Platform` | `boolean isHarmony()` | 是否为Harmony平台 |
| `cn.hutool.http.useragent.Platform` | `boolean isIPad()` | 是否为Iphone或者iPod设备 |
| `cn.hutool.http.useragent.Platform` | `boolean isIPhoneOrIPod()` | 是否为Iphone或者iPod设备 |
| `cn.hutool.http.useragent.Platform` | `boolean isIos()` | 是否为IOS平台，包括IPhone、IPod、IPad |
| `cn.hutool.http.useragent.Platform` | `boolean isMobile()` | 是否为移动平台 |
| `cn.hutool.http.useragent.UserAgent` | `Browser getBrowser()` | 获取浏览器类型 |
| `cn.hutool.http.useragent.UserAgent` | `Engine getEngine()` | 获取引擎类型 |
| `cn.hutool.http.useragent.UserAgent` | `OS getOs()` | 获取系统类型 |
| `cn.hutool.http.useragent.UserAgent` | `Platform getPlatform()` | 获取平台类型 |
| `cn.hutool.http.useragent.UserAgent` | `String getEngineVersion()` | 获取引擎版本 |
| `cn.hutool.http.useragent.UserAgent` | `String getOsVersion()` | 获取系统版本 |
| `cn.hutool.http.useragent.UserAgent` | `String getVersion()` | 获取浏览器版本 |
| `cn.hutool.http.useragent.UserAgent` | `boolean isMobile()` | 是否为移动平台 |
| `cn.hutool.http.useragent.UserAgent` | `void setBrowser(Browser browser)` | 设置浏览器类型 |
| `cn.hutool.http.useragent.UserAgent` | `void setEngine(Engine engine)` | 设置引擎类型 |
| `cn.hutool.http.useragent.UserAgent` | `void setEngineVersion(String engineVersion)` | 设置引擎版本 |
| `cn.hutool.http.useragent.UserAgent` | `void setMobile(boolean mobile)` | 设置是否为移动平台 |
| `cn.hutool.http.useragent.UserAgent` | `void setOs(OS os)` | 设置系统类型 |
| `cn.hutool.http.useragent.UserAgent` | `void setOsVersion(String osVersion)` | 设置系统版本 |
| `cn.hutool.http.useragent.UserAgent` | `void setPlatform(Platform platform)` | 设置平台类型 |
| `cn.hutool.http.useragent.UserAgent` | `void setVersion(String version)` | 设置浏览器版本 |
| `cn.hutool.http.useragent.UserAgentInfo` | `Pattern getPattern()` | 获取匹配模式 |
| `cn.hutool.http.useragent.UserAgentInfo` | `String getName()` | 获取信息名称 |
| `cn.hutool.http.useragent.UserAgentInfo` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.useragent.UserAgentInfo` | `boolean equals(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.useragent.UserAgentInfo` | `boolean isMatch(String content)` | 指定内容中是否包含匹配此信息的内容 |
| `cn.hutool.http.useragent.UserAgentInfo` | `boolean isUnknown()` | 是否为Unknown |
| `cn.hutool.http.useragent.UserAgentInfo` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.useragent.UserAgentParser` | `UserAgent parse(String userAgentString)` | 解析User-Agent |
| `cn.hutool.http.useragent.UserAgentUtil` | `UserAgent parse(String userAgentString)` | 解析User-Agent |
