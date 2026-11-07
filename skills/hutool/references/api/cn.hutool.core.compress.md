# cn.hutool.core.compress

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.compress.Deflate`

```java
public class cn.hutool.core.compress.Deflate implements java.io.Closeable {
  public static cn.hutool.core.compress.Deflate of(java.io.InputStream, java.io.OutputStream, boolean);
  public cn.hutool.core.compress.Deflate(java.io.InputStream, java.io.OutputStream, boolean);
  public java.io.OutputStream getTarget();
  public cn.hutool.core.compress.Deflate deflater(int);
  public cn.hutool.core.compress.Deflate inflater();
  public void close();
}
```

## `cn.hutool.core.compress.Gzip`

```java
public class cn.hutool.core.compress.Gzip implements java.io.Closeable {
  public static cn.hutool.core.compress.Gzip of(java.io.InputStream, java.io.OutputStream);
  public cn.hutool.core.compress.Gzip(java.io.InputStream, java.io.OutputStream);
  public java.io.OutputStream getTarget();
  public cn.hutool.core.compress.Gzip gzip();
  public cn.hutool.core.compress.Gzip unGzip();
  public void close();
}
```

## `cn.hutool.core.compress.ZipCopyVisitor`

```java
public class cn.hutool.core.compress.ZipCopyVisitor extends java.nio.file.SimpleFileVisitor<java.nio.file.Path> {
  public cn.hutool.core.compress.ZipCopyVisitor(java.nio.file.Path, java.nio.file.FileSystem, java.nio.file.CopyOption...);
  public java.nio.file.FileVisitResult preVisitDirectory(java.nio.file.Path, java.nio.file.attribute.BasicFileAttributes) throws java.io.IOException;
  public java.nio.file.FileVisitResult visitFile(java.nio.file.Path, java.nio.file.attribute.BasicFileAttributes) throws java.io.IOException;
  public java.nio.file.FileVisitResult visitFile(java.lang.Object, java.nio.file.attribute.BasicFileAttributes) throws java.io.IOException;
  public java.nio.file.FileVisitResult preVisitDirectory(java.lang.Object, java.nio.file.attribute.BasicFileAttributes) throws java.io.IOException;
}
```

## `cn.hutool.core.compress.ZipReader`

```java
public class cn.hutool.core.compress.ZipReader implements java.io.Closeable {
  public static cn.hutool.core.compress.ZipReader of(java.io.File, java.nio.charset.Charset);
  public static cn.hutool.core.compress.ZipReader of(java.io.InputStream, java.nio.charset.Charset);
  public cn.hutool.core.compress.ZipReader(java.io.File, java.nio.charset.Charset);
  public cn.hutool.core.compress.ZipReader(java.util.zip.ZipFile);
  public cn.hutool.core.compress.ZipReader(java.io.InputStream, java.nio.charset.Charset);
  public cn.hutool.core.compress.ZipReader(java.util.zip.ZipInputStream);
  public cn.hutool.core.compress.ZipReader setMaxSizeDiff(int);
  public java.io.InputStream get(java.lang.String);
  public java.io.File readTo(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public java.io.File readTo(java.io.File, cn.hutool.core.lang.Filter<java.util.zip.ZipEntry>) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.compress.ZipReader read(java.util.function.Consumer<java.util.zip.ZipEntry>) throws cn.hutool.core.io.IORuntimeException;
  public void close() throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.core.compress.ZipWriter`

```java
public class cn.hutool.core.compress.ZipWriter implements java.io.Closeable {
  public static cn.hutool.core.compress.ZipWriter of(java.io.File, java.nio.charset.Charset);
  public static cn.hutool.core.compress.ZipWriter of(java.io.OutputStream, java.nio.charset.Charset);
  public cn.hutool.core.compress.ZipWriter(java.io.File, java.nio.charset.Charset);
  public cn.hutool.core.compress.ZipWriter(java.io.OutputStream, java.nio.charset.Charset);
  public cn.hutool.core.compress.ZipWriter(java.util.zip.ZipOutputStream);
  public cn.hutool.core.compress.ZipWriter setLevel(int);
  public cn.hutool.core.compress.ZipWriter setComment(java.lang.String);
  public java.util.zip.ZipOutputStream getOut();
  public cn.hutool.core.compress.ZipWriter add(boolean, java.io.FileFilter, java.io.File...) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.compress.ZipWriter add(cn.hutool.core.io.resource.Resource...) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.compress.ZipWriter add(java.lang.String, java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.compress.ZipWriter add(java.lang.String[], java.io.InputStream[]) throws cn.hutool.core.io.IORuntimeException;
  public void close() throws cn.hutool.core.io.IORuntimeException;
}
```
