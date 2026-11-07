# com.feilong.lib.org.apache.http.client.entity

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.client.entity.DecompressingEntity`

```java
public class com.feilong.lib.org.apache.http.client.entity.DecompressingEntity extends com.feilong.lib.org.apache.http.entity.HttpEntityWrapper {
  public com.feilong.lib.org.apache.http.client.entity.DecompressingEntity(com.feilong.lib.org.apache.http.HttpEntity, com.feilong.lib.org.apache.http.client.entity.InputStreamFactory);
  public java.io.InputStream getContent() throws java.io.IOException;
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
  public com.feilong.lib.org.apache.http.Header getContentEncoding();
  public long getContentLength();
}
```

## `com.feilong.lib.org.apache.http.client.entity.DeflateDecompressingEntity`

```java
public class com.feilong.lib.org.apache.http.client.entity.DeflateDecompressingEntity extends com.feilong.lib.org.apache.http.client.entity.DecompressingEntity {
  public com.feilong.lib.org.apache.http.client.entity.DeflateDecompressingEntity(com.feilong.lib.org.apache.http.HttpEntity);
}
```

## `com.feilong.lib.org.apache.http.client.entity.DeflateInputStream`

```java
public class com.feilong.lib.org.apache.http.client.entity.DeflateInputStream extends java.io.InputStream {
  public com.feilong.lib.org.apache.http.client.entity.DeflateInputStream(java.io.InputStream) throws java.io.IOException;
  public int read() throws java.io.IOException;
  public int read(byte[]) throws java.io.IOException;
  public int read(byte[], int, int) throws java.io.IOException;
  public long skip(long) throws java.io.IOException;
  public int available() throws java.io.IOException;
  public void mark(int);
  public void reset() throws java.io.IOException;
  public boolean markSupported();
  public void close() throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.client.entity.DeflateInputStreamFactory`

```java
public class com.feilong.lib.org.apache.http.client.entity.DeflateInputStreamFactory implements com.feilong.lib.org.apache.http.client.entity.InputStreamFactory {
  public com.feilong.lib.org.apache.http.client.entity.DeflateInputStreamFactory();
  public static com.feilong.lib.org.apache.http.client.entity.DeflateInputStreamFactory getInstance();
  public java.io.InputStream create(java.io.InputStream) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.client.entity.EntityBuilder`

```java
public class com.feilong.lib.org.apache.http.client.entity.EntityBuilder {
  public static com.feilong.lib.org.apache.http.client.entity.EntityBuilder create();
  public java.lang.String getText();
  public com.feilong.lib.org.apache.http.client.entity.EntityBuilder setText(java.lang.String);
  public byte[] getBinary();
  public com.feilong.lib.org.apache.http.client.entity.EntityBuilder setBinary(byte[]);
  public java.io.InputStream getStream();
  public com.feilong.lib.org.apache.http.client.entity.EntityBuilder setStream(java.io.InputStream);
  public java.util.List<com.feilong.lib.org.apache.http.NameValuePair> getParameters();
  public com.feilong.lib.org.apache.http.client.entity.EntityBuilder setParameters(java.util.List<com.feilong.lib.org.apache.http.NameValuePair>);
  public com.feilong.lib.org.apache.http.client.entity.EntityBuilder setParameters(com.feilong.lib.org.apache.http.NameValuePair...);
  public java.io.Serializable getSerializable();
  public com.feilong.lib.org.apache.http.client.entity.EntityBuilder setSerializable(java.io.Serializable);
  public java.io.File getFile();
  public com.feilong.lib.org.apache.http.client.entity.EntityBuilder setFile(java.io.File);
  public com.feilong.lib.org.apache.http.entity.ContentType getContentType();
  public com.feilong.lib.org.apache.http.client.entity.EntityBuilder setContentType(com.feilong.lib.org.apache.http.entity.ContentType);
  public java.lang.String getContentEncoding();
  public com.feilong.lib.org.apache.http.client.entity.EntityBuilder setContentEncoding(java.lang.String);
  public boolean isChunked();
  public com.feilong.lib.org.apache.http.client.entity.EntityBuilder chunked();
  public boolean isGzipCompress();
  public com.feilong.lib.org.apache.http.client.entity.EntityBuilder gzipCompress();
  public com.feilong.lib.org.apache.http.HttpEntity build();
}
```

## `com.feilong.lib.org.apache.http.client.entity.GZIPInputStreamFactory`

```java
public class com.feilong.lib.org.apache.http.client.entity.GZIPInputStreamFactory implements com.feilong.lib.org.apache.http.client.entity.InputStreamFactory {
  public com.feilong.lib.org.apache.http.client.entity.GZIPInputStreamFactory();
  public static com.feilong.lib.org.apache.http.client.entity.GZIPInputStreamFactory getInstance();
  public java.io.InputStream create(java.io.InputStream) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.client.entity.GzipCompressingEntity`

```java
public class com.feilong.lib.org.apache.http.client.entity.GzipCompressingEntity extends com.feilong.lib.org.apache.http.entity.HttpEntityWrapper {
  public com.feilong.lib.org.apache.http.client.entity.GzipCompressingEntity(com.feilong.lib.org.apache.http.HttpEntity);
  public com.feilong.lib.org.apache.http.Header getContentEncoding();
  public long getContentLength();
  public boolean isChunked();
  public java.io.InputStream getContent() throws java.io.IOException;
  public void writeTo(java.io.OutputStream) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.client.entity.GzipDecompressingEntity`

```java
public class com.feilong.lib.org.apache.http.client.entity.GzipDecompressingEntity extends com.feilong.lib.org.apache.http.client.entity.DecompressingEntity {
  public com.feilong.lib.org.apache.http.client.entity.GzipDecompressingEntity(com.feilong.lib.org.apache.http.HttpEntity);
}
```

## `com.feilong.lib.org.apache.http.client.entity.InputStreamFactory`

```java
public interface com.feilong.lib.org.apache.http.client.entity.InputStreamFactory {
  public abstract java.io.InputStream create(java.io.InputStream) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.client.entity.UrlEncodedFormEntity`

```java
public class com.feilong.lib.org.apache.http.client.entity.UrlEncodedFormEntity extends com.feilong.lib.org.apache.http.entity.StringEntity {
  public com.feilong.lib.org.apache.http.client.entity.UrlEncodedFormEntity(java.util.List<? extends com.feilong.lib.org.apache.http.NameValuePair>, java.lang.String) throws java.io.UnsupportedEncodingException;
  public com.feilong.lib.org.apache.http.client.entity.UrlEncodedFormEntity(java.lang.Iterable<? extends com.feilong.lib.org.apache.http.NameValuePair>, java.nio.charset.Charset);
  public com.feilong.lib.org.apache.http.client.entity.UrlEncodedFormEntity(java.util.List<? extends com.feilong.lib.org.apache.http.NameValuePair>) throws java.io.UnsupportedEncodingException;
  public com.feilong.lib.org.apache.http.client.entity.UrlEncodedFormEntity(java.lang.Iterable<? extends com.feilong.lib.org.apache.http.NameValuePair>);
}
```
