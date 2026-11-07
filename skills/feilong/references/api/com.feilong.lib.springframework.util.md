# com.feilong.lib.springframework.util

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.springframework.util.Assert`

```java
public abstract class com.feilong.lib.springframework.util.Assert {
  public com.feilong.lib.springframework.util.Assert();
  public static void state(boolean, java.lang.String);
  public static void isTrue(boolean, java.lang.String);
  public static void notNull(java.lang.Object, java.lang.String);
}
```

## `com.feilong.lib.springframework.util.ClassUtils`

```java
public abstract class com.feilong.lib.springframework.util.ClassUtils {
  public com.feilong.lib.springframework.util.ClassUtils();
  public static java.lang.ClassLoader getDefaultClassLoader();
  public static java.lang.String classPackageAsResourcePath(java.lang.Class<?>);
}
```

## `com.feilong.lib.springframework.util.ConcurrentReferenceHashMap`

```java
public class com.feilong.lib.springframework.util.ConcurrentReferenceHashMap<K, V> extends java.util.AbstractMap<K, V> implements java.util.concurrent.ConcurrentMap<K, V> {
  public com.feilong.lib.springframework.util.ConcurrentReferenceHashMap(int);
  public com.feilong.lib.springframework.util.ConcurrentReferenceHashMap(int, float, int, com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$ReferenceType);
  public V get(java.lang.Object);
  public V getOrDefault(java.lang.Object, V);
  public boolean containsKey(java.lang.Object);
  public V put(K, V);
  public V putIfAbsent(K, V);
  public V remove(java.lang.Object);
  public boolean remove(java.lang.Object, java.lang.Object);
  public boolean replace(K, V, V);
  public V replace(K, V);
  public void clear();
  public void purgeUnreferencedEntries();
  public int size();
  public boolean isEmpty();
  public java.util.Set<java.util.Map$Entry<K, V>> entrySet();
}
```

## `com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Entry`

```java
public final class com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Entry<K, V> implements java.util.Map$Entry<K, V> {
  public com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Entry(K, V);
  public K getKey();
  public V getValue();
  public V setValue(V);
  public java.lang.String toString();
  public final boolean equals(java.lang.Object);
  public final int hashCode();
}
```

## `com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Reference`

```java
public interface com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Reference<K, V> {
  public abstract com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Entry<K, V> get();
  public abstract int getHash();
  public abstract com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Reference<K, V> getNext();
  public abstract void release();
}
```

## `com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$ReferenceManager`

```java
public class com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$ReferenceManager {
  public com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Reference<K, V> createReference(com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Entry<K, V>, int, com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Reference<K, V>);
  public com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Reference<K, V> pollForPurge();
}
```

## `com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$ReferenceType`

```java
public final class com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$ReferenceType extends java.lang.Enum<com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$ReferenceType> {
  public static com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$ReferenceType[] values();
  public static com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$ReferenceType valueOf(java.lang.String);
}
```

## `com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Restructure`

```java
public final class com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Restructure extends java.lang.Enum<com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Restructure> {
  public static com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Restructure[] values();
  public static com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Restructure valueOf(java.lang.String);
}
```

## `com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Segment`

```java
public final class com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Segment extends java.util.concurrent.locks.ReentrantLock {
  public com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Segment(com.feilong.lib.springframework.util.ConcurrentReferenceHashMap, int);
  public com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Reference<K, V> getReference(java.lang.Object, int, com.feilong.lib.springframework.util.ConcurrentReferenceHashMap$Restructure);
  public <T> T doTask(int, java.lang.Object, com.feilong.lib.springframework.util.ConcurrentReferenceHashMap<K, V>.Task<T>);
  public void clear();
  public final int getSize();
  public final int getCount();
}
```

## `com.feilong.lib.springframework.util.ObjectUtils`

```java
public abstract class com.feilong.lib.springframework.util.ObjectUtils {
  public com.feilong.lib.springframework.util.ObjectUtils();
  public static boolean isEmpty(java.lang.Object[]);
  public static boolean isEmpty(java.lang.Object);
  public static boolean containsConstant(java.lang.Enum<?>[], java.lang.String);
  public static boolean containsConstant(java.lang.Enum<?>[], java.lang.String, boolean);
  public static boolean nullSafeEquals(java.lang.Object, java.lang.Object);
  public static int nullSafeHashCode(java.lang.Object);
  public static int nullSafeHashCode(java.lang.Object[]);
  public static int nullSafeHashCode(boolean[]);
  public static int nullSafeHashCode(byte[]);
  public static int nullSafeHashCode(char[]);
  public static int nullSafeHashCode(double[]);
  public static int nullSafeHashCode(float[]);
  public static int nullSafeHashCode(int[]);
  public static int nullSafeHashCode(long[]);
  public static int nullSafeHashCode(short[]);
  public static int hashCode(boolean);
  public static int hashCode(double);
  public static int hashCode(float);
  public static int hashCode(long);
  public static java.lang.String identityToString(java.lang.Object);
  public static java.lang.String getIdentityHexString(java.lang.Object);
  public static java.lang.String getDisplayString(java.lang.Object);
  public static java.lang.String nullSafeClassName(java.lang.Object);
  public static java.lang.String nullSafeToString(java.lang.Object);
  public static java.lang.String nullSafeToString(java.lang.Object[]);
  public static java.lang.String nullSafeToString(boolean[]);
  public static java.lang.String nullSafeToString(byte[]);
  public static java.lang.String nullSafeToString(char[]);
  public static java.lang.String nullSafeToString(double[]);
  public static java.lang.String nullSafeToString(float[]);
  public static java.lang.String nullSafeToString(int[]);
  public static java.lang.String nullSafeToString(long[]);
  public static java.lang.String nullSafeToString(short[]);
}
```

## `com.feilong.lib.springframework.util.ReflectionUtils`

```java
public abstract class com.feilong.lib.springframework.util.ReflectionUtils {
  public com.feilong.lib.springframework.util.ReflectionUtils();
  public static java.lang.reflect.Field findField(java.lang.Class<?>, java.lang.String);
  public static java.lang.reflect.Field findField(java.lang.Class<?>, java.lang.String, java.lang.Class<?>);
  public static java.lang.Object getField(java.lang.reflect.Field, java.lang.Object);
  public static java.lang.reflect.Method findMethod(java.lang.Class<?>, java.lang.String);
  public static java.lang.reflect.Method findMethod(java.lang.Class<?>, java.lang.String, java.lang.Class<?>...);
  public static java.lang.Object invokeMethod(java.lang.reflect.Method, java.lang.Object);
  public static java.lang.Object invokeMethod(java.lang.reflect.Method, java.lang.Object, java.lang.Object...);
  public static void handleReflectionException(java.lang.Exception);
  public static void handleInvocationTargetException(java.lang.reflect.InvocationTargetException);
  public static void rethrowRuntimeException(java.lang.Throwable);
}
```

## `com.feilong.lib.springframework.util.ResourceUtils`

```java
public abstract class com.feilong.lib.springframework.util.ResourceUtils {
  public com.feilong.lib.springframework.util.ResourceUtils();
  public static boolean isUrl(java.lang.String);
  public static java.net.URL getURL(java.lang.String) throws java.io.FileNotFoundException;
  public static java.io.File getFile(java.lang.String) throws java.io.FileNotFoundException;
  public static java.io.File getFile(java.net.URL) throws java.io.FileNotFoundException;
  public static java.io.File getFile(java.net.URL, java.lang.String) throws java.io.FileNotFoundException;
  public static java.io.File getFile(java.net.URI) throws java.io.FileNotFoundException;
  public static java.io.File getFile(java.net.URI, java.lang.String) throws java.io.FileNotFoundException;
  public static boolean isFileURL(java.net.URL);
  public static boolean isJarURL(java.net.URL);
  public static boolean isJarFileURL(java.net.URL);
  public static java.net.URL extractJarFileURL(java.net.URL) throws java.net.MalformedURLException;
  public static java.net.URL extractArchiveURL(java.net.URL) throws java.net.MalformedURLException;
  public static java.net.URI toURI(java.net.URL) throws java.net.URISyntaxException;
  public static java.net.URI toURI(java.lang.String) throws java.net.URISyntaxException;
  public static void useCachesIfNecessary(java.net.URLConnection);
}
```

## `com.feilong.lib.springframework.util.StringUtils`

```java
public abstract class com.feilong.lib.springframework.util.StringUtils {
  public com.feilong.lib.springframework.util.StringUtils();
  public static boolean hasLength(java.lang.String);
  public static boolean hasText(java.lang.String);
  public static java.lang.String replace(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String deleteAny(java.lang.String, java.lang.String);
  public static java.lang.String getFilename(java.lang.String);
  public static java.lang.String applyRelativePath(java.lang.String, java.lang.String);
  public static java.lang.String cleanPath(java.lang.String);
  public static java.lang.String[] toStringArray(java.util.Collection<java.lang.String>);
  public static java.lang.String[] delimitedListToStringArray(java.lang.String, java.lang.String);
  public static java.lang.String[] delimitedListToStringArray(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String collectionToDelimitedString(java.util.Collection<?>, java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String collectionToDelimitedString(java.util.Collection<?>, java.lang.String);
}
```
