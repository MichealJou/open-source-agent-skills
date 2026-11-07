# com.feilong.taglib.display.breadcrumb.command

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity`

```java
public class com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity<T> implements java.io.Serializable {
  public com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity();
  public com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity(T, java.lang.String, java.lang.String, java.lang.String, T);
  public java.lang.String getName();
  public void setName(java.lang.String);
  public java.lang.String getTitle();
  public void setTitle(java.lang.String);
  public java.lang.String getPath();
  public void setPath(java.lang.String);
  public T getId();
  public void setId(T);
  public void setParentId(T);
  public T getParentId();
}
```

## `com.feilong.taglib.display.breadcrumb.command.BreadCrumbParams`

```java
public class com.feilong.taglib.display.breadcrumb.command.BreadCrumbParams<T> implements java.io.Serializable {
  public com.feilong.taglib.display.breadcrumb.command.BreadCrumbParams();
  public java.util.List<com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity<T>> getBreadCrumbEntityList();
  public void setBreadCrumbEntityList(java.util.List<com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity<T>>);
  public java.lang.String getConnector();
  public void setConnector(java.lang.String);
  public java.lang.String getCurrentPath();
  public void setCurrentPath(java.lang.String);
  public java.lang.String getVmPath();
  public void setVmPath(java.lang.String);
  public java.lang.String getUrlPrefix();
  public void setUrlPrefix(java.lang.String);
}
```

## `com.feilong.taglib.display.breadcrumb.command.BreadCrumbVMParams`

```java
public class com.feilong.taglib.display.breadcrumb.command.BreadCrumbVMParams<T> implements java.io.Serializable {
  public com.feilong.taglib.display.breadcrumb.command.BreadCrumbVMParams();
  public java.util.List<com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity<T>> getBreadCrumbEntityList();
  public void setBreadCrumbEntityList(java.util.List<com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity<T>>);
  public java.lang.String getConnector();
  public void setConnector(java.lang.String);
}
```
