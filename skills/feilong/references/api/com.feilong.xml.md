# com.feilong.xml

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.xml.UncheckedXmlParseException`

```java
public final class com.feilong.xml.UncheckedXmlParseException extends com.feilong.core.DefaultRuntimeException {
  public com.feilong.xml.UncheckedXmlParseException(java.lang.String, java.lang.Throwable);
  public com.feilong.xml.UncheckedXmlParseException(java.lang.Throwable);
}
```

## `com.feilong.xml.XXEUtil`

```java
public final class com.feilong.xml.XXEUtil {
  public static javax.xml.parsers.DocumentBuilderFactory disableXXE(javax.xml.parsers.DocumentBuilderFactory);
}
```

## `com.feilong.xml.XmlUtil`

```java
public class com.feilong.xml.XmlUtil {
  public static java.util.Map<java.lang.String, java.lang.String> getNodeNameAndStringValueMap(java.lang.Object, java.lang.String);
  public static java.util.Map<java.lang.String, java.lang.String> getNodeAttributeValueAndStringValueMap(java.lang.Object, java.lang.String, java.lang.String);
  public static java.lang.String format(java.lang.String);
  public static <K, V> java.lang.String toXML(java.util.Map<K, V>, java.lang.String);
  public static <K, V> java.lang.String toXML(java.util.Map<K, V>, java.lang.String, boolean);
  public static java.lang.String toXML(java.lang.Object, com.feilong.xml.xstream.XStreamConfig);
  public static java.util.Map<java.lang.String, java.lang.String> toMap(java.lang.String, java.lang.String);
  public static <T> T toBean(java.lang.String, java.lang.Class<T>);
  public static <T> T toBean(java.lang.String, com.feilong.xml.xstream.XStreamConfig);
}
```
