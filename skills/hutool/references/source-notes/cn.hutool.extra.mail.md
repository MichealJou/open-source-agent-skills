# cn.hutool.extra.mail

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.mail.GlobalMailAccount` | `MailAccount getAccount()` | 获得邮件帐户 |
| `cn.hutool.extra.mail.InternalMailUtil` | `InternetAddress parseFirstAddress(String address,Charset charset)` | 解析第一个地址 |
| `cn.hutool.extra.mail.InternalMailUtil` | `InternetAddress[] parseAddress(String address,Charset charset)` | 将一个地址字符串解析为多个地址 地址间使用" "、","、";"分隔 |
| `cn.hutool.extra.mail.InternalMailUtil` | `InternetAddress[] parseAddressFromStrs(String[] addrStrs,Charset charset)` | 将多个字符串邮件地址转为InternetAddress列表 单个字符串地址可以是多个地址合并的字符串 |
| `cn.hutool.extra.mail.InternalMailUtil` | `String encodeText(String text,Charset charset)` | 编码中文字符 编码失败返回原字符串 |
| `cn.hutool.extra.mail.JakartaInternalMailUtil` | `InternetAddress parseFirstAddress(String address,Charset charset)` | 解析第一个地址 |
| `cn.hutool.extra.mail.JakartaInternalMailUtil` | `InternetAddress[] parseAddress(String address,Charset charset)` | 将一个地址字符串解析为多个地址 地址间使用" "、","、";"分隔 |
| `cn.hutool.extra.mail.JakartaInternalMailUtil` | `InternetAddress[] parseAddressFromStrs(String[] addrStrs,Charset charset)` | 将多个字符串邮件地址转为InternetAddress列表 单个字符串地址可以是多个地址合并的字符串 |
| `cn.hutool.extra.mail.JakartaInternalMailUtil` | `String encodeText(String text,Charset charset)` | 编码中文字符 编码失败返回原字符串 |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail addImage(String cid,File imageFile)` | 增加图片，图片的键对应到邮件模板中的占位字符串 |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail addImage(String cid,InputStream imageStream)` | 增加图片，图片的键对应到邮件模板中的占位字符串，图片类型默认为"image/jpeg" |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail addImage(String cid,InputStream imageStream,String contentType)` | 增加图片，图片的键对应到邮件模板中的占位字符串 |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail create()` | 创建邮件客户端，使用全局邮件帐户 |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail create(MailAccount mailAccount)` | 创建邮件客户端 |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail setAttachments(DataSource... attachments)` | 增加附件或图片，附件使用DataSource 形式表示，可以使用FileDataSource包装文件表示文件附件 |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail setBccs(String... bccs)` | 设置多个密送人（blind carbon copy） |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail setCcs(String... ccs)` | 设置多个抄送人（carbon copy） |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail setCharset(Charset charset)` | 设置字符集编码 |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail setContent(String content)` | 设置正文 正文可以是普通文本也可以是HTML（默认普通文本），可以通过调用#setHtml(boolean) 设置是否为HTML |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail setContent(String content,boolean isHtml)` | 设置正文 |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail setDebugOutput(PrintStream debugOutput)` | 设置debug输出位置，可以自定义debug日志 |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail setFiles(File... files)` | 设置文件类型附件，文件可以是图片文件，此时自动设置cid（正文中引用图片），默认cid为文件名 |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail setHtml(boolean isHtml)` | 设置是否是HTML |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail setReply(String... reply)` | 设置多个回复地址(reply-to) |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail setTitle(String title)` | 设置标题 |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail setTos(String... tos)` | 设置多个收件人 |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail setUseGlobalSession(boolean isUseGlobalSession)` | 设置是否使用全局会话，默认为true |
| `cn.hutool.extra.mail.JakartaMail` | `JakartaMail to(String... tos)` | 设置收件人 |
| `cn.hutool.extra.mail.JakartaMail` | `MimeMessage build()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.mail.JakartaMail` | `String send()` | 发送 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `Session getSession(MailAccount mailAccount,boolean isSingleton)` | 根据配置文件，获取邮件客户端会话 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String send(Collection<String> tos,Collection<String> ccs,Collection<String> bccs,String subject,String content,Map<String, InputStream> imageMap,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送给多人 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String send(Collection<String> tos,Collection<String> ccs,Collection<String> bccs,String subject,String content,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送给多人 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String send(Collection<String> tos,String subject,String content,Map<String, InputStream> imageMap,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送给多人 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String send(Collection<String> tos,String subject,String content,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送给多人 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String send(MailAccount mailAccount,Collection<String> tos,Collection<String> ccs,Collection<String> bccs,String subject,String content,Map<String, InputStream> imageMap,boolean isHtml,File... files)` | 发送邮件给多人 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String send(MailAccount mailAccount,Collection<String> tos,Collection<String> ccs,Collection<String> bccs,String subject,String content,boolean isHtml,File... files)` | 发送邮件给多人 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String send(MailAccount mailAccount,Collection<String> tos,String subject,String content,Map<String, InputStream> imageMap,boolean isHtml,File... files)` | 发送邮件给多人 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String send(MailAccount mailAccount,Collection<String> tos,String subject,String content,boolean isHtml,File... files)` | 发送邮件给多人 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String send(MailAccount mailAccount,String to,String subject,String content,Map<String, InputStream> imageMap,boolean isHtml,File... files)` | 发送邮件给多人 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String send(MailAccount mailAccount,String to,String subject,String content,boolean isHtml,File... files)` | 发送邮件给多人 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String send(String to,String cc,String bcc,String subject,String content,Map<String, InputStream> imageMap,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送单个或多个收件人 多个收件人、抄送人、密送人可以使用逗号“,”分隔，也可以通过分号“;”分隔 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String send(String to,String cc,String bcc,String subject,String content,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送单个或多个收件人 多个收件人、抄送人、密送人可以使用逗号“,”分隔，也可以通过分号“;”分隔 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String send(String to,String subject,String content,Map<String, InputStream> imageMap,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送单个或多个收件人 多个收件人可以使用逗号“,”分隔，也可以通过分号“;”分隔 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String send(String to,String subject,String content,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送单个或多个收件人 多个收件人可以使用逗号“,”分隔，也可以通过分号“;”分隔 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String sendHtml(Collection<String> tos,String subject,String content,File... files)` | 使用配置文件中设置的账户发送HTML邮件，发送给多人 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String sendHtml(Collection<String> tos,String subject,String content,Map<String, InputStream> imageMap,File... files)` | 使用配置文件中设置的账户发送HTML邮件，发送给多人 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String sendHtml(String to,String subject,String content,File... files)` | 使用配置文件中设置的账户发送HTML邮件，发送给单个或多个收件人 多个收件人可以使用逗号“,”分隔，也可以通过分号“;”分隔 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String sendHtml(String to,String subject,String content,Map<String, InputStream> imageMap,File... files)` | 使用配置文件中设置的账户发送HTML邮件，发送给单个或多个收件人 多个收件人可以使用逗号“,”分隔，也可以通过分号“;”分隔 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String sendText(Collection<String> tos,String subject,String content,File... files)` | 使用配置文件中设置的账户发送文本邮件，发送给多人 |
| `cn.hutool.extra.mail.JakartaMailUtil` | `String sendText(String to,String subject,String content,File... files)` | 使用配置文件中设置的账户发送文本邮件，发送给单个或多个收件人 多个收件人可以使用逗号“,”分隔，也可以通过分号“;”分隔 |
| `cn.hutool.extra.mail.Mail` | `Mail addImage(String cid,File imageFile)` | 增加图片，图片的键对应到邮件模板中的占位字符串 |
| `cn.hutool.extra.mail.Mail` | `Mail addImage(String cid,InputStream imageStream)` | 增加图片，图片的键对应到邮件模板中的占位字符串，图片类型默认为"image/jpeg" |
| `cn.hutool.extra.mail.Mail` | `Mail addImage(String cid,InputStream imageStream,String contentType)` | 增加图片，图片的键对应到邮件模板中的占位字符串 |
| `cn.hutool.extra.mail.Mail` | `Mail create()` | 创建邮件客户端，使用全局邮件帐户 |
| `cn.hutool.extra.mail.Mail` | `Mail create(MailAccount mailAccount)` | 创建邮件客户端 |
| `cn.hutool.extra.mail.Mail` | `Mail setAttachments(DataSource... attachments)` | 增加附件或图片，附件使用DataSource 形式表示，可以使用FileDataSource包装文件表示文件附件 |
| `cn.hutool.extra.mail.Mail` | `Mail setBccs(String... bccs)` | 设置多个密送人（blind carbon copy） |
| `cn.hutool.extra.mail.Mail` | `Mail setCcs(String... ccs)` | 设置多个抄送人（carbon copy） |
| `cn.hutool.extra.mail.Mail` | `Mail setCharset(Charset charset)` | 设置字符集编码 |
| `cn.hutool.extra.mail.Mail` | `Mail setContent(String content)` | 设置正文 正文可以是普通文本也可以是HTML（默认普通文本），可以通过调用#setHtml(boolean) 设置是否为HTML |
| `cn.hutool.extra.mail.Mail` | `Mail setContent(String content,boolean isHtml)` | 设置正文 |
| `cn.hutool.extra.mail.Mail` | `Mail setDebugOutput(PrintStream debugOutput)` | 设置debug输出位置，可以自定义debug日志 |
| `cn.hutool.extra.mail.Mail` | `Mail setFiles(File... files)` | 设置文件类型附件，文件可以是图片文件，此时自动设置cid（正文中引用图片），默认cid为文件名 |
| `cn.hutool.extra.mail.Mail` | `Mail setHtml(boolean isHtml)` | 设置是否是HTML |
| `cn.hutool.extra.mail.Mail` | `Mail setReply(String... reply)` | 设置多个回复地址(reply-to) |
| `cn.hutool.extra.mail.Mail` | `Mail setTitle(String title)` | 设置标题 |
| `cn.hutool.extra.mail.Mail` | `Mail setTos(String... tos)` | 设置多个收件人 |
| `cn.hutool.extra.mail.Mail` | `Mail setUseGlobalSession(boolean isUseGlobalSession)` | 设置是否使用全局会话，默认为true |
| `cn.hutool.extra.mail.Mail` | `Mail to(String... tos)` | 设置收件人 |
| `cn.hutool.extra.mail.Mail` | `MimeMessage build()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.mail.Mail` | `String send()` | 发送 |
| `cn.hutool.extra.mail.MailAccount` | `Boolean isAuth()` | 是否需要用户名密码验证 |
| `cn.hutool.extra.mail.MailAccount` | `Boolean isSslEnable()` | 是否使用 SSL安全连接 |
| `cn.hutool.extra.mail.MailAccount` | `Charset getCharset()` | 获取字符集编码 |
| `cn.hutool.extra.mail.MailAccount` | `Integer getPort()` | 获得SMTP服务端口 |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount defaultIfEmpty()` | 如果某些值为null，使用默认值 |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setAuth(Boolean isAuth)` | 设置是否需要用户名密码验证 |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setCharset(Charset charset)` | 设置字符集编码，此选项不会修改全局配置，若修改全局配置，请设置此项为null并设置： |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setConnectionTimeout(long connectionTimeout)` | 设置Socket连接超时值，单位毫秒，缺省值不超时 |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setCustomProperty(String key,Object value)` | 设置自定义属性，如mail.smtp.ssl.socketFactory |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setDebug(boolean debug)` | 设置是否打开调试模式，调试模式会显示与邮件服务器通信过程，默认不开启 |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setFrom(String from)` | 设置发送方，遵循RFC-822标准 发件人可以是以下形式： |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setHost(String host)` | 设置SMTP服务器域名 |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setPass(String pass)` | 设置密码 |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setPort(Integer port)` | 设置SMTP服务端口 |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setSocketFactoryClass(String socketFactoryClass)` | 设置指定实现javax.net.SocketFactory接口的类的名称,这个类将被用于创建SMTP的套接字 |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setSocketFactoryFallback(boolean socketFactoryFallback)` | 如果设置为true,未能创建一个套接字使用指定的套接字工厂类将导致使用java.net.Socket创建的套接字类, 默认值为true |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setSocketFactoryPort(int socketFactoryPort)` | 指定的端口连接到在使用指定的套接字工厂。如果没有设置,将使用默认端口 |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setSslEnable(Boolean sslEnable)` | 设置是否使用SSL安全连接 |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setStarttlsEnable(boolean startttlsEnable)` | 设置是否使用STARTTLS安全连接，STARTTLS是对纯文本通信协议的扩展。它将纯文本连接升级为加密连接（TLS或SSL）， 而不是使用一个单独的加密通信端口。 |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setTimeout(long timeout)` | 设置SMTP超时时长，单位毫秒，缺省值不超时 |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setUser(String user)` | 设置用户名 |
| `cn.hutool.extra.mail.MailAccount` | `MailAccount setWriteTimeout(long writeTimeout)` | 设置Socket写出超时值，单位毫秒，缺省值不超时 |
| `cn.hutool.extra.mail.MailAccount` | `Map<String, Object> getCustomProperty()` | 获取自定义属性列表 |
| `cn.hutool.extra.mail.MailAccount` | `Properties getSmtpProps()` | 获得SMTP相关信息 |
| `cn.hutool.extra.mail.MailAccount` | `String getFrom()` | 获取发送方，遵循RFC-822标准 |
| `cn.hutool.extra.mail.MailAccount` | `String getHost()` | 获得SMTP服务器域名 |
| `cn.hutool.extra.mail.MailAccount` | `String getPass()` | 获取密码 |
| `cn.hutool.extra.mail.MailAccount` | `String getSocketFactoryClass()` | 获取指定实现javax.net.SocketFactory接口的类的名称,这个类将被用于创建SMTP的套接字 |
| `cn.hutool.extra.mail.MailAccount` | `String getSslProtocols()` | 获取SSL协议，多个协议用空格分隔 |
| `cn.hutool.extra.mail.MailAccount` | `String getUser()` | 获取用户名 |
| `cn.hutool.extra.mail.MailAccount` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.mail.MailAccount` | `boolean isDebug()` | 是否打开调试模式，调试模式会显示与邮件服务器通信过程，默认不开启 |
| `cn.hutool.extra.mail.MailAccount` | `boolean isEncodefilename()` | 对于文件名是否使用#charset编码，默认为 true |
| `cn.hutool.extra.mail.MailAccount` | `boolean isSocketFactoryFallback()` | 如果设置为true,未能创建一个套接字使用指定的套接字工厂类将导致使用java.net.Socket创建的套接字类, 默认值为true |
| `cn.hutool.extra.mail.MailAccount` | `boolean isSplitlongparameters()` | 对于超长参数是否切分为多份，默认为false（国内邮箱附件不支持切分的附件名） |
| `cn.hutool.extra.mail.MailAccount` | `boolean isStarttlsEnable()` | 是否使用 STARTTLS安全连接，STARTTLS是对纯文本通信协议的扩展。它将纯文本连接升级为加密连接（TLS或SSL）， 而不是使用一个单独的加密通信端口。 |
| `cn.hutool.extra.mail.MailAccount` | `int getSocketFactoryPort()` | 获取指定的端口连接到在使用指定的套接字工厂。如果没有设置,将使用默认端口 |
| `cn.hutool.extra.mail.MailAccount` | `void setEncodefilename(boolean encodefilename)` | 设置对于文件名是否使用#charset编码，此选项不会修改全局配置 如果此选项设置为false，则是否编码取决于两个系统属性： mail.mime.encodefilename 是否编码附件文件名 mail.mime.charset 编码文件名的编码 |
| `cn.hutool.extra.mail.MailAccount` | `void setSplitlongparameters(boolean splitlongparameters)` | 设置对于超长参数是否切分为多份，默认为false（国内邮箱附件不支持切分的附件名） 注意此项为全局设置，此项会调用 |
| `cn.hutool.extra.mail.MailAccount` | `void setSslProtocols(String sslProtocols)` | 设置SSL协议，多个协议用空格分隔 |
| `cn.hutool.extra.mail.MailUtil` | `Session getSession(MailAccount mailAccount,boolean isSingleton)` | 根据配置文件，获取邮件客户端会话 |
| `cn.hutool.extra.mail.MailUtil` | `String send(Collection<String> tos,Collection<String> ccs,Collection<String> bccs,String subject,String content,Map<String, InputStream> imageMap,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送给多人 |
| `cn.hutool.extra.mail.MailUtil` | `String send(Collection<String> tos,Collection<String> ccs,Collection<String> bccs,String subject,String content,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送给多人 |
| `cn.hutool.extra.mail.MailUtil` | `String send(Collection<String> tos,String subject,String content,Map<String, InputStream> imageMap,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送给多人 |
| `cn.hutool.extra.mail.MailUtil` | `String send(Collection<String> tos,String subject,String content,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送给多人 |
| `cn.hutool.extra.mail.MailUtil` | `String send(MailAccount mailAccount,Collection<String> tos,Collection<String> ccs,Collection<String> bccs,String subject,String content,Map<String, InputStream> imageMap,boolean isHtml,File... files)` | 发送邮件给多人 |
| `cn.hutool.extra.mail.MailUtil` | `String send(MailAccount mailAccount,Collection<String> tos,Collection<String> ccs,Collection<String> bccs,String subject,String content,boolean isHtml,File... files)` | 发送邮件给多人 |
| `cn.hutool.extra.mail.MailUtil` | `String send(MailAccount mailAccount,Collection<String> tos,String subject,String content,Map<String, InputStream> imageMap,boolean isHtml,File... files)` | 发送邮件给多人 |
| `cn.hutool.extra.mail.MailUtil` | `String send(MailAccount mailAccount,Collection<String> tos,String subject,String content,boolean isHtml,File... files)` | 发送邮件给多人 |
| `cn.hutool.extra.mail.MailUtil` | `String send(MailAccount mailAccount,String to,String subject,String content,Map<String, InputStream> imageMap,boolean isHtml,File... files)` | 发送邮件给多人 |
| `cn.hutool.extra.mail.MailUtil` | `String send(MailAccount mailAccount,String to,String subject,String content,boolean isHtml,File... files)` | 发送邮件给多人 |
| `cn.hutool.extra.mail.MailUtil` | `String send(String to,String cc,String bcc,String subject,String content,Map<String, InputStream> imageMap,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送单个或多个收件人 多个收件人、抄送人、密送人可以使用逗号“,”分隔，也可以通过分号“;”分隔 |
| `cn.hutool.extra.mail.MailUtil` | `String send(String to,String cc,String bcc,String subject,String content,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送单个或多个收件人 多个收件人、抄送人、密送人可以使用逗号“,”分隔，也可以通过分号“;”分隔 |
| `cn.hutool.extra.mail.MailUtil` | `String send(String to,String subject,String content,Map<String, InputStream> imageMap,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送单个或多个收件人 多个收件人可以使用逗号“,”分隔，也可以通过分号“;”分隔 |
| `cn.hutool.extra.mail.MailUtil` | `String send(String to,String subject,String content,boolean isHtml,File... files)` | 使用配置文件中设置的账户发送邮件，发送单个或多个收件人 多个收件人可以使用逗号“,”分隔，也可以通过分号“;”分隔 |
| `cn.hutool.extra.mail.MailUtil` | `String sendHtml(Collection<String> tos,String subject,String content,File... files)` | 使用配置文件中设置的账户发送HTML邮件，发送给多人 |
| `cn.hutool.extra.mail.MailUtil` | `String sendHtml(Collection<String> tos,String subject,String content,Map<String, InputStream> imageMap,File... files)` | 使用配置文件中设置的账户发送HTML邮件，发送给多人 |
| `cn.hutool.extra.mail.MailUtil` | `String sendHtml(String to,String subject,String content,File... files)` | 使用配置文件中设置的账户发送HTML邮件，发送给单个或多个收件人 多个收件人可以使用逗号“,”分隔，也可以通过分号“;”分隔 |
| `cn.hutool.extra.mail.MailUtil` | `String sendHtml(String to,String subject,String content,Map<String, InputStream> imageMap,File... files)` | 使用配置文件中设置的账户发送HTML邮件，发送给单个或多个收件人 多个收件人可以使用逗号“,”分隔，也可以通过分号“;”分隔 |
| `cn.hutool.extra.mail.MailUtil` | `String sendText(Collection<String> tos,String subject,String content,File... files)` | 使用配置文件中设置的账户发送文本邮件，发送给多人 |
| `cn.hutool.extra.mail.MailUtil` | `String sendText(String to,String subject,String content,File... files)` | 使用配置文件中设置的账户发送文本邮件，发送给单个或多个收件人 多个收件人可以使用逗号“,”分隔，也可以通过分号“;”分隔 |
