# com.feilong.net.mail

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.mail.DefaultMailSender` | `void send(MailSendRequest mailSendRequest)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.mail.DefaultMailSender` | `void setMailSendConnectionConfig(MailSendConnectionConfig mailSendConnectionConfig)` | 【原文待译】@param mailSendConnectionConfig the mailSendConnectionConfig to set |
| `com.feilong.net.mail.FeiLongMailVersion` | `String getVersion()` | 返回当前feilong代码的 version. |
| `com.feilong.net.mail.IMAPMailReader` | `List<MailInfo> read(MailReaderConfig mailReaderConfig)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.mail.IMAPMailReader` | `List<MailInfo> read(MailReaderConfig mailReaderConfig,Integer newstIndex,SearchTerm searchTerm)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.mail.MailReader` | `List<MailInfo> read(MailReaderConfig mailReaderConfig)` | 获得所有的邮件列表(不带筛选条件). |
| `com.feilong.net.mail.MailReader` | `List<MailInfo> read(MailReaderConfig mailReaderConfig,Integer newstIndex,SearchTerm searchTerm)` | 获得所有的邮件列表. 你可以通过 newstIndex来指定 最新的多少条,以及通过 searchTerm来设置筛选条件 |
| `com.feilong.net.mail.MailSender` | `void send(MailSendRequest mailSendRequest)` | 发送邮件. |
| `com.feilong.net.mail.SessionFactory` | `Session createSession(SessionConfig sessionConfig)` | 根据邮件会话属性和密码验证器构造邮件的javax.mail.Session. |
