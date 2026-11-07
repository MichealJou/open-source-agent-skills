# com.feilong.lib.io

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.io.Charsets`

```java
public class com.feilong.lib.io.Charsets {
  public com.feilong.lib.io.Charsets();
  public static java.util.SortedMap<java.lang.String, java.nio.charset.Charset> requiredCharsets();
  public static java.nio.charset.Charset toCharset(java.nio.charset.Charset);
  public static java.nio.charset.Charset toCharset(java.lang.String);
}
```

## `com.feilong.lib.io.FileUtils`

```java
public class com.feilong.lib.io.FileUtils {
  public com.feilong.lib.io.FileUtils();
  public static java.io.File getFile(java.io.File, java.lang.String...);
  public static java.io.File getFile(java.lang.String...);
  public static byte[] readFileToByteArray(java.io.File) throws java.io.IOException;
  public static java.lang.String getTempDirectoryPath();
  public static java.lang.String getUserDirectoryPath();
  public static java.io.File getUserDirectory();
  public static java.io.FileInputStream openInputStream(java.io.File) throws java.io.IOException;
  public static java.io.FileOutputStream openOutputStream(java.io.File) throws java.io.IOException;
  public static java.io.FileOutputStream openOutputStream(java.io.File, boolean) throws java.io.IOException;
  public static java.io.File toFile(java.net.URL);
  public static java.io.File[] toFiles(java.net.URL[]);
  public static java.net.URL[] toURLs(java.io.File[]) throws java.io.IOException;
  public static void deleteDirectory(java.io.File) throws java.io.IOException;
  public static boolean deleteQuietly(java.io.File);
  public static void cleanDirectory(java.io.File) throws java.io.IOException;
  public static void writeStringToFile(java.io.File, java.lang.String, java.nio.charset.Charset, boolean) throws java.io.IOException;
  public static void writeStringToFile(java.io.File, java.lang.String, java.lang.String, boolean) throws java.io.IOException;
  public static void write(java.io.File, java.lang.CharSequence, java.nio.charset.Charset) throws java.io.IOException;
  public static void write(java.io.File, java.lang.CharSequence, java.nio.charset.Charset, boolean) throws java.io.IOException;
  public static void writeLines(java.io.File, java.lang.String, java.util.Collection<?>) throws java.io.IOException;
  public static void writeLines(java.io.File, java.lang.String, java.util.Collection<?>, boolean) throws java.io.IOException;
  public static void writeLines(java.io.File, java.util.Collection<?>) throws java.io.IOException;
  public static void writeLines(java.io.File, java.util.Collection<?>, boolean) throws java.io.IOException;
  public static void writeLines(java.io.File, java.lang.String, java.util.Collection<?>, java.lang.String) throws java.io.IOException;
  public static void writeLines(java.io.File, java.lang.String, java.util.Collection<?>, java.lang.String, boolean) throws java.io.IOException;
  public static void writeLines(java.io.File, java.util.Collection<?>, java.lang.String) throws java.io.IOException;
  public static void writeLines(java.io.File, java.util.Collection<?>, java.lang.String, boolean) throws java.io.IOException;
  public static void forceDelete(java.io.File) throws java.io.IOException;
  public static void forceMkdir(java.io.File) throws java.io.IOException;
  public static long sizeOf(java.io.File);
  public static long sizeOfDirectory(java.io.File);
  public static boolean isSymlink(java.io.File) throws java.io.IOException;
}
```

## `com.feilong.lib.io.FilenameUtils`

```java
public class com.feilong.lib.io.FilenameUtils {
  public com.feilong.lib.io.FilenameUtils();
  public static int indexOfLastSeparator(java.lang.String);
  public static int indexOfExtension(java.lang.String);
  public static java.lang.String getName(java.lang.String);
  public static java.lang.String getExtension(java.lang.String);
  public static boolean isExtension(java.lang.String, java.lang.String...);
}
```

## `com.feilong.lib.io.IOUtils`

```java
public class com.feilong.lib.io.IOUtils {
  public com.feilong.lib.io.IOUtils();
  public static byte[] toByteArray(java.io.InputStream) throws java.io.IOException;
  public static int copy(java.io.InputStream, java.io.OutputStream) throws java.io.IOException;
  public static long copyLarge(java.io.InputStream, java.io.OutputStream) throws java.io.IOException;
  public static long copy(java.io.InputStream, java.io.OutputStream, int) throws java.io.IOException;
  public static long copyLarge(java.io.InputStream, java.io.OutputStream, byte[]) throws java.io.IOException;
  public static java.io.BufferedReader toBufferedReader(java.io.Reader);
  public static byte[] toByteArray(java.io.InputStream, int) throws java.io.IOException;
  public static java.lang.String toString(java.io.Reader) throws java.io.IOException;
  public static int copy(java.io.Reader, java.io.Writer) throws java.io.IOException;
  public static long copyLarge(java.io.Reader, java.io.Writer) throws java.io.IOException;
  public static long copyLarge(java.io.Reader, java.io.Writer, char[]) throws java.io.IOException;
  public static void write(byte[], java.io.Writer, java.nio.charset.Charset) throws java.io.IOException;
  public static void write(java.lang.String, java.io.OutputStream, java.nio.charset.Charset) throws java.io.IOException;
  public static void writeLines(java.util.Collection<?>, java.lang.String, java.io.OutputStream, java.nio.charset.Charset) throws java.io.IOException;
  public static void writeLines(java.util.Collection<?>, java.lang.String, java.io.OutputStream, java.lang.String) throws java.io.IOException;
}
```
