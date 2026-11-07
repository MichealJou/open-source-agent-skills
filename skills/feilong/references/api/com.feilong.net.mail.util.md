# com.feilong.net.mail.util

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.net.mail.util.FolderUtil`

```java
public final class com.feilong.net.mail.util.FolderUtil {
  public static final java.util.Map<java.lang.String, java.lang.Object> getMapForLog(javax.mail.Folder) throws javax.mail.MessagingException;
}
```

## `com.feilong.net.mail.util.InternetAddressUtil`

```java
public final class com.feilong.net.mail.util.InternetAddressUtil {
  public static javax.mail.Address[] toAddressArray(java.lang.String[]) throws javax.mail.internet.AddressException;
  public static final javax.mail.internet.InternetAddress[] toInternetAddressArray(java.util.Map<java.lang.String, java.lang.String>, java.lang.String) throws java.io.UnsupportedEncodingException;
  public static final java.util.List<java.lang.String> toUnicodeStringList(javax.mail.internet.InternetAddress[]);
  public static javax.mail.Address buildFromAddress(java.lang.String, java.lang.String);
}
```

## `com.feilong.net.mail.util.MessageSendUtil`

```java
public class com.feilong.net.mail.util.MessageSendUtil {
  public static void send(javax.mail.Message);
}
```

## `com.feilong.net.mail.util.MessageUtil`

```java
public final class com.feilong.net.mail.util.MessageUtil {
  public static final java.util.List<com.feilong.net.mail.entity.MailInfo> toMailInfoList(javax.mail.Message[]) throws javax.mail.MessagingException;
  public static final java.util.Map<java.lang.String, java.lang.Object> getMapForLog(javax.mail.Message);
}
```
