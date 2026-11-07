# com.feilong.template.extension

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.template.extension.TemplateFileData`

```java
public class com.feilong.template.extension.TemplateFileData {
  public com.feilong.template.extension.TemplateFileData();
  public com.feilong.template.extension.TemplateFileData(java.lang.String, java.util.Map<java.lang.String, ?>, java.lang.String);
  public java.lang.String getTemplatePath();
  public void setTemplatePath(java.lang.String);
  public java.util.Map<java.lang.String, ?> getData();
  public void setData(java.util.Map<java.lang.String, ?>);
  public java.lang.String getOutPutFilePath();
  public void setOutPutFilePath(java.lang.String);
}
```

## `com.feilong.template.extension.TemplateFileDataUtil`

```java
public class com.feilong.template.extension.TemplateFileDataUtil {
  public static void writeAndOpen(com.feilong.template.extension.TemplateFileData);
}
```
