# cn.hutool.core.net

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.net.DefaultTrustManager`

```java
public class cn.hutool.core.net.DefaultTrustManager extends javax.net.ssl.X509ExtendedTrustManager {
  public cn.hutool.core.net.DefaultTrustManager();
  public java.security.cert.X509Certificate[] getAcceptedIssuers();
  public void checkClientTrusted(java.security.cert.X509Certificate[], java.lang.String);
  public void checkServerTrusted(java.security.cert.X509Certificate[], java.lang.String);
  public void checkClientTrusted(java.security.cert.X509Certificate[], java.lang.String, java.net.Socket);
  public void checkServerTrusted(java.security.cert.X509Certificate[], java.lang.String, java.net.Socket);
  public void checkClientTrusted(java.security.cert.X509Certificate[], java.lang.String, javax.net.ssl.SSLEngine);
  public void checkServerTrusted(java.security.cert.X509Certificate[], java.lang.String, javax.net.ssl.SSLEngine);
}
```

## `cn.hutool.core.net.FormUrlencoded`

```java
public class cn.hutool.core.net.FormUrlencoded {
  public cn.hutool.core.net.FormUrlencoded();
}
```

## `cn.hutool.core.net.Ipv4Util`

```java
public class cn.hutool.core.net.Ipv4Util {
  public cn.hutool.core.net.Ipv4Util();
  public static java.lang.String formatIpBlock(java.lang.String, java.lang.String);
  public static java.util.List<java.lang.String> list(java.lang.String, boolean);
  public static java.util.List<java.lang.String> list(java.lang.String, int, boolean);
  public static java.util.List<java.lang.String> list(java.lang.String, java.lang.String);
  public static java.lang.String longToIpv4(long);
  public static long ipv4ToLong(java.lang.String);
  public static long ipv4ToLong(java.lang.String, long);
  public static java.lang.String getBeginIpStr(java.lang.String, int);
  public static java.lang.Long getBeginIpLong(java.lang.String, int);
  public static java.lang.String getEndIpStr(java.lang.String, int);
  public static int getMaskBitByMask(java.lang.String);
  public static int countByMaskBit(int, boolean);
  public static java.lang.String getMaskByMaskBit(int);
  public static java.lang.String getMaskByIpRange(java.lang.String, java.lang.String);
  public static int countByIpRange(java.lang.String, java.lang.String);
  public static boolean isMaskValid(java.lang.String);
  public static boolean isMaskBitValid(int);
  public static boolean isInnerIP(java.lang.String);
  public static boolean matches(java.lang.String, java.lang.String);
  public static java.lang.Long getEndIpLong(java.lang.String, int);
}
```

## `cn.hutool.core.net.LocalPortGenerater`

```java
public class cn.hutool.core.net.LocalPortGenerater implements java.io.Serializable {
  public cn.hutool.core.net.LocalPortGenerater(int);
  public int generate();
}
```

## `cn.hutool.core.net.MaskBit`

```java
public class cn.hutool.core.net.MaskBit {
  public cn.hutool.core.net.MaskBit();
  public static java.lang.String get(int);
  public static java.lang.Integer getMaskBit(java.lang.String);
}
```

## `cn.hutool.core.net.NetUtil`

```java
public class cn.hutool.core.net.NetUtil {
  public cn.hutool.core.net.NetUtil();
  public static java.lang.String longToIpv4(long);
  public static long ipv4ToLong(java.lang.String);
  public static java.math.BigInteger ipv6ToBitInteger(java.lang.String);
  public static java.math.BigInteger ipv6ToBigInteger(java.lang.String);
  public static java.lang.String bigIntegerToIPv6(java.math.BigInteger);
  public static boolean isUsableLocalPort(int);
  public static boolean isValidPort(int);
  public static int getUsableLocalPort();
  public static int getUsableLocalPort(int);
  public static int getUsableLocalPort(int, int);
  public static java.util.TreeSet<java.lang.Integer> getUsableLocalPorts(int, int, int);
  public static boolean isInnerIP(java.lang.String);
  public static java.lang.String toAbsoluteUrl(java.lang.String, java.lang.String);
  public static java.lang.String hideIpPart(java.lang.String);
  public static java.lang.String hideIpPart(long);
  public static java.net.InetSocketAddress buildInetSocketAddress(java.lang.String, int);
  public static java.lang.String getIpByHost(java.lang.String);
  public static java.net.NetworkInterface getNetworkInterface(java.lang.String);
  public static java.util.Collection<java.net.NetworkInterface> getNetworkInterfaces();
  public static java.util.LinkedHashSet<java.lang.String> localIpv4s();
  public static java.util.LinkedHashSet<java.lang.String> localIpv6s();
  public static java.util.LinkedHashSet<java.lang.String> toIpList(java.util.Set<java.net.InetAddress>);
  public static java.util.LinkedHashSet<java.lang.String> localIps();
  public static java.util.LinkedHashSet<java.net.InetAddress> localAddressList(cn.hutool.core.lang.Filter<java.net.InetAddress>);
  public static java.util.LinkedHashSet<java.net.InetAddress> localAddressList(cn.hutool.core.lang.Filter<java.net.NetworkInterface>, cn.hutool.core.lang.Filter<java.net.InetAddress>);
  public static java.lang.String getLocalhostStr();
  public static java.net.InetAddress getLocalhost();
  public static java.lang.String getLocalMacAddress();
  public static java.lang.String getMacAddress(java.net.InetAddress);
  public static java.lang.String getMacAddress(java.net.InetAddress, java.lang.String);
  public static byte[] getHardwareAddress(java.net.InetAddress);
  public static byte[] getLocalHardwareAddress();
  public static java.lang.String getLocalHostName();
  public static java.net.InetSocketAddress createAddress(java.lang.String, int);
  public static void netCat(java.lang.String, int, boolean, java.nio.ByteBuffer) throws cn.hutool.core.io.IORuntimeException;
  public static void netCat(java.lang.String, int, byte[]) throws cn.hutool.core.io.IORuntimeException;
  public static boolean isInRange(java.lang.String, java.lang.String);
  public static java.lang.String idnToASCII(java.lang.String);
  public static java.lang.String getMultistageReverseProxyIp(java.lang.String);
  public static boolean isUnknown(java.lang.String);
  public static boolean ping(java.lang.String);
  public static boolean ping(java.lang.String, int);
  public static java.util.List<java.net.HttpCookie> parseCookies(java.lang.String);
  public static boolean isOpen(java.net.InetSocketAddress, int);
  public static void setGlobalAuthenticator(java.lang.String, char[]);
  public static void setGlobalAuthenticator(java.net.Authenticator);
  public static java.util.List<java.lang.String> getDnsInfo(java.lang.String, java.lang.String...);
}
```

## `cn.hutool.core.net.PassAuth`

```java
public class cn.hutool.core.net.PassAuth extends java.net.Authenticator {
  public static cn.hutool.core.net.PassAuth of(java.lang.String, char[]);
  public cn.hutool.core.net.PassAuth(java.lang.String, char[]);
}
```

## `cn.hutool.core.net.ProxySocketFactory`

```java
public class cn.hutool.core.net.ProxySocketFactory extends javax.net.SocketFactory {
  public static cn.hutool.core.net.ProxySocketFactory of(java.net.Proxy);
  public cn.hutool.core.net.ProxySocketFactory(java.net.Proxy);
  public java.net.Socket createSocket();
  public java.net.Socket createSocket(java.net.InetAddress, int) throws java.io.IOException;
  public java.net.Socket createSocket(java.net.InetAddress, int, java.net.InetAddress, int) throws java.io.IOException;
  public java.net.Socket createSocket(java.lang.String, int) throws java.io.IOException;
  public java.net.Socket createSocket(java.lang.String, int, java.net.InetAddress, int) throws java.io.IOException;
}
```

## `cn.hutool.core.net.RFC3986`

```java
public class cn.hutool.core.net.RFC3986 {
  public cn.hutool.core.net.RFC3986();
}
```

## `cn.hutool.core.net.SSLContextBuilder`

```java
public class cn.hutool.core.net.SSLContextBuilder implements cn.hutool.core.net.SSLProtocols, cn.hutool.core.builder.Builder<javax.net.ssl.SSLContext> {
  public cn.hutool.core.net.SSLContextBuilder();
  public static cn.hutool.core.net.SSLContextBuilder create();
  public cn.hutool.core.net.SSLContextBuilder setProtocol(java.lang.String);
  public cn.hutool.core.net.SSLContextBuilder setTrustManagers(javax.net.ssl.TrustManager...);
  public cn.hutool.core.net.SSLContextBuilder setKeyManagers(javax.net.ssl.KeyManager...);
  public cn.hutool.core.net.SSLContextBuilder setSecureRandom(java.security.SecureRandom);
  public javax.net.ssl.SSLContext build();
  public javax.net.ssl.SSLContext buildChecked() throws java.security.NoSuchAlgorithmException, java.security.KeyManagementException;
  public javax.net.ssl.SSLContext buildQuietly() throws cn.hutool.core.io.IORuntimeException;
  public java.lang.Object build();
}
```

## `cn.hutool.core.net.SSLUtil`

```java
public class cn.hutool.core.net.SSLUtil {
  public cn.hutool.core.net.SSLUtil();
  public static javax.net.ssl.SSLContext createSSLContext(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static javax.net.ssl.SSLContext createSSLContext(java.lang.String, javax.net.ssl.KeyManager, javax.net.ssl.TrustManager) throws cn.hutool.core.io.IORuntimeException;
  public static javax.net.ssl.SSLContext createSSLContext(java.lang.String, javax.net.ssl.KeyManager[], javax.net.ssl.TrustManager[]) throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.core.net.URLDecoder`

```java
public class cn.hutool.core.net.URLDecoder implements java.io.Serializable {
  public cn.hutool.core.net.URLDecoder();
  public static java.lang.String decodeForPath(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String decode(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String decode(java.lang.String, java.nio.charset.Charset, boolean);
  public static byte[] decode(byte[]);
  public static byte[] decode(byte[], boolean);
}
```

## `cn.hutool.core.net.URLEncodeUtil`

```java
public class cn.hutool.core.net.URLEncodeUtil {
  public cn.hutool.core.net.URLEncodeUtil();
  public static java.lang.String encodeAll(java.lang.String);
  public static java.lang.String encodeAll(java.lang.String, java.nio.charset.Charset) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.String encode(java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.String encode(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String encodeQuery(java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.String encodeQuery(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String encodePathSegment(java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.String encodePathSegment(java.lang.String, java.nio.charset.Charset);
  public static java.lang.String encodeFragment(java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.String encodeFragment(java.lang.String, java.nio.charset.Charset);
}
```

## `cn.hutool.core.net.URLEncoder`

```java
public class cn.hutool.core.net.URLEncoder implements java.io.Serializable {
  public static cn.hutool.core.net.URLEncoder createDefault();
  public static cn.hutool.core.net.URLEncoder createPathSegment();
  public static cn.hutool.core.net.URLEncoder createFragment();
  public static cn.hutool.core.net.URLEncoder createQuery();
  public static cn.hutool.core.net.URLEncoder createAll();
  public cn.hutool.core.net.URLEncoder();
  public void addSafeCharacter(char);
  public void removeSafeCharacter(char);
  public void setEncodeSpaceAsPlus(boolean);
  public java.lang.String encode(java.lang.String, java.nio.charset.Charset);
}
```

## `cn.hutool.core.net.UserPassAuthenticator`

```java
public class cn.hutool.core.net.UserPassAuthenticator extends java.net.Authenticator {
  public cn.hutool.core.net.UserPassAuthenticator(java.lang.String, char[]);
}
```
