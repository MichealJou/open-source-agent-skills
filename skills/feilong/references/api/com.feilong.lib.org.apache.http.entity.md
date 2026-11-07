# com.feilong.lib.org.apache.http.entity

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.entity.AbstractHttpEntity`

```java
public abstract class com.feilong.lib.org.apache.http.entity.AbstractHttpEntity implements com.feilong.lib.org.apache.http.HttpEntity {
  public com.feilong.lib.org.apache.http.Header getContentType();
  public com.feilong.lib.org.apache.http.Header getContentEncoding();
  public boolean isChunked();
  public void setContentType(com.feilong.lib.org.apache.http.Header);
  public void setContentType(java.lang.String);
  public void setContentEncoding(com.feilong.lib.org.apache.http.Header);
  public void setContentEncoding(java.lang.String);
  public void setChunked(boolean);
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.entity.BasicHttpEntity`

```java
public class com.feilong.lib.org.apache.http.entity.BasicHttpEntity extends com.feilong.lib.org.apache.http.entity.AbstractHttpEntity {
  public com.feilong.lib.org.apache.http.entity.BasicHttpEntity();
  public long getContentLength();
  public java.io.InputStream getContent() throws java.lang.IllegalStateException;
  public boolean isRepeatable();
  public void setContentLength(long);
  public void setContent(java.io.InputStream);
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
  public boolean isStreaming();
}
```

## `com.feilong.lib.org.apache.http.entity.BufferedHttpEntity`

```java
public class com.feilong.lib.org.apache.http.entity.BufferedHttpEntity extends com.feilong.lib.org.apache.http.entity.HttpEntityWrapper {
  public com.feilong.lib.org.apache.http.entity.BufferedHttpEntity(com.feilong.lib.org.apache.http.HttpEntity) throws java.io.IOException;
  public long getContentLength();
  public java.io.InputStream getContent() throws java.io.IOException;
  public boolean isChunked();
  public boolean isRepeatable();
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
  public boolean isStreaming();
}
```

## `com.feilong.lib.org.apache.http.entity.ByteArrayEntity`

```java
public class com.feilong.lib.org.apache.http.entity.ByteArrayEntity extends com.feilong.lib.org.apache.http.entity.AbstractHttpEntity implements java.lang.Cloneable {
  public com.feilong.lib.org.apache.http.entity.ByteArrayEntity(byte[]);
  public com.feilong.lib.org.apache.http.entity.ByteArrayEntity(byte[], int, int);
  public com.feilong.lib.org.apache.http.entity.ByteArrayEntity(byte[], com.feilong.lib.org.apache.http.entity.ContentType);
  public com.feilong.lib.org.apache.http.entity.ByteArrayEntity(byte[], int, int, com.feilong.lib.org.apache.http.entity.ContentType);
  public boolean isRepeatable();
  public long getContentLength();
  public java.io.InputStream getContent();
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
  public boolean isStreaming();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.entity.ContentLengthStrategy`

```java
public interface com.feilong.lib.org.apache.http.entity.ContentLengthStrategy {
  public abstract long determineLength(com.feilong.lib.org.apache.http.HttpMessage) throws com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.entity.ContentProducer`

```java
public interface com.feilong.lib.org.apache.http.entity.ContentProducer {
  public abstract void writeTo(java.io.OutputStream) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.entity.ContentType`

```java
public final class com.feilong.lib.org.apache.http.entity.ContentType implements java.io.Serializable {
  public java.lang.String getMimeType();
  public java.nio.charset.Charset getCharset();
  public java.lang.String getParameter(java.lang.String);
  public java.lang.String toString();
  public static com.feilong.lib.org.apache.http.entity.ContentType create(java.lang.String, java.nio.charset.Charset);
  public static com.feilong.lib.org.apache.http.entity.ContentType create(java.lang.String);
  public static com.feilong.lib.org.apache.http.entity.ContentType create(java.lang.String, java.lang.String) throws java.nio.charset.UnsupportedCharsetException;
  public static com.feilong.lib.org.apache.http.entity.ContentType create(java.lang.String, com.feilong.lib.org.apache.http.NameValuePair...) throws java.nio.charset.UnsupportedCharsetException;
  public static com.feilong.lib.org.apache.http.entity.ContentType parse(java.lang.String) throws com.feilong.lib.org.apache.http.ParseException, java.nio.charset.UnsupportedCharsetException;
  public static com.feilong.lib.org.apache.http.entity.ContentType get(com.feilong.lib.org.apache.http.HttpEntity) throws com.feilong.lib.org.apache.http.ParseException, java.nio.charset.UnsupportedCharsetException;
  public static com.feilong.lib.org.apache.http.entity.ContentType getLenient(com.feilong.lib.org.apache.http.HttpEntity);
  public static com.feilong.lib.org.apache.http.entity.ContentType getOrDefault(com.feilong.lib.org.apache.http.HttpEntity) throws com.feilong.lib.org.apache.http.ParseException, java.nio.charset.UnsupportedCharsetException;
  public static com.feilong.lib.org.apache.http.entity.ContentType getLenientOrDefault(com.feilong.lib.org.apache.http.HttpEntity) throws com.feilong.lib.org.apache.http.ParseException, java.nio.charset.UnsupportedCharsetException;
  public static com.feilong.lib.org.apache.http.entity.ContentType getByMimeType(java.lang.String);
  public com.feilong.lib.org.apache.http.entity.ContentType withCharset(java.nio.charset.Charset);
  public com.feilong.lib.org.apache.http.entity.ContentType withCharset(java.lang.String);
  public com.feilong.lib.org.apache.http.entity.ContentType withParameters(com.feilong.lib.org.apache.http.NameValuePair...) throws java.nio.charset.UnsupportedCharsetException;
}
```

## `com.feilong.lib.org.apache.http.entity.EntityTemplate`

```java
public class com.feilong.lib.org.apache.http.entity.EntityTemplate extends com.feilong.lib.org.apache.http.entity.AbstractHttpEntity {
  public com.feilong.lib.org.apache.http.entity.EntityTemplate(com.feilong.lib.org.apache.http.entity.ContentProducer);
  public long getContentLength();
  public java.io.InputStream getContent() throws java.io.IOException;
  public boolean isRepeatable();
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
  public boolean isStreaming();
}
```

## `com.feilong.lib.org.apache.http.entity.FileEntity`

```java
public class com.feilong.lib.org.apache.http.entity.FileEntity extends com.feilong.lib.org.apache.http.entity.AbstractHttpEntity implements java.lang.Cloneable {
  public com.feilong.lib.org.apache.http.entity.FileEntity(java.io.File, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.FileEntity(java.io.File, com.feilong.lib.org.apache.http.entity.ContentType);
  public com.feilong.lib.org.apache.http.entity.FileEntity(java.io.File);
  public boolean isRepeatable();
  public long getContentLength();
  public java.io.InputStream getContent() throws java.io.IOException;
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
  public boolean isStreaming();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.entity.HttpEntityWrapper`

```java
public class com.feilong.lib.org.apache.http.entity.HttpEntityWrapper implements com.feilong.lib.org.apache.http.HttpEntity {
  public com.feilong.lib.org.apache.http.entity.HttpEntityWrapper(com.feilong.lib.org.apache.http.HttpEntity);
  public boolean isRepeatable();
  public boolean isChunked();
  public long getContentLength();
  public com.feilong.lib.org.apache.http.Header getContentType();
  public com.feilong.lib.org.apache.http.Header getContentEncoding();
  public java.io.InputStream getContent() throws java.io.IOException;
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
  public boolean isStreaming();
}
```

## `com.feilong.lib.org.apache.http.entity.InputStreamEntity`

```java
public class com.feilong.lib.org.apache.http.entity.InputStreamEntity extends com.feilong.lib.org.apache.http.entity.AbstractHttpEntity {
  public com.feilong.lib.org.apache.http.entity.InputStreamEntity(java.io.InputStream);
  public com.feilong.lib.org.apache.http.entity.InputStreamEntity(java.io.InputStream, long);
  public com.feilong.lib.org.apache.http.entity.InputStreamEntity(java.io.InputStream, com.feilong.lib.org.apache.http.entity.ContentType);
  public com.feilong.lib.org.apache.http.entity.InputStreamEntity(java.io.InputStream, long, com.feilong.lib.org.apache.http.entity.ContentType);
  public boolean isRepeatable();
  public long getContentLength();
  public java.io.InputStream getContent() throws java.io.IOException;
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
  public boolean isStreaming();
}
```

## `com.feilong.lib.org.apache.http.entity.SerializableEntity`

```java
public class com.feilong.lib.org.apache.http.entity.SerializableEntity extends com.feilong.lib.org.apache.http.entity.AbstractHttpEntity {
  public com.feilong.lib.org.apache.http.entity.SerializableEntity(java.io.Serializable, boolean) throws java.io.IOException;
  public com.feilong.lib.org.apache.http.entity.SerializableEntity(java.io.Serializable);
  public java.io.InputStream getContent() throws java.io.IOException, java.lang.IllegalStateException;
  public long getContentLength();
  public boolean isRepeatable();
  public boolean isStreaming();
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.entity.StringEntity`

```java
public class com.feilong.lib.org.apache.http.entity.StringEntity extends com.feilong.lib.org.apache.http.entity.AbstractHttpEntity implements java.lang.Cloneable {
  public com.feilong.lib.org.apache.http.entity.StringEntity(java.lang.String, com.feilong.lib.org.apache.http.entity.ContentType) throws java.nio.charset.UnsupportedCharsetException;
  public com.feilong.lib.org.apache.http.entity.StringEntity(java.lang.String, java.lang.String) throws java.nio.charset.UnsupportedCharsetException;
  public com.feilong.lib.org.apache.http.entity.StringEntity(java.lang.String, java.nio.charset.Charset);
  public com.feilong.lib.org.apache.http.entity.StringEntity(java.lang.String) throws java.io.UnsupportedEncodingException;
  public boolean isRepeatable();
  public long getContentLength();
  public java.io.InputStream getContent() throws java.io.IOException;
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
  public boolean isStreaming();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```
