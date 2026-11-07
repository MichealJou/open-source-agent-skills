# com.feilong.taglib.display.loadbundle

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.taglib.display.loadbundle.LoadBundleBuilder`

```java
public class com.feilong.taglib.display.loadbundle.LoadBundleBuilder implements com.feilong.taglib.display.CacheContentBuilder<com.feilong.taglib.display.loadbundle.LoadBundleParam, java.util.Map<java.lang.String, java.lang.String>> {
  public com.feilong.taglib.display.loadbundle.LoadBundleBuilder();
  public java.util.Map<java.lang.String, java.lang.String> build(com.feilong.taglib.display.loadbundle.LoadBundleParam);
  public java.lang.Object build(com.feilong.taglib.display.CacheParam);
}
```

## `com.feilong.taglib.display.loadbundle.LoadBundleParam`

```java
public class com.feilong.taglib.display.loadbundle.LoadBundleParam implements java.io.Serializable,com.feilong.taglib.display.CacheParam {
  public com.feilong.taglib.display.loadbundle.LoadBundleParam();
  public java.lang.String getBaseName();
  public void setBaseName(java.lang.String);
  public java.util.Locale getLocale();
  public void setLocale(java.util.Locale);
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```

## `com.feilong.taglib.display.loadbundle.LoadBundleTag`

```java
public class com.feilong.taglib.display.loadbundle.LoadBundleTag extends com.feilong.taglib.AbstractLocaleSupportTag {
  public com.feilong.taglib.display.loadbundle.LoadBundleTag();
  public void setVar(java.lang.String);
}
```
