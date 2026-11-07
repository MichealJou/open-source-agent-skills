# com.feilong.json.builder

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.json.builder.JavaToJsonConfigBuilder`

```java
public final class com.feilong.json.builder.JavaToJsonConfigBuilder {
  public static com.feilong.json.JavaToJsonConfig buildUseJavaToJsonConfig(java.lang.Object, com.feilong.json.JavaToJsonConfig);
  public static com.feilong.json.JavaToJsonConfig buildDefaultJavaToJsonConfig(java.lang.Object);
  public static com.feilong.json.JavaToJsonConfig build(java.lang.String[], java.lang.String[]);
}
```

## `com.feilong.json.builder.JsonConfigBuilder`

```java
public final class com.feilong.json.builder.JsonConfigBuilder {
  public static com.feilong.lib.json.JsonConfig build(java.lang.Object, com.feilong.json.JavaToJsonConfig);
}
```

## `com.feilong.json.builder.JsonToJavaConfigBuilder`

```java
public final class com.feilong.json.builder.JsonToJavaConfigBuilder {
  public static com.feilong.lib.json.JsonConfig build(java.lang.Class<?>, com.feilong.json.JsonToJavaConfig);
}
```
