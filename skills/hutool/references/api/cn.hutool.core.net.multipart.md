# cn.hutool.core.net.multipart

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.net.multipart.MultipartFormData`

```java
public class cn.hutool.core.net.multipart.MultipartFormData {
  public cn.hutool.core.net.multipart.MultipartFormData();
  public cn.hutool.core.net.multipart.MultipartFormData(cn.hutool.core.net.multipart.UploadSetting);
  public void parseRequestStream(java.io.InputStream, java.nio.charset.Charset) throws java.io.IOException;
  public java.lang.String getParam(java.lang.String);
  public java.util.Set<java.lang.String> getParamNames();
  public java.lang.String[] getArrayParam(java.lang.String);
  public java.util.List<java.lang.String> getListParam(java.lang.String);
  public java.util.Map<java.lang.String, java.lang.String[]> getParamMap();
  public cn.hutool.core.map.multi.ListValueMap<java.lang.String, java.lang.String> getParamListMap();
  public cn.hutool.core.net.multipart.UploadFile getFile(java.lang.String);
  public cn.hutool.core.net.multipart.UploadFile[] getFiles(java.lang.String);
  public java.util.List<cn.hutool.core.net.multipart.UploadFile> getFileList(java.lang.String);
  public java.util.Set<java.lang.String> getFileParamNames();
  public java.util.Map<java.lang.String, cn.hutool.core.net.multipart.UploadFile[]> getFileMap();
  public cn.hutool.core.map.multi.ListValueMap<java.lang.String, cn.hutool.core.net.multipart.UploadFile> getFileListValueMap();
  public boolean isLoaded();
}
```

## `cn.hutool.core.net.multipart.MultipartRequestInputStream`

```java
public class cn.hutool.core.net.multipart.MultipartRequestInputStream extends java.io.BufferedInputStream {
  public cn.hutool.core.net.multipart.MultipartRequestInputStream(java.io.InputStream);
  public byte readByte() throws java.io.IOException;
  public void skipBytes(long) throws java.io.IOException;
  public byte[] readBoundary() throws java.io.IOException;
  public cn.hutool.core.net.multipart.UploadFileHeader getLastHeader();
  public cn.hutool.core.net.multipart.UploadFileHeader readDataHeader(java.nio.charset.Charset) throws java.io.IOException;
  public java.lang.String readString(java.nio.charset.Charset) throws java.io.IOException;
  public long copy(java.io.OutputStream) throws java.io.IOException;
  public long copy(java.io.OutputStream, long) throws java.io.IOException;
  public long skipToBoundary() throws java.io.IOException;
  public boolean isBoundary(byte) throws java.io.IOException;
}
```

## `cn.hutool.core.net.multipart.UploadFile`

```java
public class cn.hutool.core.net.multipart.UploadFile {
  public cn.hutool.core.net.multipart.UploadFile(cn.hutool.core.net.multipart.UploadFileHeader, cn.hutool.core.net.multipart.UploadSetting);
  public void delete();
  public java.io.File write(java.lang.String) throws java.io.IOException;
  public java.io.File write(java.io.File) throws java.io.IOException;
  public byte[] getFileContent() throws java.io.IOException;
  public java.io.InputStream getFileInputStream() throws java.io.IOException;
  public cn.hutool.core.net.multipart.UploadFileHeader getHeader();
  public java.lang.String getFileName();
  public long size();
  public boolean isUploaded();
  public boolean isInMemory();
}
```

## `cn.hutool.core.net.multipart.UploadFileHeader`

```java
public class cn.hutool.core.net.multipart.UploadFileHeader {
  public boolean isFile();
  public java.lang.String getFormFieldName();
  public java.lang.String getFormFileName();
  public java.lang.String getFileName();
  public java.lang.String getContentType();
  public java.lang.String getMimeType();
  public java.lang.String getMimeSubtype();
  public java.lang.String getContentDisposition();
}
```

## `cn.hutool.core.net.multipart.UploadSetting`

```java
public class cn.hutool.core.net.multipart.UploadSetting {
  public cn.hutool.core.net.multipart.UploadSetting();
  public long getMaxFileSize();
  public void setMaxFileSize(long);
  public int getMemoryThreshold();
  public void setMemoryThreshold(int);
  public java.lang.String getTmpUploadPath();
  public void setTmpUploadPath(java.lang.String);
  public java.lang.String[] getFileExts();
  public void setFileExts(java.lang.String[]);
  public boolean isAllowFileExts();
  public void setAllowFileExts(boolean);
}
```
