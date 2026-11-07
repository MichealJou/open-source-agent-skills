# com.feilong.zip

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.zip.AbstractUnzipHandler`

```java
public abstract class com.feilong.zip.AbstractUnzipHandler implements com.feilong.zip.UnzipHandler {
  public com.feilong.zip.AbstractUnzipHandler();
  public void unzip(java.lang.String, java.lang.String);
}
```

## `com.feilong.zip.AbstractZipHandler`

```java
public abstract class com.feilong.zip.AbstractZipHandler implements com.feilong.zip.ZipHandler {
  public com.feilong.zip.AbstractZipHandler();
  public void zip(java.lang.String, java.lang.String);
}
```

## `com.feilong.zip.CompressUnzipHandler`

```java
public class com.feilong.zip.CompressUnzipHandler extends com.feilong.zip.AbstractUnzipHandler {
  public com.feilong.zip.CompressUnzipHandler();
}
```

## `com.feilong.zip.CompressZipHandler`

```java
public class com.feilong.zip.CompressZipHandler extends com.feilong.zip.AbstractZipHandler {
  public com.feilong.zip.CompressZipHandler();
}
```

## `com.feilong.zip.UnzipHandler`

```java
public interface com.feilong.zip.UnzipHandler {
  public abstract void unzip(java.lang.String, java.lang.String);
}
```

## `com.feilong.zip.ZipHandler`

```java
public interface com.feilong.zip.ZipHandler {
  public abstract void zip(java.lang.String, java.lang.String);
}
```
