# com.feilong.taglib

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.taglib.AbstractConditionalTag`

```java
public abstract class com.feilong.taglib.AbstractConditionalTag extends com.feilong.taglib.BaseTag {
  public com.feilong.taglib.AbstractConditionalTag();
  public int doStartTag();
}
```

## `com.feilong.taglib.AbstractEndWriteContentTag`

```java
public abstract class com.feilong.taglib.AbstractEndWriteContentTag extends com.feilong.taglib.AbstractWriteContentTag {
  public com.feilong.taglib.AbstractEndWriteContentTag();
  public int doStartTag();
  public int doEndTag() throws javax.servlet.jsp.JspException;
}
```

## `com.feilong.taglib.AbstractLocaleSupportTag`

```java
public abstract class com.feilong.taglib.AbstractLocaleSupportTag extends com.feilong.taglib.AbstractStartWriteContentTag implements com.feilong.taglib.LocaleSupport {
  public com.feilong.taglib.AbstractLocaleSupportTag();
  public void setBaseName(java.lang.String);
  public void setLocale(java.lang.Object);
}
```

## `com.feilong.taglib.AbstractStartWriteContentTag`

```java
public abstract class com.feilong.taglib.AbstractStartWriteContentTag extends com.feilong.taglib.AbstractWriteContentTag {
  public com.feilong.taglib.AbstractStartWriteContentTag();
  public int doStartTag();
}
```

## `com.feilong.taglib.BaseTEI`

```java
public abstract class com.feilong.taglib.BaseTEI extends javax.servlet.jsp.tagext.TagExtraInfo {
  public com.feilong.taglib.BaseTEI();
}
```

## `com.feilong.taglib.BaseTag`

```java
public abstract class com.feilong.taglib.BaseTag extends javax.servlet.jsp.tagext.BodyTagSupport implements javax.servlet.jsp.tagext.TryCatchFinally {
  public com.feilong.taglib.BaseTag();
  public void doCatch(java.lang.Throwable) throws java.lang.Throwable;
  public void doFinally();
}
```

## `com.feilong.taglib.CacheTag`

```java
public interface com.feilong.taglib.CacheTag {
  public abstract java.lang.String buildCacheTagKey();
}
```

## `com.feilong.taglib.LocaleSupport`

```java
public interface com.feilong.taglib.LocaleSupport {
  public abstract void setLocale(java.lang.Object);
}
```

## `com.feilong.taglib.SimpleTagStringCacheManager`

```java
public final class com.feilong.taglib.SimpleTagStringCacheManager {
  public static java.lang.Object get(java.lang.String);
  public static void put(java.lang.String, java.lang.Object);
}
```

## `com.feilong.taglib.TagUtils`

```java
public final class com.feilong.taglib.TagUtils {
  public static int getScope(java.lang.String);
  public static <T> T findAttributeValue(javax.servlet.jsp.PageContext, java.lang.String, java.lang.String);
}
```
