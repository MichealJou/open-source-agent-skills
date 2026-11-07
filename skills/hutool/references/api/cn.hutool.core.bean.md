# cn.hutool.core.bean

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.bean.BeanDesc`

```java
public class cn.hutool.core.bean.BeanDesc implements java.io.Serializable {
  public cn.hutool.core.bean.BeanDesc(java.lang.Class<?>);
  public java.lang.String getName();
  public java.lang.String getSimpleName();
  public java.util.Map<java.lang.String, cn.hutool.core.bean.PropDesc> getPropMap(boolean);
  public java.util.Collection<cn.hutool.core.bean.PropDesc> getProps();
  public cn.hutool.core.bean.PropDesc getProp(java.lang.String);
  public java.lang.reflect.Field getField(java.lang.String);
  public java.lang.reflect.Method getGetter(java.lang.String);
  public java.lang.reflect.Method getSetter(java.lang.String);
}
```

## `cn.hutool.core.bean.BeanDescCache`

```java
public final class cn.hutool.core.bean.BeanDescCache extends java.lang.Enum<cn.hutool.core.bean.BeanDescCache> {
  public static cn.hutool.core.bean.BeanDescCache[] values();
  public static cn.hutool.core.bean.BeanDescCache valueOf(java.lang.String);
  public cn.hutool.core.bean.BeanDesc getBeanDesc(java.lang.Class<?>, cn.hutool.core.lang.func.Func0<cn.hutool.core.bean.BeanDesc>);
  public void clear();
}
```

## `cn.hutool.core.bean.BeanException`

```java
public class cn.hutool.core.bean.BeanException extends java.lang.RuntimeException {
  public cn.hutool.core.bean.BeanException(java.lang.Throwable);
  public cn.hutool.core.bean.BeanException(java.lang.String);
  public cn.hutool.core.bean.BeanException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.bean.BeanException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.bean.BeanException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.core.bean.BeanInfoCache`

```java
public final class cn.hutool.core.bean.BeanInfoCache extends java.lang.Enum<cn.hutool.core.bean.BeanInfoCache> {
  public static cn.hutool.core.bean.BeanInfoCache[] values();
  public static cn.hutool.core.bean.BeanInfoCache valueOf(java.lang.String);
  public java.util.Map<java.lang.String, java.beans.PropertyDescriptor> getPropertyDescriptorMap(java.lang.Class<?>, boolean);
  public java.util.Map<java.lang.String, java.beans.PropertyDescriptor> getPropertyDescriptorMap(java.lang.Class<?>, boolean, cn.hutool.core.lang.func.Func0<java.util.Map<java.lang.String, java.beans.PropertyDescriptor>>);
  public void putPropertyDescriptorMap(java.lang.Class<?>, java.util.Map<java.lang.String, java.beans.PropertyDescriptor>, boolean);
  public void clear();
}
```

## `cn.hutool.core.bean.BeanPath`

```java
public class cn.hutool.core.bean.BeanPath implements java.io.Serializable {
  public static cn.hutool.core.bean.BeanPath create(java.lang.String);
  public cn.hutool.core.bean.BeanPath(java.lang.String);
  public java.util.List<java.lang.String> getPatternParts();
  public java.lang.Object get(java.lang.Object);
  public void set(java.lang.Object, java.lang.Object);
  public java.lang.String toString();
}
```

## `cn.hutool.core.bean.BeanUtil`

```java
public class cn.hutool.core.bean.BeanUtil {
  public cn.hutool.core.bean.BeanUtil();
  public static boolean isReadableBean(java.lang.Class<?>);
  public static boolean isBean(java.lang.Class<?>);
  public static boolean hasSetter(java.lang.Class<?>);
  public static boolean hasGetter(java.lang.Class<?>);
  public static boolean hasPublicField(java.lang.Class<?>);
  public static cn.hutool.core.bean.DynaBean createDynaBean(java.lang.Object);
  public static java.beans.PropertyEditor findEditor(java.lang.Class<?>);
  public static cn.hutool.core.bean.BeanDesc getBeanDesc(java.lang.Class<?>);
  public static void descForEach(java.lang.Class<?>, java.util.function.Consumer<? super cn.hutool.core.bean.PropDesc>);
  public static java.beans.PropertyDescriptor[] getPropertyDescriptors(java.lang.Class<?>) throws cn.hutool.core.bean.BeanException;
  public static java.util.Map<java.lang.String, java.beans.PropertyDescriptor> getPropertyDescriptorMap(java.lang.Class<?>, boolean) throws cn.hutool.core.bean.BeanException;
  public static java.beans.PropertyDescriptor getPropertyDescriptor(java.lang.Class<?>, java.lang.String) throws cn.hutool.core.bean.BeanException;
  public static java.beans.PropertyDescriptor getPropertyDescriptor(java.lang.Class<?>, java.lang.String, boolean) throws cn.hutool.core.bean.BeanException;
  public static java.lang.Object getFieldValue(java.lang.Object, java.lang.String);
  public static java.lang.Object setFieldValue(java.lang.Object, java.lang.String, java.lang.Object);
  public static <T> T getProperty(java.lang.Object, java.lang.String);
  public static void setProperty(java.lang.Object, java.lang.String, java.lang.Object);
  public static <T> T mapToBean(java.util.Map<?, ?>, java.lang.Class<T>, boolean);
  public static <T> T mapToBeanIgnoreCase(java.util.Map<?, ?>, java.lang.Class<T>, boolean);
  public static <T> T mapToBean(java.util.Map<?, ?>, java.lang.Class<T>, cn.hutool.core.bean.copier.CopyOptions);
  public static <T> T mapToBean(java.util.Map<?, ?>, java.lang.Class<T>, boolean, cn.hutool.core.bean.copier.CopyOptions);
  public static <T> T fillBeanWithMap(java.util.Map<?, ?>, T, boolean);
  public static <T> T fillBeanWithMap(java.util.Map<?, ?>, T, boolean, boolean);
  public static <T> T fillBeanWithMapIgnoreCase(java.util.Map<?, ?>, T, boolean);
  public static <T> T fillBeanWithMap(java.util.Map<?, ?>, T, cn.hutool.core.bean.copier.CopyOptions);
  public static <T> T fillBeanWithMap(java.util.Map<?, ?>, T, boolean, cn.hutool.core.bean.copier.CopyOptions);
  public static <T> T toBean(java.lang.Object, java.lang.Class<T>);
  public static <T> T toBeanIgnoreError(java.lang.Object, java.lang.Class<T>);
  public static <T> T toBeanIgnoreCase(java.lang.Object, java.lang.Class<T>, boolean);
  public static <T> T toBean(java.lang.Object, java.lang.Class<T>, cn.hutool.core.bean.copier.CopyOptions);
  public static <T> T toBean(java.lang.Object, java.util.function.Supplier<T>, cn.hutool.core.bean.copier.CopyOptions);
  public static <T> T toBean(java.lang.Class<T>, cn.hutool.core.bean.copier.ValueProvider<java.lang.String>, cn.hutool.core.bean.copier.CopyOptions);
  public static <T> T fillBean(T, cn.hutool.core.bean.copier.ValueProvider<java.lang.String>, cn.hutool.core.bean.copier.CopyOptions);
  public static java.util.Map<java.lang.String, java.lang.Object> beanToMap(java.lang.Object, java.lang.String...);
  public static java.util.Map<java.lang.String, java.lang.Object> beanToMap(java.lang.Object, boolean, boolean);
  public static java.util.Map<java.lang.String, java.lang.Object> beanToMap(java.lang.Object, java.util.Map<java.lang.String, java.lang.Object>, boolean, boolean);
  public static java.util.Map<java.lang.String, java.lang.Object> beanToMap(java.lang.Object, java.util.Map<java.lang.String, java.lang.Object>, boolean, cn.hutool.core.lang.Editor<java.lang.String>);
  public static java.util.Map<java.lang.String, java.lang.Object> beanToMap(java.lang.Object, java.util.Map<java.lang.String, java.lang.Object>, cn.hutool.core.bean.copier.CopyOptions);
  public static <T> T copyProperties(java.lang.Object, java.lang.Class<T>, java.lang.String...);
  public static void copyProperties(java.lang.Object, java.lang.Object, java.lang.String...);
  public static void copyProperties(java.lang.Object, java.lang.Object, boolean);
  public static void copyProperties(java.lang.Object, java.lang.Object, cn.hutool.core.bean.copier.CopyOptions);
  public static <T> java.util.List<T> copyToList(java.util.Collection<?>, java.lang.Class<T>, cn.hutool.core.bean.copier.CopyOptions);
  public static <T> java.util.List<T> copyToList(java.util.Collection<?>, java.lang.Class<T>);
  public static boolean isMatchName(java.lang.Object, java.lang.String, boolean);
  public static <T> T edit(T, cn.hutool.core.lang.Editor<java.lang.reflect.Field>);
  public static <T> T trimStrFields(T, java.lang.String...);
  public static boolean isNotEmpty(java.lang.Object, java.lang.String...);
  public static boolean isEmpty(java.lang.Object, java.lang.String...);
  public static boolean hasNullField(java.lang.Object, java.lang.String...);
  public static java.lang.String getFieldName(java.lang.String);
  public static boolean isCommonFieldsEqual(java.lang.Object, java.lang.Object, java.lang.String...);
}
```

## `cn.hutool.core.bean.DynaBean`

```java
public class cn.hutool.core.bean.DynaBean extends cn.hutool.core.clone.CloneSupport<cn.hutool.core.bean.DynaBean> implements java.io.Serializable {
  public static cn.hutool.core.bean.DynaBean create(java.lang.Object);
  public static cn.hutool.core.bean.DynaBean create(java.lang.Class<?>);
  public static cn.hutool.core.bean.DynaBean create(java.lang.Class<?>, java.lang.Object...);
  public cn.hutool.core.bean.DynaBean(java.lang.Class<?>, java.lang.Object...);
  public cn.hutool.core.bean.DynaBean(java.lang.Class<?>);
  public cn.hutool.core.bean.DynaBean(java.lang.Object);
  public <T> T get(java.lang.String) throws cn.hutool.core.bean.BeanException;
  public boolean containsProp(java.lang.String);
  public <T> T safeGet(java.lang.String);
  public void set(java.lang.String, java.lang.Object) throws cn.hutool.core.bean.BeanException;
  public java.lang.Object invoke(java.lang.String, java.lang.Object...);
  public <T> T getBean();
  public <T> java.lang.Class<T> getBeanClass();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
}
```

## `cn.hutool.core.bean.NullWrapperBean`

```java
public class cn.hutool.core.bean.NullWrapperBean<T> {
  public cn.hutool.core.bean.NullWrapperBean(java.lang.Class<T>);
  public java.lang.Class<T> getWrappedClass();
}
```

## `cn.hutool.core.bean.PropDesc`

```java
public class cn.hutool.core.bean.PropDesc {
  public cn.hutool.core.bean.PropDesc(java.lang.reflect.Field, java.lang.reflect.Method, java.lang.reflect.Method);
  public void initialize();
  public java.lang.String getFieldName();
  public java.lang.String getRawFieldName();
  public java.lang.reflect.Field getField();
  public java.lang.reflect.Type getFieldType();
  public java.lang.Class<?> getFieldClass();
  public java.lang.reflect.Method getGetter();
  public java.lang.reflect.Method getSetter();
  public boolean isReadable(boolean);
  public java.lang.Object getValue(java.lang.Object);
  public java.lang.Object getValue(java.lang.Object, java.lang.reflect.Type, boolean);
  public boolean isWritable(boolean);
  public cn.hutool.core.bean.PropDesc setValue(java.lang.Object, java.lang.Object);
  public cn.hutool.core.bean.PropDesc setValue(java.lang.Object, java.lang.Object, boolean, boolean);
  public cn.hutool.core.bean.PropDesc setValue(java.lang.Object, java.lang.Object, boolean, boolean, boolean);
}
```

## `cn.hutool.core.bean.RecordUtil`

```java
public class cn.hutool.core.bean.RecordUtil {
  public cn.hutool.core.bean.RecordUtil();
  public static boolean isRecord(java.lang.Class<?>);
  public static java.util.Map$Entry<java.lang.String, java.lang.reflect.Type>[] getRecordComponents(java.lang.Class<?>);
  public static java.lang.Object newInstance(java.lang.Class<?>, cn.hutool.core.bean.copier.ValueProvider<java.lang.String>);
}
```
