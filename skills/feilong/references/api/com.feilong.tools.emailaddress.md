# com.feilong.tools.emailaddress

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.tools.emailaddress.EmailAddressUtil`

```java
public final class com.feilong.tools.emailaddress.EmailAddressUtil {
  public static com.feilong.tools.emailaddress.EmailProvider getEmailProvider(java.lang.String);
  public static java.lang.String getDomain(java.lang.String);
  public static java.lang.String getUser(java.lang.String);
}
```

## `com.feilong.tools.emailaddress.EmailProvider`

```java
public class com.feilong.tools.emailaddress.EmailProvider implements java.io.Serializable {
  public java.lang.String getDomain();
  public void setDomain(java.lang.String);
  public java.lang.String getName();
  public void setName(java.lang.String);
  public java.lang.String getWebSite();
  public void setWebSite(java.lang.String);
  public java.lang.String toString();
}
```
