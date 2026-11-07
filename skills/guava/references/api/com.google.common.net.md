# com.google.common.net

版本：33.4.8-jre。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.google.common.net.HostAndPort`

```java
public final class com.google.common.net.HostAndPort implements java.io.Serializable {
  public java.lang.String getHost();
  public boolean hasPort();
  public int getPort();
  public int getPortOrDefault(int);
  public static com.google.common.net.HostAndPort fromParts(java.lang.String, int);
  public static com.google.common.net.HostAndPort fromHost(java.lang.String);
  public static com.google.common.net.HostAndPort fromString(java.lang.String);
  public com.google.common.net.HostAndPort withDefaultPort(int);
  public com.google.common.net.HostAndPort requireBracketsForIPv6();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.google.common.net.HostSpecifier`

```java
public final class com.google.common.net.HostSpecifier {
  public static com.google.common.net.HostSpecifier fromValid(java.lang.String);
  public static com.google.common.net.HostSpecifier from(java.lang.String) throws java.text.ParseException;
  public static boolean isValid(java.lang.String);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.google.common.net.InetAddresses`

```java
public final class com.google.common.net.InetAddresses {
  public static java.net.InetAddress forString(java.lang.String);
  public static boolean isInetAddress(java.lang.String);
  public static java.lang.String toAddrString(java.net.InetAddress);
  public static java.lang.String toUriString(java.net.InetAddress);
  public static java.net.InetAddress forUriString(java.lang.String);
  public static boolean isUriInetAddress(java.lang.String);
  public static boolean isCompatIPv4Address(java.net.Inet6Address);
  public static java.net.Inet4Address getCompatIPv4Address(java.net.Inet6Address);
  public static boolean is6to4Address(java.net.Inet6Address);
  public static java.net.Inet4Address get6to4IPv4Address(java.net.Inet6Address);
  public static boolean isTeredoAddress(java.net.Inet6Address);
  public static com.google.common.net.InetAddresses$TeredoInfo getTeredoInfo(java.net.Inet6Address);
  public static boolean isIsatapAddress(java.net.Inet6Address);
  public static java.net.Inet4Address getIsatapIPv4Address(java.net.Inet6Address);
  public static boolean hasEmbeddedIPv4ClientAddress(java.net.Inet6Address);
  public static java.net.Inet4Address getEmbeddedIPv4ClientAddress(java.net.Inet6Address);
  public static boolean isMappedIPv4Address(java.lang.String);
  public static java.net.Inet4Address getCoercedIPv4Address(java.net.InetAddress);
  public static int coerceToInteger(java.net.InetAddress);
  public static java.math.BigInteger toBigInteger(java.net.InetAddress);
  public static java.net.Inet4Address fromInteger(int);
  public static java.net.Inet4Address fromIPv4BigInteger(java.math.BigInteger);
  public static java.net.Inet6Address fromIPv6BigInteger(java.math.BigInteger);
  public static java.net.InetAddress fromLittleEndianByteArray(byte[]) throws java.net.UnknownHostException;
  public static java.net.InetAddress decrement(java.net.InetAddress);
  public static java.net.InetAddress increment(java.net.InetAddress);
  public static boolean isMaximum(java.net.InetAddress);
}
```

## `com.google.common.net.InetAddresses$TeredoInfo`

```java
public final class com.google.common.net.InetAddresses$TeredoInfo {
  public com.google.common.net.InetAddresses$TeredoInfo(java.net.Inet4Address, java.net.Inet4Address, int, int);
  public java.net.Inet4Address getServer();
  public java.net.Inet4Address getClient();
  public int getPort();
  public int getFlags();
}
```

## `com.google.common.net.InternetDomainName`

```java
public final class com.google.common.net.InternetDomainName {
  public static com.google.common.net.InternetDomainName from(java.lang.String);
  public com.google.common.collect.ImmutableList<java.lang.String> parts();
  public boolean isPublicSuffix();
  public boolean hasPublicSuffix();
  public com.google.common.net.InternetDomainName publicSuffix();
  public boolean isUnderPublicSuffix();
  public boolean isTopPrivateDomain();
  public com.google.common.net.InternetDomainName topPrivateDomain();
  public boolean isRegistrySuffix();
  public boolean hasRegistrySuffix();
  public com.google.common.net.InternetDomainName registrySuffix();
  public boolean isUnderRegistrySuffix();
  public boolean isTopDomainUnderRegistrySuffix();
  public com.google.common.net.InternetDomainName topDomainUnderRegistrySuffix();
  public boolean hasParent();
  public com.google.common.net.InternetDomainName parent();
  public com.google.common.net.InternetDomainName child(java.lang.String);
  public static boolean isValid(java.lang.String);
  public java.lang.String toString();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.google.common.net.MediaType`

```java
public final class com.google.common.net.MediaType {
  public java.lang.String type();
  public java.lang.String subtype();
  public com.google.common.collect.ImmutableListMultimap<java.lang.String, java.lang.String> parameters();
  public com.google.common.base.Optional<java.nio.charset.Charset> charset();
  public com.google.common.net.MediaType withoutParameters();
  public com.google.common.net.MediaType withParameters(com.google.common.collect.Multimap<java.lang.String, java.lang.String>);
  public com.google.common.net.MediaType withParameters(java.lang.String, java.lang.Iterable<java.lang.String>);
  public com.google.common.net.MediaType withParameter(java.lang.String, java.lang.String);
  public com.google.common.net.MediaType withCharset(java.nio.charset.Charset);
  public boolean hasWildcard();
  public boolean is(com.google.common.net.MediaType);
  public static com.google.common.net.MediaType create(java.lang.String, java.lang.String);
  public static com.google.common.net.MediaType parse(java.lang.String);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.google.common.net.PercentEscaper`

```java
public final class com.google.common.net.PercentEscaper extends com.google.common.escape.UnicodeEscaper {
  public com.google.common.net.PercentEscaper(java.lang.String, boolean);
  public java.lang.String escape(java.lang.String);
}
```

## `com.google.common.net.UrlEscapers`

```java
public final class com.google.common.net.UrlEscapers {
  public static com.google.common.escape.Escaper urlFormParameterEscaper();
  public static com.google.common.escape.Escaper urlPathSegmentEscaper();
  public static com.google.common.escape.Escaper urlFragmentEscaper();
}
```
