# cn.hutool.socket.protocol

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.socket.protocol.MsgDecoder` | `T decode(AioSession session,ByteBuffer readBuffer)` | 对于从Socket流中获取到的数据采用当前MsgDecoder的实现类协议进行解析。 |
| `cn.hutool.socket.protocol.MsgEncoder` | `void encode(AioSession session,ByteBuffer writeBuffer,T data)` | 编码数据用于写出 |
