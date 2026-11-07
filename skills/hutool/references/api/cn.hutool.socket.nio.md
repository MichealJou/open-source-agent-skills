# cn.hutool.socket.nio

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.socket.nio.AcceptHandler`

```java
public class cn.hutool.socket.nio.AcceptHandler implements java.nio.channels.CompletionHandler<java.nio.channels.ServerSocketChannel, cn.hutool.socket.nio.NioServer> {
  public cn.hutool.socket.nio.AcceptHandler();
  public void completed(java.nio.channels.ServerSocketChannel, cn.hutool.socket.nio.NioServer);
  public void failed(java.lang.Throwable, cn.hutool.socket.nio.NioServer);
  public void failed(java.lang.Throwable, java.lang.Object);
  public void completed(java.lang.Object, java.lang.Object);
}
```

## `cn.hutool.socket.nio.ChannelHandler`

```java
public interface cn.hutool.socket.nio.ChannelHandler {
  public abstract void handle(java.nio.channels.SocketChannel) throws java.lang.Exception;
}
```

## `cn.hutool.socket.nio.NioClient`

```java
public class cn.hutool.socket.nio.NioClient implements java.io.Closeable {
  public cn.hutool.socket.nio.NioClient(java.lang.String, int);
  public cn.hutool.socket.nio.NioClient(java.net.InetSocketAddress);
  public cn.hutool.socket.nio.NioClient init(java.net.InetSocketAddress);
  public cn.hutool.socket.nio.NioClient setChannelHandler(cn.hutool.socket.nio.ChannelHandler);
  public void listen();
  public cn.hutool.socket.nio.NioClient write(java.nio.ByteBuffer...);
  public java.nio.channels.SocketChannel getChannel();
  public void close();
}
```

## `cn.hutool.socket.nio.NioServer`

```java
public class cn.hutool.socket.nio.NioServer implements java.io.Closeable {
  public cn.hutool.socket.nio.NioServer(int);
  public cn.hutool.socket.nio.NioServer init(java.net.InetSocketAddress);
  public cn.hutool.socket.nio.NioServer setChannelHandler(cn.hutool.socket.nio.ChannelHandler);
  public java.nio.channels.Selector getSelector();
  public void start();
  public void listen();
  public void close();
}
```

## `cn.hutool.socket.nio.NioUtil`

```java
public class cn.hutool.socket.nio.NioUtil {
  public cn.hutool.socket.nio.NioUtil();
  public static void registerChannel(java.nio.channels.Selector, java.nio.channels.SelectableChannel, cn.hutool.socket.nio.Operation);
}
```

## `cn.hutool.socket.nio.Operation`

```java
public final class cn.hutool.socket.nio.Operation extends java.lang.Enum<cn.hutool.socket.nio.Operation> {
  public static cn.hutool.socket.nio.Operation[] values();
  public static cn.hutool.socket.nio.Operation valueOf(java.lang.String);
  public int getValue();
}
```
