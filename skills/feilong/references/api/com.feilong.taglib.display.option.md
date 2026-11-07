# com.feilong.taglib.display.option

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.taglib.display.option.OptionCacheContentBuilder`

```java
public class com.feilong.taglib.display.option.OptionCacheContentBuilder implements com.feilong.taglib.display.CacheContentBuilder<com.feilong.taglib.display.option.OptionParam, java.lang.String> {
  public com.feilong.taglib.display.option.OptionCacheContentBuilder();
  public java.lang.String build(com.feilong.taglib.display.option.OptionParam);
  public java.lang.Object build(com.feilong.taglib.display.CacheParam);
}
```

## `com.feilong.taglib.display.option.OptionParam`

```java
public class com.feilong.taglib.display.option.OptionParam extends com.feilong.taglib.display.loadbundle.LoadBundleParam {
  public com.feilong.taglib.display.option.OptionParam();
  public java.lang.String getSelectedKey();
  public void setSelectedKey(java.lang.String);
}
```

## `com.feilong.taglib.display.option.OptionTag`

```java
public class com.feilong.taglib.display.option.OptionTag extends com.feilong.taglib.AbstractLocaleSupportTag {
  public com.feilong.taglib.display.option.OptionTag();
  public void setSelectedKey(java.lang.String);
}
```
