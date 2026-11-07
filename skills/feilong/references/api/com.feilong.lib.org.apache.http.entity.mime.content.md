# com.feilong.lib.org.apache.http.entity.mime.content

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.entity.mime.content.AbstractContentBody`

```java
public abstract class com.feilong.lib.org.apache.http.entity.mime.content.AbstractContentBody implements com.feilong.lib.org.apache.http.entity.mime.content.ContentBody {
  public com.feilong.lib.org.apache.http.entity.mime.content.AbstractContentBody(com.feilong.lib.org.apache.http.entity.ContentType);
  public com.feilong.lib.org.apache.http.entity.mime.content.AbstractContentBody(java.lang.String);
  public com.feilong.lib.org.apache.http.entity.ContentType getContentType();
  public java.lang.String getMimeType();
  public java.lang.String getMediaType();
  public java.lang.String getSubType();
  public java.lang.String getCharset();
}
```

## `com.feilong.lib.org.apache.http.entity.mime.content.ByteArrayBody`

```java
public class com.feilong.lib.org.apache.http.entity.mime.content.ByteArrayBody extends com.feilong.lib.org.apache.http.entity.mime.content.AbstractContentBody {
  public com.feilong.lib.org.apache.http.entity.mime.content.ByteArrayBody(byte[], java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.content.ByteArrayBody(byte[], com.feilong.lib.org.apache.http.entity.ContentType, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.content.ByteArrayBody(byte[], java.lang.String);
  public java.lang.String getFilename();
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
  public java.lang.String getCharset();
  public java.lang.String getTransferEncoding();
  public long getContentLength();
}
```

## `com.feilong.lib.org.apache.http.entity.mime.content.ContentBody`

```java
public interface com.feilong.lib.org.apache.http.entity.mime.content.ContentBody extends com.feilong.lib.org.apache.http.entity.mime.content.ContentDescriptor {
  public abstract java.lang.String getFilename();
  public abstract void writeTo(java.io.OutputStream) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.entity.mime.content.ContentDescriptor`

```java
public interface com.feilong.lib.org.apache.http.entity.mime.content.ContentDescriptor {
  public abstract java.lang.String getMimeType();
  public abstract java.lang.String getMediaType();
  public abstract java.lang.String getSubType();
  public abstract java.lang.String getCharset();
  public abstract java.lang.String getTransferEncoding();
  public abstract long getContentLength();
}
```

## `com.feilong.lib.org.apache.http.entity.mime.content.FileBody`

```java
public class com.feilong.lib.org.apache.http.entity.mime.content.FileBody extends com.feilong.lib.org.apache.http.entity.mime.content.AbstractContentBody {
  public com.feilong.lib.org.apache.http.entity.mime.content.FileBody(java.io.File, java.lang.String, java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.content.FileBody(java.io.File, java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.content.FileBody(java.io.File, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.content.FileBody(java.io.File);
  public com.feilong.lib.org.apache.http.entity.mime.content.FileBody(java.io.File, com.feilong.lib.org.apache.http.entity.ContentType, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.content.FileBody(java.io.File, com.feilong.lib.org.apache.http.entity.ContentType);
  public java.io.InputStream getInputStream() throws java.io.IOException;
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
  public java.lang.String getTransferEncoding();
  public long getContentLength();
  public java.lang.String getFilename();
  public java.io.File getFile();
}
```

## `com.feilong.lib.org.apache.http.entity.mime.content.InputStreamBody`

```java
public class com.feilong.lib.org.apache.http.entity.mime.content.InputStreamBody extends com.feilong.lib.org.apache.http.entity.mime.content.AbstractContentBody {
  public com.feilong.lib.org.apache.http.entity.mime.content.InputStreamBody(java.io.InputStream, java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.content.InputStreamBody(java.io.InputStream, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.content.InputStreamBody(java.io.InputStream, com.feilong.lib.org.apache.http.entity.ContentType, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.content.InputStreamBody(java.io.InputStream, com.feilong.lib.org.apache.http.entity.ContentType);
  public java.io.InputStream getInputStream();
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
  public java.lang.String getTransferEncoding();
  public long getContentLength();
  public java.lang.String getFilename();
}
```

## `com.feilong.lib.org.apache.http.entity.mime.content.StringBody`

```java
public class com.feilong.lib.org.apache.http.entity.mime.content.StringBody extends com.feilong.lib.org.apache.http.entity.mime.content.AbstractContentBody {
  public static com.feilong.lib.org.apache.http.entity.mime.content.StringBody create(java.lang.String, java.lang.String, java.nio.charset.Charset) throws java.lang.IllegalArgumentException;
  public static com.feilong.lib.org.apache.http.entity.mime.content.StringBody create(java.lang.String, java.nio.charset.Charset) throws java.lang.IllegalArgumentException;
  public static com.feilong.lib.org.apache.http.entity.mime.content.StringBody create(java.lang.String) throws java.lang.IllegalArgumentException;
  public com.feilong.lib.org.apache.http.entity.mime.content.StringBody(java.lang.String, java.lang.String, java.nio.charset.Charset) throws java.io.UnsupportedEncodingException;
  public com.feilong.lib.org.apache.http.entity.mime.content.StringBody(java.lang.String, java.nio.charset.Charset) throws java.io.UnsupportedEncodingException;
  public com.feilong.lib.org.apache.http.entity.mime.content.StringBody(java.lang.String) throws java.io.UnsupportedEncodingException;
  public com.feilong.lib.org.apache.http.entity.mime.content.StringBody(java.lang.String, com.feilong.lib.org.apache.http.entity.ContentType);
  public java.io.Reader getReader();
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
  public java.lang.String getTransferEncoding();
  public long getContentLength();
  public java.lang.String getFilename();
}
```
