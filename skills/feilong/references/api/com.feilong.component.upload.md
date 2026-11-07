# com.feilong.component.upload

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.component.upload.AbstractSimpleListDataHandler`

```java
public abstract class com.feilong.component.upload.AbstractSimpleListDataHandler<T> implements com.feilong.context.DataHandler {
  public com.feilong.component.upload.AbstractSimpleListDataHandler();
  public void handle(java.util.Map<java.lang.String, java.lang.Object>);
}
```

## `com.feilong.component.upload.DefaultMultipartFileResolver`

```java
public class com.feilong.component.upload.DefaultMultipartFileResolver implements com.feilong.component.upload.MultipartFileResolver {
  public com.feilong.component.upload.DefaultMultipartFileResolver();
  public java.lang.String upload(org.springframework.web.multipart.MultipartFile, java.lang.String, java.lang.String);
  public java.util.List<java.lang.String> upload(org.springframework.web.multipart.MultipartFile[], java.lang.String, java.lang.String[]);
}
```

## `com.feilong.component.upload.DefaultRequestFileParserDetector`

```java
public class com.feilong.component.upload.DefaultRequestFileParserDetector implements com.feilong.context.fileparser.RequestFileParserDetector {
  public com.feilong.component.upload.DefaultRequestFileParserDetector();
  public com.feilong.context.fileparser.FileParser detect(javax.servlet.http.HttpServletRequest);
  public void setIdentifyParamName(java.lang.String);
}
```

## `com.feilong.component.upload.ExcelFileParser`

```java
public class com.feilong.component.upload.ExcelFileParser implements com.feilong.context.fileparser.FileParser {
  public com.feilong.component.upload.ExcelFileParser();
  public void parse(java.lang.String);
  public void setSheetDefinitionLocation(java.lang.String);
  public void setSheetName(java.lang.String);
  public void setDataName(java.lang.String);
  public void setDataHandler(com.feilong.context.DataHandler);
}
```

## `com.feilong.component.upload.MultipartFileResolver`

```java
public interface com.feilong.component.upload.MultipartFileResolver {
  public abstract java.lang.String upload(org.springframework.web.multipart.MultipartFile, java.lang.String, java.lang.String);
  public abstract java.util.List<java.lang.String> upload(org.springframework.web.multipart.MultipartFile[], java.lang.String, java.lang.String[]);
}
```

## `com.feilong.component.upload.UploadController`

```java
public class com.feilong.component.upload.UploadController {
  public com.feilong.component.upload.UploadController();
  public void upload(javax.servlet.http.HttpServletRequest, javax.servlet.http.HttpServletResponse, org.springframework.web.multipart.MultipartFile[]);
}
```
