# com.feilong.taglib.display.pager

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.taglib.display.pager.PagerBuilder`

```java
public final class com.feilong.taglib.display.pager.PagerBuilder {
  public static <T> com.feilong.taglib.display.pager.command.PagerAndContent<T> buildPagerAndContent(com.feilong.taglib.display.pager.command.PagerParams, java.util.List<T>);
  public static java.lang.String buildContent(com.feilong.taglib.display.pager.command.PagerParams);
}
```

## `com.feilong.taglib.display.pager.PagerCacheContentBuilder`

```java
public class com.feilong.taglib.display.pager.PagerCacheContentBuilder implements com.feilong.taglib.display.CacheContentBuilder<com.feilong.taglib.display.pager.command.PagerParams, java.lang.String> {
  public com.feilong.taglib.display.pager.PagerCacheContentBuilder();
  public java.lang.String build(com.feilong.taglib.display.pager.command.PagerParams);
  public java.lang.Object build(com.feilong.taglib.display.CacheParam);
}
```

## `com.feilong.taglib.display.pager.PagerHelper`

```java
public final class com.feilong.taglib.display.pager.PagerHelper {
  public static java.lang.Integer getCurrentPageNo(javax.servlet.http.HttpServletRequest, java.lang.String);
}
```

## `com.feilong.taglib.display.pager.PagerTag`

```java
public class com.feilong.taglib.display.pager.PagerTag extends com.feilong.taglib.AbstractStartWriteContentTag implements com.feilong.taglib.LocaleSupport {
  public com.feilong.taglib.display.pager.PagerTag();
  public java.lang.String buildContent(javax.servlet.http.HttpServletRequest);
  public void setCount(java.lang.Integer);
  public void setPageSize(java.lang.Integer);
  public void setPageParamName(java.lang.String);
  public void setVmPath(java.lang.String);
  public void setSkin(java.lang.String);
  public void setMaxShowPageNo(java.lang.Integer);
  public void setCharsetType(java.lang.String);
  public void setPagerHtmlAttributeName(java.lang.String);
  public void setLocale(java.lang.Object);
  public void setDynamicNavigationPageNumberConfig(java.lang.String);
  public java.lang.Object buildContent(javax.servlet.http.HttpServletRequest);
}
```

## `com.feilong.taglib.display.pager.PagerTagExtraInfo`

```java
public class com.feilong.taglib.display.pager.PagerTagExtraInfo extends com.feilong.taglib.BaseTEI {
  public com.feilong.taglib.display.pager.PagerTagExtraInfo();
  public javax.servlet.jsp.tagext.VariableInfo[] getVariableInfo(javax.servlet.jsp.tagext.TagData);
  public javax.servlet.jsp.tagext.ValidationMessage[] validate(javax.servlet.jsp.tagext.TagData);
}
```
