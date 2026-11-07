# com.feilong.core.lang

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.core.lang.ArrayUtil`

```java
public final class com.feilong.core.lang.ArrayUtil {
  public static <T> T getElement(java.lang.Object, int);
  public static <T> T[] newArray(java.lang.Class<T>, int);
}
```

## `com.feilong.core.lang.ClassLoaderUtil`

```java
public final class com.feilong.core.lang.ClassLoaderUtil {
  public static java.net.URL getResource(java.lang.String);
  public static java.io.InputStream getResourceAsStream(java.lang.String, java.lang.Class<?>);
  public static java.net.URL getResourceInAllClassLoader(java.lang.String, java.lang.Class<?>);
}
```

## `com.feilong.core.lang.ClassUtil`

```java
public final class com.feilong.core.lang.ClassUtil {
  public static boolean isInstance(java.lang.Object, java.lang.Class<?>);
  public static boolean isInstanceAnyClass(java.lang.Object, java.lang.Class<?>...);
  public static boolean isAssignableFrom(java.lang.Class<?>, java.lang.Class<?>);
  public static boolean isInterface(java.lang.Class<?>);
  public static java.lang.Class<?>[] toClass(java.lang.Object...);
  public static java.lang.Class<?> getClass(java.lang.String);
}
```

## `com.feilong.core.lang.EnumUtil`

```java
public final class com.feilong.core.lang.EnumUtil {
  public static <E extends java.lang.Enum<?>, T> E getEnumByPropertyValueIgnoreCase(java.lang.Class<E>, java.lang.String, T);
  public static <E extends java.lang.Enum<?>, T> E getEnumByPropertyValue(java.lang.Class<E>, java.lang.String, T);
}
```

## `com.feilong.core.lang.NumberUtil`

```java
public final class com.feilong.core.lang.NumberUtil {
  public static boolean isGreaterThan(java.lang.Number, java.lang.Number);
  public static boolean isGreaterThanOrEquals(java.lang.Number, java.lang.Number);
  public static boolean isEquals(java.lang.Number, java.lang.Number);
  public static boolean isLessThan(java.lang.Number, java.lang.Number);
  public static boolean isLessThanOrEquals(java.lang.Number, java.lang.Number);
  public static java.math.BigDecimal getDivideValue(java.lang.Number, java.lang.Number, int);
  public static java.math.BigDecimal getDivideValue(java.lang.Number, java.lang.Number, int, java.math.RoundingMode);
  public static java.math.BigDecimal getMultiplyValue(java.lang.Number, java.lang.Number, int);
  public static java.math.BigDecimal getAddValue(java.lang.Number...);
  public static java.math.BigDecimal getSubtractValue(java.lang.Number, java.lang.Number...);
  public static java.math.BigDecimal getSubtractValueWithScale(java.lang.Number, java.lang.Number, int);
  public static java.lang.String toString(java.lang.Number, java.lang.String);
  public static java.lang.String getProgress(java.lang.Number, java.lang.Number);
  public static java.lang.String getProgress(java.lang.Number, java.lang.Number, java.lang.String);
  public static java.math.BigDecimal setScale(java.lang.Number, int);
  public static java.math.BigDecimal setScale(java.lang.Number, int, java.math.RoundingMode);
}
```

## `com.feilong.core.lang.ObjectUtil`

```java
public final class com.feilong.core.lang.ObjectUtil {
  public static <T> T newFrom(java.lang.Class<T>, java.lang.Object, java.lang.String...);
  public static <T> T defaultIfNullOrEmpty(T, T);
  public static boolean defaultTrueIfNull(java.lang.Boolean);
  public static boolean defaultFalseIfNull(java.lang.Boolean);
  public static <T> T defaultIfNull(T, T);
  public static java.lang.String defaultEmptyStringIfNull(java.lang.String);
  public static <T> java.util.List<T> defaultEmptyListIfNull(java.util.List<T>);
  public static <T> java.util.Set<T> defaultEmptySetIfNull(java.util.Set<T>);
  public static <K, V> java.util.Map<K, V> defaultEmptyMapIfNull(java.util.Map<K, V>);
  public static <T> java.util.List<T> defaultNewArrayListIfNull(java.util.List<T>);
  public static <T> java.util.Set<T> defaultNewHashSetIfNull(java.util.Set<T>);
  public static <K, V> java.util.Map<K, V> defaultNewHashMapIfNull(java.util.Map<K, V>);
  public static <K, V> java.util.Map<K, V> defaultNewLinkedHashMapIfNull(java.util.Map<K, V>);
  public static java.lang.Integer defaultPageNo(java.lang.Integer);
  public static java.lang.Integer defaultZero(java.lang.Integer);
  public static java.lang.Integer defaultIfNullOrLessThanOne(java.lang.Integer, java.lang.Integer);
  public static java.lang.Integer defaultCountIfNullZeroOrGreaterThan(java.lang.Integer, java.lang.Integer);
  public static boolean isArray(java.lang.Object);
  public static boolean isPrimitiveArray(java.lang.Object);
  public static <T> boolean equalsAny(T, T...);
}
```

## `com.feilong.core.lang.StringUtil`

```java
public final class com.feilong.core.lang.StringUtil {
  public static java.lang.String newString(byte[]);
  public static java.lang.String newString(byte[], java.lang.String);
  public static byte[] getBytes(java.lang.String);
  public static byte[] getBytes(java.lang.String, java.lang.String);
  public static java.lang.String replace(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String replaceAll(java.lang.CharSequence, java.lang.String, java.lang.String);
  public static <V> java.lang.String replace(java.lang.CharSequence, java.util.Map<java.lang.String, V>);
  public static java.lang.String substring(java.lang.String, int);
  public static java.lang.String substring(java.lang.String, int, int);
  public static java.lang.String substringLast(java.lang.String, int);
  public static java.lang.String substringWithoutLast(java.lang.String, int);
  public static java.lang.String substringWithoutLast(java.lang.CharSequence, java.lang.String);
  public static java.lang.String[] split(java.lang.String, java.lang.String);
  public static java.lang.String[] tokenizeToStringArray(java.lang.String);
  public static java.util.Set<java.lang.String> tokenizeToSet(java.lang.String);
  public static java.util.List<java.lang.String> tokenizeToList(java.lang.String);
  public static <T> java.util.Set<T> tokenizeToSet(java.lang.String, java.lang.Class<T>);
  public static <T> java.util.List<T> tokenizeToList(java.lang.String, java.lang.Class<T>);
  public static java.lang.String[] tokenizeToStringArray(java.lang.String, java.lang.String);
  public static java.lang.String[] tokenizeToStringArray(java.lang.String, java.lang.String, boolean, boolean);
  public static <T> boolean tokenizeToArrayContains(java.lang.String, T);
  public static <T> boolean tokenizeToArrayContains(java.lang.String, java.lang.String, T);
  public static java.util.Map<java.lang.String, java.lang.String> toSingleValueMap(java.lang.String);
  public static <T, V> java.util.Map<T, V> toSingleValueMap(java.lang.String, java.lang.Class<T>, java.lang.Class<V>);
  public static <T, V> java.util.Map<T, V> toMap(java.lang.String, java.lang.Class<T>, com.feilong.context.converter.StringToBeanConverter<V>);
  public static java.util.Map<java.lang.String, java.util.List<java.lang.String>> toMultiValueMap(java.lang.String);
  public static <V> java.util.Map<java.lang.String, java.util.List<V>> toMultiValueMap(java.lang.String, java.lang.Class<V>);
  public static <T, V> java.util.Map<T, java.util.List<V>> toMultiValueMap(java.lang.String, java.lang.Class<T>, java.lang.Class<V>);
  public static java.lang.String format(java.lang.String, java.lang.Object...);
  public static java.lang.String formatPattern(java.lang.String, java.lang.Object...);
  public static boolean trimAndEqualsIgnoreCase(java.lang.String, java.lang.String);
  public static java.lang.String clean(java.lang.CharSequence);
  public static java.lang.String removeSpecialSpace(java.lang.CharSequence);
}
```

## `com.feilong.core.lang.SystemUtil`

```java
public final class com.feilong.core.lang.SystemUtil {
  public static java.lang.String getSystemProperty(java.lang.String);
  public static java.util.Map<java.lang.String, java.lang.String> getPropertiesMap();
  public static java.util.Map<java.lang.String, java.lang.String> getEnvMap();
  public static java.lang.String getEnv(java.lang.String);
  public static void setPropertiesFromMap(java.util.Map<java.lang.String, java.lang.String>);
  public static void setPropertiesFromProperties(java.util.Properties);
}
```

## `com.feilong.core.lang.ThreadUtil`

```java
public final class com.feilong.core.lang.ThreadUtil {
  public static final void sleepSeconds(int);
  public static final void sleep(int);
  public static final void sleep(long);
  public static void execute(java.lang.Runnable, int);
  public static <T> void execute(java.util.List<T>, int, com.feilong.core.lang.thread.PartitionRunnableBuilder<T>);
  public static <T> void execute(java.util.List<T>, int, com.feilong.core.lang.thread.PartitionPerHandler<T>);
  public static <T> void execute(java.util.List<T>, int, java.util.Map<java.lang.String, ?>, com.feilong.core.lang.thread.PartitionRunnableBuilder<T>);
  public static <T> void execute(java.util.List<T>, int, java.util.Map<java.lang.String, ?>, com.feilong.core.lang.thread.PartitionPerHandler<T>);
  public static <T> void execute(java.util.List<T>, com.feilong.core.lang.thread.PartitionThreadConfig, java.util.Map<java.lang.String, ?>, com.feilong.core.lang.thread.PartitionPerHandler<T>);
  public static <T> void execute(java.util.List<T>, com.feilong.core.lang.thread.PartitionPerHandler<T>);
  public static <T> void execute(java.util.List<T>, java.util.Map<java.lang.String, ?>, com.feilong.core.lang.thread.PartitionPerHandler<T>);
  public static <T> void executeUsePerElement(java.util.List<T>, com.feilong.core.lang.thread.PartitionPerElementHandler<T>);
  public static <T> void executeUsePerElement(java.util.List<T>, java.util.Map<java.lang.String, ?>, com.feilong.core.lang.thread.PartitionPerElementHandler<T>);
  public static <T> void executeUsePerElement(java.util.List<T>, com.feilong.core.lang.thread.PartitionThreadConfig, java.util.Map<java.lang.String, ?>, com.feilong.core.lang.thread.PartitionPerElementHandler<T>);
  public static void startAndJoin(java.lang.Thread[]);
}
```
