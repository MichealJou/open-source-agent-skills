# cn.hutool.http.useragent

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.http.useragent.Browser`

```java
public class cn.hutool.http.useragent.Browser extends cn.hutool.http.useragent.UserAgentInfo {
  public static synchronized void addCustomBrowser(java.lang.String, java.lang.String, java.lang.String);
  public cn.hutool.http.useragent.Browser(java.lang.String, java.lang.String, java.lang.String);
  public java.lang.String getVersion(java.lang.String);
  public boolean isMobile();
}
```

## `cn.hutool.http.useragent.Engine`

```java
public class cn.hutool.http.useragent.Engine extends cn.hutool.http.useragent.UserAgentInfo {
  public cn.hutool.http.useragent.Engine(java.lang.String, java.lang.String);
  public java.lang.String getVersion(java.lang.String);
}
```

## `cn.hutool.http.useragent.OS`

```java
public class cn.hutool.http.useragent.OS extends cn.hutool.http.useragent.UserAgentInfo {
  public static synchronized void addCustomOs(java.lang.String, java.lang.String, java.lang.String);
  public cn.hutool.http.useragent.OS(java.lang.String, java.lang.String);
  public cn.hutool.http.useragent.OS(java.lang.String, java.lang.String, java.lang.String);
  public java.lang.String getVersion(java.lang.String);
  public boolean isMacOS();
}
```

## `cn.hutool.http.useragent.Platform`

```java
public class cn.hutool.http.useragent.Platform extends cn.hutool.http.useragent.UserAgentInfo {
  public cn.hutool.http.useragent.Platform(java.lang.String, java.lang.String);
  public boolean isMobile();
  public boolean isIPhoneOrIPod();
  public boolean isIPad();
  public boolean isIos();
  public boolean isAndroid();
  public boolean isHarmony();
}
```

## `cn.hutool.http.useragent.UserAgent`

```java
public class cn.hutool.http.useragent.UserAgent implements java.io.Serializable {
  public cn.hutool.http.useragent.UserAgent();
  public boolean isMobile();
  public void setMobile(boolean);
  public cn.hutool.http.useragent.Browser getBrowser();
  public void setBrowser(cn.hutool.http.useragent.Browser);
  public cn.hutool.http.useragent.Platform getPlatform();
  public void setPlatform(cn.hutool.http.useragent.Platform);
  public cn.hutool.http.useragent.OS getOs();
  public void setOs(cn.hutool.http.useragent.OS);
  public java.lang.String getOsVersion();
  public void setOsVersion(java.lang.String);
  public cn.hutool.http.useragent.Engine getEngine();
  public void setEngine(cn.hutool.http.useragent.Engine);
  public java.lang.String getVersion();
  public void setVersion(java.lang.String);
  public java.lang.String getEngineVersion();
  public void setEngineVersion(java.lang.String);
}
```

## `cn.hutool.http.useragent.UserAgentInfo`

```java
public class cn.hutool.http.useragent.UserAgentInfo implements java.io.Serializable {
  public cn.hutool.http.useragent.UserAgentInfo(java.lang.String, java.lang.String);
  public cn.hutool.http.useragent.UserAgentInfo(java.lang.String, java.util.regex.Pattern);
  public java.lang.String getName();
  public java.util.regex.Pattern getPattern();
  public boolean isMatch(java.lang.String);
  public boolean isUnknown();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
}
```

## `cn.hutool.http.useragent.UserAgentParser`

```java
public class cn.hutool.http.useragent.UserAgentParser {
  public cn.hutool.http.useragent.UserAgentParser();
  public static cn.hutool.http.useragent.UserAgent parse(java.lang.String);
}
```

## `cn.hutool.http.useragent.UserAgentUtil`

```java
public class cn.hutool.http.useragent.UserAgentUtil {
  public cn.hutool.http.useragent.UserAgentUtil();
  public static cn.hutool.http.useragent.UserAgent parse(java.lang.String);
}
```
