# cn.hutool.extra.mail

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.mail.GlobalMailAccount`

```java
public final class cn.hutool.extra.mail.GlobalMailAccount extends java.lang.Enum<cn.hutool.extra.mail.GlobalMailAccount> {
  public static cn.hutool.extra.mail.GlobalMailAccount[] values();
  public static cn.hutool.extra.mail.GlobalMailAccount valueOf(java.lang.String);
  public cn.hutool.extra.mail.MailAccount getAccount();
}
```

## `cn.hutool.extra.mail.InternalMailUtil`

```java
public class cn.hutool.extra.mail.InternalMailUtil {
  public cn.hutool.extra.mail.InternalMailUtil();
  public static javax.mail.internet.InternetAddress[] parseAddressFromStrs(java.lang.String[], java.nio.charset.Charset);
  public static javax.mail.internet.InternetAddress parseFirstAddress(java.lang.String, java.nio.charset.Charset);
  public static javax.mail.internet.InternetAddress[] parseAddress(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String encodeText(java.lang.String, java.nio.charset.Charset);
}
```

## `cn.hutool.extra.mail.JakartaInternalMailUtil`

```java
public class cn.hutool.extra.mail.JakartaInternalMailUtil {
  public cn.hutool.extra.mail.JakartaInternalMailUtil();
  public static jakarta.mail.internet.InternetAddress[] parseAddressFromStrs(java.lang.String[], java.nio.charset.Charset);
  public static jakarta.mail.internet.InternetAddress parseFirstAddress(java.lang.String, java.nio.charset.Charset);
  public static jakarta.mail.internet.InternetAddress[] parseAddress(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String encodeText(java.lang.String, java.nio.charset.Charset);
}
```

## `cn.hutool.extra.mail.JakartaMail`

```java
public class cn.hutool.extra.mail.JakartaMail implements cn.hutool.core.builder.Builder<jakarta.mail.internet.MimeMessage> {
  public static cn.hutool.extra.mail.JakartaMail create(cn.hutool.extra.mail.MailAccount);
  public static cn.hutool.extra.mail.JakartaMail create();
  public cn.hutool.extra.mail.JakartaMail();
  public cn.hutool.extra.mail.JakartaMail(cn.hutool.extra.mail.MailAccount);
  public cn.hutool.extra.mail.JakartaMail to(java.lang.String...);
  public cn.hutool.extra.mail.JakartaMail setTos(java.lang.String...);
  public cn.hutool.extra.mail.JakartaMail setCcs(java.lang.String...);
  public cn.hutool.extra.mail.JakartaMail setBccs(java.lang.String...);
  public cn.hutool.extra.mail.JakartaMail setReply(java.lang.String...);
  public cn.hutool.extra.mail.JakartaMail setTitle(java.lang.String);
  public cn.hutool.extra.mail.JakartaMail setContent(java.lang.String);
  public cn.hutool.extra.mail.JakartaMail setHtml(boolean);
  public cn.hutool.extra.mail.JakartaMail setContent(java.lang.String, boolean);
  public cn.hutool.extra.mail.JakartaMail setFiles(java.io.File...);
  public cn.hutool.extra.mail.JakartaMail setAttachments(jakarta.activation.DataSource...);
  public cn.hutool.extra.mail.JakartaMail addImage(java.lang.String, java.io.InputStream);
  public cn.hutool.extra.mail.JakartaMail addImage(java.lang.String, java.io.InputStream, java.lang.String);
  public cn.hutool.extra.mail.JakartaMail addImage(java.lang.String, java.io.File);
  public cn.hutool.extra.mail.JakartaMail setCharset(java.nio.charset.Charset);
  public cn.hutool.extra.mail.JakartaMail setUseGlobalSession(boolean);
  public cn.hutool.extra.mail.JakartaMail setDebugOutput(java.io.PrintStream);
  public jakarta.mail.internet.MimeMessage build();
  public java.lang.String send() throws cn.hutool.extra.mail.MailException;
  public java.lang.Object build();
}
```

## `cn.hutool.extra.mail.JakartaMailUtil`

```java
public class cn.hutool.extra.mail.JakartaMailUtil {
  public cn.hutool.extra.mail.JakartaMailUtil();
  public static java.lang.String sendText(java.lang.String, java.lang.String, java.lang.String, java.io.File...);
  public static java.lang.String sendHtml(java.lang.String, java.lang.String, java.lang.String, java.io.File...);
  public static java.lang.String send(java.lang.String, java.lang.String, java.lang.String, boolean, java.io.File...);
  public static java.lang.String send(java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String, boolean, java.io.File...);
  public static java.lang.String sendText(java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, java.io.File...);
  public static java.lang.String sendHtml(java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, java.io.File...);
  public static java.lang.String send(java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, boolean, java.io.File...);
  public static java.lang.String send(java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, boolean, java.io.File...);
  public static java.lang.String send(cn.hutool.extra.mail.MailAccount, java.lang.String, java.lang.String, java.lang.String, boolean, java.io.File...);
  public static java.lang.String send(cn.hutool.extra.mail.MailAccount, java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, boolean, java.io.File...);
  public static java.lang.String send(cn.hutool.extra.mail.MailAccount, java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, boolean, java.io.File...);
  public static java.lang.String sendHtml(java.lang.String, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, java.io.File...);
  public static java.lang.String send(java.lang.String, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, boolean, java.io.File...);
  public static java.lang.String send(java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, boolean, java.io.File...);
  public static java.lang.String sendHtml(java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, java.io.File...);
  public static java.lang.String send(java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, boolean, java.io.File...);
  public static java.lang.String send(java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, boolean, java.io.File...);
  public static java.lang.String send(cn.hutool.extra.mail.MailAccount, java.lang.String, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, boolean, java.io.File...);
  public static java.lang.String send(cn.hutool.extra.mail.MailAccount, java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, boolean, java.io.File...);
  public static java.lang.String send(cn.hutool.extra.mail.MailAccount, java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, boolean, java.io.File...);
  public static jakarta.mail.Session getSession(cn.hutool.extra.mail.MailAccount, boolean);
}
```

## `cn.hutool.extra.mail.JakartaUserPassAuthenticator`

```java
public class cn.hutool.extra.mail.JakartaUserPassAuthenticator extends jakarta.mail.Authenticator {
  public cn.hutool.extra.mail.JakartaUserPassAuthenticator(java.lang.String, java.lang.String);
}
```

## `cn.hutool.extra.mail.Mail`

```java
public class cn.hutool.extra.mail.Mail implements cn.hutool.core.builder.Builder<javax.mail.internet.MimeMessage> {
  public static cn.hutool.extra.mail.Mail create(cn.hutool.extra.mail.MailAccount);
  public static cn.hutool.extra.mail.Mail create();
  public cn.hutool.extra.mail.Mail();
  public cn.hutool.extra.mail.Mail(cn.hutool.extra.mail.MailAccount);
  public cn.hutool.extra.mail.Mail to(java.lang.String...);
  public cn.hutool.extra.mail.Mail setTos(java.lang.String...);
  public cn.hutool.extra.mail.Mail setCcs(java.lang.String...);
  public cn.hutool.extra.mail.Mail setBccs(java.lang.String...);
  public cn.hutool.extra.mail.Mail setReply(java.lang.String...);
  public cn.hutool.extra.mail.Mail setTitle(java.lang.String);
  public cn.hutool.extra.mail.Mail setContent(java.lang.String);
  public cn.hutool.extra.mail.Mail setHtml(boolean);
  public cn.hutool.extra.mail.Mail setContent(java.lang.String, boolean);
  public cn.hutool.extra.mail.Mail setFiles(java.io.File...);
  public cn.hutool.extra.mail.Mail setAttachments(javax.activation.DataSource...);
  public cn.hutool.extra.mail.Mail addImage(java.lang.String, java.io.InputStream);
  public cn.hutool.extra.mail.Mail addImage(java.lang.String, java.io.InputStream, java.lang.String);
  public cn.hutool.extra.mail.Mail addImage(java.lang.String, java.io.File);
  public cn.hutool.extra.mail.Mail setCharset(java.nio.charset.Charset);
  public cn.hutool.extra.mail.Mail setUseGlobalSession(boolean);
  public cn.hutool.extra.mail.Mail setDebugOutput(java.io.PrintStream);
  public javax.mail.internet.MimeMessage build();
  public java.lang.String send() throws cn.hutool.extra.mail.MailException;
  public java.lang.Object build();
}
```

## `cn.hutool.extra.mail.MailAccount`

```java
public class cn.hutool.extra.mail.MailAccount implements java.io.Serializable {
  public cn.hutool.extra.mail.MailAccount();
  public cn.hutool.extra.mail.MailAccount(java.lang.String);
  public cn.hutool.extra.mail.MailAccount(cn.hutool.setting.Setting);
  public java.lang.String getHost();
  public cn.hutool.extra.mail.MailAccount setHost(java.lang.String);
  public java.lang.Integer getPort();
  public cn.hutool.extra.mail.MailAccount setPort(java.lang.Integer);
  public java.lang.Boolean isAuth();
  public cn.hutool.extra.mail.MailAccount setAuth(java.lang.Boolean);
  public java.lang.String getUser();
  public cn.hutool.extra.mail.MailAccount setUser(java.lang.String);
  public java.lang.String getPass();
  public cn.hutool.extra.mail.MailAccount setPass(java.lang.String);
  public java.lang.String getFrom();
  public cn.hutool.extra.mail.MailAccount setFrom(java.lang.String);
  public boolean isDebug();
  public cn.hutool.extra.mail.MailAccount setDebug(boolean);
  public java.nio.charset.Charset getCharset();
  public cn.hutool.extra.mail.MailAccount setCharset(java.nio.charset.Charset);
  public boolean isSplitlongparameters();
  public void setSplitlongparameters(boolean);
  public boolean isEncodefilename();
  public void setEncodefilename(boolean);
  public boolean isStarttlsEnable();
  public cn.hutool.extra.mail.MailAccount setStarttlsEnable(boolean);
  public java.lang.Boolean isSslEnable();
  public cn.hutool.extra.mail.MailAccount setSslEnable(java.lang.Boolean);
  public java.lang.String getSslProtocols();
  public void setSslProtocols(java.lang.String);
  public java.lang.String getSocketFactoryClass();
  public cn.hutool.extra.mail.MailAccount setSocketFactoryClass(java.lang.String);
  public boolean isSocketFactoryFallback();
  public cn.hutool.extra.mail.MailAccount setSocketFactoryFallback(boolean);
  public int getSocketFactoryPort();
  public cn.hutool.extra.mail.MailAccount setSocketFactoryPort(int);
  public cn.hutool.extra.mail.MailAccount setTimeout(long);
  public cn.hutool.extra.mail.MailAccount setConnectionTimeout(long);
  public cn.hutool.extra.mail.MailAccount setWriteTimeout(long);
  public java.util.Map<java.lang.String, java.lang.Object> getCustomProperty();
  public cn.hutool.extra.mail.MailAccount setCustomProperty(java.lang.String, java.lang.Object);
  public java.util.Properties getSmtpProps();
  public cn.hutool.extra.mail.MailAccount defaultIfEmpty();
  public java.lang.String toString();
}
```

## `cn.hutool.extra.mail.MailException`

```java
public class cn.hutool.extra.mail.MailException extends java.lang.RuntimeException {
  public cn.hutool.extra.mail.MailException(java.lang.Throwable);
  public cn.hutool.extra.mail.MailException(java.lang.String);
  public cn.hutool.extra.mail.MailException(java.lang.String, java.lang.Object...);
  public cn.hutool.extra.mail.MailException(java.lang.String, java.lang.Throwable);
  public cn.hutool.extra.mail.MailException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.extra.mail.MailException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.extra.mail.MailUtil`

```java
public class cn.hutool.extra.mail.MailUtil {
  public cn.hutool.extra.mail.MailUtil();
  public static java.lang.String sendText(java.lang.String, java.lang.String, java.lang.String, java.io.File...);
  public static java.lang.String sendHtml(java.lang.String, java.lang.String, java.lang.String, java.io.File...);
  public static java.lang.String send(java.lang.String, java.lang.String, java.lang.String, boolean, java.io.File...);
  public static java.lang.String send(java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String, boolean, java.io.File...);
  public static java.lang.String sendText(java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, java.io.File...);
  public static java.lang.String sendHtml(java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, java.io.File...);
  public static java.lang.String send(java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, boolean, java.io.File...);
  public static java.lang.String send(java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, boolean, java.io.File...);
  public static java.lang.String send(cn.hutool.extra.mail.MailAccount, java.lang.String, java.lang.String, java.lang.String, boolean, java.io.File...);
  public static java.lang.String send(cn.hutool.extra.mail.MailAccount, java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, boolean, java.io.File...);
  public static java.lang.String send(cn.hutool.extra.mail.MailAccount, java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, boolean, java.io.File...);
  public static java.lang.String sendHtml(java.lang.String, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, java.io.File...);
  public static java.lang.String send(java.lang.String, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, boolean, java.io.File...);
  public static java.lang.String send(java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, boolean, java.io.File...);
  public static java.lang.String sendHtml(java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, java.io.File...);
  public static java.lang.String send(java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, boolean, java.io.File...);
  public static java.lang.String send(java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, boolean, java.io.File...);
  public static java.lang.String send(cn.hutool.extra.mail.MailAccount, java.lang.String, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, boolean, java.io.File...);
  public static java.lang.String send(cn.hutool.extra.mail.MailAccount, java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, boolean, java.io.File...);
  public static java.lang.String send(cn.hutool.extra.mail.MailAccount, java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.io.InputStream>, boolean, java.io.File...);
  public static javax.mail.Session getSession(cn.hutool.extra.mail.MailAccount, boolean);
}
```

## `cn.hutool.extra.mail.UserPassAuthenticator`

```java
public class cn.hutool.extra.mail.UserPassAuthenticator extends javax.mail.Authenticator {
  public cn.hutool.extra.mail.UserPassAuthenticator(java.lang.String, java.lang.String);
}
```
