# com.feilong.lib.org.apache.http.impl.pool

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.impl.pool.BasicConnFactory`

```java
public class com.feilong.lib.org.apache.http.impl.pool.BasicConnFactory implements com.feilong.lib.org.apache.http.pool.ConnFactory<com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpClientConnection> {
  public com.feilong.lib.org.apache.http.impl.pool.BasicConnFactory(javax.net.SocketFactory, javax.net.ssl.SSLSocketFactory, int, com.feilong.lib.org.apache.http.config.SocketConfig, com.feilong.lib.org.apache.http.config.ConnectionConfig);
  public com.feilong.lib.org.apache.http.impl.pool.BasicConnFactory(int, com.feilong.lib.org.apache.http.config.SocketConfig, com.feilong.lib.org.apache.http.config.ConnectionConfig);
  public com.feilong.lib.org.apache.http.impl.pool.BasicConnFactory(com.feilong.lib.org.apache.http.config.SocketConfig, com.feilong.lib.org.apache.http.config.ConnectionConfig);
  public com.feilong.lib.org.apache.http.impl.pool.BasicConnFactory();
  public com.feilong.lib.org.apache.http.HttpClientConnection create(com.feilong.lib.org.apache.http.HttpHost) throws java.io.IOException;
  public java.lang.Object create(java.lang.Object) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.impl.pool.BasicConnPool`

```java
public class com.feilong.lib.org.apache.http.impl.pool.BasicConnPool extends com.feilong.lib.org.apache.http.pool.AbstractConnPool<com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpClientConnection, com.feilong.lib.org.apache.http.impl.pool.BasicPoolEntry> {
  public com.feilong.lib.org.apache.http.impl.pool.BasicConnPool(com.feilong.lib.org.apache.http.pool.ConnFactory<com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpClientConnection>);
  public com.feilong.lib.org.apache.http.impl.pool.BasicConnPool(com.feilong.lib.org.apache.http.config.SocketConfig, com.feilong.lib.org.apache.http.config.ConnectionConfig);
  public com.feilong.lib.org.apache.http.impl.pool.BasicConnPool();
}
```

## `com.feilong.lib.org.apache.http.impl.pool.BasicPoolEntry`

```java
public class com.feilong.lib.org.apache.http.impl.pool.BasicPoolEntry extends com.feilong.lib.org.apache.http.pool.PoolEntry<com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpClientConnection> {
  public com.feilong.lib.org.apache.http.impl.pool.BasicPoolEntry(java.lang.String, com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpClientConnection);
  public void close();
  public boolean isClosed();
}
```
