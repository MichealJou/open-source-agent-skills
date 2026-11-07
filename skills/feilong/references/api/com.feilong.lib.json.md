# com.feilong.lib.json

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.json.JSON`

```java
public interface com.feilong.lib.json.JSON extends java.io.Serializable {
  public abstract int size();
  public abstract java.lang.String toString(int, int);
}
```

## `com.feilong.lib.json.JSONArray`

```java
public final class com.feilong.lib.json.JSONArray implements com.feilong.lib.json.JSON {
  public com.feilong.lib.json.JSONArray();
  public java.lang.Object get(int);
  public com.feilong.lib.json.JSONObject getJSONObject(int);
  public boolean isEmpty();
  public int size();
  public java.lang.String toString();
  public java.lang.String toString(int, int);
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```

## `com.feilong.lib.json.JSONArrayBuilder`

```java
public class com.feilong.lib.json.JSONArrayBuilder {
  public static com.feilong.lib.json.JSONArray build(java.lang.Object, com.feilong.lib.json.JsonConfig);
}
```

## `com.feilong.lib.json.JSONException`

```java
public class com.feilong.lib.json.JSONException extends com.feilong.core.DefaultRuntimeException {
  public com.feilong.lib.json.JSONException(java.lang.String);
  public com.feilong.lib.json.JSONException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.json.JSONNull`

```java
public final class com.feilong.lib.json.JSONNull implements com.feilong.lib.json.JSON {
  public static com.feilong.lib.json.JSONNull getInstance();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public int size();
  public java.lang.String toString();
  public java.lang.String toString(int, int);
}
```

## `com.feilong.lib.json.JSONObject`

```java
public final class com.feilong.lib.json.JSONObject implements com.feilong.lib.json.JSON {
  public com.feilong.lib.json.JSONObject();
  public com.feilong.lib.json.JSONObject(boolean);
  public com.feilong.lib.json.JSONObject accumulate(java.lang.String, java.lang.Object, com.feilong.lib.json.JsonConfig);
  public java.lang.Object get(java.lang.String);
  public boolean isNullObject();
  public java.util.Set<java.lang.String> keys();
  public java.util.List<java.lang.String> names(com.feilong.lib.json.JsonConfig);
  public int size();
  public java.lang.String toString();
  public java.lang.String toString(int, int);
}
```

## `com.feilong.lib.json.JSONObjectBuilder`

```java
public class com.feilong.lib.json.JSONObjectBuilder {
  public static com.feilong.lib.json.JSONObject build(java.lang.Object, com.feilong.lib.json.JsonConfig);
}
```

## `com.feilong.lib.json.JSONObjectToBeanUtil`

```java
public class com.feilong.lib.json.JSONObjectToBeanUtil {
  public static java.lang.Object toBean(com.feilong.lib.json.JSONObject, com.feilong.lib.json.JsonConfig);
}
```

## `com.feilong.lib.json.JSONObjectValueSetter`

```java
public class com.feilong.lib.json.JSONObjectValueSetter {
  public static com.feilong.lib.json.processors.DefaultValueProcessor findDefaultValueProcessor(java.lang.Class<?>, com.feilong.lib.json.JsonConfig);
}
```

## `com.feilong.lib.json.JSONSerializer`

```java
public class com.feilong.lib.json.JSONSerializer {
  public static java.lang.Object toJava(com.feilong.lib.json.JSON);
  public static com.feilong.lib.json.JSON toJSON(java.lang.Object);
  public static com.feilong.lib.json.JSON toJSON(java.lang.Object, com.feilong.lib.json.JsonConfig);
}
```

## `com.feilong.lib.json.JSONTokener`

```java
public class com.feilong.lib.json.JSONTokener {
  public com.feilong.lib.json.JSONTokener(java.lang.String);
  public void back();
  public char next();
  public java.lang.String next(int);
  public char nextClean();
  public java.lang.Object nextValue(com.feilong.lib.json.JsonConfig);
  public char peek();
  public void reset();
  public com.feilong.lib.json.JSONException syntaxError(java.lang.String);
  public java.lang.String toString();
}
```

## `com.feilong.lib.json.JSONTokenerParser`

```java
public class com.feilong.lib.json.JSONTokenerParser {
  public com.feilong.lib.json.JSONTokenerParser();
}
```

## `com.feilong.lib.json.JsonConfig`

```java
public class com.feilong.lib.json.JsonConfig {
  public com.feilong.lib.json.JsonConfig();
  public com.feilong.lib.json.processors.JsonValueProcessor findJsonValueProcessor(java.lang.Class<?>, java.lang.String);
  public int getArrayMode();
  public java.util.Map<java.lang.String, java.lang.Class<?>> getClassMap();
  public java.lang.Class<?> getCollectionType();
  public java.lang.String[] getExcludes();
  public com.feilong.lib.json.util.JavaIdentifierTransformer getJavaIdentifierTransformer();
  public com.feilong.lib.json.util.PropertyFilter getJavaPropertyFilter();
  public com.feilong.lib.json.util.PropertyFilter getJsonPropertyFilter();
  public java.util.Collection<java.lang.String> getMergedExcludes();
  public java.lang.Class<?> getRootClass();
  public void registerDefaultValueProcessor(java.lang.Class<?>, com.feilong.lib.json.processors.DefaultValueProcessor);
  public void registerJavaPropertyNameProcessor(java.lang.Class<?>, com.feilong.lib.json.processors.PropertyNameProcessor);
  public void registerJsonPropertyNameProcessor(java.lang.Class<?>, com.feilong.lib.json.processors.PropertyNameProcessor);
  public void registerJsonValueProcessor(java.lang.Class<?>, com.feilong.lib.json.processors.JsonValueProcessor);
  public void registerJsonValueProcessor(java.lang.String, com.feilong.lib.json.processors.JsonValueProcessor);
  public void setArrayMode(int);
  public void setClassMap(java.util.Map<java.lang.String, java.lang.Class<?>>);
  public void setCollectionType(java.lang.Class<?>);
  public void setExcludes(java.lang.String[]);
  public void setJavaIdentifierTransformer(com.feilong.lib.json.util.JavaIdentifierTransformer);
  public void setJavaPropertyFilter(com.feilong.lib.json.util.PropertyFilter);
  public void setJsonPropertyFilter(com.feilong.lib.json.util.PropertyFilter);
  public void setRootClass(java.lang.Class<?>);
  public com.feilong.lib.json.JsonConfig copy();
  public java.lang.String toString();
  public java.util.Map<java.lang.Class<?>, com.feilong.lib.json.processors.PropertyNameProcessor> getJavaPropertyNameProcessorMap();
  public java.util.Map<java.lang.Class<?>, com.feilong.lib.json.processors.DefaultValueProcessor> getDefaultValueMap();
  public java.util.Map<java.lang.Class<?>, com.feilong.lib.json.processors.PropertyNameProcessor> getJsonPropertyNameProcessorMap();
  public java.util.Map<java.lang.String, com.feilong.lib.json.processors.JsonValueProcessor> getKeyMap();
  public java.util.Map<java.lang.Class<?>, com.feilong.lib.json.processors.JsonValueProcessor> getTypeMap();
}
```
