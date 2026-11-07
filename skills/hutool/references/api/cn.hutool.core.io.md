# cn.hutool.core.io

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.io.AppendableWriter`

```java
public class cn.hutool.core.io.AppendableWriter extends java.io.Writer implements java.lang.Appendable {
  public cn.hutool.core.io.AppendableWriter(java.lang.Appendable);
  public void write(char[], int, int) throws java.io.IOException;
  public void write(int) throws java.io.IOException;
  public java.io.Writer append(char) throws java.io.IOException;
  public java.io.Writer append(java.lang.CharSequence, int, int) throws java.io.IOException;
  public java.io.Writer append(java.lang.CharSequence) throws java.io.IOException;
  public void write(java.lang.String, int, int) throws java.io.IOException;
  public void write(java.lang.String) throws java.io.IOException;
  public void write(char[]) throws java.io.IOException;
  public void flush() throws java.io.IOException;
  public void close() throws java.io.IOException;
  public java.lang.Appendable append(char) throws java.io.IOException;
  public java.lang.Appendable append(java.lang.CharSequence, int, int) throws java.io.IOException;
  public java.lang.Appendable append(java.lang.CharSequence) throws java.io.IOException;
}
```

## `cn.hutool.core.io.BOMInputStream`

```java
public class cn.hutool.core.io.BOMInputStream extends java.io.InputStream {
  public cn.hutool.core.io.BOMInputStream(java.io.InputStream);
  public cn.hutool.core.io.BOMInputStream(java.io.InputStream, java.lang.String);
  public java.lang.String getDefaultCharset();
  public java.lang.String getCharset();
  public void close() throws java.io.IOException;
  public int read() throws java.io.IOException;
}
```

## `cn.hutool.core.io.BomReader`

```java
public class cn.hutool.core.io.BomReader extends java.io.Reader {
  public cn.hutool.core.io.BomReader(java.io.InputStream);
  public int read(char[], int, int) throws java.io.IOException;
  public void close() throws java.io.IOException;
}
```

## `cn.hutool.core.io.BufferUtil`

```java
public class cn.hutool.core.io.BufferUtil {
  public cn.hutool.core.io.BufferUtil();
  public static java.nio.ByteBuffer copy(java.nio.ByteBuffer, int, int);
  public static java.nio.ByteBuffer copy(java.nio.ByteBuffer, java.nio.ByteBuffer);
  public static java.nio.ByteBuffer copy(java.nio.ByteBuffer, java.nio.ByteBuffer, int);
  public static java.nio.ByteBuffer copy(java.nio.ByteBuffer, int, java.nio.ByteBuffer, int, int);
  public static java.lang.String readUtf8Str(java.nio.ByteBuffer);
  public static java.lang.String readStr(java.nio.ByteBuffer, java.nio.charset.Charset);
  public static byte[] readBytes(java.nio.ByteBuffer);
  public static byte[] readBytes(java.nio.ByteBuffer, int);
  public static byte[] readBytes(java.nio.ByteBuffer, int, int);
  public static int lineEnd(java.nio.ByteBuffer);
  public static int lineEnd(java.nio.ByteBuffer, int);
  public static java.lang.String readLine(java.nio.ByteBuffer, java.nio.charset.Charset);
  public static java.nio.ByteBuffer create(byte[]);
  public static java.nio.ByteBuffer create(java.lang.CharSequence, java.nio.charset.Charset);
  public static java.nio.ByteBuffer createUtf8(java.lang.CharSequence);
  public static java.nio.CharBuffer createCharBuffer(int);
}
```

## `cn.hutool.core.io.CharsetDetector`

```java
public class cn.hutool.core.io.CharsetDetector {
  public cn.hutool.core.io.CharsetDetector();
  public static java.nio.charset.Charset detect(java.io.File, java.nio.charset.Charset...);
  public static java.nio.charset.Charset detect(java.io.InputStream, java.nio.charset.Charset...);
  public static java.nio.charset.Charset detect(int, java.io.InputStream, java.nio.charset.Charset...);
}
```

## `cn.hutool.core.io.FastByteArrayOutputStream`

```java
public class cn.hutool.core.io.FastByteArrayOutputStream extends java.io.OutputStream {
  public cn.hutool.core.io.FastByteArrayOutputStream();
  public cn.hutool.core.io.FastByteArrayOutputStream(int);
  public void write(byte[], int, int);
  public void write(int);
  public int size();
  public void close();
  public void reset();
  public void writeTo(java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public byte[] toByteArray();
  public java.lang.String toString();
  public java.lang.String toString(java.lang.String);
  public java.lang.String toString(java.nio.charset.Charset);
}
```

## `cn.hutool.core.io.FastByteBuffer`

```java
public class cn.hutool.core.io.FastByteBuffer {
  public cn.hutool.core.io.FastByteBuffer();
  public cn.hutool.core.io.FastByteBuffer(int);
  public cn.hutool.core.io.FastByteBuffer append(byte[], int, int);
  public cn.hutool.core.io.FastByteBuffer append(byte[]);
  public cn.hutool.core.io.FastByteBuffer append(byte);
  public cn.hutool.core.io.FastByteBuffer append(cn.hutool.core.io.FastByteBuffer);
  public int size();
  public boolean isEmpty();
  public int index();
  public int offset();
  public byte[] array(int);
  public void reset();
  public byte[] toArray();
  public byte[] toArray(int, int);
  public byte get(int);
}
```

## `cn.hutool.core.io.FastStringWriter`

```java
public final class cn.hutool.core.io.FastStringWriter extends java.io.Writer {
  public cn.hutool.core.io.FastStringWriter();
  public cn.hutool.core.io.FastStringWriter(int);
  public void write(int);
  public void write(java.lang.String);
  public void write(java.lang.String, int, int);
  public void write(char[]);
  public void write(char[], int, int);
  public void flush();
  public void close();
  public java.lang.String toString();
}
```

## `cn.hutool.core.io.FileMagicNumber`

```java
public abstract class cn.hutool.core.io.FileMagicNumber extends java.lang.Enum<cn.hutool.core.io.FileMagicNumber> {
  public static cn.hutool.core.io.FileMagicNumber[] values();
  public static cn.hutool.core.io.FileMagicNumber valueOf(java.lang.String);
  public static cn.hutool.core.io.FileMagicNumber getMagicNumber(byte[]);
  public java.lang.String getMimeType();
  public java.lang.String getExtension();
  public abstract boolean match(byte[]);
}
```

## `cn.hutool.core.io.FileTypeUtil`

```java
public class cn.hutool.core.io.FileTypeUtil {
  public cn.hutool.core.io.FileTypeUtil();
  public static java.lang.String putFileType(java.lang.String, java.lang.String);
  public static java.lang.String removeFileType(java.lang.String);
  public static java.lang.String getType(java.lang.String);
  public static java.lang.String getType(java.io.InputStream, int) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String getType(java.io.InputStream, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String getType(java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String getType(java.io.InputStream, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String getType(java.io.InputStream, java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String getType(java.io.File, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String getType(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String getTypeByPath(java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String getTypeByPath(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.core.io.FileUtil`

```java
public class cn.hutool.core.io.FileUtil extends cn.hutool.core.io.file.PathUtil {
  public cn.hutool.core.io.FileUtil();
  public static boolean isWindows();
  public static java.io.File[] ls(java.lang.String);
  public static boolean isEmpty(java.io.File);
  public static boolean isNotEmpty(java.io.File);
  public static boolean isDirEmpty(java.io.File);
  public static java.util.List<java.io.File> loopFiles(java.lang.String, java.io.FileFilter);
  public static java.util.List<java.io.File> loopFiles(java.io.File, java.io.FileFilter);
  public static void walkFiles(java.io.File, java.util.function.Consumer<java.io.File>);
  public static java.util.List<java.io.File> loopFiles(java.io.File, int, java.io.FileFilter);
  public static java.util.List<java.io.File> loopFiles(java.lang.String);
  public static java.util.List<java.io.File> loopFiles(java.io.File);
  public static java.util.List<java.lang.String> listFileNames(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File newFile(java.lang.String);
  public static java.io.File file(java.lang.String);
  public static java.io.File file(java.lang.String, java.lang.String);
  public static java.io.File file(java.io.File, java.lang.String);
  public static java.io.File file(java.io.File, java.lang.String...);
  public static java.io.File file(java.lang.String...);
  public static java.io.File file(java.net.URI);
  public static java.io.File file(java.net.URL);
  public static java.lang.String getTmpDirPath();
  public static java.io.File getTmpDir();
  public static java.lang.String getUserHomePath();
  public static java.io.File getUserHomeDir();
  public static boolean exist(java.lang.String);
  public static boolean exist(java.io.File);
  public static boolean exist(java.lang.String, java.lang.String);
  public static java.util.Date lastModifiedTime(java.io.File);
  public static java.util.Date lastModifiedTime(java.lang.String);
  public static long size(java.io.File);
  public static long size(java.io.File, boolean);
  public static int getTotalLines(java.io.File);
  public static int getTotalLines(java.io.File, int);
  public static int getTotalLines(java.io.File, int, boolean);
  public static boolean newerThan(java.io.File, java.io.File);
  public static boolean newerThan(java.io.File, long);
  public static java.io.File touch(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File touch(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File touch(java.io.File, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File touch(java.lang.String, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File mkParentDirs(java.io.File);
  public static java.io.File mkParentDirs(java.lang.String);
  public static boolean del(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static boolean del(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static boolean clean(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static boolean clean(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static boolean cleanEmpty(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File mkdir(java.lang.String);
  public static java.io.File mkdir(java.io.File);
  public static boolean mkdirsSafely(java.io.File, int, long);
  public static java.io.File createTempFile(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File createTempFile() throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File createTempFile(java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File createTempFile(java.lang.String, java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File createTempFile(java.io.File, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File createTempFile(java.lang.String, java.lang.String, java.io.File, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File copyFile(java.lang.String, java.lang.String, java.nio.file.StandardCopyOption...) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File copyFile(cn.hutool.core.io.resource.Resource, java.io.File, java.nio.file.StandardCopyOption...) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File copyFile(java.io.InputStream, java.io.File, java.nio.file.StandardCopyOption...) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File copyFile(java.io.File, java.io.File, java.nio.file.StandardCopyOption...) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File copy(java.lang.String, java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File copy(java.io.File, java.io.File, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File copyContent(java.io.File, java.io.File, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File copyFilesFromDir(java.io.File, java.io.File, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static void move(java.io.File, java.io.File, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static void moveContent(java.io.File, java.io.File, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File rename(java.io.File, java.lang.String, boolean);
  public static java.io.File rename(java.io.File, java.lang.String, boolean, boolean);
  public static java.lang.String getCanonicalPath(java.io.File);
  public static java.lang.String getAbsolutePath(java.lang.String, java.lang.Class<?>);
  public static java.lang.String getAbsolutePath(java.lang.String);
  public static java.lang.String getAbsolutePath(java.io.File);
  public static boolean isAbsolutePath(java.lang.String);
  public static boolean isDirectory(java.lang.String);
  public static boolean isDirectory(java.io.File);
  public static boolean isFile(java.lang.String);
  public static boolean isFile(java.io.File);
  public static boolean equals(java.io.File, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static boolean contentEquals(java.io.File, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static boolean contentEqualsIgnoreEOL(java.io.File, java.io.File, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static boolean pathEquals(java.io.File, java.io.File);
  public static int lastIndexOfSeparator(java.lang.String);
  public static boolean isModifed(java.io.File, long);
  public static boolean isModified(java.io.File, long);
  public static java.lang.String normalize(java.lang.String);
  public static java.lang.String subPath(java.lang.String, java.io.File);
  public static java.lang.String subPath(java.lang.String, java.lang.String);
  public static java.lang.String getName(java.io.File);
  public static java.lang.String getName(java.lang.String);
  public static java.lang.String getSuffix(java.io.File);
  public static java.lang.String getSuffix(java.lang.String);
  public static java.lang.String getPrefix(java.io.File);
  public static java.lang.String getPrefix(java.lang.String);
  public static java.lang.String mainName(java.io.File);
  public static java.lang.String mainName(java.lang.String);
  public static java.lang.String extName(java.io.File);
  public static java.lang.String extName(java.lang.String);
  public static boolean pathEndsWith(java.io.File, java.lang.String);
  public static java.lang.String getType(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedInputStream getInputStream(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedInputStream getInputStream(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static cn.hutool.core.io.BOMInputStream getBOMInputStream(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedReader getBOMReader(java.io.File);
  public static java.io.BufferedReader getUtf8Reader(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedReader getUtf8Reader(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedReader getReader(java.io.File, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedReader getReader(java.io.File, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedReader getReader(java.lang.String, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedReader getReader(java.lang.String, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static byte[] readBytes(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static byte[] readBytes(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String readUtf8String(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String readUtf8String(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String readString(java.io.File, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String readString(java.io.File, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String readString(java.lang.String, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String readString(java.lang.String, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String readString(java.net.URL, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String readString(java.net.URL, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static <T extends java.util.Collection<java.lang.String>> T readUtf8Lines(java.lang.String, T) throws cn.hutool.core.io.IORuntimeException;
  public static <T extends java.util.Collection<java.lang.String>> T readLines(java.lang.String, java.lang.String, T) throws cn.hutool.core.io.IORuntimeException;
  public static <T extends java.util.Collection<java.lang.String>> T readLines(java.lang.String, java.nio.charset.Charset, T) throws cn.hutool.core.io.IORuntimeException;
  public static <T extends java.util.Collection<java.lang.String>> T readUtf8Lines(java.io.File, T) throws cn.hutool.core.io.IORuntimeException;
  public static <T extends java.util.Collection<java.lang.String>> T readLines(java.io.File, java.lang.String, T) throws cn.hutool.core.io.IORuntimeException;
  public static <T extends java.util.Collection<java.lang.String>> T readLines(java.io.File, java.nio.charset.Charset, T) throws cn.hutool.core.io.IORuntimeException;
  public static <T extends java.util.Collection<java.lang.String>> T readUtf8Lines(java.net.URL, T) throws cn.hutool.core.io.IORuntimeException;
  public static <T extends java.util.Collection<java.lang.String>> T readLines(java.net.URL, java.lang.String, T) throws cn.hutool.core.io.IORuntimeException;
  public static <T extends java.util.Collection<java.lang.String>> T readLines(java.net.URL, java.nio.charset.Charset, T) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.lang.String> readUtf8Lines(java.net.URL) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.lang.String> readLines(java.net.URL, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.lang.String> readLines(java.net.URL, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.lang.String> readUtf8Lines(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.lang.String> readLines(java.lang.String, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.lang.String> readLines(java.lang.String, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.lang.String> readUtf8Lines(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.lang.String> readUtf8Lines(java.io.File, java.util.function.Predicate<java.lang.String>) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.lang.String> readLines(java.io.File, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.lang.String> readLines(java.io.File, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.List<java.lang.String> readLines(java.io.File, java.nio.charset.Charset, java.util.function.Predicate<java.lang.String>) throws cn.hutool.core.io.IORuntimeException;
  public static void readUtf8Lines(java.io.File, cn.hutool.core.io.LineHandler) throws cn.hutool.core.io.IORuntimeException;
  public static void readLines(java.io.File, java.nio.charset.Charset, cn.hutool.core.io.LineHandler) throws cn.hutool.core.io.IORuntimeException;
  public static void readLines(java.io.RandomAccessFile, java.nio.charset.Charset, cn.hutool.core.io.LineHandler);
  public static void readLine(java.io.RandomAccessFile, java.nio.charset.Charset, cn.hutool.core.io.LineHandler);
  public static java.lang.String readLine(java.io.RandomAccessFile, java.nio.charset.Charset);
  public static <T> T loadUtf8(java.lang.String, cn.hutool.core.io.file.FileReader$ReaderHandler<T>) throws cn.hutool.core.io.IORuntimeException;
  public static <T> T load(java.lang.String, java.lang.String, cn.hutool.core.io.file.FileReader$ReaderHandler<T>) throws cn.hutool.core.io.IORuntimeException;
  public static <T> T load(java.lang.String, java.nio.charset.Charset, cn.hutool.core.io.file.FileReader$ReaderHandler<T>) throws cn.hutool.core.io.IORuntimeException;
  public static <T> T loadUtf8(java.io.File, cn.hutool.core.io.file.FileReader$ReaderHandler<T>) throws cn.hutool.core.io.IORuntimeException;
  public static <T> T load(java.io.File, java.nio.charset.Charset, cn.hutool.core.io.file.FileReader$ReaderHandler<T>) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedOutputStream getOutputStream(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedOutputStream getOutputStream(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedWriter getWriter(java.lang.String, java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedWriter getWriter(java.lang.String, java.nio.charset.Charset, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedWriter getWriter(java.io.File, java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedWriter getWriter(java.io.File, java.nio.charset.Charset, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.PrintWriter getPrintWriter(java.lang.String, java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.PrintWriter getPrintWriter(java.lang.String, java.nio.charset.Charset, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.PrintWriter getPrintWriter(java.io.File, java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.PrintWriter getPrintWriter(java.io.File, java.nio.charset.Charset, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String getLineSeparator();
  public static java.io.File writeUtf8String(java.lang.String, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File writeUtf8String(java.lang.String, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File writeString(java.lang.String, java.lang.String, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File writeString(java.lang.String, java.lang.String, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File writeString(java.lang.String, java.io.File, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File writeString(java.lang.String, java.io.File, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File appendUtf8String(java.lang.String, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File appendString(java.lang.String, java.lang.String, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File appendString(java.lang.String, java.lang.String, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File appendUtf8String(java.lang.String, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File appendString(java.lang.String, java.io.File, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File appendString(java.lang.String, java.io.File, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File writeUtf8Lines(java.util.Collection<T>, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File writeUtf8Lines(java.util.Collection<T>, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File writeLines(java.util.Collection<T>, java.lang.String, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File writeLines(java.util.Collection<T>, java.lang.String, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File writeLines(java.util.Collection<T>, java.io.File, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File writeLines(java.util.Collection<T>, java.io.File, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File appendUtf8Lines(java.util.Collection<T>, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File appendUtf8Lines(java.util.Collection<T>, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File appendLines(java.util.Collection<T>, java.lang.String, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File appendLines(java.util.Collection<T>, java.io.File, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File appendLines(java.util.Collection<T>, java.lang.String, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File appendLines(java.util.Collection<T>, java.io.File, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File writeLines(java.util.Collection<T>, java.lang.String, java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File writeLines(java.util.Collection<T>, java.lang.String, java.nio.charset.Charset, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File writeLines(java.util.Collection<T>, java.io.File, java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static <T> java.io.File writeLines(java.util.Collection<T>, java.io.File, java.nio.charset.Charset, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File writeUtf8Map(java.util.Map<?, ?>, java.io.File, java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File writeMap(java.util.Map<?, ?>, java.io.File, java.nio.charset.Charset, java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File writeBytes(byte[], java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File writeBytes(byte[], java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File writeBytes(byte[], java.io.File, int, int, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File writeFromStream(java.io.InputStream, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File writeFromStream(java.io.InputStream, java.io.File, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File writeFromStream(java.io.InputStream, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static long writeToStream(java.io.File, java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static long writeToStream(java.lang.String, java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String readableFileSize(java.io.File);
  public static java.lang.String readableFileSize(long);
  public static java.io.File convertCharset(java.io.File, java.nio.charset.Charset, java.nio.charset.Charset);
  public static java.io.File convertLineSeparator(java.io.File, java.nio.charset.Charset, cn.hutool.core.io.file.LineSeparator);
  public static java.lang.String cleanInvalid(java.lang.String);
  public static boolean containsInvalid(java.lang.String);
  public static long checksumCRC32(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.zip.Checksum checksum(java.io.File, java.util.zip.Checksum) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.File getWebRoot();
  public static java.lang.String getParent(java.lang.String, int);
  public static java.io.File getParent(java.io.File, int);
  public static java.io.File checkSlip(java.io.File, java.io.File) throws java.lang.IllegalArgumentException;
  public static java.lang.String getMimeType(java.lang.String);
  public static boolean isSymlink(java.io.File);
  public static boolean isSub(java.io.File, java.io.File);
  public static java.io.RandomAccessFile createRandomAccessFile(java.nio.file.Path, cn.hutool.core.io.file.FileMode);
  public static java.io.RandomAccessFile createRandomAccessFile(java.io.File, cn.hutool.core.io.file.FileMode);
  public static void tail(java.io.File, cn.hutool.core.io.LineHandler);
  public static void tail(java.io.File, java.nio.charset.Charset, cn.hutool.core.io.LineHandler);
  public static void tail(java.io.File, java.nio.charset.Charset);
}
```

## `cn.hutool.core.io.IORuntimeException`

```java
public class cn.hutool.core.io.IORuntimeException extends java.lang.RuntimeException {
  public cn.hutool.core.io.IORuntimeException(java.lang.Throwable);
  public cn.hutool.core.io.IORuntimeException(java.lang.String);
  public cn.hutool.core.io.IORuntimeException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.io.IORuntimeException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.io.IORuntimeException(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public boolean causeInstanceOf(java.lang.Class<? extends java.lang.Throwable>);
}
```

## `cn.hutool.core.io.IoUtil`

```java
public class cn.hutool.core.io.IoUtil extends cn.hutool.core.io.NioUtil {
  public cn.hutool.core.io.IoUtil();
  public static long copy(java.io.Reader, java.io.Writer) throws cn.hutool.core.io.IORuntimeException;
  public static long copy(java.io.Reader, java.io.Writer, int) throws cn.hutool.core.io.IORuntimeException;
  public static long copy(java.io.Reader, java.io.Writer, int, cn.hutool.core.io.StreamProgress) throws cn.hutool.core.io.IORuntimeException;
  public static long copy(java.io.Reader, java.io.Writer, int, long, cn.hutool.core.io.StreamProgress) throws cn.hutool.core.io.IORuntimeException;
  public static long copy(java.io.InputStream, java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static long copy(java.io.InputStream, java.io.OutputStream, int) throws cn.hutool.core.io.IORuntimeException;
  public static long copy(java.io.InputStream, java.io.OutputStream, int, cn.hutool.core.io.StreamProgress) throws cn.hutool.core.io.IORuntimeException;
  public static long copy(java.io.InputStream, java.io.OutputStream, int, long, cn.hutool.core.io.StreamProgress) throws cn.hutool.core.io.IORuntimeException;
  public static long copy(java.io.FileInputStream, java.io.FileOutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedReader getUtf8Reader(java.io.InputStream);
  public static java.io.BufferedReader getReader(java.io.InputStream, java.lang.String);
  public static java.io.BufferedReader getReader(cn.hutool.core.io.BOMInputStream);
  public static cn.hutool.core.io.BomReader getBomReader(java.io.InputStream);
  public static java.io.BufferedReader getReader(java.io.InputStream, java.nio.charset.Charset);
  public static java.io.BufferedReader getReader(java.io.Reader);
  public static java.io.PushbackReader getPushBackReader(java.io.Reader, int);
  public static java.io.OutputStreamWriter getUtf8Writer(java.io.OutputStream);
  public static java.io.OutputStreamWriter getWriter(java.io.OutputStream, java.lang.String);
  public static java.io.OutputStreamWriter getWriter(java.io.OutputStream, java.nio.charset.Charset);
  public static java.lang.String readUtf8(java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String read(java.io.InputStream, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String read(java.io.InputStream, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static cn.hutool.core.io.FastByteArrayOutputStream read(java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public static cn.hutool.core.io.FastByteArrayOutputStream read(java.io.InputStream, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String read(java.io.Reader) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String read(java.io.Reader, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static byte[] readBytes(java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public static byte[] readBytes(java.io.InputStream, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static byte[] readBytes(java.io.InputStream, int) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String readHex(java.io.InputStream, int, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String readHex64Upper(java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String readHex8192Upper(java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String readHex64Lower(java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public static <T> T readObj(java.io.InputStream) throws cn.hutool.core.io.IORuntimeException, cn.hutool.core.exceptions.UtilException;
  public static <T> T readObj(java.io.InputStream, java.lang.Class<T>) throws cn.hutool.core.io.IORuntimeException, cn.hutool.core.exceptions.UtilException;
  public static <T> T readObj(cn.hutool.core.io.ValidateObjectInputStream, java.lang.Class<T>) throws cn.hutool.core.io.IORuntimeException, cn.hutool.core.exceptions.UtilException;
  public static <T extends java.util.Collection<java.lang.String>> T readUtf8Lines(java.io.InputStream, T) throws cn.hutool.core.io.IORuntimeException;
  public static <T extends java.util.Collection<java.lang.String>> T readLines(java.io.InputStream, java.lang.String, T) throws cn.hutool.core.io.IORuntimeException;
  public static <T extends java.util.Collection<java.lang.String>> T readLines(java.io.InputStream, java.nio.charset.Charset, T) throws cn.hutool.core.io.IORuntimeException;
  public static <T extends java.util.Collection<java.lang.String>> T readLines(java.io.Reader, T) throws cn.hutool.core.io.IORuntimeException;
  public static void readUtf8Lines(java.io.InputStream, cn.hutool.core.io.LineHandler) throws cn.hutool.core.io.IORuntimeException;
  public static void readLines(java.io.InputStream, java.nio.charset.Charset, cn.hutool.core.io.LineHandler) throws cn.hutool.core.io.IORuntimeException;
  public static void readLines(java.io.Reader, cn.hutool.core.io.LineHandler) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.ByteArrayInputStream toStream(java.lang.String, java.lang.String);
  public static java.io.ByteArrayInputStream toStream(java.lang.String, java.nio.charset.Charset);
  public static java.io.ByteArrayInputStream toUtf8Stream(java.lang.String);
  public static java.io.FileInputStream toStream(java.io.File);
  public static java.io.ByteArrayInputStream toStream(byte[]);
  public static java.io.ByteArrayInputStream toStream(java.io.ByteArrayOutputStream);
  public static java.io.BufferedInputStream toBuffered(java.io.InputStream);
  public static java.io.BufferedInputStream toBuffered(java.io.InputStream, int);
  public static java.io.BufferedOutputStream toBuffered(java.io.OutputStream);
  public static java.io.BufferedOutputStream toBuffered(java.io.OutputStream, int);
  public static java.io.BufferedReader toBuffered(java.io.Reader);
  public static java.io.BufferedReader toBuffered(java.io.Reader, int);
  public static java.io.BufferedWriter toBuffered(java.io.Writer);
  public static java.io.BufferedWriter toBuffered(java.io.Writer, int);
  public static java.io.InputStream toMarkSupportStream(java.io.InputStream);
  public static java.io.PushbackInputStream toPushbackStream(java.io.InputStream, int);
  public static java.io.InputStream toAvailableStream(java.io.InputStream);
  public static void write(java.io.OutputStream, boolean, byte[]) throws cn.hutool.core.io.IORuntimeException;
  public static void writeUtf8(java.io.OutputStream, boolean, java.lang.Object...) throws cn.hutool.core.io.IORuntimeException;
  public static void write(java.io.OutputStream, java.lang.String, boolean, java.lang.Object...) throws cn.hutool.core.io.IORuntimeException;
  public static void write(java.io.OutputStream, java.nio.charset.Charset, boolean, java.lang.Object...) throws cn.hutool.core.io.IORuntimeException;
  public static void writeObj(java.io.OutputStream, boolean, java.io.Serializable) throws cn.hutool.core.io.IORuntimeException;
  public static void writeObjects(java.io.OutputStream, boolean, java.io.Serializable...) throws cn.hutool.core.io.IORuntimeException;
  public static void flush(java.io.Flushable);
  public static void close(java.io.Closeable);
  public static void closeIfPosible(java.lang.Object);
  public static void closeIfPossible(java.lang.Object);
  public static boolean contentEquals(java.io.InputStream, java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public static boolean contentEquals(java.io.Reader, java.io.Reader) throws cn.hutool.core.io.IORuntimeException;
  public static boolean contentEqualsIgnoreEOL(java.io.Reader, java.io.Reader) throws cn.hutool.core.io.IORuntimeException;
  public static long checksumCRC32(java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.zip.Checksum checksum(java.io.InputStream, java.util.zip.Checksum) throws cn.hutool.core.io.IORuntimeException;
  public static long checksumValue(java.io.InputStream, java.util.zip.Checksum);
  public static cn.hutool.core.collection.LineIter lineIter(java.io.Reader);
  public static cn.hutool.core.collection.LineIter lineIter(java.io.InputStream, java.nio.charset.Charset);
  public static java.lang.String toStr(java.io.ByteArrayOutputStream, java.nio.charset.Charset);
}
```

## `cn.hutool.core.io.LimitedInputStream`

```java
public class cn.hutool.core.io.LimitedInputStream extends java.io.FilterInputStream {
  public cn.hutool.core.io.LimitedInputStream(java.io.InputStream, long);
  public int read() throws java.io.IOException;
  public int read(byte[], int, int) throws java.io.IOException;
  public long skip(long) throws java.io.IOException;
}
```

## `cn.hutool.core.io.LineHandler`

```java
public interface cn.hutool.core.io.LineHandler {
  public abstract void handle(java.lang.String);
}
```

## `cn.hutool.core.io.ManifestUtil`

```java
public class cn.hutool.core.io.ManifestUtil {
  public cn.hutool.core.io.ManifestUtil();
  public static java.util.jar.Manifest getManifest(java.lang.Class<?>) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.jar.Manifest getManifest(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.jar.Manifest getManifest(java.net.JarURLConnection) throws cn.hutool.core.io.IORuntimeException;
  public static java.util.jar.Manifest getManifest(java.util.jar.JarFile) throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.core.io.NioUtil`

```java
public class cn.hutool.core.io.NioUtil {
  public cn.hutool.core.io.NioUtil();
  public static long copyByNIO(java.io.InputStream, java.io.OutputStream, int, cn.hutool.core.io.StreamProgress) throws cn.hutool.core.io.IORuntimeException;
  public static long copyByNIO(java.io.InputStream, java.io.OutputStream, int, long, cn.hutool.core.io.StreamProgress) throws cn.hutool.core.io.IORuntimeException;
  public static long copy(java.nio.channels.FileChannel, java.nio.channels.FileChannel) throws cn.hutool.core.io.IORuntimeException;
  public static long copy(java.nio.channels.ReadableByteChannel, java.nio.channels.WritableByteChannel) throws cn.hutool.core.io.IORuntimeException;
  public static long copy(java.nio.channels.ReadableByteChannel, java.nio.channels.WritableByteChannel, int) throws cn.hutool.core.io.IORuntimeException;
  public static long copy(java.nio.channels.ReadableByteChannel, java.nio.channels.WritableByteChannel, int, cn.hutool.core.io.StreamProgress) throws cn.hutool.core.io.IORuntimeException;
  public static long copy(java.nio.channels.ReadableByteChannel, java.nio.channels.WritableByteChannel, int, long, cn.hutool.core.io.StreamProgress) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String read(java.nio.channels.ReadableByteChannel, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static cn.hutool.core.io.FastByteArrayOutputStream read(java.nio.channels.ReadableByteChannel) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String readUtf8(java.nio.channels.FileChannel) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String read(java.nio.channels.FileChannel, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.lang.String read(java.nio.channels.FileChannel, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static void close(java.lang.AutoCloseable);
}
```

## `cn.hutool.core.io.NullOutputStream`

```java
public class cn.hutool.core.io.NullOutputStream extends java.io.OutputStream {
  public cn.hutool.core.io.NullOutputStream();
  public void write(byte[], int, int);
  public void write(int);
  public void write(byte[]) throws java.io.IOException;
}
```

## `cn.hutool.core.io.StreamProgress`

```java
public interface cn.hutool.core.io.StreamProgress {
  public abstract void start();
  public abstract void progress(long, long);
  public abstract void finish();
}
```

## `cn.hutool.core.io.ValidateObjectInputStream`

```java
public class cn.hutool.core.io.ValidateObjectInputStream extends java.io.ObjectInputStream {
  public cn.hutool.core.io.ValidateObjectInputStream(java.io.InputStream, java.lang.Class<?>...) throws java.io.IOException;
  public void refuse(java.lang.Class<?>...);
  public void accept(java.lang.Class<?>...);
}
```
