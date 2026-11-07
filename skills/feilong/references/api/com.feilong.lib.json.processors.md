# com.feilong.lib.json.processors

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.json.processors.DefaultDefaultValueProcessor`

```java
public class com.feilong.lib.json.processors.DefaultDefaultValueProcessor implements com.feilong.lib.json.processors.DefaultValueProcessor {
  public com.feilong.lib.json.processors.DefaultDefaultValueProcessor();
  public java.lang.Object getDefaultValue(java.lang.Class<?>);
}
```

## `com.feilong.lib.json.processors.DefaultValueProcessor`

```java
public interface com.feilong.lib.json.processors.DefaultValueProcessor {
  public abstract java.lang.Object getDefaultValue(java.lang.Class<?>);
}
```

## `com.feilong.lib.json.processors.JsonValueProcessor`

```java
public interface com.feilong.lib.json.processors.JsonValueProcessor {
  public abstract java.lang.Object processArrayValue(java.lang.Object, com.feilong.lib.json.JsonConfig);
  public abstract java.lang.Object processObjectValue(java.lang.String, java.lang.Object, com.feilong.lib.json.JsonConfig);
}
```

## `com.feilong.lib.json.processors.JsonVerifier`

```java
public final class com.feilong.lib.json.processors.JsonVerifier {
  public static boolean isValidJsonValue(java.lang.Object);
}
```

## `com.feilong.lib.json.processors.PropertyNameProcessor`

```java
public interface com.feilong.lib.json.processors.PropertyNameProcessor {
  public abstract java.lang.String processPropertyName(java.lang.Class<?>, java.lang.String);
}
```

## `com.feilong.lib.json.processors.PropertyNameProcessorMatcher`

```java
public class com.feilong.lib.json.processors.PropertyNameProcessorMatcher {
  public com.feilong.lib.json.processors.PropertyNameProcessorMatcher();
  public static java.lang.Object getMatch(java.lang.Class<?>, java.util.Set);
}
```
