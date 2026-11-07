# com.feilong.lib.beanutils

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.beanutils.BaseDynaBeanMapDecorator`

```java
public abstract class com.feilong.lib.beanutils.BaseDynaBeanMapDecorator<K> implements java.util.Map<K, java.lang.Object> {
  public com.feilong.lib.beanutils.BaseDynaBeanMapDecorator(org.apache.commons.beanutils.DynaBean);
  public com.feilong.lib.beanutils.BaseDynaBeanMapDecorator(org.apache.commons.beanutils.DynaBean, boolean);
  public boolean isReadOnly();
  public void clear();
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public java.util.Set<java.util.Map$Entry<K, java.lang.Object>> entrySet();
  public java.lang.Object get(java.lang.Object);
  public boolean isEmpty();
  public java.util.Set<K> keySet();
  public java.lang.Object put(K, java.lang.Object);
  public void putAll(java.util.Map<? extends K, ? extends java.lang.Object>);
  public java.lang.Object remove(java.lang.Object);
  public int size();
  public java.util.Collection<java.lang.Object> values();
  public org.apache.commons.beanutils.DynaBean getDynaBean();
}
```

## `com.feilong.lib.beanutils.BasicDynaBean`

```java
public class com.feilong.lib.beanutils.BasicDynaBean implements org.apache.commons.beanutils.DynaBean,java.io.Serializable {
  public com.feilong.lib.beanutils.BasicDynaBean(com.feilong.lib.beanutils.DynaClass);
  public java.util.Map<java.lang.String, java.lang.Object> getMap();
  public boolean contains(java.lang.String, java.lang.String);
  public java.lang.Object get(java.lang.String);
  public java.lang.Object get(java.lang.String, int);
  public java.lang.Object get(java.lang.String, java.lang.String);
  public com.feilong.lib.beanutils.DynaClass getDynaClass();
  public void remove(java.lang.String, java.lang.String);
  public void set(java.lang.String, java.lang.Object);
  public void set(java.lang.String, int, java.lang.Object);
  public void set(java.lang.String, java.lang.String, java.lang.Object);
}
```

## `com.feilong.lib.beanutils.BasicDynaClass`

```java
public class com.feilong.lib.beanutils.BasicDynaClass implements com.feilong.lib.beanutils.DynaClass,java.io.Serializable {
  public com.feilong.lib.beanutils.BasicDynaClass();
  public com.feilong.lib.beanutils.BasicDynaClass(java.lang.String, java.lang.Class<?>);
  public com.feilong.lib.beanutils.BasicDynaClass(java.lang.String, java.lang.Class<?>, com.feilong.lib.beanutils.DynaProperty[]);
  public java.lang.String getName();
  public com.feilong.lib.beanutils.DynaProperty getDynaProperty(java.lang.String);
  public com.feilong.lib.beanutils.DynaProperty[] getDynaProperties();
  public org.apache.commons.beanutils.DynaBean newInstance() throws java.lang.IllegalAccessException, java.lang.InstantiationException;
  public java.lang.Class<?> getDynaBeanClass();
}
```

## `com.feilong.lib.beanutils.BeanComparator`

```java
public class com.feilong.lib.beanutils.BeanComparator<T> implements java.util.Comparator<T>, java.io.Serializable {
  public com.feilong.lib.beanutils.BeanComparator();
  public com.feilong.lib.beanutils.BeanComparator(java.lang.String);
  public com.feilong.lib.beanutils.BeanComparator(java.lang.String, java.util.Comparator<?>);
  public void setProperty(java.lang.String);
  public java.lang.String getProperty();
  public java.util.Comparator<?> getComparator();
  public int compare(T, T);
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.feilong.lib.beanutils.BeanIntrospector`

```java
public interface com.feilong.lib.beanutils.BeanIntrospector {
  public abstract void introspect(com.feilong.lib.beanutils.IntrospectionContext) throws java.beans.IntrospectionException;
}
```

## `com.feilong.lib.beanutils.BeanUtils`

```java
public class com.feilong.lib.beanutils.BeanUtils {
  public com.feilong.lib.beanutils.BeanUtils();
  public static java.lang.Object cloneBean(java.lang.Object) throws java.lang.IllegalAccessException, java.lang.InstantiationException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static void copyProperties(java.lang.Object, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static void copyProperty(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.util.Map<java.lang.String, java.lang.String> describe(java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.String getProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static void populate(java.lang.Object, java.util.Map<java.lang.String, ? extends java.lang.Object>) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static void setProperty(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static <K, V> java.util.Map<K, V> createCache();
  public static boolean getCacheFast(java.util.Map<?, ?>);
  public static void setCacheFast(java.util.Map<?, ?>, boolean);
}
```

## `com.feilong.lib.beanutils.BeanUtilsBean`

```java
public class com.feilong.lib.beanutils.BeanUtilsBean {
  public static com.feilong.lib.beanutils.BeanUtilsBean getInstance();
  public static void setInstance(com.feilong.lib.beanutils.BeanUtilsBean);
  public com.feilong.lib.beanutils.BeanUtilsBean();
  public com.feilong.lib.beanutils.BeanUtilsBean(com.feilong.lib.beanutils.ConvertUtilsBean);
  public com.feilong.lib.beanutils.BeanUtilsBean(com.feilong.lib.beanutils.ConvertUtilsBean, com.feilong.lib.beanutils.PropertyUtilsBean);
  public java.lang.Object cloneBean(java.lang.Object) throws java.lang.IllegalAccessException, java.lang.InstantiationException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public void copyProperties(java.lang.Object, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public void copyProperty(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public java.util.Map<java.lang.String, java.lang.String> describe(java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String[] getArrayProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getIndexedProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getIndexedProperty(java.lang.Object, java.lang.String, int) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getMappedProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getMappedProperty(java.lang.Object, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getNestedProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getSimpleProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public void populate(java.lang.Object, java.util.Map<java.lang.String, ? extends java.lang.Object>) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public void setProperty(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public com.feilong.lib.beanutils.ConvertUtilsBean getConvertUtils();
  public com.feilong.lib.beanutils.PropertyUtilsBean getPropertyUtils();
}
```

## `com.feilong.lib.beanutils.ContextClassLoaderLocal`

```java
public class com.feilong.lib.beanutils.ContextClassLoaderLocal<T> {
  public com.feilong.lib.beanutils.ContextClassLoaderLocal();
  public synchronized T get();
  public synchronized void set(T);
  public synchronized void unset();
  public synchronized void unset(java.lang.ClassLoader);
}
```

## `com.feilong.lib.beanutils.ConversionException`

```java
public class com.feilong.lib.beanutils.ConversionException extends java.lang.RuntimeException {
  public com.feilong.lib.beanutils.ConversionException(java.lang.String);
  public com.feilong.lib.beanutils.ConversionException(java.lang.String, java.lang.Throwable);
  public com.feilong.lib.beanutils.ConversionException(java.lang.Throwable);
  public java.lang.Throwable getCause();
}
```

## `com.feilong.lib.beanutils.ConvertUtils`

```java
public class com.feilong.lib.beanutils.ConvertUtils {
  public com.feilong.lib.beanutils.ConvertUtils();
  public static java.lang.String convert(java.lang.Object);
  public static java.lang.Object convert(java.lang.String, java.lang.Class<?>);
  public static java.lang.Object convert(java.lang.String[], java.lang.Class<?>);
  public static java.lang.Object convert(java.lang.Object, java.lang.Class<?>);
  public static void deregister();
  public static void deregister(java.lang.Class<?>);
  public static com.feilong.lib.beanutils.Converter lookup(java.lang.Class<?>);
  public static void register(com.feilong.lib.beanutils.Converter, java.lang.Class<?>);
  public static <T> java.lang.Class<T> primitiveToWrapper(java.lang.Class<T>);
}
```

## `com.feilong.lib.beanutils.ConvertUtilsBean`

```java
public class com.feilong.lib.beanutils.ConvertUtilsBean {
  public com.feilong.lib.beanutils.ConvertUtilsBean();
  public java.lang.String convert(java.lang.Object);
  public java.lang.Object convert(java.lang.String, java.lang.Class<?>);
  public java.lang.Object convert(java.lang.String[], java.lang.Class<?>);
  public java.lang.Object convert(java.lang.Object, java.lang.Class<?>);
  public void deregister();
  public void register(boolean, boolean, int);
  public void deregister(java.lang.Class<?>);
  public com.feilong.lib.beanutils.Converter lookup(java.lang.Class<?>);
  public com.feilong.lib.beanutils.Converter lookup(java.lang.Class<?>, java.lang.Class<?>);
  public void register(com.feilong.lib.beanutils.Converter, java.lang.Class<?>);
}
```

## `com.feilong.lib.beanutils.Converter`

```java
public interface com.feilong.lib.beanutils.Converter {
  public abstract <T> T convert(java.lang.Class<T>, java.lang.Object);
}
```

## `com.feilong.lib.beanutils.ConvertingWrapDynaBean`

```java
public class com.feilong.lib.beanutils.ConvertingWrapDynaBean extends com.feilong.lib.beanutils.WrapDynaBean {
  public com.feilong.lib.beanutils.ConvertingWrapDynaBean(java.lang.Object);
  public void set(java.lang.String, java.lang.Object);
}
```

## `com.feilong.lib.beanutils.DefaultBeanIntrospector`

```java
public class com.feilong.lib.beanutils.DefaultBeanIntrospector implements com.feilong.lib.beanutils.BeanIntrospector {
  public void introspect(com.feilong.lib.beanutils.IntrospectionContext);
}
```

## `com.feilong.lib.beanutils.DynaBeanPropertyMapDecorator`

```java
public class com.feilong.lib.beanutils.DynaBeanPropertyMapDecorator extends com.feilong.lib.beanutils.BaseDynaBeanMapDecorator<java.lang.String> {
  public com.feilong.lib.beanutils.DynaBeanPropertyMapDecorator(org.apache.commons.beanutils.DynaBean, boolean);
  public com.feilong.lib.beanutils.DynaBeanPropertyMapDecorator(org.apache.commons.beanutils.DynaBean);
}
```

## `com.feilong.lib.beanutils.DynaClass`

```java
public interface com.feilong.lib.beanutils.DynaClass {
  public abstract java.lang.String getName();
  public abstract com.feilong.lib.beanutils.DynaProperty getDynaProperty(java.lang.String);
  public abstract com.feilong.lib.beanutils.DynaProperty[] getDynaProperties();
  public abstract org.apache.commons.beanutils.DynaBean newInstance() throws java.lang.IllegalAccessException, java.lang.InstantiationException;
}
```

## `com.feilong.lib.beanutils.DynaProperty`

```java
public class com.feilong.lib.beanutils.DynaProperty implements java.io.Serializable {
  public com.feilong.lib.beanutils.DynaProperty(java.lang.String);
  public com.feilong.lib.beanutils.DynaProperty(java.lang.String, java.lang.Class<?>);
  public com.feilong.lib.beanutils.DynaProperty(java.lang.String, java.lang.Class<?>, java.lang.Class<?>);
  public java.lang.String getName();
  public java.lang.Class<?> getType();
  public java.lang.Class<?> getContentType();
  public boolean isIndexed();
  public boolean isMapped();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.feilong.lib.beanutils.FastHashMap`

```java
public class com.feilong.lib.beanutils.FastHashMap extends java.util.HashMap {
  public com.feilong.lib.beanutils.FastHashMap();
  public com.feilong.lib.beanutils.FastHashMap(int);
  public com.feilong.lib.beanutils.FastHashMap(int, float);
  public com.feilong.lib.beanutils.FastHashMap(java.util.Map);
  public boolean getFast();
  public void setFast(boolean);
  public java.lang.Object get(java.lang.Object);
  public int size();
  public boolean isEmpty();
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public java.lang.Object put(java.lang.Object, java.lang.Object);
  public void putAll(java.util.Map);
  public java.lang.Object remove(java.lang.Object);
  public void clear();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.Object clone();
  public java.util.Set entrySet();
  public java.util.Set keySet();
  public java.util.Collection values();
}
```

## `com.feilong.lib.beanutils.FluentPropertyBeanIntrospector`

```java
public class com.feilong.lib.beanutils.FluentPropertyBeanIntrospector implements com.feilong.lib.beanutils.BeanIntrospector {
  public com.feilong.lib.beanutils.FluentPropertyBeanIntrospector(java.lang.String);
  public com.feilong.lib.beanutils.FluentPropertyBeanIntrospector();
  public java.lang.String getWriteMethodPrefix();
  public void introspect(com.feilong.lib.beanutils.IntrospectionContext) throws java.beans.IntrospectionException;
}
```

## `com.feilong.lib.beanutils.IntrospectionContext`

```java
public interface com.feilong.lib.beanutils.IntrospectionContext {
  public abstract java.lang.Class<?> getTargetClass();
  public abstract void addPropertyDescriptor(java.beans.PropertyDescriptor);
  public abstract void addPropertyDescriptors(java.beans.PropertyDescriptor[]);
  public abstract boolean hasProperty(java.lang.String);
  public abstract java.beans.PropertyDescriptor getPropertyDescriptor(java.lang.String);
  public abstract void removePropertyDescriptor(java.lang.String);
  public abstract java.util.Set<java.lang.String> propertyNames();
}
```

## `com.feilong.lib.beanutils.LazyDynaBean`

```java
public class com.feilong.lib.beanutils.LazyDynaBean implements org.apache.commons.beanutils.DynaBean,java.io.Serializable {
  public com.feilong.lib.beanutils.LazyDynaBean();
  public com.feilong.lib.beanutils.LazyDynaBean(java.lang.String);
  public com.feilong.lib.beanutils.LazyDynaBean(com.feilong.lib.beanutils.DynaClass);
  public java.util.Map<java.lang.String, java.lang.Object> getMap();
  public int size(java.lang.String);
  public boolean contains(java.lang.String, java.lang.String);
  public java.lang.Object get(java.lang.String);
  public java.lang.Object get(java.lang.String, int);
  public java.lang.Object get(java.lang.String, java.lang.String);
  public com.feilong.lib.beanutils.DynaClass getDynaClass();
  public void remove(java.lang.String, java.lang.String);
  public void set(java.lang.String, java.lang.Object);
  public void set(java.lang.String, int, java.lang.Object);
  public void set(java.lang.String, java.lang.String, java.lang.Object);
}
```

## `com.feilong.lib.beanutils.LazyDynaClass`

```java
public class com.feilong.lib.beanutils.LazyDynaClass extends com.feilong.lib.beanutils.BasicDynaClass implements com.feilong.lib.beanutils.MutableDynaClass {
  public com.feilong.lib.beanutils.LazyDynaClass();
  public com.feilong.lib.beanutils.LazyDynaClass(java.lang.String);
  public com.feilong.lib.beanutils.LazyDynaClass(java.lang.String, java.lang.Class<?>);
  public com.feilong.lib.beanutils.LazyDynaClass(java.lang.String, com.feilong.lib.beanutils.DynaProperty[]);
  public com.feilong.lib.beanutils.LazyDynaClass(java.lang.String, java.lang.Class<?>, com.feilong.lib.beanutils.DynaProperty[]);
  public boolean isRestricted();
  public void setRestricted(boolean);
  public boolean isReturnNull();
  public void setReturnNull(boolean);
  public void add(java.lang.String);
  public void add(java.lang.String, java.lang.Class<?>);
  public void add(java.lang.String, java.lang.Class<?>, boolean, boolean);
  public void remove(java.lang.String);
  public com.feilong.lib.beanutils.DynaProperty getDynaProperty(java.lang.String);
  public boolean isDynaProperty(java.lang.String);
}
```

## `com.feilong.lib.beanutils.LazyDynaList`

```java
public class com.feilong.lib.beanutils.LazyDynaList extends java.util.ArrayList<java.lang.Object> {
  public com.feilong.lib.beanutils.LazyDynaList();
  public com.feilong.lib.beanutils.LazyDynaList(int);
  public com.feilong.lib.beanutils.LazyDynaList(com.feilong.lib.beanutils.DynaClass);
  public com.feilong.lib.beanutils.LazyDynaList(java.lang.Class<?>);
  public com.feilong.lib.beanutils.LazyDynaList(java.util.Collection<?>);
  public com.feilong.lib.beanutils.LazyDynaList(java.lang.Object[]);
  public void add(int, java.lang.Object);
  public boolean add(java.lang.Object);
  public boolean addAll(java.util.Collection<?>);
  public boolean addAll(int, java.util.Collection<?>);
  public java.lang.Object get(int);
  public java.lang.Object set(int, java.lang.Object);
  public java.lang.Object[] toArray();
  public <T> T[] toArray(T[]);
  public org.apache.commons.beanutils.DynaBean[] toDynaBeanArray();
  public void setElementType(java.lang.Class<?>);
  public void setElementDynaClass(com.feilong.lib.beanutils.DynaClass);
}
```

## `com.feilong.lib.beanutils.LazyDynaMap`

```java
public class com.feilong.lib.beanutils.LazyDynaMap extends com.feilong.lib.beanutils.LazyDynaBean implements com.feilong.lib.beanutils.MutableDynaClass {
  public com.feilong.lib.beanutils.LazyDynaMap();
  public com.feilong.lib.beanutils.LazyDynaMap(java.lang.String);
  public com.feilong.lib.beanutils.LazyDynaMap(java.util.Map<java.lang.String, java.lang.Object>);
  public com.feilong.lib.beanutils.LazyDynaMap(java.lang.String, java.util.Map<java.lang.String, java.lang.Object>);
  public com.feilong.lib.beanutils.LazyDynaMap(com.feilong.lib.beanutils.DynaProperty[]);
  public com.feilong.lib.beanutils.LazyDynaMap(java.lang.String, com.feilong.lib.beanutils.DynaProperty[]);
  public com.feilong.lib.beanutils.LazyDynaMap(com.feilong.lib.beanutils.DynaClass);
  public void setMap(java.util.Map<java.lang.String, java.lang.Object>);
  public java.util.Map<java.lang.String, java.lang.Object> getMap();
  public void set(java.lang.String, java.lang.Object);
  public java.lang.String getName();
  public com.feilong.lib.beanutils.DynaProperty getDynaProperty(java.lang.String);
  public com.feilong.lib.beanutils.DynaProperty[] getDynaProperties();
  public org.apache.commons.beanutils.DynaBean newInstance();
  public boolean isRestricted();
  public void setRestricted(boolean);
  public void add(java.lang.String);
  public void add(java.lang.String, java.lang.Class<?>);
  public void add(java.lang.String, java.lang.Class<?>, boolean, boolean);
  public void remove(java.lang.String);
  public boolean isReturnNull();
  public void setReturnNull(boolean);
}
```

## `com.feilong.lib.beanutils.MappedPropertyDescriptor`

```java
public class com.feilong.lib.beanutils.MappedPropertyDescriptor extends java.beans.PropertyDescriptor {
  public com.feilong.lib.beanutils.MappedPropertyDescriptor(java.lang.String, java.lang.Class<?>) throws java.beans.IntrospectionException;
  public com.feilong.lib.beanutils.MappedPropertyDescriptor(java.lang.String, java.lang.Class<?>, java.lang.String, java.lang.String) throws java.beans.IntrospectionException;
  public com.feilong.lib.beanutils.MappedPropertyDescriptor(java.lang.String, java.lang.reflect.Method, java.lang.reflect.Method) throws java.beans.IntrospectionException;
  public java.lang.Class<?> getMappedPropertyType();
  public java.lang.reflect.Method getMappedReadMethod();
  public void setMappedReadMethod(java.lang.reflect.Method) throws java.beans.IntrospectionException;
  public java.lang.reflect.Method getMappedWriteMethod();
  public void setMappedWriteMethod(java.lang.reflect.Method) throws java.beans.IntrospectionException;
}
```

## `com.feilong.lib.beanutils.MethodUtils`

```java
public class com.feilong.lib.beanutils.MethodUtils {
  public com.feilong.lib.beanutils.MethodUtils();
  public static synchronized void setCacheMethods(boolean);
  public static synchronized int clearCache();
  public static java.lang.Object invokeMethod(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeMethod(java.lang.Object, java.lang.String, java.lang.Object[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeMethod(java.lang.Object, java.lang.String, java.lang.Object[], java.lang.Class<?>[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeExactMethod(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeExactMethod(java.lang.Object, java.lang.String, java.lang.Object[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeExactMethod(java.lang.Object, java.lang.String, java.lang.Object[], java.lang.Class<?>[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeExactStaticMethod(java.lang.Class<?>, java.lang.String, java.lang.Object[], java.lang.Class<?>[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeStaticMethod(java.lang.Class<?>, java.lang.String, java.lang.Object) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeStaticMethod(java.lang.Class<?>, java.lang.String, java.lang.Object[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeStaticMethod(java.lang.Class<?>, java.lang.String, java.lang.Object[], java.lang.Class<?>[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeExactStaticMethod(java.lang.Class<?>, java.lang.String, java.lang.Object) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeExactStaticMethod(java.lang.Class<?>, java.lang.String, java.lang.Object[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.reflect.Method getAccessibleMethod(java.lang.Class<?>, java.lang.String, java.lang.Class<?>);
  public static java.lang.reflect.Method getAccessibleMethod(java.lang.Class<?>, java.lang.String, java.lang.Class<?>[]);
  public static java.lang.reflect.Method getAccessibleMethod(java.lang.reflect.Method);
  public static java.lang.reflect.Method getAccessibleMethod(java.lang.Class<?>, java.lang.reflect.Method);
  public static java.lang.reflect.Method getMatchingAccessibleMethod(java.lang.Class<?>, java.lang.String, java.lang.Class<?>[]);
  public static final boolean isAssignmentCompatible(java.lang.Class<?>, java.lang.Class<?>);
  public static java.lang.Class<?> getPrimitiveWrapper(java.lang.Class<?>);
  public static java.lang.Class<?> getPrimitiveType(java.lang.Class<?>);
  public static java.lang.Class<?> toNonPrimitiveClass(java.lang.Class<?>);
}
```

## `com.feilong.lib.beanutils.MutableDynaClass`

```java
public interface com.feilong.lib.beanutils.MutableDynaClass extends com.feilong.lib.beanutils.DynaClass {
  public abstract void add(java.lang.String);
  public abstract void add(java.lang.String, java.lang.Class<?>);
  public abstract void add(java.lang.String, java.lang.Class<?>, boolean, boolean);
  public abstract boolean isRestricted();
  public abstract void remove(java.lang.String);
  public abstract void setRestricted(boolean);
}
```

## `com.feilong.lib.beanutils.NestedNullException`

```java
public class com.feilong.lib.beanutils.NestedNullException extends java.lang.IllegalArgumentException {
  public com.feilong.lib.beanutils.NestedNullException();
  public com.feilong.lib.beanutils.NestedNullException(java.lang.String);
}
```

## `com.feilong.lib.beanutils.PropertyUtils`

```java
public class com.feilong.lib.beanutils.PropertyUtils {
  public com.feilong.lib.beanutils.PropertyUtils();
  public static void copyProperties(java.lang.Object, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.util.Map<java.lang.String, java.lang.Object> describe(java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static com.feilong.lib.beanutils.FastHashMap getMappedPropertyDescriptors(java.lang.Class<?>);
  public static java.lang.Object getProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.beans.PropertyDescriptor getPropertyDescriptor(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.beans.PropertyDescriptor[] getPropertyDescriptors(java.lang.Class<?>);
  public static java.lang.reflect.Method getReadMethod(java.beans.PropertyDescriptor);
  public static java.lang.Object getSimpleProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.reflect.Method getWriteMethod(java.beans.PropertyDescriptor);
  public static boolean isWriteable(java.lang.Object, java.lang.String);
  public static void setProperty(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static void setSimpleProperty(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
}
```

## `com.feilong.lib.beanutils.PropertyUtilsBean`

```java
public class com.feilong.lib.beanutils.PropertyUtilsBean {
  public com.feilong.lib.beanutils.PropertyUtilsBean();
  public com.feilong.lib.beanutils.expression.Resolver getResolver();
  public void setResolver(com.feilong.lib.beanutils.expression.Resolver);
  public final void resetBeanIntrospectors();
  public void copyProperties(java.lang.Object, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.util.Map<java.lang.String, java.lang.Object> describe(java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.Object getIndexedProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.Object getIndexedProperty(java.lang.Object, java.lang.String, int) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.Object getMappedProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.Object getMappedProperty(java.lang.Object, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public com.feilong.lib.beanutils.FastHashMap getMappedPropertyDescriptors(java.lang.Class<?>);
  public java.lang.Object getProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.beans.PropertyDescriptor getPropertyDescriptor(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.beans.PropertyDescriptor[] getPropertyDescriptors(java.lang.Class<?>);
  public java.beans.PropertyDescriptor[] getPropertyDescriptors(java.lang.Object);
  public java.lang.reflect.Method getReadMethod(java.beans.PropertyDescriptor);
  public java.lang.Object getSimpleProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.reflect.Method getWriteMethod(java.beans.PropertyDescriptor);
  public boolean isReadable(java.lang.Object, java.lang.String);
  public boolean isWriteable(java.lang.Object, java.lang.String);
  public void setIndexedProperty(java.lang.Object, java.lang.String, int, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public void setMappedProperty(java.lang.Object, java.lang.String, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public void setNestedProperty(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public void setProperty(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public void setSimpleProperty(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
}
```

## `com.feilong.lib.beanutils.SuppressPropertiesBeanIntrospector`

```java
public class com.feilong.lib.beanutils.SuppressPropertiesBeanIntrospector implements com.feilong.lib.beanutils.BeanIntrospector {
  public com.feilong.lib.beanutils.SuppressPropertiesBeanIntrospector(java.util.Collection<java.lang.String>);
  public java.util.Set<java.lang.String> getSuppressedProperties();
  public void introspect(com.feilong.lib.beanutils.IntrospectionContext) throws java.beans.IntrospectionException;
}
```

## `com.feilong.lib.beanutils.WrapDynaBean`

```java
public class com.feilong.lib.beanutils.WrapDynaBean implements org.apache.commons.beanutils.DynaBean,java.io.Serializable {
  public com.feilong.lib.beanutils.WrapDynaBean(java.lang.Object);
  public com.feilong.lib.beanutils.WrapDynaBean(java.lang.Object, com.feilong.lib.beanutils.WrapDynaClass);
  public boolean contains(java.lang.String, java.lang.String);
  public java.lang.Object get(java.lang.String);
  public java.lang.Object get(java.lang.String, int);
  public java.lang.Object get(java.lang.String, java.lang.String);
  public com.feilong.lib.beanutils.DynaClass getDynaClass();
  public void remove(java.lang.String, java.lang.String);
  public void set(java.lang.String, java.lang.Object);
  public void set(java.lang.String, int, java.lang.Object);
  public void set(java.lang.String, java.lang.String, java.lang.Object);
  public java.lang.Object getInstance();
}
```

## `com.feilong.lib.beanutils.WrapDynaClass`

```java
public class com.feilong.lib.beanutils.WrapDynaClass implements com.feilong.lib.beanutils.DynaClass {
  public java.lang.String getName();
  public com.feilong.lib.beanutils.DynaProperty getDynaProperty(java.lang.String);
  public com.feilong.lib.beanutils.DynaProperty[] getDynaProperties();
  public org.apache.commons.beanutils.DynaBean newInstance() throws java.lang.IllegalAccessException, java.lang.InstantiationException;
  public java.beans.PropertyDescriptor getPropertyDescriptor(java.lang.String);
  public static void clear();
  public static com.feilong.lib.beanutils.WrapDynaClass createDynaClass(java.lang.Class<?>);
  public static com.feilong.lib.beanutils.WrapDynaClass createDynaClass(java.lang.Class<?>, com.feilong.lib.beanutils.PropertyUtilsBean);
}
```
