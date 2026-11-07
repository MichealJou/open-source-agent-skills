# com.feilong.lib.org.apache.http.config

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.config.ConnectionConfig`

```java
public class com.feilong.lib.org.apache.http.config.ConnectionConfig implements java.lang.Cloneable {
  public int getBufferSize();
  public int getFragmentSizeHint();
  public java.nio.charset.Charset getCharset();
  public java.nio.charset.CodingErrorAction getMalformedInputAction();
  public java.nio.charset.CodingErrorAction getUnmappableInputAction();
  public com.feilong.lib.org.apache.http.config.MessageConstraints getMessageConstraints();
  public java.lang.String toString();
  public static com.feilong.lib.org.apache.http.config.ConnectionConfig$Builder custom();
  public static com.feilong.lib.org.apache.http.config.ConnectionConfig$Builder copy(com.feilong.lib.org.apache.http.config.ConnectionConfig);
}
```

## `com.feilong.lib.org.apache.http.config.ConnectionConfig$Builder`

```java
public class com.feilong.lib.org.apache.http.config.ConnectionConfig$Builder {
  public com.feilong.lib.org.apache.http.config.ConnectionConfig$Builder setBufferSize(int);
  public com.feilong.lib.org.apache.http.config.ConnectionConfig$Builder setFragmentSizeHint(int);
  public com.feilong.lib.org.apache.http.config.ConnectionConfig$Builder setCharset(java.nio.charset.Charset);
  public com.feilong.lib.org.apache.http.config.ConnectionConfig$Builder setMalformedInputAction(java.nio.charset.CodingErrorAction);
  public com.feilong.lib.org.apache.http.config.ConnectionConfig$Builder setUnmappableInputAction(java.nio.charset.CodingErrorAction);
  public com.feilong.lib.org.apache.http.config.ConnectionConfig$Builder setMessageConstraints(com.feilong.lib.org.apache.http.config.MessageConstraints);
  public com.feilong.lib.org.apache.http.config.ConnectionConfig build();
}
```

## `com.feilong.lib.org.apache.http.config.Lookup`

```java
public interface com.feilong.lib.org.apache.http.config.Lookup<I> {
  public abstract I lookup(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.config.MessageConstraints`

```java
public class com.feilong.lib.org.apache.http.config.MessageConstraints implements java.lang.Cloneable {
  public int getMaxLineLength();
  public int getMaxHeaderCount();
  public java.lang.String toString();
  public static com.feilong.lib.org.apache.http.config.MessageConstraints lineLen(int);
  public static com.feilong.lib.org.apache.http.config.MessageConstraints$Builder custom();
  public static com.feilong.lib.org.apache.http.config.MessageConstraints$Builder copy(com.feilong.lib.org.apache.http.config.MessageConstraints);
}
```

## `com.feilong.lib.org.apache.http.config.MessageConstraints$Builder`

```java
public class com.feilong.lib.org.apache.http.config.MessageConstraints$Builder {
  public com.feilong.lib.org.apache.http.config.MessageConstraints$Builder setMaxLineLength(int);
  public com.feilong.lib.org.apache.http.config.MessageConstraints$Builder setMaxHeaderCount(int);
  public com.feilong.lib.org.apache.http.config.MessageConstraints build();
}
```

## `com.feilong.lib.org.apache.http.config.Registry`

```java
public final class com.feilong.lib.org.apache.http.config.Registry<I> implements com.feilong.lib.org.apache.http.config.Lookup<I> {
  public I lookup(java.lang.String);
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.config.RegistryBuilder`

```java
public final class com.feilong.lib.org.apache.http.config.RegistryBuilder<I> {
  public static <I> com.feilong.lib.org.apache.http.config.RegistryBuilder<I> create();
  public com.feilong.lib.org.apache.http.config.RegistryBuilder<I> register(java.lang.String, I);
  public com.feilong.lib.org.apache.http.config.Registry<I> build();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.config.SocketConfig`

```java
public class com.feilong.lib.org.apache.http.config.SocketConfig implements java.lang.Cloneable {
  public int getSoTimeout();
  public boolean isSoReuseAddress();
  public int getSoLinger();
  public boolean isSoKeepAlive();
  public boolean isTcpNoDelay();
  public int getSndBufSize();
  public int getRcvBufSize();
  public int getBacklogSize();
  public java.lang.String toString();
  public static com.feilong.lib.org.apache.http.config.SocketConfig$Builder custom();
  public static com.feilong.lib.org.apache.http.config.SocketConfig$Builder copy(com.feilong.lib.org.apache.http.config.SocketConfig);
}
```

## `com.feilong.lib.org.apache.http.config.SocketConfig$Builder`

```java
public class com.feilong.lib.org.apache.http.config.SocketConfig$Builder {
  public com.feilong.lib.org.apache.http.config.SocketConfig$Builder setSoTimeout(int);
  public com.feilong.lib.org.apache.http.config.SocketConfig$Builder setSoReuseAddress(boolean);
  public com.feilong.lib.org.apache.http.config.SocketConfig$Builder setSoLinger(int);
  public com.feilong.lib.org.apache.http.config.SocketConfig$Builder setSoKeepAlive(boolean);
  public com.feilong.lib.org.apache.http.config.SocketConfig$Builder setTcpNoDelay(boolean);
  public com.feilong.lib.org.apache.http.config.SocketConfig$Builder setSndBufSize(int);
  public com.feilong.lib.org.apache.http.config.SocketConfig$Builder setRcvBufSize(int);
  public com.feilong.lib.org.apache.http.config.SocketConfig$Builder setBacklogSize(int);
  public com.feilong.lib.org.apache.http.config.SocketConfig build();
}
```
