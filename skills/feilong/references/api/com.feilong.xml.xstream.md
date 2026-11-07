# com.feilong.xml.xstream

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.xml.xstream.XStreamBuilder`

```java
public final class com.feilong.xml.xstream.XStreamBuilder {
  public static com.thoughtworks.xstream.XStream build(com.feilong.xml.xstream.XStreamConfig);
}
```

## `com.feilong.xml.xstream.XStreamConfig`

```java
public final class com.feilong.xml.xstream.XStreamConfig {
  public com.feilong.xml.xstream.XStreamConfig();
  public com.feilong.xml.xstream.XStreamConfig(java.util.Map<java.lang.String, java.lang.Class<?>>);
  public com.feilong.xml.xstream.XStreamConfig(java.lang.String, java.lang.Class<?>);
  public com.feilong.xml.xstream.XStreamConfig(java.lang.Class<?>...);
  public java.util.Map<java.lang.String, java.lang.Class<?>> getAliasMap();
  public void setAliasMap(java.util.Map<java.lang.String, java.lang.Class<?>>);
  public java.util.Map<java.lang.String, java.lang.Class<?>> getImplicitCollectionMap();
  public void setImplicitCollectionMap(java.util.Map<java.lang.String, java.lang.Class<?>>);
  public java.util.List<com.thoughtworks.xstream.converters.Converter> getConverterList();
  public void setConverterList(java.util.List<com.thoughtworks.xstream.converters.Converter>);
  public java.lang.Class<?>[] getProcessAnnotationsTypes();
  public void setProcessAnnotationsTypes(java.lang.Class<?>[]);
  public boolean getIsPrettyPrint();
  public void setIsPrettyPrint(boolean);
  public java.util.Map<java.lang.Class<?>, java.lang.Class<?>> getDefaultImplementationMap();
  public void setDefaultImplementationMap(java.util.Map<java.lang.Class<?>, java.lang.Class<?>>);
}
```

## `com.feilong.xml.xstream.XStreamConfigBuilder`

```java
public final class com.feilong.xml.xstream.XStreamConfigBuilder {
  public static com.feilong.xml.xstream.XStreamConfig buildSimpleMapXStreamConfig(java.lang.String);
  public static com.feilong.xml.xstream.XStreamConfig buildSimpleMapXStreamConfig(java.lang.String, boolean);
}
```
