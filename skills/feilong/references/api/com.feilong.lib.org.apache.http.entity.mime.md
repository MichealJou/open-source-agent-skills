# com.feilong.lib.org.apache.http.entity.mime

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.entity.mime.FormBodyPart`

```java
public class com.feilong.lib.org.apache.http.entity.mime.FormBodyPart {
  public com.feilong.lib.org.apache.http.entity.mime.FormBodyPart(java.lang.String, com.feilong.lib.org.apache.http.entity.mime.content.ContentBody);
  public java.lang.String getName();
  public com.feilong.lib.org.apache.http.entity.mime.content.ContentBody getBody();
  public com.feilong.lib.org.apache.http.entity.mime.Header getHeader();
  public void addField(java.lang.String, java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.entity.mime.FormBodyPartBuilder`

```java
public class com.feilong.lib.org.apache.http.entity.mime.FormBodyPartBuilder {
  public static com.feilong.lib.org.apache.http.entity.mime.FormBodyPartBuilder create(java.lang.String, com.feilong.lib.org.apache.http.entity.mime.content.ContentBody);
  public static com.feilong.lib.org.apache.http.entity.mime.FormBodyPartBuilder create();
  public com.feilong.lib.org.apache.http.entity.mime.FormBodyPartBuilder setName(java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.FormBodyPartBuilder setBody(com.feilong.lib.org.apache.http.entity.mime.content.ContentBody);
  public com.feilong.lib.org.apache.http.entity.mime.FormBodyPartBuilder addField(java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.FormBodyPartBuilder setField(java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.FormBodyPartBuilder removeFields(java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.FormBodyPart build();
}
```

## `com.feilong.lib.org.apache.http.entity.mime.Header`

```java
public class com.feilong.lib.org.apache.http.entity.mime.Header implements java.lang.Iterable<com.feilong.lib.org.apache.http.entity.mime.MinimalField> {
  public com.feilong.lib.org.apache.http.entity.mime.Header();
  public void addField(com.feilong.lib.org.apache.http.entity.mime.MinimalField);
  public java.util.List<com.feilong.lib.org.apache.http.entity.mime.MinimalField> getFields();
  public com.feilong.lib.org.apache.http.entity.mime.MinimalField getField(java.lang.String);
  public java.util.List<com.feilong.lib.org.apache.http.entity.mime.MinimalField> getFields(java.lang.String);
  public int removeFields(java.lang.String);
  public void setField(com.feilong.lib.org.apache.http.entity.mime.MinimalField);
  public java.util.Iterator<com.feilong.lib.org.apache.http.entity.mime.MinimalField> iterator();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.entity.mime.HttpMultipartMode`

```java
public final class com.feilong.lib.org.apache.http.entity.mime.HttpMultipartMode extends java.lang.Enum<com.feilong.lib.org.apache.http.entity.mime.HttpMultipartMode> {
  public static com.feilong.lib.org.apache.http.entity.mime.HttpMultipartMode[] values();
  public static com.feilong.lib.org.apache.http.entity.mime.HttpMultipartMode valueOf(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.entity.mime.MIME`

```java
public final class com.feilong.lib.org.apache.http.entity.mime.MIME {
  public com.feilong.lib.org.apache.http.entity.mime.MIME();
}
```

## `com.feilong.lib.org.apache.http.entity.mime.MinimalField`

```java
public class com.feilong.lib.org.apache.http.entity.mime.MinimalField {
  public com.feilong.lib.org.apache.http.entity.mime.MinimalField(java.lang.String, java.lang.String);
  public java.lang.String getName();
  public java.lang.String getBody();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder`

```java
public class com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder {
  public static com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder create();
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder setMode(com.feilong.lib.org.apache.http.entity.mime.HttpMultipartMode);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder setLaxMode();
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder setStrictMode();
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder setBoundary(java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder setMimeSubtype(java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder seContentType(com.feilong.lib.org.apache.http.entity.ContentType);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder setContentType(com.feilong.lib.org.apache.http.entity.ContentType);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder setCharset(java.nio.charset.Charset);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder addPart(com.feilong.lib.org.apache.http.entity.mime.FormBodyPart);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder addPart(java.lang.String, com.feilong.lib.org.apache.http.entity.mime.content.ContentBody);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder addTextBody(java.lang.String, java.lang.String, com.feilong.lib.org.apache.http.entity.ContentType);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder addTextBody(java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder addBinaryBody(java.lang.String, byte[], com.feilong.lib.org.apache.http.entity.ContentType, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder addBinaryBody(java.lang.String, byte[]);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder addBinaryBody(java.lang.String, java.io.File, com.feilong.lib.org.apache.http.entity.ContentType, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder addBinaryBody(java.lang.String, java.io.File);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder addBinaryBody(java.lang.String, java.io.InputStream, com.feilong.lib.org.apache.http.entity.ContentType, java.lang.String);
  public com.feilong.lib.org.apache.http.entity.mime.MultipartEntityBuilder addBinaryBody(java.lang.String, java.io.InputStream);
  public com.feilong.lib.org.apache.http.HttpEntity build();
}
```
