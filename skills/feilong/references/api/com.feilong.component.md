# com.feilong.component

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.component.DataFileEmailComponent`

```java
public class com.feilong.component.DataFileEmailComponent<T extends com.feilong.context.Data> implements com.feilong.context.Task<java.lang.Void>, com.feilong.context.log.UseTimeLogable, com.feilong.component.Component {
  public com.feilong.component.DataFileEmailComponent();
  public java.lang.Void run();
  public void setDataListQuery(com.feilong.context.DataListQuery<T>);
  public void setMailSender(com.feilong.net.mail.MailSender);
  public void setListDataFileCreator(com.feilong.context.filecreator.ListDataFileCreator<T>);
  public void setFileReworker(com.feilong.context.FileReworker);
  public void setMailSendRequest(com.feilong.net.mail.entity.MailSendRequest);
  public java.lang.Object run();
}
```

## `com.feilong.component.DataFileZipEmailComponent`

```java
public class com.feilong.component.DataFileZipEmailComponent<T extends com.feilong.context.Data> extends com.feilong.component.DataFileEmailComponent<T> {
  public com.feilong.component.DataFileZipEmailComponent();
  public void setOutputZipPathExpression(java.lang.String);
}
```

## `com.feilong.component.SimpleListLoopExcelFileCreator`

```java
public class com.feilong.component.SimpleListLoopExcelFileCreator<T extends com.feilong.context.Data> implements com.feilong.context.filecreator.ListDataFileCreator<T> {
  public com.feilong.component.SimpleListLoopExcelFileCreator();
  public java.lang.String create(java.util.List<T>);
  public void setXmlSheetConfigurations(java.lang.String);
  public void setSheetName(java.lang.String);
  public void setDataName(java.lang.String);
  public void setOutputFilePathExpression(java.lang.String);
  public void setTemplateLocation(java.lang.String);
  public java.lang.String create(java.lang.Object);
}
```

## `com.feilong.component.ZipFileReworker`

```java
public class com.feilong.component.ZipFileReworker implements com.feilong.context.FileReworker {
  public com.feilong.component.ZipFileReworker(java.lang.String);
  public com.feilong.component.ZipFileReworker();
  public com.feilong.component.ZipFileReworker(com.feilong.zip.ZipHandler, java.lang.String);
  public java.lang.String rework(java.lang.String);
  public void setOutputZipPathExpression(java.lang.String);
  public void setZipHandler(com.feilong.zip.ZipHandler);
}
```
