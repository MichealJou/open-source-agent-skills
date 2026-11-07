# com.feilong.lib.org.apache.http.conn.socket

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.conn.socket.ConnectionSocketFactory`

```java
public interface com.feilong.lib.org.apache.http.conn.socket.ConnectionSocketFactory {
  public abstract java.net.Socket createSocket(com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public abstract java.net.Socket connectSocket(int, java.net.Socket, com.feilong.lib.org.apache.http.HttpHost, java.net.InetSocketAddress, java.net.InetSocketAddress, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.conn.socket.LayeredConnectionSocketFactory`

```java
public interface com.feilong.lib.org.apache.http.conn.socket.LayeredConnectionSocketFactory extends com.feilong.lib.org.apache.http.conn.socket.ConnectionSocketFactory {
  public abstract java.net.Socket createLayeredSocket(java.net.Socket, java.lang.String, int, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException, java.net.UnknownHostException;
}
```

## `com.feilong.lib.org.apache.http.conn.socket.PlainConnectionSocketFactory`

```java
public class com.feilong.lib.org.apache.http.conn.socket.PlainConnectionSocketFactory implements com.feilong.lib.org.apache.http.conn.socket.ConnectionSocketFactory {
  public static com.feilong.lib.org.apache.http.conn.socket.PlainConnectionSocketFactory getSocketFactory();
  public com.feilong.lib.org.apache.http.conn.socket.PlainConnectionSocketFactory();
  public java.net.Socket createSocket(com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
  public java.net.Socket connectSocket(int, java.net.Socket, com.feilong.lib.org.apache.http.HttpHost, java.net.InetSocketAddress, java.net.InetSocketAddress, com.feilong.lib.org.apache.http.protocol.HttpContext) throws java.io.IOException;
}
```
