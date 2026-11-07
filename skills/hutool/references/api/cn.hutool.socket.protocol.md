# cn.hutool.socket.protocol

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.socket.protocol.MsgDecoder`

```java
public interface cn.hutool.socket.protocol.MsgDecoder<T> {
  public abstract T decode(cn.hutool.socket.aio.AioSession, java.nio.ByteBuffer);
}
```

## `cn.hutool.socket.protocol.MsgEncoder`

```java
public interface cn.hutool.socket.protocol.MsgEncoder<T> {
  public abstract void encode(cn.hutool.socket.aio.AioSession, java.nio.ByteBuffer, T);
}
```
