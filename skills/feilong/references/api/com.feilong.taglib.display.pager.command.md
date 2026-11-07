# com.feilong.taglib.display.pager.command

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.taglib.display.pager.command.Pager`

```java
public final class com.feilong.taglib.display.pager.command.Pager<T> implements java.io.Serializable {
  public com.feilong.taglib.display.pager.command.Pager();
  public com.feilong.taglib.display.pager.command.Pager(java.lang.Integer, java.lang.Integer, java.lang.Integer);
  public int getAllPageNo();
  public int getOriginatingAllPageNo();
  public int getPrePageNo();
  public int getNextPageNo();
  public int getOriginatingNextPageNo();
  public java.lang.Integer getCurrentPageNo();
  public void setCurrentPageNo(java.lang.Integer);
  public java.lang.Integer getPageSize();
  public void setPageSize(java.lang.Integer);
  public java.lang.Integer getCount();
  public void setCount(java.lang.Integer);
  public java.lang.Integer getMaxShowPageNo();
  public void setMaxShowPageNo(java.lang.Integer);
  public java.util.List<T> getItemList();
  public void setItemList(java.util.List<T>);
}
```

## `com.feilong.taglib.display.pager.command.PagerAndContent`

```java
public class com.feilong.taglib.display.pager.command.PagerAndContent<T> implements java.io.Serializable {
  public com.feilong.taglib.display.pager.command.PagerAndContent();
  public com.feilong.taglib.display.pager.command.PagerAndContent(com.feilong.taglib.display.pager.command.Pager<T>, java.lang.String);
  public com.feilong.taglib.display.pager.command.Pager<T> getPager();
  public void setPager(com.feilong.taglib.display.pager.command.Pager<T>);
  public java.lang.String getContent();
  public void setContent(java.lang.String);
}
```

## `com.feilong.taglib.display.pager.command.PagerParams`

```java
public class com.feilong.taglib.display.pager.command.PagerParams implements java.io.Serializable,com.feilong.taglib.display.CacheParam {
  public com.feilong.taglib.display.pager.command.PagerParams(java.lang.Integer, java.lang.String);
  public com.feilong.taglib.display.pager.command.PagerParams(java.lang.Integer, com.feilong.taglib.display.pager.command.PagerType);
  public java.lang.String getPageUrl();
  public void setPageUrl(java.lang.String);
  public java.lang.Integer getTotalCount();
  public void setTotalCount(java.lang.Integer);
  public java.lang.Integer getCurrentPageNo();
  public void setCurrentPageNo(java.lang.Integer);
  public java.lang.Integer getPageSize();
  public void setPageSize(java.lang.Integer);
  public java.lang.String getSkin();
  public void setSkin(java.lang.String);
  public java.lang.String getPageParamName();
  public void setPageParamName(java.lang.String);
  public java.lang.String getVmPath();
  public void setVmPath(java.lang.String);
  public java.lang.Integer getMaxShowPageNo();
  public void setMaxShowPageNo(java.lang.Integer);
  public java.lang.String getCharsetType();
  public void setCharsetType(java.lang.String);
  public java.util.Locale getLocale();
  public void setLocale(java.util.Locale);
  public boolean getDebugIsNotParseVM();
  public void setDebugIsNotParseVM(boolean);
  public void setPagerType(com.feilong.taglib.display.pager.command.PagerType);
  public com.feilong.taglib.display.pager.command.PagerType getPagerType();
  public java.lang.String getDynamicNavigationPageNumberConfig();
  public void setDynamicNavigationPageNumberConfig(java.lang.String);
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```

## `com.feilong.taglib.display.pager.command.PagerType`

```java
public final class com.feilong.taglib.display.pager.command.PagerType extends java.lang.Enum<com.feilong.taglib.display.pager.command.PagerType> {
  public static com.feilong.taglib.display.pager.command.PagerType[] values();
  public static com.feilong.taglib.display.pager.command.PagerType valueOf(java.lang.String);
}
```

## `com.feilong.taglib.display.pager.command.PagerUrlTemplate`

```java
public class com.feilong.taglib.display.pager.command.PagerUrlTemplate implements java.io.Serializable {
  public com.feilong.taglib.display.pager.command.PagerUrlTemplate();
  public java.lang.String getHref();
  public void setHref(java.lang.String);
  public java.lang.Integer getTemplateValue();
  public void setTemplateValue(java.lang.Integer);
}
```

## `com.feilong.taglib.display.pager.command.PagerVMParam`

```java
public class com.feilong.taglib.display.pager.command.PagerVMParam implements java.io.Serializable {
  public com.feilong.taglib.display.pager.command.PagerVMParam();
  public java.lang.String getSkin();
  public void setSkin(java.lang.String);
  public java.lang.Integer getTotalCount();
  public void setTotalCount(java.lang.Integer);
  public java.lang.Integer getCurrentPageNo();
  public void setCurrentPageNo(java.lang.Integer);
  public java.lang.Integer getAllPageNo();
  public void setAllPageNo(java.lang.Integer);
  public java.lang.Integer getMaxShowPageNo();
  public void setMaxShowPageNo(java.lang.Integer);
  public java.lang.String getPreUrl();
  public void setPreUrl(java.lang.String);
  public java.lang.String getNextUrl();
  public void setNextUrl(java.lang.String);
  public java.lang.String getFirstUrl();
  public void setFirstUrl(java.lang.String);
  public java.lang.String getLastUrl();
  public void setLastUrl(java.lang.String);
  public java.lang.Integer getStartIteratorIndex();
  public void setStartIteratorIndex(java.lang.Integer);
  public java.lang.Integer getEndIteratorIndex();
  public void setEndIteratorIndex(java.lang.Integer);
  public com.feilong.taglib.display.pager.command.PagerUrlTemplate getPagerUrlTemplate();
  public void setPagerUrlTemplate(com.feilong.taglib.display.pager.command.PagerUrlTemplate);
  public java.lang.String getPageParamName();
  public void setPageParamName(java.lang.String);
  public com.feilong.taglib.display.pager.command.PagerType getPagerType();
  public void setPagerType(com.feilong.taglib.display.pager.command.PagerType);
  public java.lang.Integer getPrePageNo();
  public void setPrePageNo(java.lang.Integer);
  public java.lang.Integer getNextPageNo();
  public void setNextPageNo(java.lang.Integer);
  public java.util.Map<java.lang.Integer, java.lang.String> getIteratorIndexMap();
  public void setIteratorIndexMap(java.util.Map<java.lang.Integer, java.lang.String>);
}
```
