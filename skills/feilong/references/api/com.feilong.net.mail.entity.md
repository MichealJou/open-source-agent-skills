# com.feilong.net.mail.entity

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.net.mail.entity.BaseConfig`

```java
public abstract class com.feilong.net.mail.entity.BaseConfig implements com.feilong.net.mail.entity.SessionConfig {
  public com.feilong.net.mail.entity.BaseConfig();
  public java.lang.String getUserName();
  public void setUserName(java.lang.String);
  public java.lang.String getPassword();
  public void setPassword(java.lang.String);
  public java.lang.String getServerHost();
  public void setServerHost(java.lang.String);
  public java.lang.String getServerPort();
  public void setServerPort(java.lang.String);
  public boolean getIsDebug();
  public void setIsDebug(boolean);
  public boolean getIsValidate();
  public void setIsValidate(boolean);
}
```

## `com.feilong.net.mail.entity.ICalendar`

```java
public class com.feilong.net.mail.entity.ICalendar {
  public com.feilong.net.mail.entity.ICalendar();
  public java.util.Date getBeginDate();
  public void setBeginDate(java.util.Date);
  public java.util.Date getEndDate();
  public void setEndDate(java.util.Date);
  public java.lang.String getDescription();
  public void setDescription(java.lang.String);
  public java.lang.String getLocation();
  public void setLocation(java.lang.String);
  public java.lang.String getSummary();
  public void setSummary(java.lang.String);
}
```

## `com.feilong.net.mail.entity.MailInfo`

```java
public class com.feilong.net.mail.entity.MailInfo {
  public com.feilong.net.mail.entity.MailInfo();
  public java.lang.String getFrom();
  public void setFrom(java.lang.String);
  public java.util.Date getSentDate();
  public void setSentDate(java.util.Date);
  public java.lang.String getSize();
  public void setSize(java.lang.String);
  public java.lang.String getSubject();
  public void setSubject(java.lang.String);
  public java.lang.String[] getRecipients();
  public void setRecipients(java.lang.String[]);
  public java.lang.String getContentType();
  public void setContentType(java.lang.String);
  public java.lang.String getContent();
  public void setContent(java.lang.String);
  public java.util.Date getReceivedDate();
  public void setReceivedDate(java.util.Date);
}
```

## `com.feilong.net.mail.entity.MailReaderConfig`

```java
public class com.feilong.net.mail.entity.MailReaderConfig extends com.feilong.net.mail.entity.BaseConfig {
  public com.feilong.net.mail.entity.MailReaderConfig();
}
```

## `com.feilong.net.mail.entity.MailSendConnectionConfig`

```java
public class com.feilong.net.mail.entity.MailSendConnectionConfig extends com.feilong.net.mail.entity.BaseConfig {
  public com.feilong.net.mail.entity.MailSendConnectionConfig();
  public boolean getIsSmtpSSLEnable();
  public void setIsSmtpSSLEnable(boolean);
  public boolean getIsSmtpStarttlsEnable();
  public void setIsSmtpStarttlsEnable(boolean);
}
```

## `com.feilong.net.mail.entity.MailSendRequest`

```java
public class com.feilong.net.mail.entity.MailSendRequest {
  public com.feilong.net.mail.entity.MailSendRequest();
  public void setAttachFileLocations(java.lang.String...);
  public java.lang.String[] getAttachFileLocations();
  public boolean getIsNeedReturnReceipt();
  public void setIsNeedReturnReceipt(boolean);
  public java.lang.String[] getTos();
  public void setTos(java.lang.String...);
  public java.lang.String[] getCcs();
  public void setCcs(java.lang.String...);
  public java.lang.String[] getBccs();
  public void setBccs(java.lang.String...);
  public com.feilong.net.mail.entity.Priority getPriority();
  public void setPriority(com.feilong.net.mail.entity.Priority);
  public java.lang.String getSubject();
  public void setSubject(java.lang.String);
  public java.lang.String getContent();
  public void setContent(java.lang.String);
  public java.lang.String getContentMimeType();
  public void setContentMimeType(java.lang.String);
  public com.feilong.net.mail.entity.ICalendar getiCalendar();
  public void setiCalendar(com.feilong.net.mail.entity.ICalendar);
  public boolean getIsDefaultCcSelf();
  public void setIsDefaultCcSelf(boolean);
  public java.lang.String getFromAddress();
  public void setFromAddress(java.lang.String);
  public java.lang.String getPersonal();
  public void setPersonal(java.lang.String);
}
```

## `com.feilong.net.mail.entity.Priority`

```java
public final class com.feilong.net.mail.entity.Priority extends java.lang.Enum<com.feilong.net.mail.entity.Priority> {
  public static com.feilong.net.mail.entity.Priority[] values();
  public static com.feilong.net.mail.entity.Priority valueOf(java.lang.String);
  public java.lang.String getLevelValue();
}
```

## `com.feilong.net.mail.entity.SessionConfig`

```java
public interface com.feilong.net.mail.entity.SessionConfig {
  public abstract java.lang.String getUserName();
  public abstract java.lang.String getPassword();
  public abstract java.lang.String getServerHost();
  public abstract java.lang.String getServerPort();
  public abstract boolean getIsDebug();
  public abstract boolean getIsValidate();
}
```
