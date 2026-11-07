# cn.hutool.socket.nio

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.socket.nio.AcceptHandler` | `void completed(ServerSocketChannel serverSocketChannel,NioServer nioServer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.socket.nio.AcceptHandler` | `void failed(Throwable exc,NioServer nioServer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.socket.nio.ChannelHandler` | `void handle(SocketChannel socketChannel)` | 处理NIO数据 |
| `cn.hutool.socket.nio.NioClient` | `NioClient init(InetSocketAddress address)` | 初始化 |
| `cn.hutool.socket.nio.NioClient` | `NioClient setChannelHandler(ChannelHandler handler)` | 设置NIO数据处理器 |
| `cn.hutool.socket.nio.NioClient` | `NioClient write(ByteBuffer... datas)` | 实现写逻辑 当收到写出准备就绪的信号后，回调此方法，用户可向客户端发送消息 |
| `cn.hutool.socket.nio.NioClient` | `SocketChannel getChannel()` | 获取SocketChannel |
| `cn.hutool.socket.nio.NioClient` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.socket.nio.NioClient` | `void listen()` | 开始监听 |
| `cn.hutool.socket.nio.NioServer` | `NioServer init(InetSocketAddress address)` | 初始化 |
| `cn.hutool.socket.nio.NioServer` | `NioServer setChannelHandler(ChannelHandler handler)` | 设置NIO数据处理器 |
| `cn.hutool.socket.nio.NioServer` | `Selector getSelector()` | 获取Selector |
| `cn.hutool.socket.nio.NioServer` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.socket.nio.NioServer` | `void listen()` | 开始监听 |
| `cn.hutool.socket.nio.NioServer` | `void start()` | 启动NIO服务端，即开始监听 |
| `cn.hutool.socket.nio.NioUtil` | `void registerChannel(Selector selector,SelectableChannel channel,Operation ops)` | 注册通道的指定操作到指定Selector上 |
| `cn.hutool.socket.nio.Operation` | `int getValue()` | 获取值 |
