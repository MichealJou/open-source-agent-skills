# cn.hutool.extra.compress.archiver

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.compress.archiver.Archiver`

```java
public interface cn.hutool.extra.compress.archiver.Archiver extends java.io.Closeable {
  public default cn.hutool.extra.compress.archiver.Archiver add(java.io.File);
  public default cn.hutool.extra.compress.archiver.Archiver add(java.io.File, cn.hutool.core.lang.Filter<java.io.File>);
  public abstract cn.hutool.extra.compress.archiver.Archiver add(java.io.File, java.lang.String, cn.hutool.core.lang.Filter<java.io.File>);
  public abstract cn.hutool.extra.compress.archiver.Archiver finish();
  public abstract void close();
}
```

## `cn.hutool.extra.compress.archiver.SevenZArchiver`

```java
public class cn.hutool.extra.compress.archiver.SevenZArchiver implements cn.hutool.extra.compress.archiver.Archiver {
  public cn.hutool.extra.compress.archiver.SevenZArchiver(java.io.File);
  public cn.hutool.extra.compress.archiver.SevenZArchiver(java.io.OutputStream);
  public cn.hutool.extra.compress.archiver.SevenZArchiver(java.nio.channels.SeekableByteChannel);
  public org.apache.commons.compress.archivers.sevenz.SevenZOutputFile getSevenZOutputFile();
  public cn.hutool.extra.compress.archiver.SevenZArchiver add(java.io.File, java.lang.String, cn.hutool.core.lang.Filter<java.io.File>);
  public cn.hutool.extra.compress.archiver.SevenZArchiver finish();
  public void close();
  public cn.hutool.extra.compress.archiver.Archiver finish();
  public cn.hutool.extra.compress.archiver.Archiver add(java.io.File, java.lang.String, cn.hutool.core.lang.Filter);
}
```

## `cn.hutool.extra.compress.archiver.StreamArchiver`

```java
public class cn.hutool.extra.compress.archiver.StreamArchiver implements cn.hutool.extra.compress.archiver.Archiver {
  public static cn.hutool.extra.compress.archiver.StreamArchiver create(java.nio.charset.Charset, java.lang.String, java.io.File);
  public static cn.hutool.extra.compress.archiver.StreamArchiver create(java.nio.charset.Charset, java.lang.String, java.io.OutputStream);
  public cn.hutool.extra.compress.archiver.StreamArchiver(java.nio.charset.Charset, java.lang.String, java.io.File);
  public cn.hutool.extra.compress.archiver.StreamArchiver(java.nio.charset.Charset, java.lang.String, java.io.OutputStream);
  public cn.hutool.extra.compress.archiver.StreamArchiver add(java.io.File, java.lang.String, cn.hutool.core.lang.Filter<java.io.File>) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.extra.compress.archiver.StreamArchiver finish();
  public void close();
  public cn.hutool.extra.compress.archiver.Archiver finish();
  public cn.hutool.extra.compress.archiver.Archiver add(java.io.File, java.lang.String, cn.hutool.core.lang.Filter);
}
```
