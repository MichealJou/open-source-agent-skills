# cn.hutool.socket

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.socket.ChannelUtil`

```java
public class cn.hutool.socket.ChannelUtil {
  public cn.hutool.socket.ChannelUtil();
  public static java.nio.channels.AsynchronousChannelGroup createFixedGroup(int);
  public static java.nio.channels.AsynchronousSocketChannel connect(java.nio.channels.AsynchronousChannelGroup, java.net.InetSocketAddress);
}
```

## `cn.hutool.socket.SocketConfig`

```java
public class cn.hutool.socket.SocketConfig implements java.io.Serializable {
  public cn.hutool.socket.SocketConfig();
  public int getThreadPoolSize();
  public void setThreadPoolSize(int);
  public long getReadTimeout();
  public void setReadTimeout(long);
  public long getWriteTimeout();
  public void setWriteTimeout(long);
  public int getReadBufferSize();
  public void setReadBufferSize(int);
  public int getWriteBufferSize();
  public void setWriteBufferSize(int);
}
```

## `cn.hutool.socket.SocketRuntimeException`

```java
public class cn.hutool.socket.SocketRuntimeException extends java.lang.RuntimeException {
  public cn.hutool.socket.SocketRuntimeException(java.lang.Throwable);
  public cn.hutool.socket.SocketRuntimeException(java.lang.String);
  public cn.hutool.socket.SocketRuntimeException(java.lang.String, java.lang.Object...);
  public cn.hutool.socket.SocketRuntimeException(java.lang.String, java.lang.Throwable);
  public cn.hutool.socket.SocketRuntimeException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.socket.SocketRuntimeException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.socket.SocketUtil`

```java
public class cn.hutool.socket.SocketUtil {
  public cn.hutool.socket.SocketUtil();
  public static java.net.SocketAddress getRemoteAddress(java.nio.channels.AsynchronousSocketChannel) throws cn.hutool.core.io.IORuntimeException;
  public static boolean isConnected(java.nio.channels.AsynchronousSocketChannel) throws cn.hutool.core.io.IORuntimeException;
  public static java.net.Socket connect(java.lang.String, int) throws cn.hutool.core.io.IORuntimeException;
  public static java.net.Socket connect(java.lang.String, int, int) throws cn.hutool.core.io.IORuntimeException;
  public static java.net.Socket connect(java.net.InetSocketAddress, int) throws cn.hutool.core.io.IORuntimeException;
}
```
