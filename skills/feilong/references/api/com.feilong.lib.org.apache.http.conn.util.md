# com.feilong.lib.org.apache.http.conn.util

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.conn.util.DnsUtils`

```java
public class com.feilong.lib.org.apache.http.conn.util.DnsUtils {
  public static java.lang.String normalize(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.conn.util.DomainType`

```java
public final class com.feilong.lib.org.apache.http.conn.util.DomainType extends java.lang.Enum<com.feilong.lib.org.apache.http.conn.util.DomainType> {
  public static com.feilong.lib.org.apache.http.conn.util.DomainType[] values();
  public static com.feilong.lib.org.apache.http.conn.util.DomainType valueOf(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.conn.util.InetAddressUtils`

```java
public class com.feilong.lib.org.apache.http.conn.util.InetAddressUtils {
  public static boolean isIPv4Address(java.lang.String);
  public static boolean isIPv4MappedIPv64Address(java.lang.String);
  public static boolean isIPv6StdAddress(java.lang.String);
  public static boolean isIPv6HexCompressedAddress(java.lang.String);
  public static boolean isIPv6Address(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.conn.util.PublicSuffixList`

```java
public final class com.feilong.lib.org.apache.http.conn.util.PublicSuffixList {
  public com.feilong.lib.org.apache.http.conn.util.PublicSuffixList(com.feilong.lib.org.apache.http.conn.util.DomainType, java.util.List<java.lang.String>, java.util.List<java.lang.String>);
  public com.feilong.lib.org.apache.http.conn.util.PublicSuffixList(java.util.List<java.lang.String>, java.util.List<java.lang.String>);
  public com.feilong.lib.org.apache.http.conn.util.DomainType getType();
  public java.util.List<java.lang.String> getRules();
  public java.util.List<java.lang.String> getExceptions();
}
```

## `com.feilong.lib.org.apache.http.conn.util.PublicSuffixListParser`

```java
public final class com.feilong.lib.org.apache.http.conn.util.PublicSuffixListParser {
  public com.feilong.lib.org.apache.http.conn.util.PublicSuffixListParser();
  public com.feilong.lib.org.apache.http.conn.util.PublicSuffixList parse(java.io.Reader) throws java.io.IOException;
  public java.util.List<com.feilong.lib.org.apache.http.conn.util.PublicSuffixList> parseByType(java.io.Reader) throws java.io.IOException;
}
```

## `com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher`

```java
public final class com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher {
  public com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher(java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>);
  public com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher(com.feilong.lib.org.apache.http.conn.util.DomainType, java.util.Collection<java.lang.String>, java.util.Collection<java.lang.String>);
  public com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher(java.util.Collection<com.feilong.lib.org.apache.http.conn.util.PublicSuffixList>);
  public java.lang.String getDomainRoot(java.lang.String);
  public java.lang.String getDomainRoot(java.lang.String, com.feilong.lib.org.apache.http.conn.util.DomainType);
  public boolean matches(java.lang.String);
  public boolean matches(java.lang.String, com.feilong.lib.org.apache.http.conn.util.DomainType);
}
```

## `com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcherLoader`

```java
public final class com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcherLoader {
  public com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcherLoader();
  public static com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher load(java.net.URL) throws java.io.IOException;
  public static com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher load(java.io.File) throws java.io.IOException;
  public static com.feilong.lib.org.apache.http.conn.util.PublicSuffixMatcher getDefault();
}
```
