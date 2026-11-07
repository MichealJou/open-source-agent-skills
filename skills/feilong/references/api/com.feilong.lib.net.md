# com.feilong.lib.net

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.net.DefaultSocketFactory`

```java
public class com.feilong.lib.net.DefaultSocketFactory extends javax.net.SocketFactory {
  public com.feilong.lib.net.DefaultSocketFactory(java.net.Proxy);
  public java.net.Socket createSocket() throws java.io.IOException;
  public java.net.Socket createSocket(java.lang.String, int) throws java.net.UnknownHostException, java.io.IOException;
  public java.net.Socket createSocket(java.net.InetAddress, int) throws java.io.IOException;
  public java.net.Socket createSocket(java.lang.String, int, java.net.InetAddress, int) throws java.net.UnknownHostException, java.io.IOException;
  public java.net.Socket createSocket(java.net.InetAddress, int, java.net.InetAddress, int) throws java.io.IOException;
  public java.net.ServerSocket createServerSocket(int) throws java.io.IOException;
  public java.net.ServerSocket createServerSocket(int, int) throws java.io.IOException;
  public java.net.ServerSocket createServerSocket(int, int, java.net.InetAddress) throws java.io.IOException;
}
```

## `com.feilong.lib.net.MalformedServerReplyException`

```java
public class com.feilong.lib.net.MalformedServerReplyException extends java.io.IOException {
  public com.feilong.lib.net.MalformedServerReplyException(java.lang.String);
}
```

## `com.feilong.lib.net.ProtocolCommandEvent`

```java
public class com.feilong.lib.net.ProtocolCommandEvent extends java.util.EventObject {
  public com.feilong.lib.net.ProtocolCommandEvent(java.lang.Object, java.lang.String, java.lang.String);
  public com.feilong.lib.net.ProtocolCommandEvent(java.lang.Object, int, java.lang.String);
  public java.lang.String getCommand();
  public int getReplyCode();
  public boolean isCommand();
  public boolean isReply();
  public java.lang.String getMessage();
}
```

## `com.feilong.lib.net.ProtocolCommandListener`

```java
public interface com.feilong.lib.net.ProtocolCommandListener extends java.util.EventListener {
  public abstract void protocolCommandSent(com.feilong.lib.net.ProtocolCommandEvent);
  public abstract void protocolReplyReceived(com.feilong.lib.net.ProtocolCommandEvent);
}
```

## `com.feilong.lib.net.ProtocolCommandSupport`

```java
public class com.feilong.lib.net.ProtocolCommandSupport implements java.io.Serializable {
  public com.feilong.lib.net.ProtocolCommandSupport(java.lang.Object);
  public void fireCommandSent(java.lang.String, java.lang.String);
  public void fireReplyReceived(int, java.lang.String);
  public void addProtocolCommandListener(com.feilong.lib.net.ProtocolCommandListener);
  public void removeProtocolCommandListener(com.feilong.lib.net.ProtocolCommandListener);
  public int getListenerCount();
}
```

## `com.feilong.lib.net.SocketClient`

```java
public abstract class com.feilong.lib.net.SocketClient {
  public com.feilong.lib.net.SocketClient();
  public void connect(java.net.InetAddress, int) throws java.net.SocketException, java.io.IOException;
  public void connect(java.lang.String, int) throws java.net.SocketException, java.io.IOException;
  public void connect(java.net.InetAddress, int, java.net.InetAddress, int) throws java.net.SocketException, java.io.IOException;
  public void connect(java.lang.String, int, java.net.InetAddress, int) throws java.net.SocketException, java.io.IOException;
  public void connect(java.net.InetAddress) throws java.net.SocketException, java.io.IOException;
  public void connect(java.lang.String) throws java.net.SocketException, java.io.IOException;
  public void disconnect() throws java.io.IOException;
  public boolean isConnected();
  public boolean isAvailable();
  public void setDefaultPort(int);
  public int getDefaultPort();
  public void setDefaultTimeout(int);
  public int getDefaultTimeout();
  public void setSoTimeout(int) throws java.net.SocketException;
  public void setSendBufferSize(int) throws java.net.SocketException;
  public void setReceiveBufferSize(int) throws java.net.SocketException;
  public int getSoTimeout() throws java.net.SocketException;
  public void setTcpNoDelay(boolean) throws java.net.SocketException;
  public boolean getTcpNoDelay() throws java.net.SocketException;
  public void setKeepAlive(boolean) throws java.net.SocketException;
  public boolean getKeepAlive() throws java.net.SocketException;
  public void setSoLinger(boolean, int) throws java.net.SocketException;
  public int getSoLinger() throws java.net.SocketException;
  public int getLocalPort();
  public java.net.InetAddress getLocalAddress();
  public int getRemotePort();
  public java.net.InetAddress getRemoteAddress();
  public boolean verifyRemote(java.net.Socket);
  public void setSocketFactory(javax.net.SocketFactory);
  public void setServerSocketFactory(javax.net.ServerSocketFactory);
  public void setConnectTimeout(int);
  public int getConnectTimeout();
  public javax.net.ServerSocketFactory getServerSocketFactory();
  public void addProtocolCommandListener(com.feilong.lib.net.ProtocolCommandListener);
  public void removeProtocolCommandListener(com.feilong.lib.net.ProtocolCommandListener);
  public void setProxy(java.net.Proxy);
  public java.net.Proxy getProxy();
  public java.nio.charset.Charset getCharset();
  public void setCharset(java.nio.charset.Charset);
}
```
