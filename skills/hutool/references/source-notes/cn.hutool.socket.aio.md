# cn.hutool.socket.aio

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.socket.aio.AcceptHandler` | `void completed(AsynchronousSocketChannel socketChannel,AioServer aioServer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.socket.aio.AcceptHandler` | `void failed(Throwable exc,AioServer aioServer)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.socket.aio.AioClient` | `AioClient read()` | 从服务端读取数据 |
| `cn.hutool.socket.aio.AioClient` | `AioClient setOption(SocketOption<T> name,T value)` | 设置 Socket 的 Option 选项 选项见：java.net.StandardSocketOptions |
| `cn.hutool.socket.aio.AioClient` | `AioClient write(ByteBuffer data)` | 写数据到服务端 |
| `cn.hutool.socket.aio.AioClient` | `IoAction<ByteBuffer> getIoAction()` | 获取IO处理器 |
| `cn.hutool.socket.aio.AioClient` | `void close()` | 关闭客户端 |
| `cn.hutool.socket.aio.AioServer` | `AioServer accept()` | 处理接入的客户端 |
| `cn.hutool.socket.aio.AioServer` | `AioServer init(InetSocketAddress address)` | 初始化 |
| `cn.hutool.socket.aio.AioServer` | `AioServer setIoAction(IoAction<ByteBuffer> ioAction)` | 设置IO处理器，单例存在 |
| `cn.hutool.socket.aio.AioServer` | `AioServer setOption(SocketOption<T> name,T value)` | 设置 Socket 的 Option 选项 选项见：java.net.StandardSocketOptions |
| `cn.hutool.socket.aio.AioServer` | `AsynchronousServerSocketChannel getChannel()` | 获取AsynchronousServerSocketChannel |
| `cn.hutool.socket.aio.AioServer` | `IoAction<ByteBuffer> getIoAction()` | 获取IO处理器 |
| `cn.hutool.socket.aio.AioServer` | `boolean isOpen()` | 服务是否开启状态 |
| `cn.hutool.socket.aio.AioServer` | `void close()` | 关闭服务 |
| `cn.hutool.socket.aio.AioServer` | `void start(boolean sync)` | 开始监听 |
| `cn.hutool.socket.aio.AioSession` | `AioSession closeIn()` | 关闭输出 |
| `cn.hutool.socket.aio.AioSession` | `AioSession closeOut()` | 关闭输出 |
| `cn.hutool.socket.aio.AioSession` | `AioSession read()` | 读取数据到Buffer |
| `cn.hutool.socket.aio.AioSession` | `AioSession read(CompletionHandler<Integer, AioSession> handler)` | 读取数据到Buffer |
| `cn.hutool.socket.aio.AioSession` | `AioSession write(ByteBuffer data,CompletionHandler<Integer, AioSession> handler)` | 写数据到目标端 |
| `cn.hutool.socket.aio.AioSession` | `AioSession writeAndClose(ByteBuffer data)` | 写数据到目标端，并关闭输出 |
| `cn.hutool.socket.aio.AioSession` | `AsynchronousSocketChannel getChannel()` | 获取AsynchronousSocketChannel |
| `cn.hutool.socket.aio.AioSession` | `ByteBuffer getReadBuffer()` | 获取读取Buffer |
| `cn.hutool.socket.aio.AioSession` | `ByteBuffer getWriteBuffer()` | 获取写Buffer |
| `cn.hutool.socket.aio.AioSession` | `Future<Integer> write(ByteBuffer data)` | 写数据到目标端 |
| `cn.hutool.socket.aio.AioSession` | `IoAction<ByteBuffer> getIoAction()` | 获取消息处理器 |
| `cn.hutool.socket.aio.AioSession` | `SocketAddress getRemoteAddress()` | 获取远程主机（客户端）地址和端口 |
| `cn.hutool.socket.aio.AioSession` | `boolean isOpen()` | 会话是否打开状态 当Socket保持连接时会话始终打开 |
| `cn.hutool.socket.aio.AioSession` | `void close()` | 关闭会话 |
| `cn.hutool.socket.aio.IoAction` | `void accept(AioSession session)` | 接收客户端连接（会话建立）事件处理 |
| `cn.hutool.socket.aio.IoAction` | `void doAction(AioSession session,T data)` | 执行数据处理（消息读取） |
| `cn.hutool.socket.aio.IoAction` | `void failed(Throwable exc,AioSession session)` | 数据读取失败的回调事件处理（消息读取失败） |
| `cn.hutool.socket.aio.ReadHandler` | `void completed(Integer result,AioSession session)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.socket.aio.ReadHandler` | `void failed(Throwable exc,AioSession session)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.socket.aio.SimpleIoAction` | `void accept(AioSession session)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.socket.aio.SimpleIoAction` | `void failed(Throwable exc,AioSession session)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
