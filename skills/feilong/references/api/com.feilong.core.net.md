# com.feilong.core.net

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.core.net.ParamUtil`

```java
public final class com.feilong.core.net.ParamUtil {
  public static java.lang.String addParameter(java.lang.String, java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String addParameterSingleValueMap(java.lang.String, java.util.Map<java.lang.String, java.lang.String>, java.lang.String);
  public static java.lang.String addParameterArrayValueMap(java.lang.String, java.util.Map<java.lang.String, java.lang.String[]>, java.lang.String);
  public static java.util.Map<java.lang.String, java.lang.String> toSingleValueMap(java.lang.String, java.lang.String);
  public static java.lang.String toNaturalOrderingKeyJoinValue(java.util.Map<java.lang.String, java.lang.String>);
  public static java.lang.String toNaturalOrderingJoinValue(java.util.Map<java.lang.String, java.lang.String>);
  public static java.lang.String toNaturalOrderingQueryString(java.util.Map<java.lang.String, java.lang.String>);
  public static java.lang.String toQueryStringUseSingleValueMap(java.util.Map<java.lang.String, java.lang.String>);
  public static java.lang.String toQueryStringUseArrayValueMap(java.util.Map<java.lang.String, java.lang.String[]>);
  public static <K> java.lang.String joinValuesOrderByIncludeKeys(java.util.Map<K, java.lang.String>, K...);
}
```

## `com.feilong.core.net.URIParseException`

```java
public final class com.feilong.core.net.URIParseException extends com.feilong.core.DefaultRuntimeException {
  public com.feilong.core.net.URIParseException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.core.net.URIUtil`

```java
public final class com.feilong.core.net.URIUtil {
  public static java.net.URI create(java.lang.String);
  public static java.net.URI create(java.lang.String, java.lang.String);
  public static java.lang.String encodeUri(java.lang.String, java.lang.String);
  public static java.lang.String encode(java.lang.String);
  public static java.lang.String encode(java.lang.String, java.lang.String);
  public static java.lang.String decode(java.lang.String);
  public static java.lang.String decodeIfExceptionDefault(java.lang.String, java.lang.String);
  public static java.lang.String decodeIfExceptionDefault(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String decode(java.lang.String, java.lang.String);
}
```

## `com.feilong.core.net.URLUtil`

```java
public final class com.feilong.core.net.URLUtil {
  public static java.net.URL toURL(java.lang.String);
  public static java.net.URI toURI(java.net.URL);
  public static java.io.InputStream openStream(java.net.URL);
  public static java.lang.String getUnionUrl(java.net.URL, java.lang.String);
  public static java.lang.String getUnionUrl(java.lang.String, java.lang.String);
  public static java.lang.String ifNoHttpOrHttpsProtocolPrependPre(java.lang.String, java.lang.String);
  public static java.lang.String ifNoProtocolPrependPre(java.lang.String, java.lang.String[], java.lang.String);
  public static java.lang.String transformHttpToHttps(java.lang.String);
  public static java.lang.String transformHttpsToHttp(java.lang.String);
  public static java.lang.String transformProtocol(java.lang.String, java.lang.String, java.lang.String);
}
```
