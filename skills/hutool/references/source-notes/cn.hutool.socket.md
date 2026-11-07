# cn.hutool.socket

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.socket.ChannelUtil` | `AsynchronousChannelGroup createFixedGroup(int poolSize)` | 创建AsynchronousChannelGroup |
| `cn.hutool.socket.ChannelUtil` | `AsynchronousSocketChannel connect(AsynchronousChannelGroup group,InetSocketAddress address)` | 连接到指定地址 |
| `cn.hutool.socket.SocketConfig` | `int getReadBufferSize()` | 获取读取缓存大小 |
| `cn.hutool.socket.SocketConfig` | `int getThreadPoolSize()` | 获取共享线程池大小，此线程池用于接收和处理用户连接 |
| `cn.hutool.socket.SocketConfig` | `int getWriteBufferSize()` | 获取写出缓存大小 |
| `cn.hutool.socket.SocketConfig` | `long getReadTimeout()` | 获取读取超时时长，小于等于0表示默认 |
| `cn.hutool.socket.SocketConfig` | `long getWriteTimeout()` | 获取写出超时时长，小于等于0表示默认 |
| `cn.hutool.socket.SocketConfig` | `void setReadBufferSize(int readBufferSize)` | 设置读取缓存大小 |
| `cn.hutool.socket.SocketConfig` | `void setReadTimeout(long readTimeout)` | 设置读取超时时长，小于等于0表示默认 |
| `cn.hutool.socket.SocketConfig` | `void setThreadPoolSize(int threadPoolSize)` | 设置共享线程池大小，此线程池用于接收和处理用户连接 |
| `cn.hutool.socket.SocketConfig` | `void setWriteBufferSize(int writeBufferSize)` | 设置写出缓存大小 |
| `cn.hutool.socket.SocketConfig` | `void setWriteTimeout(long writeTimeout)` | 设置写出超时时长，小于等于0表示默认 |
| `cn.hutool.socket.SocketUtil` | `Socket connect(InetSocketAddress address,int connectionTimeout)` | 创建Socket并连接到指定地址的服务器 |
| `cn.hutool.socket.SocketUtil` | `Socket connect(String hostname,int port)` | 创建Socket并连接到指定地址的服务器 |
| `cn.hutool.socket.SocketUtil` | `Socket connect(final String hostname,int port,int connectionTimeout)` | 创建Socket并连接到指定地址的服务器 |
| `cn.hutool.socket.SocketUtil` | `SocketAddress getRemoteAddress(AsynchronousSocketChannel channel)` | 获取远程端的地址信息，包括host和端口 null表示channel为null或者远程主机未连接 |
| `cn.hutool.socket.SocketUtil` | `boolean isConnected(AsynchronousSocketChannel channel)` | 远程主机是否处于连接状态 通过判断远程地址获取成功与否判断 |
