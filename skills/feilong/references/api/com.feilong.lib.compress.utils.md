# com.feilong.lib.compress.utils

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.compress.utils.ArchiveUtils`

```java
public class com.feilong.lib.compress.utils.ArchiveUtils {
  public static java.lang.String toString(com.feilong.lib.compress.archivers.ArchiveEntry);
  public static boolean matchAsciiBuffer(java.lang.String, byte[], int, int);
  public static boolean matchAsciiBuffer(java.lang.String, byte[]);
  public static byte[] toAsciiBytes(java.lang.String);
  public static java.lang.String toAsciiString(byte[]);
  public static java.lang.String toAsciiString(byte[], int, int);
  public static boolean isEqual(byte[], int, int, byte[], int, int, boolean);
  public static boolean isEqual(byte[], int, int, byte[], int, int);
  public static boolean isEqual(byte[], byte[]);
  public static boolean isEqual(byte[], byte[], boolean);
  public static boolean isEqualWithNull(byte[], int, int, byte[], int, int);
  public static boolean isArrayZero(byte[], int);
  public static java.lang.String sanitize(java.lang.String);
}
```

## `com.feilong.lib.compress.utils.BitInputStream`

```java
public class com.feilong.lib.compress.utils.BitInputStream implements java.io.Closeable {
  public com.feilong.lib.compress.utils.BitInputStream(java.io.InputStream, java.nio.ByteOrder);
  public void close() throws java.io.IOException;
  public void clearBitCache();
  public long readBits(int) throws java.io.IOException;
  public int bitsCached();
  public long bitsAvailable() throws java.io.IOException;
  public void alignWithByteBoundary();
  public long getBytesRead();
}
```

## `com.feilong.lib.compress.utils.ByteUtils`

```java
public final class com.feilong.lib.compress.utils.ByteUtils {
  public static long fromLittleEndian(byte[]);
  public static long fromLittleEndian(byte[], int, int);
  public static long fromLittleEndian(java.io.InputStream, int) throws java.io.IOException;
  public static long fromLittleEndian(com.feilong.lib.compress.utils.ByteUtils$ByteSupplier, int) throws java.io.IOException;
  public static long fromLittleEndian(java.io.DataInput, int) throws java.io.IOException;
  public static void toLittleEndian(byte[], long, int, int);
  public static void toLittleEndian(java.io.OutputStream, long, int) throws java.io.IOException;
  public static void toLittleEndian(com.feilong.lib.compress.utils.ByteUtils$ByteConsumer, long, int) throws java.io.IOException;
  public static void toLittleEndian(java.io.DataOutput, long, int) throws java.io.IOException;
}
```

## `com.feilong.lib.compress.utils.ByteUtils$ByteConsumer`

```java
public interface com.feilong.lib.compress.utils.ByteUtils$ByteConsumer {
  public abstract void accept(int) throws java.io.IOException;
}
```

## `com.feilong.lib.compress.utils.ByteUtils$ByteSupplier`

```java
public interface com.feilong.lib.compress.utils.ByteUtils$ByteSupplier {
  public abstract int getAsByte() throws java.io.IOException;
}
```

## `com.feilong.lib.compress.utils.ByteUtils$InputStreamByteSupplier`

```java
public class com.feilong.lib.compress.utils.ByteUtils$InputStreamByteSupplier implements com.feilong.lib.compress.utils.ByteUtils$ByteSupplier {
  public com.feilong.lib.compress.utils.ByteUtils$InputStreamByteSupplier(java.io.InputStream);
  public int getAsByte() throws java.io.IOException;
}
```

## `com.feilong.lib.compress.utils.ByteUtils$OutputStreamByteConsumer`

```java
public class com.feilong.lib.compress.utils.ByteUtils$OutputStreamByteConsumer implements com.feilong.lib.compress.utils.ByteUtils$ByteConsumer {
  public com.feilong.lib.compress.utils.ByteUtils$OutputStreamByteConsumer(java.io.OutputStream);
  public void accept(int) throws java.io.IOException;
}
```

## `com.feilong.lib.compress.utils.CharsetNames`

```java
public class com.feilong.lib.compress.utils.CharsetNames {
  public com.feilong.lib.compress.utils.CharsetNames();
}
```

## `com.feilong.lib.compress.utils.CloseShieldFilterInputStream`

```java
public class com.feilong.lib.compress.utils.CloseShieldFilterInputStream extends java.io.FilterInputStream {
  public com.feilong.lib.compress.utils.CloseShieldFilterInputStream(java.io.InputStream);
  public void close() throws java.io.IOException;
}
```

## `com.feilong.lib.compress.utils.CountingInputStream`

```java
public class com.feilong.lib.compress.utils.CountingInputStream extends java.io.FilterInputStream {
  public com.feilong.lib.compress.utils.CountingInputStream(java.io.InputStream);
  public int read() throws java.io.IOException;
  public int read(byte[]) throws java.io.IOException;
  public int read(byte[], int, int) throws java.io.IOException;
  public long getBytesRead();
}
```

## `com.feilong.lib.compress.utils.FileNameUtils`

```java
public class com.feilong.lib.compress.utils.FileNameUtils {
  public com.feilong.lib.compress.utils.FileNameUtils();
  public static java.lang.String getExtension(java.lang.String);
  public static java.lang.String getBaseName(java.lang.String);
}
```

## `com.feilong.lib.compress.utils.IOUtils`

```java
public final class com.feilong.lib.compress.utils.IOUtils {
  public static long copy(java.io.InputStream, java.io.OutputStream) throws java.io.IOException;
  public static long copy(java.io.InputStream, java.io.OutputStream, int) throws java.io.IOException;
  public static long skip(java.io.InputStream, long) throws java.io.IOException;
  public static int read(java.io.File, byte[]) throws java.io.IOException;
  public static int readFully(java.io.InputStream, byte[]) throws java.io.IOException;
  public static int readFully(java.io.InputStream, byte[], int, int) throws java.io.IOException;
  public static void readFully(java.nio.channels.ReadableByteChannel, java.nio.ByteBuffer) throws java.io.IOException;
  public static byte[] toByteArray(java.io.InputStream) throws java.io.IOException;
  public static void closeQuietly(java.io.Closeable);
}
```

## `com.feilong.lib.compress.utils.InputStreamStatistics`

```java
public interface com.feilong.lib.compress.utils.InputStreamStatistics {
  public abstract long getCompressedCount();
  public abstract long getUncompressedCount();
}
```

## `com.feilong.lib.compress.utils.MultiReadOnlySeekableByteChannel`

```java
public class com.feilong.lib.compress.utils.MultiReadOnlySeekableByteChannel implements java.nio.channels.SeekableByteChannel {
  public com.feilong.lib.compress.utils.MultiReadOnlySeekableByteChannel(java.util.List<java.nio.channels.SeekableByteChannel>);
  public synchronized int read(java.nio.ByteBuffer) throws java.io.IOException;
  public void close() throws java.io.IOException;
  public boolean isOpen();
  public long position();
  public synchronized java.nio.channels.SeekableByteChannel position(long, long) throws java.io.IOException;
  public long size() throws java.io.IOException;
  public java.nio.channels.SeekableByteChannel truncate(long);
  public int write(java.nio.ByteBuffer);
  public synchronized java.nio.channels.SeekableByteChannel position(long) throws java.io.IOException;
  public static java.nio.channels.SeekableByteChannel forSeekableByteChannels(java.nio.channels.SeekableByteChannel...);
  public static java.nio.channels.SeekableByteChannel forFiles(java.io.File...) throws java.io.IOException;
}
```

## `com.feilong.lib.compress.utils.SeekableInMemoryByteChannel`

```java
public class com.feilong.lib.compress.utils.SeekableInMemoryByteChannel implements java.nio.channels.SeekableByteChannel {
  public com.feilong.lib.compress.utils.SeekableInMemoryByteChannel(byte[]);
  public com.feilong.lib.compress.utils.SeekableInMemoryByteChannel();
  public com.feilong.lib.compress.utils.SeekableInMemoryByteChannel(int);
  public long position();
  public java.nio.channels.SeekableByteChannel position(long) throws java.io.IOException;
  public long size();
  public java.nio.channels.SeekableByteChannel truncate(long);
  public int read(java.nio.ByteBuffer) throws java.io.IOException;
  public void close();
  public boolean isOpen();
  public int write(java.nio.ByteBuffer) throws java.io.IOException;
  public byte[] array();
}
```
