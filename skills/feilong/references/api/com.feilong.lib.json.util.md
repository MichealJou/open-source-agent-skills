# com.feilong.lib.json.util

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.json.util.ClassResolver`

```java
public class com.feilong.lib.json.util.ClassResolver {
  public static java.lang.Class<?> resolve(java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.lang.Class<?>>);
  public static java.lang.Class<?> resolve(java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.lang.Class<?>>, java.lang.Class<?>);
  public static java.lang.Class<?> resolve(java.lang.String, java.lang.String, java.lang.Class<?>, java.util.Map<java.lang.String, java.lang.Class<?>>);
}
```

## `com.feilong.lib.json.util.CycleDetectionStrategy`

```java
public abstract class com.feilong.lib.json.util.CycleDetectionStrategy {
  public com.feilong.lib.json.util.CycleDetectionStrategy();
  public abstract com.feilong.lib.json.JSONArray handleRepeatedReferenceAsArray(java.lang.Object);
  public abstract com.feilong.lib.json.JSONObject handleRepeatedReferenceAsObject(java.lang.Object);
}
```

## `com.feilong.lib.json.util.CycleSetUtil`

```java
public class com.feilong.lib.json.util.CycleSetUtil {
  public static boolean addInstance(java.lang.Object);
  public static void removeInstance(java.lang.Object);
}
```

## `com.feilong.lib.json.util.IsIgnoreUtil`

```java
public class com.feilong.lib.json.util.IsIgnoreUtil {
  public static boolean isIgnore(java.lang.Class<?>, java.beans.PropertyDescriptor, java.util.Collection<java.lang.String>);
}
```

## `com.feilong.lib.json.util.JSONUtils`

```java
public final class com.feilong.lib.json.util.JSONUtils {
  public static com.feilong.lib.ezmorph.MorpherRegistry getMorpherRegistry();
  public static java.lang.Class<?> getInnerComponentType(java.lang.Class<?>);
  public static java.util.Map<java.lang.String, java.lang.Class<?>> getKeyAndTypeMap(com.feilong.lib.json.JSONObject);
  public static int hashCode(java.lang.Object);
  public static boolean isArray(java.lang.Class<?>);
  public static boolean isArray(java.lang.Object);
  public static boolean isBoolean(java.lang.Class<?>);
  public static boolean isBoolean(java.lang.Object);
  public static boolean isJavaIdentifier(java.lang.String);
  public static boolean isNull(java.lang.Object);
  public static boolean isNumber(java.lang.Class<?>);
  public static boolean isNumber(java.lang.Object);
  public static boolean isObject(java.lang.Object);
  public static boolean isString(java.lang.Class<?>);
  public static boolean isString(java.lang.Object);
  public static boolean mayBeJSON(java.lang.String);
  public static org.apache.commons.beanutils.DynaBean newDynaBean(com.feilong.lib.json.JSONObject, com.feilong.lib.json.JsonConfig);
  public static java.lang.String numberToString(java.lang.Number);
  public static java.lang.String stripQuotes(java.lang.String);
  public static boolean hasQuotes(java.lang.String);
  public static boolean isJsonKeyword(java.lang.String);
  public static void testValidity(java.lang.Object);
  public static java.lang.Number transformNumber(java.lang.Number);
}
```

## `com.feilong.lib.json.util.JavaIdentifierTransformer`

```java
public abstract class com.feilong.lib.json.util.JavaIdentifierTransformer {
  public com.feilong.lib.json.util.JavaIdentifierTransformer();
  public abstract java.lang.String transformToJavaIdentifier(java.lang.String);
}
```

## `com.feilong.lib.json.util.KeyUpdater`

```java
public class com.feilong.lib.json.util.KeyUpdater {
  public static java.lang.String update(java.lang.Class<?>, java.lang.String, com.feilong.lib.json.processors.PropertyNameProcessor);
}
```

## `com.feilong.lib.json.util.PropertyFilter`

```java
public interface com.feilong.lib.json.util.PropertyFilter {
  public abstract boolean apply(java.lang.Object, java.lang.String, java.lang.Object);
}
```

## `com.feilong.lib.json.util.PropertySetStrategy`

```java
public class com.feilong.lib.json.util.PropertySetStrategy {
  public com.feilong.lib.json.util.PropertySetStrategy();
  public static void setProperty(java.lang.Object, java.lang.String, java.lang.Object);
}
```
