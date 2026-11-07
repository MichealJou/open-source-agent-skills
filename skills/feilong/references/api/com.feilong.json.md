# com.feilong.json

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.json.JavaToJsonConfig`

```java
public class com.feilong.json.JavaToJsonConfig extends com.feilong.json.AbstractConfig {
  public com.feilong.json.JavaToJsonConfig();
  public com.feilong.json.JavaToJsonConfig(boolean);
  public com.feilong.json.JavaToJsonConfig(boolean, java.lang.String[]);
  public com.feilong.json.JavaToJsonConfig(java.util.Map<java.lang.String, com.feilong.lib.json.processors.JsonValueProcessor>);
  public com.feilong.json.JavaToJsonConfig(java.lang.String[], java.lang.String[]);
  public java.lang.String[] getIncludes();
  public void setIncludes(java.lang.String...);
  public java.util.Map<java.lang.String, com.feilong.lib.json.processors.JsonValueProcessor> getPropertyNameAndJsonValueProcessorMap();
  public void setPropertyNameAndJsonValueProcessorMap(java.util.Map<java.lang.String, com.feilong.lib.json.processors.JsonValueProcessor>);
  public java.util.Map<java.lang.Class<?>, com.feilong.lib.json.processors.PropertyNameProcessor> getJsonTargetClassAndPropertyNameProcessorMap();
  public void setJsonTargetClassAndPropertyNameProcessorMap(java.util.Map<java.lang.Class<?>, com.feilong.lib.json.processors.PropertyNameProcessor>);
  public boolean getIsMaskDefaultSensitiveWords();
  public void setIsMaskDefaultSensitiveWords(boolean);
  public boolean getIsIgnoreNullValueElement();
  public void setIsIgnoreNullValueElement(boolean);
  public com.feilong.lib.json.util.PropertyFilter getPropertyFilter();
  public void setPropertyFilter(com.feilong.lib.json.util.PropertyFilter);
  public java.lang.String[] getIfIgnoreNullValueElementIncludes();
  public void setIfIgnoreNullValueElementIncludes(java.lang.String[]);
  public java.lang.String toString();
  public void setExcludes(java.lang.String[]);
  public java.lang.String[] getExcludes();
}
```

## `com.feilong.json.JsonHelper`

```java
public final class com.feilong.json.JsonHelper {
  public static com.feilong.lib.json.JSON toJSON(java.lang.Object, com.feilong.lib.json.JsonConfig);
  public static boolean isNeedConvertToJSONArray(java.lang.Object);
  public static boolean isCommonString(java.lang.Object);
}
```

## `com.feilong.json.JsonToJavaConfig`

```java
public class com.feilong.json.JsonToJavaConfig extends com.feilong.json.AbstractConfig {
  public com.feilong.json.JsonToJavaConfig();
  public com.feilong.json.JsonToJavaConfig(java.lang.Class<?>);
  public com.feilong.json.JsonToJavaConfig(java.lang.Class<?>, com.feilong.lib.json.util.JavaIdentifierTransformer);
  public com.feilong.json.JsonToJavaConfig(java.lang.Class<?>, java.util.Map<java.lang.String, java.lang.Class<?>>);
  public com.feilong.lib.json.util.JavaIdentifierTransformer getJavaIdentifierTransformer();
  public void setJavaIdentifierTransformer(com.feilong.lib.json.util.JavaIdentifierTransformer);
  public java.lang.Class<?> getRootClass();
  public void setRootClass(java.lang.Class<?>);
  public java.util.Map<java.lang.String, java.lang.Class<?>> getClassMap();
  public void setClassMap(java.util.Map<java.lang.String, java.lang.Class<?>>);
  public java.lang.String toString();
  public void setExcludes(java.lang.String[]);
  public java.lang.String[] getExcludes();
}
```

## `com.feilong.json.JsonToJavaException`

```java
public final class com.feilong.json.JsonToJavaException extends com.feilong.core.DefaultRuntimeException {
  public com.feilong.json.JsonToJavaException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.json.JsonUtil`

```java
public final class com.feilong.json.JsonUtil {
  public static java.lang.String format(java.lang.Object);
  public static java.lang.String format(java.lang.Object, boolean);
  public static java.lang.String format(java.lang.Object, boolean, java.lang.String...);
  public static <K, V> java.lang.String formatSimpleMap(java.util.Map<K, V>);
  public static <K, V> java.lang.String formatSimpleMap(java.util.Map<K, V>, java.lang.Class<?>...);
  public static java.lang.String toString(java.lang.Object);
  public static java.lang.String toString(java.lang.Object, java.lang.String...);
  public static java.lang.String toString(java.lang.Object, boolean);
  public static java.lang.String toString(java.lang.Object, boolean, java.lang.String...);
  public static java.lang.String toString(java.lang.Object, com.feilong.json.JavaToJsonConfig);
  public static java.lang.String format(java.lang.Object, java.lang.String...);
  public static java.lang.String format(java.lang.Object, java.lang.String[], int, int);
  public static java.lang.String formatWithIncludes(java.lang.Object, java.lang.String...);
  public static java.lang.String format(java.lang.Object, int, int);
  public static java.lang.String format(java.lang.Object, com.feilong.json.JavaToJsonConfig);
  public static java.lang.String format(java.lang.Object, com.feilong.json.JavaToJsonConfig, int, int);
  public static java.lang.String formatObjectFieldsNameAndValueMap(java.lang.Object);
  public static <T> T[] toArray(java.lang.String, com.feilong.json.JsonToJavaConfig);
  public static <T> java.util.List<T> toList(java.lang.String, java.lang.Class<T>);
  public static <T> java.util.List<T> toList(java.lang.String, com.feilong.json.JsonToJavaConfig);
  public static <T> java.util.Map<java.lang.String, T> toMap(java.lang.String);
  public static <T> java.util.Map<java.lang.String, T> toMap(java.lang.String, com.feilong.json.JsonToJavaConfig);
  public static <T> T toBean(java.lang.String, java.lang.Class<T>);
  public static <T> T toBean(java.lang.String, com.feilong.json.JsonToJavaConfig);
}
```
