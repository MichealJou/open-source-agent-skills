# com.feilong.taglib.display.breadcrumb

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.taglib.display.breadcrumb.BreadCrumbTag`

```java
public class com.feilong.taglib.display.breadcrumb.BreadCrumbTag extends com.feilong.taglib.AbstractStartWriteContentTag {
  public com.feilong.taglib.display.breadcrumb.BreadCrumbTag();
  public void setConnector(java.lang.String);
  public void setBreadCrumbEntityList(java.util.List<com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity<java.lang.Object>>);
  public void setVmPath(java.lang.String);
  public void setUrlPrefix(java.lang.String);
  public java.lang.String getUrlPrefix();
  public java.lang.String getConnector();
  public java.lang.String getVmPath();
}
```

## `com.feilong.taglib.display.breadcrumb.BreadCrumbUtil`

```java
public class com.feilong.taglib.display.breadcrumb.BreadCrumbUtil {
  public static java.lang.String getBreadCrumbContent(com.feilong.taglib.display.breadcrumb.command.BreadCrumbParams);
}
```
