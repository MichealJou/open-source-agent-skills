# com.feilong.lib.net.io

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.net.io.CRLFLineReader`

```java
public final class com.feilong.lib.net.io.CRLFLineReader extends java.io.BufferedReader {
  public com.feilong.lib.net.io.CRLFLineReader(java.io.Reader);
  public java.lang.String readLine() throws java.io.IOException;
}
```

## `com.feilong.lib.net.io.CopyStreamAdapter`

```java
public class com.feilong.lib.net.io.CopyStreamAdapter implements com.feilong.lib.net.io.CopyStreamListener {
  public com.feilong.lib.net.io.CopyStreamAdapter();
  public void bytesTransferred(com.feilong.lib.net.io.CopyStreamEvent);
  public void bytesTransferred(long, int, long);
  public void addCopyStreamListener(com.feilong.lib.net.io.CopyStreamListener);
  public void removeCopyStreamListener(com.feilong.lib.net.io.CopyStreamListener);
}
```

## `com.feilong.lib.net.io.CopyStreamEvent`

```java
public class com.feilong.lib.net.io.CopyStreamEvent extends java.util.EventObject {
  public com.feilong.lib.net.io.CopyStreamEvent(java.lang.Object, long, int, long);
  public int getBytesTransferred();
  public long getTotalBytesTransferred();
  public long getStreamSize();
  public java.lang.String toString();
}
```

## `com.feilong.lib.net.io.CopyStreamException`

```java
public class com.feilong.lib.net.io.CopyStreamException extends java.io.IOException {
  public com.feilong.lib.net.io.CopyStreamException(java.lang.String, long, java.io.IOException);
  public long getTotalBytesTransferred();
  public java.io.IOException getIOException();
}
```

## `com.feilong.lib.net.io.CopyStreamListener`

```java
public interface com.feilong.lib.net.io.CopyStreamListener extends java.util.EventListener {
  public abstract void bytesTransferred(com.feilong.lib.net.io.CopyStreamEvent);
  public abstract void bytesTransferred(long, int, long);
}
```

## `com.feilong.lib.net.io.FromNetASCIIInputStream`

```java
public final class com.feilong.lib.net.io.FromNetASCIIInputStream extends java.io.PushbackInputStream {
  public static boolean isConversionRequired();
  public com.feilong.lib.net.io.FromNetASCIIInputStream(java.io.InputStream);
  public int read() throws java.io.IOException;
  public int read(byte[]) throws java.io.IOException;
  public int read(byte[], int, int) throws java.io.IOException;
  public int available() throws java.io.IOException;
}
```

## `com.feilong.lib.net.io.SocketInputStream`

```java
public class com.feilong.lib.net.io.SocketInputStream extends java.io.FilterInputStream {
  public com.feilong.lib.net.io.SocketInputStream(java.net.Socket, java.io.InputStream);
  public void close() throws java.io.IOException;
}
```

## `com.feilong.lib.net.io.SocketOutputStream`

```java
public class com.feilong.lib.net.io.SocketOutputStream extends java.io.FilterOutputStream {
  public com.feilong.lib.net.io.SocketOutputStream(java.net.Socket, java.io.OutputStream);
  public void write(byte[], int, int) throws java.io.IOException;
  public void close() throws java.io.IOException;
}
```

## `com.feilong.lib.net.io.ToNetASCIIOutputStream`

```java
public final class com.feilong.lib.net.io.ToNetASCIIOutputStream extends java.io.FilterOutputStream {
  public com.feilong.lib.net.io.ToNetASCIIOutputStream(java.io.OutputStream);
  public synchronized void write(int) throws java.io.IOException;
  public synchronized void write(byte[]) throws java.io.IOException;
  public synchronized void write(byte[], int, int) throws java.io.IOException;
}
```

## `com.feilong.lib.net.io.Util`

```java
public final class com.feilong.lib.net.io.Util {
  public static long copyStream(java.io.InputStream, java.io.OutputStream, int, long, com.feilong.lib.net.io.CopyStreamListener, boolean) throws com.feilong.lib.net.io.CopyStreamException;
  public static void closeQuietly(java.io.Closeable);
  public static void closeQuietly(java.net.Socket);
}
```
