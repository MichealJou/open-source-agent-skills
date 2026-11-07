# com.feilong.lib.compress.archivers

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.compress.archivers.ArchiveEntry`

```java
public interface com.feilong.lib.compress.archivers.ArchiveEntry {
  public abstract java.lang.String getName();
  public abstract long getSize();
  public abstract boolean isDirectory();
  public abstract java.util.Date getLastModifiedDate();
}
```

## `com.feilong.lib.compress.archivers.ArchiveException`

```java
public class com.feilong.lib.compress.archivers.ArchiveException extends java.lang.Exception {
  public com.feilong.lib.compress.archivers.ArchiveException(java.lang.String);
  public com.feilong.lib.compress.archivers.ArchiveException(java.lang.String, java.lang.Exception);
}
```

## `com.feilong.lib.compress.archivers.ArchiveInputStream`

```java
public abstract class com.feilong.lib.compress.archivers.ArchiveInputStream extends java.io.InputStream {
  public com.feilong.lib.compress.archivers.ArchiveInputStream();
  public abstract com.feilong.lib.compress.archivers.ArchiveEntry getNextEntry() throws java.io.IOException;
  public int read() throws java.io.IOException;
  public long getBytesRead();
  public boolean canReadEntryData(com.feilong.lib.compress.archivers.ArchiveEntry);
}
```

## `com.feilong.lib.compress.archivers.ArchiveOutputStream`

```java
public abstract class com.feilong.lib.compress.archivers.ArchiveOutputStream extends java.io.OutputStream {
  public com.feilong.lib.compress.archivers.ArchiveOutputStream();
  public abstract void putArchiveEntry(com.feilong.lib.compress.archivers.ArchiveEntry) throws java.io.IOException;
  public abstract void closeArchiveEntry() throws java.io.IOException;
  public abstract void finish() throws java.io.IOException;
  public abstract com.feilong.lib.compress.archivers.ArchiveEntry createArchiveEntry(java.io.File, java.lang.String) throws java.io.IOException;
  public void write(int) throws java.io.IOException;
  public long getBytesWritten();
  public boolean canWriteEntryData(com.feilong.lib.compress.archivers.ArchiveEntry);
}
```

## `com.feilong.lib.compress.archivers.EntryStreamOffsets`

```java
public interface com.feilong.lib.compress.archivers.EntryStreamOffsets {
  public abstract long getDataOffset();
  public abstract boolean isStreamContiguous();
}
```
