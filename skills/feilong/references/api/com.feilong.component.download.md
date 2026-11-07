# com.feilong.component.download

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.component.download.DefaultRequestFileCreatorDetector`

```java
public class com.feilong.component.download.DefaultRequestFileCreatorDetector implements com.feilong.context.filecreator.RequestFileCreatorDetector {
  public com.feilong.component.download.DefaultRequestFileCreatorDetector();
  public com.feilong.context.filecreator.RequestFileCreator detect(javax.servlet.http.HttpServletRequest);
  public void setIdentifyParamName(java.lang.String);
}
```

## `com.feilong.component.download.DownloadController`

```java
public class com.feilong.component.download.DownloadController {
  public com.feilong.component.download.DownloadController();
  public void download(javax.servlet.http.HttpServletRequest, javax.servlet.http.HttpServletResponse);
}
```

## `com.feilong.component.download.ExcelRequestFileCreator`

```java
public class com.feilong.component.download.ExcelRequestFileCreator implements com.feilong.context.filecreator.RequestFileCreator {
  public com.feilong.component.download.ExcelRequestFileCreator();
  public java.lang.String create(javax.servlet.http.HttpServletRequest);
  public void setTemplateLocation(java.lang.String);
  public void setSheetDefinitionLocation(java.lang.String);
  public void setRequestDataBuilder(com.feilong.context.RequestDataBuilder);
  public void setSheetName(java.lang.String);
  public void setOutputFileName(java.lang.String);
  public java.lang.String create(java.lang.Object);
}
```
