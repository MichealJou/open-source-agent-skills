# com.feilong.lib.org.apache.http.conn.routing

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.conn.routing.BasicRouteDirector`

```java
public class com.feilong.lib.org.apache.http.conn.routing.BasicRouteDirector implements com.feilong.lib.org.apache.http.conn.routing.HttpRouteDirector {
  public com.feilong.lib.org.apache.http.conn.routing.BasicRouteDirector();
  public int nextStep(com.feilong.lib.org.apache.http.conn.routing.RouteInfo, com.feilong.lib.org.apache.http.conn.routing.RouteInfo);
}
```

## `com.feilong.lib.org.apache.http.conn.routing.HttpRoute`

```java
public final class com.feilong.lib.org.apache.http.conn.routing.HttpRoute implements com.feilong.lib.org.apache.http.conn.routing.RouteInfo,java.lang.Cloneable {
  public com.feilong.lib.org.apache.http.conn.routing.HttpRoute(com.feilong.lib.org.apache.http.HttpHost, java.net.InetAddress, com.feilong.lib.org.apache.http.HttpHost[], boolean, com.feilong.lib.org.apache.http.conn.routing.RouteInfo$TunnelType, com.feilong.lib.org.apache.http.conn.routing.RouteInfo$LayerType);
  public com.feilong.lib.org.apache.http.conn.routing.HttpRoute(com.feilong.lib.org.apache.http.HttpHost, java.net.InetAddress, com.feilong.lib.org.apache.http.HttpHost, boolean, com.feilong.lib.org.apache.http.conn.routing.RouteInfo$TunnelType, com.feilong.lib.org.apache.http.conn.routing.RouteInfo$LayerType);
  public com.feilong.lib.org.apache.http.conn.routing.HttpRoute(com.feilong.lib.org.apache.http.HttpHost, java.net.InetAddress, boolean);
  public com.feilong.lib.org.apache.http.conn.routing.HttpRoute(com.feilong.lib.org.apache.http.HttpHost);
  public com.feilong.lib.org.apache.http.conn.routing.HttpRoute(com.feilong.lib.org.apache.http.HttpHost, java.net.InetAddress, com.feilong.lib.org.apache.http.HttpHost, boolean);
  public com.feilong.lib.org.apache.http.conn.routing.HttpRoute(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpHost);
  public com.feilong.lib.org.apache.http.HttpHost getTargetHost();
  public java.net.InetAddress getLocalAddress();
  public java.net.InetSocketAddress getLocalSocketAddress();
  public int getHopCount();
  public com.feilong.lib.org.apache.http.HttpHost getHopTarget(int);
  public com.feilong.lib.org.apache.http.HttpHost getProxyHost();
  public com.feilong.lib.org.apache.http.conn.routing.RouteInfo$TunnelType getTunnelType();
  public boolean isTunnelled();
  public com.feilong.lib.org.apache.http.conn.routing.RouteInfo$LayerType getLayerType();
  public boolean isLayered();
  public boolean isSecure();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.conn.routing.HttpRouteDirector`

```java
public interface com.feilong.lib.org.apache.http.conn.routing.HttpRouteDirector {
  public abstract int nextStep(com.feilong.lib.org.apache.http.conn.routing.RouteInfo, com.feilong.lib.org.apache.http.conn.routing.RouteInfo);
}
```

## `com.feilong.lib.org.apache.http.conn.routing.HttpRoutePlanner`

```java
public interface com.feilong.lib.org.apache.http.conn.routing.HttpRoutePlanner {
  public abstract com.feilong.lib.org.apache.http.conn.routing.HttpRoute determineRoute(com.feilong.lib.org.apache.http.HttpHost, com.feilong.lib.org.apache.http.HttpRequest, com.feilong.lib.org.apache.http.protocol.HttpContext) throws com.feilong.lib.org.apache.http.HttpException;
}
```

## `com.feilong.lib.org.apache.http.conn.routing.RouteInfo`

```java
public interface com.feilong.lib.org.apache.http.conn.routing.RouteInfo {
  public abstract com.feilong.lib.org.apache.http.HttpHost getTargetHost();
  public abstract java.net.InetAddress getLocalAddress();
  public abstract int getHopCount();
  public abstract com.feilong.lib.org.apache.http.HttpHost getHopTarget(int);
  public abstract com.feilong.lib.org.apache.http.HttpHost getProxyHost();
  public abstract com.feilong.lib.org.apache.http.conn.routing.RouteInfo$TunnelType getTunnelType();
  public abstract boolean isTunnelled();
  public abstract com.feilong.lib.org.apache.http.conn.routing.RouteInfo$LayerType getLayerType();
  public abstract boolean isLayered();
  public abstract boolean isSecure();
}
```

## `com.feilong.lib.org.apache.http.conn.routing.RouteInfo$LayerType`

```java
public final class com.feilong.lib.org.apache.http.conn.routing.RouteInfo$LayerType extends java.lang.Enum<com.feilong.lib.org.apache.http.conn.routing.RouteInfo$LayerType> {
  public static com.feilong.lib.org.apache.http.conn.routing.RouteInfo$LayerType[] values();
  public static com.feilong.lib.org.apache.http.conn.routing.RouteInfo$LayerType valueOf(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.conn.routing.RouteInfo$TunnelType`

```java
public final class com.feilong.lib.org.apache.http.conn.routing.RouteInfo$TunnelType extends java.lang.Enum<com.feilong.lib.org.apache.http.conn.routing.RouteInfo$TunnelType> {
  public static com.feilong.lib.org.apache.http.conn.routing.RouteInfo$TunnelType[] values();
  public static com.feilong.lib.org.apache.http.conn.routing.RouteInfo$TunnelType valueOf(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.conn.routing.RouteTracker`

```java
public final class com.feilong.lib.org.apache.http.conn.routing.RouteTracker implements com.feilong.lib.org.apache.http.conn.routing.RouteInfo,java.lang.Cloneable {
  public com.feilong.lib.org.apache.http.conn.routing.RouteTracker(com.feilong.lib.org.apache.http.HttpHost, java.net.InetAddress);
  public void reset();
  public com.feilong.lib.org.apache.http.conn.routing.RouteTracker(com.feilong.lib.org.apache.http.conn.routing.HttpRoute);
  public void connectTarget(boolean);
  public void connectProxy(com.feilong.lib.org.apache.http.HttpHost, boolean);
  public void tunnelTarget(boolean);
  public void tunnelProxy(com.feilong.lib.org.apache.http.HttpHost, boolean);
  public void layerProtocol(boolean);
  public com.feilong.lib.org.apache.http.HttpHost getTargetHost();
  public java.net.InetAddress getLocalAddress();
  public int getHopCount();
  public com.feilong.lib.org.apache.http.HttpHost getHopTarget(int);
  public com.feilong.lib.org.apache.http.HttpHost getProxyHost();
  public boolean isConnected();
  public com.feilong.lib.org.apache.http.conn.routing.RouteInfo$TunnelType getTunnelType();
  public boolean isTunnelled();
  public com.feilong.lib.org.apache.http.conn.routing.RouteInfo$LayerType getLayerType();
  public boolean isLayered();
  public boolean isSecure();
  public com.feilong.lib.org.apache.http.conn.routing.HttpRoute toRoute();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```
