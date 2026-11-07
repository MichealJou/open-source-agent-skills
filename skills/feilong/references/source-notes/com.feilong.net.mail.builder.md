# com.feilong.net.mail.builder

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.mail.builder.AuthenticatorBuilder` | `Authenticator build(final SessionConfig sessionConfig)` | 判断是否需要身份认证,如果需要身份认证,则创建一个密码验证器. |
| `com.feilong.net.mail.builder.MessageBuilder` | `Message build(MailSendRequest mailSendRequest,MailSendConnectionConfig mailSendConnectionConfig)` | 构造Message. 基于 mailSenderConfig 构建 通用的 MimeMessage,然后设置message公共属性(含发件人 收件人等信息) |
| `com.feilong.net.mail.builder.SessionPropertiesBuilder` | `Properties build(SessionConfig sessionConfig)` | 【原文待译】Properties object. Used only if a new Session object is created. It is expected that the client supplies values for the properties listed in Appendix A of the JavaMail spec (particularly mail.store.protocol, mail.transport.protocol, mail.host, mail.user, and mail.from) as the defaults are unlikely t… |
