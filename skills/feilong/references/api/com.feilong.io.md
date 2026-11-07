# com.feilong.io

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.io.FileUtil`

```java
public final class com.feilong.io.FileUtil {
  public static byte[] toByteArray(java.lang.String);
  public static byte[] toByteArray(java.io.File);
  public static java.io.FileOutputStream getFileOutputStream(java.lang.String);
  public static java.io.FileOutputStream getFileOutputStream(java.lang.String, com.feilong.io.entity.FileWriteMode);
  public static java.io.FileInputStream getFileInputStream(java.lang.String);
  public static java.io.FileInputStream getFileInputStream(java.io.File);
  public static boolean isEmptyDirectory(java.lang.String);
  public static void createDirectoryByFilePath(java.lang.String);
  public static void createDirectory(java.lang.String);
  public static boolean deleteFileOrDirectory(java.lang.String);
  public static boolean deleteFileOrDirectory(java.io.File);
  public static java.lang.String getParent(java.lang.String);
  public static boolean isExistFile(java.lang.String);
  public static boolean isNotExistFile(java.lang.String);
  public static long getFileSize(java.io.File);
  public static java.lang.String getFileFormatSize(java.io.File);
  public static java.lang.String formatSize(long);
  public static java.net.URL[] toURLs(java.util.List<java.lang.String>);
  public static java.net.URL[] toURLs(java.lang.String...);
}
```

## `com.feilong.io.FilenameUtil`

```java
public final class com.feilong.io.FilenameUtil {
  public static java.lang.String getFormatFileName(java.lang.String);
  public static java.lang.String getFileName(java.lang.String);
  public static java.lang.String getFilePreName(java.lang.String);
  public static boolean isExtensionIgnoreCase(java.lang.String, java.lang.String...);
  public static java.lang.String getExtension(java.lang.String);
  public static java.lang.String getExtensionLowerCase(java.lang.String);
  public static java.lang.String getNewFileName(java.lang.String, java.lang.String);
  public static java.lang.String getFileTopParentName(java.lang.String);
  public static java.lang.String getFileTopParentName(java.io.File);
  public static java.util.List<java.lang.String> getParentPathList(java.lang.String);
}
```

## `com.feilong.io.IOReaderUtil`

```java
public final class com.feilong.io.IOReaderUtil {
  public static byte[] readToByteArray(java.lang.String);
  public static java.lang.String readToString(java.lang.String);
  public static java.lang.String readToString(java.lang.String, java.lang.String);
  public static java.lang.String readToString(java.io.File, java.lang.String);
  public static java.lang.String readToString(java.io.FileInputStream, java.lang.String);
  public static java.lang.String readToString(java.io.InputStream, java.lang.String);
  public static java.util.Set<java.lang.String> readToSet(java.lang.String);
  public static java.util.Set<java.lang.String> readToSet(java.lang.String, com.feilong.io.ReaderConfig);
  public static java.util.Set<java.lang.String> readToSet(java.io.File, com.feilong.io.ReaderConfig);
  public static java.util.Set<java.lang.String> readToSet(java.io.Reader, com.feilong.io.ReaderConfig);
  public static java.util.List<java.lang.String> readToList(java.lang.String);
  public static java.util.List<java.lang.String> readToList(java.lang.String, com.feilong.io.ReaderConfig);
  public static java.util.List<java.lang.String> readToList(java.io.File, com.feilong.io.ReaderConfig);
  public static java.util.List<java.lang.String> readToList(java.io.Reader, com.feilong.io.ReaderConfig);
  public static <T extends java.util.Collection<java.lang.String>> T readToCollection(java.io.Reader, com.feilong.io.ReaderConfig, T);
  public static void resolverFile(java.lang.String, com.feilong.io.LineNumberReaderResolver);
  public static void resolverFile(java.io.File, com.feilong.io.LineNumberReaderResolver);
  public static void resolverFile(java.io.Reader, com.feilong.io.LineNumberReaderResolver);
}
```

## `com.feilong.io.IOUtil`

```java
public final class com.feilong.io.IOUtil {
  public static void closeQuietly(java.io.Closeable...);
  public static int copy(java.io.InputStream, java.io.OutputStream) throws java.io.IOException;
}
```

## `com.feilong.io.IOWriteUtil`

```java
public final class com.feilong.io.IOWriteUtil {
  public static void writeStringToFile(java.lang.String, java.lang.String);
  public static void writeStringToFile(java.lang.String, java.lang.String, java.lang.String);
  public static void writeStringToFile(java.lang.String, java.lang.String, java.lang.String, com.feilong.io.entity.FileWriteMode);
  public static java.lang.String write(java.io.InputStream, java.lang.String, java.lang.String);
  public static void write(java.io.InputStream, java.io.OutputStream);
  public static void write(java.io.InputStream, java.io.OutputStream, int);
}
```

## `com.feilong.io.InputStreamUtil`

```java
public final class com.feilong.io.InputStreamUtil {
  public static java.io.InputStream getInputStream(java.lang.String);
  public static java.io.InputStream newByteArrayInputStream(java.lang.String, java.lang.String);
  public static java.lang.String toString(java.io.InputStream);
  public static java.lang.String toString(java.io.InputStream, java.lang.String);
  public static java.io.BufferedReader toBufferedReader(java.io.InputStream, java.lang.String);
}
```

## `com.feilong.io.LineNumberReaderResolver`

```java
public interface com.feilong.io.LineNumberReaderResolver {
  public abstract boolean resolve(int, java.lang.String);
}
```

## `com.feilong.io.MimeTypeUtil`

```java
public final class com.feilong.io.MimeTypeUtil {
  public static java.lang.String getContentTypeByFileName(java.lang.String);
}
```

## `com.feilong.io.ReaderConfig`

```java
public class com.feilong.io.ReaderConfig implements java.io.Serializable {
  public com.feilong.io.ReaderConfig();
  public com.feilong.io.ReaderConfig(java.lang.String);
  public com.feilong.io.ReaderConfig(boolean, boolean);
  public com.feilong.io.ReaderConfig(boolean, boolean, java.lang.String);
  public boolean getIgnoreBlankLine();
  public void setIgnoreBlankLine(boolean);
  public boolean getIsTrim();
  public void setIsTrim(boolean);
  public java.lang.String getRegexPattern();
  public void setRegexPattern(java.lang.String);
}
```

## `com.feilong.io.ReaderUtil`

```java
public final class com.feilong.io.ReaderUtil {
  public static java.io.StringReader newStringReader(java.lang.String);
  public static java.lang.String toString(java.io.Reader);
  public static java.lang.String readLine(java.io.Reader);
}
```
