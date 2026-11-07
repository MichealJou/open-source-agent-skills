# com.feilong.net.mail

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.net.mail.DefaultMailSender`

```java
public final class com.feilong.net.mail.DefaultMailSender implements com.feilong.net.mail.MailSender {
  public com.feilong.net.mail.DefaultMailSender();
  public com.feilong.net.mail.DefaultMailSender(com.feilong.net.mail.entity.MailSendConnectionConfig);
  public void send(com.feilong.net.mail.entity.MailSendRequest);
  public void setMailSendConnectionConfig(com.feilong.net.mail.entity.MailSendConnectionConfig);
}
```

## `com.feilong.net.mail.FeiLongMailVersion`

```java
public final class com.feilong.net.mail.FeiLongMailVersion {
  public static java.lang.String getVersion();
}
```

## `com.feilong.net.mail.IMAPMailReader`

```java
public class com.feilong.net.mail.IMAPMailReader implements com.feilong.net.mail.MailReader {
  public com.feilong.net.mail.IMAPMailReader();
  public java.util.List<com.feilong.net.mail.entity.MailInfo> read(com.feilong.net.mail.entity.MailReaderConfig);
  public java.util.List<com.feilong.net.mail.entity.MailInfo> read(com.feilong.net.mail.entity.MailReaderConfig, java.lang.Integer, javax.mail.search.SearchTerm);
}
```

## `com.feilong.net.mail.MailReader`

```java
public interface com.feilong.net.mail.MailReader {
  public abstract java.util.List<com.feilong.net.mail.entity.MailInfo> read(com.feilong.net.mail.entity.MailReaderConfig);
  public abstract java.util.List<com.feilong.net.mail.entity.MailInfo> read(com.feilong.net.mail.entity.MailReaderConfig, java.lang.Integer, javax.mail.search.SearchTerm);
}
```

## `com.feilong.net.mail.MailSender`

```java
public interface com.feilong.net.mail.MailSender {
  public abstract void send(com.feilong.net.mail.entity.MailSendRequest);
}
```

## `com.feilong.net.mail.SessionFactory`

```java
public class com.feilong.net.mail.SessionFactory {
  public static javax.mail.Session createSession(com.feilong.net.mail.entity.SessionConfig);
}
```
