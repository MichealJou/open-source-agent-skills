# com.feilong.net.mail.util

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.mail.util.FolderUtil` | `Map<String, Object> getMapForLog(Folder folder)` | 获得 map for log. |
| `com.feilong.net.mail.util.InternetAddressUtil` | `Address buildFromAddress(String personal,String fromAddress)` | 【原文待译】To from address. |
| `com.feilong.net.mail.util.InternetAddressUtil` | `Address[] toAddressArray(String[] addresseArray)` | 【原文待译】To address array. |
| `com.feilong.net.mail.util.InternetAddressUtil` | `InternetAddress[] toInternetAddressArray(Map<String, String> nameAndEmailMap,String charset)` | 将nameAndEmail map转成 InternetAddress数组. |
| `com.feilong.net.mail.util.InternetAddressUtil` | `List<String> toUnicodeStringList(InternetAddress[] internetAddresses)` | 将 internetAddresses 数组 转成 toUnicodeString方法 list. |
| `com.feilong.net.mail.util.MessageSendUtil` | `void send(Message message)` | 发送. |
| `com.feilong.net.mail.util.MessageUtil` | `List<MailInfo> toMailInfoList(Message[] messages)` | 【原文待译】To mail info list. |
| `com.feilong.net.mail.util.MessageUtil` | `Map<String, Object> getMapForLog(Message message)` | 获得 map for log. |
