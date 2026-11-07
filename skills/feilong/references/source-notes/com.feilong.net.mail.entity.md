# com.feilong.net.mail.entity

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.mail.entity.BaseConfig` | `String getPassword()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.mail.entity.BaseConfig` | `String getServerHost()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.mail.entity.BaseConfig` | `String getServerPort()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.mail.entity.BaseConfig` | `String getUserName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.mail.entity.BaseConfig` | `boolean getIsDebug()` | 获得 是否debug 输出. |
| `com.feilong.net.mail.entity.BaseConfig` | `boolean getIsValidate()` | 获得 是否需要身份验证,默认 true. |
| `com.feilong.net.mail.entity.BaseConfig` | `void setIsDebug(boolean isDebug)` | 设置 是否debug 输出. |
| `com.feilong.net.mail.entity.BaseConfig` | `void setIsValidate(boolean isValidate)` | 设置 是否需要身份验证,默认 true. |
| `com.feilong.net.mail.entity.BaseConfig` | `void setPassword(String password)` | 设置 登录邮件发送服务器的密码. |
| `com.feilong.net.mail.entity.BaseConfig` | `void setServerHost(String serverHost)` | 设置 发送邮件的服务器的IP. |
| `com.feilong.net.mail.entity.BaseConfig` | `void setServerPort(String serverPort)` | 设置 邮件服务的端口 默认25. |
| `com.feilong.net.mail.entity.BaseConfig` | `void setUserName(String userName)` | 设置 登录邮件发送服务器的用户名. |
| `com.feilong.net.mail.entity.ICalendar` | `Date getBeginDate()` | 【原文待译】@return the beginDate |
| `com.feilong.net.mail.entity.ICalendar` | `Date getEndDate()` | 【原文待译】@return the endDate |
| `com.feilong.net.mail.entity.ICalendar` | `String getDescription()` | 【原文待译】@return the description |
| `com.feilong.net.mail.entity.ICalendar` | `String getLocation()` | 【原文待译】@return the location |
| `com.feilong.net.mail.entity.ICalendar` | `String getSummary()` | 【原文待译】@return the summary |
| `com.feilong.net.mail.entity.ICalendar` | `void setBeginDate(Date beginDate)` | 【原文待译】@param beginDate the beginDate to set |
| `com.feilong.net.mail.entity.ICalendar` | `void setDescription(String description)` | 【原文待译】@param description the description to set |
| `com.feilong.net.mail.entity.ICalendar` | `void setEndDate(Date endDate)` | 【原文待译】@param endDate the endDate to set |
| `com.feilong.net.mail.entity.ICalendar` | `void setLocation(String location)` | 【原文待译】@param location the location to set |
| `com.feilong.net.mail.entity.ICalendar` | `void setSummary(String summary)` | 【原文待译】@param summary the summary to set |
| `com.feilong.net.mail.entity.MailInfo` | `Date getReceivedDate()` | 获得 接收时间. |
| `com.feilong.net.mail.entity.MailInfo` | `Date getSentDate()` | 获得 发送时间. |
| `com.feilong.net.mail.entity.MailInfo` | `String getContent()` | 获得 内容. |
| `com.feilong.net.mail.entity.MailInfo` | `String getContentType()` | 获得 content type. |
| `com.feilong.net.mail.entity.MailInfo` | `String getFrom()` | 获得 发件人. |
| `com.feilong.net.mail.entity.MailInfo` | `String getSize()` | 获得 大小. |
| `com.feilong.net.mail.entity.MailInfo` | `String getSubject()` | 获得 标题. |
| `com.feilong.net.mail.entity.MailInfo` | `String[] getRecipients()` | 获得 收件人. |
| `com.feilong.net.mail.entity.MailInfo` | `void setContent(String content)` | 设置 内容. |
| `com.feilong.net.mail.entity.MailInfo` | `void setContentType(String contentType)` | 设置 content type. |
| `com.feilong.net.mail.entity.MailInfo` | `void setFrom(String from)` | 设置 发件人. |
| `com.feilong.net.mail.entity.MailInfo` | `void setReceivedDate(Date receivedDate)` | 设置 接收时间. |
| `com.feilong.net.mail.entity.MailInfo` | `void setRecipients(String[] recipients)` | 设置 收件人. |
| `com.feilong.net.mail.entity.MailInfo` | `void setSentDate(Date sentDate)` | 设置 发送时间. |
| `com.feilong.net.mail.entity.MailInfo` | `void setSize(String size)` | 设置 大小. |
| `com.feilong.net.mail.entity.MailInfo` | `void setSubject(String subject)` | 设置 标题. |
| `com.feilong.net.mail.entity.MailSendConnectionConfig` | `boolean getIsSmtpSSLEnable()` | mail.smtp.ssl.enable SSL 开关. If set to true, use SSL to connect and use the SSL port by default. Defaults to false for the "smtp" protocol and true for the "smtps" protocol. |
| `com.feilong.net.mail.entity.MailSendConnectionConfig` | `boolean getIsSmtpStarttlsEnable()` | 【原文待译】The is tls enable. If true, enables the use of the STARTTLS command (if supported by the server) to switch the connection to a TLS-protected connection before issuing any login commands. Note that an appropriate trust store must configured so that the client will trust the server's certificate. Defa… |
| `com.feilong.net.mail.entity.MailSendConnectionConfig` | `void setIsSmtpSSLEnable(boolean isSmtpSSLEnable)` | mail.smtp.ssl.enable SSL 开关. If set to true, use SSL to connect and use the SSL port by default. Defaults to false for the "smtp" protocol and true for the "smtps" protocol. |
| `com.feilong.net.mail.entity.MailSendConnectionConfig` | `void setIsSmtpStarttlsEnable(boolean isSmtpStarttlsEnable)` | 【原文待译】The is tls enable. If true, enables the use of the STARTTLS command (if supported by the server) to switch the connection to a TLS-protected connection before issuing any login commands. Note that an appropriate trust store must configured so that the client will trust the server's certificate. Defa… |
| `com.feilong.net.mail.entity.MailSendRequest` | `ICalendar getiCalendar()` | 【原文待译】Gets the i calendar. |
| `com.feilong.net.mail.entity.MailSendRequest` | `Priority getPriority()` | 获得 优先级. |
| `com.feilong.net.mail.entity.MailSendRequest` | `String getContent()` | 获得 邮件的文本内容. |
| `com.feilong.net.mail.entity.MailSendRequest` | `String getContentMimeType()` | 获得 mIME type of this object. |
| `com.feilong.net.mail.entity.MailSendRequest` | `String getFromAddress()` | 获得 邮件发送者的地址. example:huanyuansp@126.com |
| `com.feilong.net.mail.entity.MailSendRequest` | `String getPersonal()` | 获得 个人名义. |
| `com.feilong.net.mail.entity.MailSendRequest` | `String getSubject()` | 获得 邮件主题. |
| `com.feilong.net.mail.entity.MailSendRequest` | `String[] getAttachFileLocations()` | 获得 邮件附件的文件全路径, 比如 E:\Workspaces\train\20150417Spring事务\ppt-contents. |
| `com.feilong.net.mail.entity.MailSendRequest` | `String[] getBccs()` | 获得 邮件多人接收地址. |
| `com.feilong.net.mail.entity.MailSendRequest` | `String[] getCcs()` | 获得 邮件多人接收地址(抄送). |
| `com.feilong.net.mail.entity.MailSendRequest` | `String[] getTos()` | 获得 邮件多人接收地址. |
| `com.feilong.net.mail.entity.MailSendRequest` | `boolean getIsDefaultCcSelf()` | 是否默认抄送给自己. 有时候163邮件发送会提示 554 DT:SPM smtp12 原来这时因为网易将发的邮件当成了垃圾邮件！这时候你只要在发邮件的时候抄送上自己，就再也不会报这个错误了！ |
| `com.feilong.net.mail.entity.MailSendRequest` | `boolean getIsNeedReturnReceipt()` | 获得 是否需要回执, 默认不需要. |
| `com.feilong.net.mail.entity.MailSendRequest` | `void setAttachFileLocations(String... attachFileLocations)` | 设置 邮件附件的文件全路径, 比如 E:\Workspaces\train\20150417Spring事务\ppt-contents. |
| `com.feilong.net.mail.entity.MailSendRequest` | `void setBccs(String... bccs)` | 设置 邮件多人接收地址. |
| `com.feilong.net.mail.entity.MailSendRequest` | `void setCcs(String... ccs)` | 设置 邮件多人接收地址(抄送). |
| `com.feilong.net.mail.entity.MailSendRequest` | `void setContent(String content)` | 设置 邮件的文本内容. |
| `com.feilong.net.mail.entity.MailSendRequest` | `void setContentMimeType(String contentMimeType)` | 设置 mIME type of this object. |
| `com.feilong.net.mail.entity.MailSendRequest` | `void setFromAddress(String fromAddress)` | 设置 邮件发送者的地址. example:huanyuansp@126.com |
| `com.feilong.net.mail.entity.MailSendRequest` | `void setIsDefaultCcSelf(boolean isDefaultCcSelf)` | 是否默认抄送给自己. 有时候163邮件发送会提示 554 DT:SPM smtp12 原来这时因为网易将发的邮件当成了垃圾邮件！这时候你只要在发邮件的时候抄送上自己，就再也不会报这个错误了！ |
| `com.feilong.net.mail.entity.MailSendRequest` | `void setIsNeedReturnReceipt(boolean isNeedReturnReceipt)` | 设置 是否需要回执, 默认不需要. |
| `com.feilong.net.mail.entity.MailSendRequest` | `void setPersonal(String personal)` | 设置 个人名义. |
| `com.feilong.net.mail.entity.MailSendRequest` | `void setPriority(Priority priority)` | 设置 优先级. |
| `com.feilong.net.mail.entity.MailSendRequest` | `void setSubject(String subject)` | 设置 邮件主题. |
| `com.feilong.net.mail.entity.MailSendRequest` | `void setTos(String... tos)` | 设置 邮件多人接收地址. |
| `com.feilong.net.mail.entity.MailSendRequest` | `void setiCalendar(ICalendar iCalendar)` | 【原文待译】Sets the i calendar. |
| `com.feilong.net.mail.entity.Priority` | `String getLevelValue()` | Gets the 级别. |
| `com.feilong.net.mail.entity.SessionConfig` | `String getPassword()` | 获得 登录邮件发送服务器的密码. |
| `com.feilong.net.mail.entity.SessionConfig` | `String getServerHost()` | 获得 发送邮件的服务器的IP. |
| `com.feilong.net.mail.entity.SessionConfig` | `String getServerPort()` | 获得 邮件服务的端口 默认25. |
| `com.feilong.net.mail.entity.SessionConfig` | `String getUserName()` | 获得 登录邮件发送服务器的用户名. |
| `com.feilong.net.mail.entity.SessionConfig` | `boolean getIsDebug()` | 获得 是否debug 输出. |
| `com.feilong.net.mail.entity.SessionConfig` | `boolean getIsValidate()` | 获得 是否需要身份验证,默认 true. |
