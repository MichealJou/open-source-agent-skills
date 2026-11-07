# cn.hutool.core.io.copy

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.io.copy.ChannelCopier`

```java
public class cn.hutool.core.io.copy.ChannelCopier extends cn.hutool.core.io.copy.IoCopier<java.nio.channels.ReadableByteChannel, java.nio.channels.WritableByteChannel> {
  public cn.hutool.core.io.copy.ChannelCopier();
  public cn.hutool.core.io.copy.ChannelCopier(int);
  public cn.hutool.core.io.copy.ChannelCopier(int, long);
  public cn.hutool.core.io.copy.ChannelCopier(int, long, cn.hutool.core.io.StreamProgress);
  public long copy(java.nio.channels.ReadableByteChannel, java.nio.channels.WritableByteChannel);
  public long copy(java.lang.Object, java.lang.Object);
}
```

## `cn.hutool.core.io.copy.IoCopier`

```java
public abstract class cn.hutool.core.io.copy.IoCopier<S, T> {
  public cn.hutool.core.io.copy.IoCopier(int, long, cn.hutool.core.io.StreamProgress);
  public abstract long copy(S, T);
  public cn.hutool.core.io.copy.IoCopier<S, T> setFlushEveryBuffer(boolean);
}
```

## `cn.hutool.core.io.copy.ReaderWriterCopier`

```java
public class cn.hutool.core.io.copy.ReaderWriterCopier extends cn.hutool.core.io.copy.IoCopier<java.io.Reader, java.io.Writer> {
  public cn.hutool.core.io.copy.ReaderWriterCopier();
  public cn.hutool.core.io.copy.ReaderWriterCopier(int);
  public cn.hutool.core.io.copy.ReaderWriterCopier(int, long);
  public cn.hutool.core.io.copy.ReaderWriterCopier(int, long, cn.hutool.core.io.StreamProgress);
  public long copy(java.io.Reader, java.io.Writer);
  public long copy(java.lang.Object, java.lang.Object);
}
```

## `cn.hutool.core.io.copy.StreamCopier`

```java
public class cn.hutool.core.io.copy.StreamCopier extends cn.hutool.core.io.copy.IoCopier<java.io.InputStream, java.io.OutputStream> {
  public cn.hutool.core.io.copy.StreamCopier();
  public cn.hutool.core.io.copy.StreamCopier(int);
  public cn.hutool.core.io.copy.StreamCopier(int, long);
  public cn.hutool.core.io.copy.StreamCopier(int, long, cn.hutool.core.io.StreamProgress);
  public long copy(java.io.InputStream, java.io.OutputStream);
  public long copy(java.lang.Object, java.lang.Object);
}
```
