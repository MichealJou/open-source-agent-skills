# com.feilong.io.entity

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.io.entity.FileInfoEntity`

```java
public class com.feilong.io.entity.FileInfoEntity implements java.io.Serializable {
  public com.feilong.io.entity.FileInfoEntity();
  public com.feilong.io.entity.FileInfoEntity(java.lang.String, com.feilong.io.entity.FileType, java.lang.Long, java.lang.Long);
  public java.lang.String getFormatLastModified();
  public java.lang.String getFormatSize();
  public java.lang.String getName();
  public void setName(java.lang.String);
  public com.feilong.io.entity.FileType getFileType();
  public void setFileType(com.feilong.io.entity.FileType);
  public java.lang.Long getSize();
  public void setSize(java.lang.Long);
  public java.lang.Long getLastModified();
  public void setLastModified(java.lang.Long);
}
```

## `com.feilong.io.entity.FileType`

```java
public final class com.feilong.io.entity.FileType extends java.lang.Enum<com.feilong.io.entity.FileType> {
  public static com.feilong.io.entity.FileType[] values();
  public static com.feilong.io.entity.FileType valueOf(java.lang.String);
}
```

## `com.feilong.io.entity.FileWriteMode`

```java
public final class com.feilong.io.entity.FileWriteMode extends java.lang.Enum<com.feilong.io.entity.FileWriteMode> {
  public static com.feilong.io.entity.FileWriteMode[] values();
  public static com.feilong.io.entity.FileWriteMode valueOf(java.lang.String);
}
```

## `com.feilong.io.entity.MimeType`

```java
public final class com.feilong.io.entity.MimeType extends java.lang.Enum<com.feilong.io.entity.MimeType> {
  public static com.feilong.io.entity.MimeType[] values();
  public static com.feilong.io.entity.MimeType valueOf(java.lang.String);
  public java.lang.String getExtension();
  public java.lang.String getMime();
}
```
