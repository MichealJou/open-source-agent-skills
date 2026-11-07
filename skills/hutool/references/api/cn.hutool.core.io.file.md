# cn.hutool.core.io.file

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.io.file.FileAppender`

```java
public class cn.hutool.core.io.file.FileAppender implements java.io.Serializable {
  public cn.hutool.core.io.file.FileAppender(java.io.File, int, boolean);
  public cn.hutool.core.io.file.FileAppender(java.io.File, java.nio.charset.Charset, int, boolean);
  public cn.hutool.core.io.file.FileAppender(java.io.File, java.nio.charset.Charset, int, boolean, java.util.concurrent.locks.Lock);
  public cn.hutool.core.io.file.FileAppender append(java.lang.String);
  public cn.hutool.core.io.file.FileAppender flush();
}
```

## `cn.hutool.core.io.file.FileCopier`

```java
public class cn.hutool.core.io.file.FileCopier extends cn.hutool.core.lang.copier.SrcToDestCopier<java.io.File, cn.hutool.core.io.file.FileCopier> {
  public static cn.hutool.core.io.file.FileCopier create(java.lang.String, java.lang.String);
  public static cn.hutool.core.io.file.FileCopier create(java.io.File, java.io.File);
  public cn.hutool.core.io.file.FileCopier(java.io.File, java.io.File);
  public boolean isOverride();
  public cn.hutool.core.io.file.FileCopier setOverride(boolean);
  public boolean isCopyAttributes();
  public cn.hutool.core.io.file.FileCopier setCopyAttributes(boolean);
  public boolean isCopyContentIfDir();
  public cn.hutool.core.io.file.FileCopier setCopyContentIfDir(boolean);
  public boolean isOnlyCopyFile();
  public cn.hutool.core.io.file.FileCopier setOnlyCopyFile(boolean);
  public java.io.File copy() throws cn.hutool.core.io.IORuntimeException;
  public java.lang.Object copy();
}
```

## `cn.hutool.core.io.file.FileMode`

```java
public final class cn.hutool.core.io.file.FileMode extends java.lang.Enum<cn.hutool.core.io.file.FileMode> {
  public static cn.hutool.core.io.file.FileMode[] values();
  public static cn.hutool.core.io.file.FileMode valueOf(java.lang.String);
}
```

## `cn.hutool.core.io.file.FileNameUtil`

```java
public class cn.hutool.core.io.file.FileNameUtil {
  public cn.hutool.core.io.file.FileNameUtil();
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
  public static java.lang.String cleanInvalid(java.lang.String);
  public static boolean containsInvalid(java.lang.String);
  public static boolean isType(java.lang.String, java.lang.String...);
}
```

## `cn.hutool.core.io.file.FileReader`

```java
public class cn.hutool.core.io.file.FileReader extends cn.hutool.core.io.file.FileWrapper {
  public static cn.hutool.core.io.file.FileReader create(java.io.File, java.nio.charset.Charset);
  public static cn.hutool.core.io.file.FileReader create(java.io.File);
  public cn.hutool.core.io.file.FileReader(java.io.File, java.nio.charset.Charset);
  public cn.hutool.core.io.file.FileReader(java.io.File, java.lang.String);
  public cn.hutool.core.io.file.FileReader(java.lang.String, java.nio.charset.Charset);
  public cn.hutool.core.io.file.FileReader(java.lang.String, java.lang.String);
  public cn.hutool.core.io.file.FileReader(java.io.File);
  public cn.hutool.core.io.file.FileReader(java.lang.String);
  public byte[] readBytes() throws cn.hutool.core.io.IORuntimeException;
  public java.lang.String readString() throws cn.hutool.core.io.IORuntimeException;
  public <T extends java.util.Collection<java.lang.String>> T readLines(T) throws cn.hutool.core.io.IORuntimeException;
  public void readLines(cn.hutool.core.io.LineHandler) throws cn.hutool.core.io.IORuntimeException;
  public java.util.List<java.lang.String> readLines() throws cn.hutool.core.io.IORuntimeException;
  public <T> T read(cn.hutool.core.io.file.FileReader$ReaderHandler<T>) throws cn.hutool.core.io.IORuntimeException;
  public java.io.BufferedReader getReader() throws cn.hutool.core.io.IORuntimeException;
  public java.io.BufferedInputStream getInputStream() throws cn.hutool.core.io.IORuntimeException;
  public long writeToStream(java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public long writeToStream(java.io.OutputStream, boolean) throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.core.io.file.FileReader$ReaderHandler`

```java
public interface cn.hutool.core.io.file.FileReader$ReaderHandler<T> {
  public abstract T handle(java.io.BufferedReader) throws java.io.IOException;
}
```

## `cn.hutool.core.io.file.FileSystemUtil`

```java
public class cn.hutool.core.io.file.FileSystemUtil {
  public cn.hutool.core.io.file.FileSystemUtil();
  public static java.nio.file.FileSystem create(java.lang.String);
  public static java.nio.file.FileSystem createZip(java.lang.String);
  public static java.nio.file.FileSystem createZip(java.lang.String, java.nio.charset.Charset);
  public static java.nio.file.Path getRoot(java.nio.file.FileSystem);
}
```

## `cn.hutool.core.io.file.FileWrapper`

```java
public class cn.hutool.core.io.file.FileWrapper implements java.io.Serializable {
  public cn.hutool.core.io.file.FileWrapper(java.io.File, java.nio.charset.Charset);
  public java.io.File getFile();
  public cn.hutool.core.io.file.FileWrapper setFile(java.io.File);
  public java.nio.charset.Charset getCharset();
  public cn.hutool.core.io.file.FileWrapper setCharset(java.nio.charset.Charset);
  public java.lang.String readableFileSize();
}
```

## `cn.hutool.core.io.file.FileWriter`

```java
public class cn.hutool.core.io.file.FileWriter extends cn.hutool.core.io.file.FileWrapper {
  public static cn.hutool.core.io.file.FileWriter create(java.io.File, java.nio.charset.Charset);
  public static cn.hutool.core.io.file.FileWriter create(java.io.File);
  public cn.hutool.core.io.file.FileWriter(java.io.File, java.nio.charset.Charset);
  public cn.hutool.core.io.file.FileWriter(java.io.File, java.lang.String);
  public cn.hutool.core.io.file.FileWriter(java.lang.String, java.nio.charset.Charset);
  public cn.hutool.core.io.file.FileWriter(java.lang.String, java.lang.String);
  public cn.hutool.core.io.file.FileWriter(java.io.File);
  public cn.hutool.core.io.file.FileWriter(java.lang.String);
  public java.io.File write(java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public java.io.File write(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public java.io.File append(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public <T> java.io.File writeLines(java.lang.Iterable<T>) throws cn.hutool.core.io.IORuntimeException;
  public <T> java.io.File appendLines(java.lang.Iterable<T>) throws cn.hutool.core.io.IORuntimeException;
  public <T> java.io.File writeLines(java.lang.Iterable<T>, boolean) throws cn.hutool.core.io.IORuntimeException;
  public <T> java.io.File writeLines(java.lang.Iterable<T>, cn.hutool.core.io.file.LineSeparator, boolean) throws cn.hutool.core.io.IORuntimeException;
  public <T> java.io.File writeLines(java.lang.Iterable<T>, cn.hutool.core.io.file.LineSeparator, boolean, boolean) throws cn.hutool.core.io.IORuntimeException;
  public java.io.File writeMap(java.util.Map<?, ?>, java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public java.io.File writeMap(java.util.Map<?, ?>, cn.hutool.core.io.file.LineSeparator, java.lang.String, boolean) throws cn.hutool.core.io.IORuntimeException;
  public java.io.File write(byte[], int, int) throws cn.hutool.core.io.IORuntimeException;
  public java.io.File append(byte[], int, int) throws cn.hutool.core.io.IORuntimeException;
  public java.io.File write(byte[], int, int, boolean) throws cn.hutool.core.io.IORuntimeException;
  public java.io.File writeFromStream(java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public java.io.File writeFromStream(java.io.InputStream, boolean) throws cn.hutool.core.io.IORuntimeException;
  public java.io.BufferedOutputStream getOutputStream() throws cn.hutool.core.io.IORuntimeException;
  public java.io.BufferedWriter getWriter(boolean) throws cn.hutool.core.io.IORuntimeException;
  public java.io.PrintWriter getPrintWriter(boolean) throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.core.io.file.LineReadWatcher`

```java
public class cn.hutool.core.io.file.LineReadWatcher extends cn.hutool.core.io.watch.SimpleWatcher implements java.lang.Runnable {
  public cn.hutool.core.io.file.LineReadWatcher(java.io.RandomAccessFile, java.nio.charset.Charset, cn.hutool.core.io.LineHandler);
  public void run();
  public void onModify(java.nio.file.WatchEvent<?>, java.nio.file.Path);
}
```

## `cn.hutool.core.io.file.LineSeparator`

```java
public final class cn.hutool.core.io.file.LineSeparator extends java.lang.Enum<cn.hutool.core.io.file.LineSeparator> {
  public static cn.hutool.core.io.file.LineSeparator[] values();
  public static cn.hutool.core.io.file.LineSeparator valueOf(java.lang.String);
  public java.lang.String getValue();
}
```

## `cn.hutool.core.io.file.PathMover`

```java
public class cn.hutool.core.io.file.PathMover {
  public static cn.hutool.core.io.file.PathMover of(java.nio.file.Path, java.nio.file.Path, boolean);
  public static cn.hutool.core.io.file.PathMover of(java.nio.file.Path, java.nio.file.Path, java.nio.file.CopyOption[]);
  public cn.hutool.core.io.file.PathMover(java.nio.file.Path, java.nio.file.Path, java.nio.file.CopyOption[]);
  public java.nio.file.Path move();
  public java.nio.file.Path moveContent();
}
```

## `cn.hutool.core.io.file.PathUtil`

```java
public class cn.hutool.core.io.file.PathUtil {
  public cn.hutool.core.io.file.PathUtil();
  public static boolean isDirEmpty(java.nio.file.Path);
  public static java.util.List<java.io.File> loopFiles(java.nio.file.Path, java.io.FileFilter);
  public static java.util.List<java.io.File> loopFiles(java.nio.file.Path, int, java.io.FileFilter);
  public static java.util.List<java.io.File> loopFiles(java.nio.file.Path, int, boolean, java.io.FileFilter);
  public static void walkFiles(java.nio.file.Path, java.nio.file.FileVisitor<? super java.nio.file.Path>);
  public static void walkFiles(java.nio.file.Path, int, java.nio.file.FileVisitor<? super java.nio.file.Path>);
  public static void walkFiles(java.nio.file.Path, int, boolean, java.nio.file.FileVisitor<? super java.nio.file.Path>);
  public static boolean del(java.nio.file.Path) throws cn.hutool.core.io.IORuntimeException;
  public static java.nio.file.Path copyFile(cn.hutool.core.io.resource.Resource, java.nio.file.Path, java.nio.file.CopyOption...) throws cn.hutool.core.io.IORuntimeException;
  public static java.nio.file.Path copyFile(java.io.InputStream, java.nio.file.Path, java.nio.file.CopyOption...) throws cn.hutool.core.io.IORuntimeException;
  public static java.nio.file.Path copyFile(java.nio.file.Path, java.nio.file.Path, java.nio.file.StandardCopyOption...) throws cn.hutool.core.io.IORuntimeException;
  public static java.nio.file.Path copyFile(java.nio.file.Path, java.nio.file.Path, java.nio.file.CopyOption...) throws cn.hutool.core.io.IORuntimeException;
  public static java.nio.file.Path copy(java.nio.file.Path, java.nio.file.Path, java.nio.file.CopyOption...) throws cn.hutool.core.io.IORuntimeException;
  public static java.nio.file.Path copyContent(java.nio.file.Path, java.nio.file.Path, java.nio.file.CopyOption...) throws cn.hutool.core.io.IORuntimeException;
  public static boolean isDirectory(java.nio.file.Path);
  public static boolean isDirectory(java.nio.file.Path, boolean);
  public static java.nio.file.Path getPathEle(java.nio.file.Path, int);
  public static java.nio.file.Path getLastPathEle(java.nio.file.Path);
  public static java.nio.file.Path subPath(java.nio.file.Path, int, int);
  public static java.nio.file.attribute.BasicFileAttributes getAttributes(java.nio.file.Path, boolean) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedInputStream getInputStream(java.nio.file.Path) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedReader getUtf8Reader(java.nio.file.Path) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.BufferedReader getReader(java.nio.file.Path, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public static byte[] readBytes(java.nio.file.Path);
  public static java.io.BufferedOutputStream getOutputStream(java.nio.file.Path) throws cn.hutool.core.io.IORuntimeException;
  public static java.nio.file.Path rename(java.nio.file.Path, java.lang.String, boolean);
  public static java.nio.file.Path move(java.nio.file.Path, java.nio.file.Path, boolean);
  public static java.nio.file.Path moveContent(java.nio.file.Path, java.nio.file.Path, boolean);
  public static boolean equals(java.nio.file.Path, java.nio.file.Path) throws cn.hutool.core.io.IORuntimeException;
  public static boolean isFile(java.nio.file.Path, boolean);
  public static boolean isSymlink(java.nio.file.Path);
  public static boolean exists(java.nio.file.Path, boolean);
  public static boolean isExistsAndNotDirectory(java.nio.file.Path, boolean);
  public static boolean isSub(java.nio.file.Path, java.nio.file.Path);
  public static java.nio.file.Path toAbsNormal(java.nio.file.Path);
  public static java.lang.String getMimeType(java.nio.file.Path);
  public static java.nio.file.Path mkdir(java.nio.file.Path);
  public static java.nio.file.Path mkParentDirs(java.nio.file.Path);
  public static java.lang.String getName(java.nio.file.Path);
  public static java.nio.file.Path createTempFile(java.lang.String, java.lang.String, java.nio.file.Path) throws cn.hutool.core.io.IORuntimeException;
  public static java.nio.file.LinkOption[] getLinkOptions(boolean);
  public static java.util.Set<java.nio.file.FileVisitOption> getFileVisitOption(boolean);
}
```

## `cn.hutool.core.io.file.Tailer`

```java
public class cn.hutool.core.io.file.Tailer implements java.io.Serializable {
  public cn.hutool.core.io.file.Tailer(java.io.File, cn.hutool.core.io.LineHandler);
  public cn.hutool.core.io.file.Tailer(java.io.File, cn.hutool.core.io.LineHandler, int);
  public cn.hutool.core.io.file.Tailer(java.io.File, java.nio.charset.Charset, cn.hutool.core.io.LineHandler);
  public cn.hutool.core.io.file.Tailer(java.io.File, java.nio.charset.Charset, cn.hutool.core.io.LineHandler, int, long);
  public void setStopOnDelete(boolean);
  public void start();
  public void start(boolean);
  public void stop();
}
```

## `cn.hutool.core.io.file.Tailer$ConsoleLineHandler`

```java
public class cn.hutool.core.io.file.Tailer$ConsoleLineHandler implements cn.hutool.core.io.LineHandler {
  public cn.hutool.core.io.file.Tailer$ConsoleLineHandler();
  public void handle(java.lang.String);
}
```
