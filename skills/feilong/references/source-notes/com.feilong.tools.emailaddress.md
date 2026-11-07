# com.feilong.tools.emailaddress

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.tools.emailaddress.EmailAddressUtil` | `EmailProvider getEmailProvider(String emailAddress)` | 基于 emailAddress 获得 EmailProvider . |
| `com.feilong.tools.emailaddress.EmailAddressUtil` | `String getDomain(String emailAddress)` | 获得邮件地址的后缀名. |
| `com.feilong.tools.emailaddress.EmailAddressUtil` | `String getUser(String emailAddress)` | 获得邮件地址的前缀. |
| `com.feilong.tools.emailaddress.EmailProvider` | `String getDomain()` | 邮箱domain部分, 如果邮箱是 feilong@163.com, 那么值是 163.com. |
| `com.feilong.tools.emailaddress.EmailProvider` | `String getName()` | 邮箱名, 如果邮箱是 feilong@163.com, 那么值是 网易163邮箱 |
| `com.feilong.tools.emailaddress.EmailProvider` | `String getWebSite()` | 网址, 如果邮箱是 feilong@163.com, 那么值是 http://mail.163.com/ |
| `com.feilong.tools.emailaddress.EmailProvider` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.tools.emailaddress.EmailProvider` | `void setDomain(String domain)` | 邮箱domain部分, 如果邮箱是 feilong@163.com, 那么值是 163.com. |
| `com.feilong.tools.emailaddress.EmailProvider` | `void setName(String name)` | 邮箱名, 如果邮箱是 feilong@163.com, 那么值是 网易163邮箱 |
| `com.feilong.tools.emailaddress.EmailProvider` | `void setWebSite(String webSite)` | 网址, 如果邮箱是 feilong@163.com, 那么值是 http://mail.163.com/ |
