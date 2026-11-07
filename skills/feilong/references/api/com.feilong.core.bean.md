# com.feilong.core.bean

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.core.bean.Alias`

```java
public interface com.feilong.core.bean.Alias extends java.lang.annotation.Annotation {
  public abstract java.lang.String name();
  public abstract java.lang.String sampleValue();
}
```

## `com.feilong.core.bean.BeanOperationException`

```java
public final class com.feilong.core.bean.BeanOperationException extends com.feilong.core.DefaultRuntimeException {
  public com.feilong.core.bean.BeanOperationException(java.lang.String, java.lang.Throwable);
  public com.feilong.core.bean.BeanOperationException(java.lang.Throwable);
}
```

## `com.feilong.core.bean.BeanUtil`

```java
public final class com.feilong.core.bean.BeanUtil {
  public static void copyProperties(java.lang.Object, java.lang.Object, java.lang.String...);
  public static <T> T cloneBean(T);
  public static <T> T populate(T, java.util.Map<java.lang.String, ?>);
  public static <T> T populateAliasBean(T, java.util.Map<java.lang.String, ?>);
  public static org.apache.commons.beanutils.DynaBean newDynaBean(java.util.Map<?, ?>);
}
```

## `com.feilong.core.bean.ConvertUtil`

```java
public final class com.feilong.core.bean.ConvertUtil {
  public static void registerStandardDefaultNull();
  public static void registerSimpleDateLocaleConverter(java.lang.String);
  public static java.lang.Boolean toBoolean(java.lang.Object);
  public static java.lang.Boolean toBoolean(java.lang.Object, java.lang.Boolean);
  public static java.lang.Integer toInteger(java.lang.Object);
  public static java.lang.Integer toInteger(java.lang.Object, java.lang.Integer);
  public static java.lang.Long toLong(java.lang.Object);
  public static java.lang.Long toLong(java.lang.Object, java.lang.Long);
  public static java.math.BigDecimal toBigDecimal(java.lang.Object);
  public static java.math.BigDecimal toBigDecimal(java.lang.Object, java.math.BigDecimal);
  public static java.lang.Integer[] toIntegers(java.lang.Object);
  public static java.lang.Long[] toLongs(java.lang.Object);
  public static java.util.List<java.lang.Long> toLongList(java.lang.Object);
  public static java.util.List<java.lang.Integer> toIntegerList(java.lang.Object);
  public static java.lang.String toString(java.lang.Object);
  public static java.lang.String toString(java.util.Collection<?>, java.lang.String);
  public static java.lang.String toString(java.lang.Object[], java.lang.String);
  public static java.lang.String toString(java.util.Collection<?>, com.feilong.core.bean.ToStringConfig);
  public static java.lang.String toString(java.lang.Object[], com.feilong.core.bean.ToStringConfig);
  public static <T> java.util.Enumeration<T> toEnumeration(java.util.Collection<T>);
  public static <K, V> java.util.Map<K, V> toMap(K, V);
  public static <K, V> java.util.Map<K, V> toMap(K, V, K, V);
  public static java.util.Map<java.lang.String, java.lang.String> toMap(java.util.Properties);
  public static <K, V, J> java.util.Map<K, J> toMap(java.util.Map<K, V>, java.lang.Class<J>);
  public static <K, V, I, J> java.util.Map<I, J> toMap(java.util.Map<K, V>, java.lang.Class<I>, java.lang.Class<J>);
  public static <K, V, I, J> java.util.Map<I, J> toMap(java.util.Map<K, V>, org.apache.commons.collections4.Transformer<K, I>, org.apache.commons.collections4.Transformer<V, J>);
  public static <V, K, E extends java.util.Map$Entry<K, V>> java.util.Map<K, V> toMap(java.util.Collection<E>);
  public static <V, K> java.util.Map<K, V> toMapUseEntrys(java.util.Map$Entry<K, V>...);
  public static java.util.Properties toProperties(java.util.Map<java.lang.String, java.lang.String>);
  public static <T> java.util.List<T> toList(java.util.Enumeration<T>);
  public static <T> java.util.List<T> toList(java.util.Collection<T>);
  public static <T> java.util.List<T> toList(T...);
  public static <T> java.util.Set<T> toSet(T...);
  public static <T> T[] toArray(T...);
  public static <T> T[] toArray(java.util.Collection<T>, java.lang.Class<T>);
  public static <T> T[] toArray(java.lang.String[], java.lang.Class<T>);
  public static java.util.List<java.lang.String> toStringList(java.lang.Object);
  public static java.lang.String[] toStrings(java.lang.Object);
  public static <T> java.util.Iterator<T> toIterator(java.lang.Object);
  public static <T> T convert(java.lang.Object, java.lang.Class<T>);
  public static java.util.Locale toLocale(java.lang.Object);
}
```

## `com.feilong.core.bean.PropertyUtil`

```java
public final class com.feilong.core.bean.PropertyUtil {
  public static java.beans.PropertyDescriptor[] getPropertyDescriptors(java.lang.Class<?>);
  public static void copyProperties(java.lang.Object, java.lang.Object, java.lang.String...);
  public static java.util.Map<java.lang.String, java.lang.Object> describe(java.lang.Object, java.lang.String...);
  public static void setProperty(java.lang.Object, java.lang.String, java.lang.Object);
  public static void setPropertyIfValueNotNullOrEmpty(java.lang.Object, java.lang.String, java.lang.Object);
  public static void setPropertyIfValueNotNull(java.lang.Object, java.lang.String, java.lang.Object);
  public static <T> T getProperty(java.lang.Object, java.lang.String);
  public static <T> T findValueOfType(java.lang.Object, java.lang.Class<T>);
}
```

## `com.feilong.core.bean.PropertyValueObtainer`

```java
public final class com.feilong.core.bean.PropertyValueObtainer {
  public static <T, O, K extends java.util.Collection<T>> K getPropertyValueCollection(java.lang.Iterable<O>, java.lang.String, K);
  public static <T, O, K extends java.util.Collection<T>> K getPropertyValueCollection(java.lang.Iterable<O>, java.lang.String, K, java.lang.Class<T>);
  public static <T, O> T getValue(O, java.beans.PropertyDescriptor);
}
```

## `com.feilong.core.bean.ToStringConfig`

```java
public final class com.feilong.core.bean.ToStringConfig implements java.io.Serializable {
  public com.feilong.core.bean.ToStringConfig();
  public com.feilong.core.bean.ToStringConfig(java.lang.String);
  public com.feilong.core.bean.ToStringConfig(java.lang.String, boolean);
  public com.feilong.core.bean.ToStringConfig(java.lang.String, boolean, java.lang.String);
  public java.lang.String getConnector();
  public void setConnector(java.lang.String);
  public boolean getIsJoinNullOrEmpty();
  public void setIsJoinNullOrEmpty(boolean);
  public java.lang.String getPrefix();
  public void setPrefix(java.lang.String);
  public java.lang.String toString();
}
```
