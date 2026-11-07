# cn.hutool.extra.compress.extractor

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.compress.extractor.Extractor`

```java
public interface cn.hutool.extra.compress.extractor.Extractor extends java.io.Closeable {
  public default void extract(java.io.File);
  public default void extract(java.io.File, cn.hutool.core.lang.Filter<org.apache.commons.compress.archivers.ArchiveEntry>);
  public default void extract(java.io.File, int);
  public abstract void extract(java.io.File, int, cn.hutool.core.lang.Filter<org.apache.commons.compress.archivers.ArchiveEntry>);
  public default java.lang.String stripName(java.lang.String, int);
  public abstract void close();
}
```

## `cn.hutool.extra.compress.extractor.Seven7EntryInputStream`

```java
public class cn.hutool.extra.compress.extractor.Seven7EntryInputStream extends java.io.InputStream {
  public cn.hutool.extra.compress.extractor.Seven7EntryInputStream(org.apache.commons.compress.archivers.sevenz.SevenZFile, org.apache.commons.compress.archivers.sevenz.SevenZArchiveEntry);
  public int available() throws java.io.IOException;
  public long getReadSize();
  public int read() throws java.io.IOException;
}
```

## `cn.hutool.extra.compress.extractor.SevenZExtractor`

```java
public class cn.hutool.extra.compress.extractor.SevenZExtractor implements cn.hutool.extra.compress.extractor.Extractor,java.util.RandomAccess {
  public cn.hutool.extra.compress.extractor.SevenZExtractor(java.io.File);
  public cn.hutool.extra.compress.extractor.SevenZExtractor(java.io.File, char[]);
  public cn.hutool.extra.compress.extractor.SevenZExtractor(java.io.InputStream);
  public cn.hutool.extra.compress.extractor.SevenZExtractor(java.io.InputStream, char[]);
  public cn.hutool.extra.compress.extractor.SevenZExtractor(java.nio.channels.SeekableByteChannel);
  public cn.hutool.extra.compress.extractor.SevenZExtractor(java.nio.channels.SeekableByteChannel, char[]);
  public void extract(java.io.File, int, cn.hutool.core.lang.Filter<org.apache.commons.compress.archivers.ArchiveEntry>);
  public java.io.InputStream getFirst(cn.hutool.core.lang.Filter<org.apache.commons.compress.archivers.ArchiveEntry>);
  public java.io.InputStream get(java.lang.String);
  public void close();
}
```

## `cn.hutool.extra.compress.extractor.StreamExtractor`

```java
public class cn.hutool.extra.compress.extractor.StreamExtractor implements cn.hutool.extra.compress.extractor.Extractor {
  public cn.hutool.extra.compress.extractor.StreamExtractor(java.nio.charset.Charset, java.io.File);
  public cn.hutool.extra.compress.extractor.StreamExtractor(java.nio.charset.Charset, java.lang.String, java.io.File);
  public cn.hutool.extra.compress.extractor.StreamExtractor(java.nio.charset.Charset, java.io.InputStream);
  public cn.hutool.extra.compress.extractor.StreamExtractor(java.nio.charset.Charset, java.lang.String, java.io.InputStream);
  public void extract(java.io.File, int, cn.hutool.core.lang.Filter<org.apache.commons.compress.archivers.ArchiveEntry>);
  public void close();
}
```
