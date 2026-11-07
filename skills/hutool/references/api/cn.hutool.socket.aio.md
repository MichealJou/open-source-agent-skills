# cn.hutool.socket.aio

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.socket.aio.AcceptHandler`

```java
public class cn.hutool.socket.aio.AcceptHandler implements java.nio.channels.CompletionHandler<java.nio.channels.AsynchronousSocketChannel, cn.hutool.socket.aio.AioServer> {
  public cn.hutool.socket.aio.AcceptHandler();
  public void completed(java.nio.channels.AsynchronousSocketChannel, cn.hutool.socket.aio.AioServer);
  public void failed(java.lang.Throwable, cn.hutool.socket.aio.AioServer);
  public void failed(java.lang.Throwable, java.lang.Object);
  public void completed(java.lang.Object, java.lang.Object);
}
```

## `cn.hutool.socket.aio.AioClient`

```java
public class cn.hutool.socket.aio.AioClient implements java.io.Closeable {
  public cn.hutool.socket.aio.AioClient(java.net.InetSocketAddress, cn.hutool.socket.aio.IoAction<java.nio.ByteBuffer>);
  public cn.hutool.socket.aio.AioClient(java.net.InetSocketAddress, cn.hutool.socket.aio.IoAction<java.nio.ByteBuffer>, cn.hutool.socket.SocketConfig);
  public cn.hutool.socket.aio.AioClient(java.nio.channels.AsynchronousSocketChannel, cn.hutool.socket.aio.IoAction<java.nio.ByteBuffer>, cn.hutool.socket.SocketConfig);
  public <T> cn.hutool.socket.aio.AioClient setOption(java.net.SocketOption<T>, T) throws java.io.IOException;
  public cn.hutool.socket.aio.IoAction<java.nio.ByteBuffer> getIoAction();
  public cn.hutool.socket.aio.AioClient read();
  public cn.hutool.socket.aio.AioClient write(java.nio.ByteBuffer);
  public void close();
}
```

## `cn.hutool.socket.aio.AioServer`

```java
public class cn.hutool.socket.aio.AioServer implements java.io.Closeable {
  public cn.hutool.socket.aio.AioServer(int);
  public cn.hutool.socket.aio.AioServer(java.net.InetSocketAddress, cn.hutool.socket.SocketConfig);
  public cn.hutool.socket.aio.AioServer init(java.net.InetSocketAddress);
  public void start(boolean);
  public <T> cn.hutool.socket.aio.AioServer setOption(java.net.SocketOption<T>, T) throws java.io.IOException;
  public cn.hutool.socket.aio.IoAction<java.nio.ByteBuffer> getIoAction();
  public cn.hutool.socket.aio.AioServer setIoAction(cn.hutool.socket.aio.IoAction<java.nio.ByteBuffer>);
  public java.nio.channels.AsynchronousServerSocketChannel getChannel();
  public cn.hutool.socket.aio.AioServer accept();
  public boolean isOpen();
  public void close();
}
```

## `cn.hutool.socket.aio.AioSession`

```java
public class cn.hutool.socket.aio.AioSession implements java.io.Closeable {
  public cn.hutool.socket.aio.AioSession(java.nio.channels.AsynchronousSocketChannel, cn.hutool.socket.aio.IoAction<java.nio.ByteBuffer>, cn.hutool.socket.SocketConfig);
  public java.nio.channels.AsynchronousSocketChannel getChannel();
  public java.nio.ByteBuffer getReadBuffer();
  public java.nio.ByteBuffer getWriteBuffer();
  public cn.hutool.socket.aio.IoAction<java.nio.ByteBuffer> getIoAction();
  public java.net.SocketAddress getRemoteAddress();
  public cn.hutool.socket.aio.AioSession read();
  public cn.hutool.socket.aio.AioSession read(java.nio.channels.CompletionHandler<java.lang.Integer, cn.hutool.socket.aio.AioSession>);
  public cn.hutool.socket.aio.AioSession writeAndClose(java.nio.ByteBuffer);
  public java.util.concurrent.Future<java.lang.Integer> write(java.nio.ByteBuffer);
  public cn.hutool.socket.aio.AioSession write(java.nio.ByteBuffer, java.nio.channels.CompletionHandler<java.lang.Integer, cn.hutool.socket.aio.AioSession>);
  public boolean isOpen();
  public cn.hutool.socket.aio.AioSession closeIn();
  public cn.hutool.socket.aio.AioSession closeOut();
  public void close();
}
```

## `cn.hutool.socket.aio.IoAction`

```java
public interface cn.hutool.socket.aio.IoAction<T> {
  public abstract void accept(cn.hutool.socket.aio.AioSession);
  public abstract void doAction(cn.hutool.socket.aio.AioSession, T);
  public abstract void failed(java.lang.Throwable, cn.hutool.socket.aio.AioSession);
}
```

## `cn.hutool.socket.aio.ReadHandler`

```java
public class cn.hutool.socket.aio.ReadHandler implements java.nio.channels.CompletionHandler<java.lang.Integer, cn.hutool.socket.aio.AioSession> {
  public cn.hutool.socket.aio.ReadHandler();
  public void completed(java.lang.Integer, cn.hutool.socket.aio.AioSession);
  public void failed(java.lang.Throwable, cn.hutool.socket.aio.AioSession);
  public void failed(java.lang.Throwable, java.lang.Object);
  public void completed(java.lang.Object, java.lang.Object);
}
```

## `cn.hutool.socket.aio.SimpleIoAction`

```java
public abstract class cn.hutool.socket.aio.SimpleIoAction implements cn.hutool.socket.aio.IoAction<java.nio.ByteBuffer> {
  public cn.hutool.socket.aio.SimpleIoAction();
  public void accept(cn.hutool.socket.aio.AioSession);
  public void failed(java.lang.Throwable, cn.hutool.socket.aio.AioSession);
}
```
