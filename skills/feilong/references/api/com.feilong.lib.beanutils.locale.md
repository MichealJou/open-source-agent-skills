# com.feilong.lib.beanutils.locale

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.beanutils.locale.BaseLocaleConverter`

```java
public abstract class com.feilong.lib.beanutils.locale.BaseLocaleConverter implements com.feilong.lib.beanutils.locale.LocaleConverter {
  public java.lang.Object convert(java.lang.Object);
  public java.lang.Object convert(java.lang.Object, java.lang.String);
  public <T> T convert(java.lang.Class<T>, java.lang.Object);
  public <T> T convert(java.lang.Class<T>, java.lang.Object, java.lang.String);
}
```

## `com.feilong.lib.beanutils.locale.LocaleBeanUtils`

```java
public class com.feilong.lib.beanutils.locale.LocaleBeanUtils extends com.feilong.lib.beanutils.BeanUtils {
  public com.feilong.lib.beanutils.locale.LocaleBeanUtils();
  public static java.util.Locale getDefaultLocale();
  public static void setDefaultLocale(java.util.Locale);
  public static boolean getApplyLocalized();
  public static void setApplyLocalized(boolean);
  public static java.lang.String getIndexedProperty(java.lang.Object, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.String getIndexedProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.String getIndexedProperty(java.lang.Object, java.lang.String, int, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.String getIndexedProperty(java.lang.Object, java.lang.String, int) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.String getSimpleProperty(java.lang.Object, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.String getSimpleProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.String getMappedProperty(java.lang.Object, java.lang.String, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.String getMappedProperty(java.lang.Object, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.String getMappedPropertyLocale(java.lang.Object, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.String getMappedProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.String getNestedProperty(java.lang.Object, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.String getNestedProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.String getProperty(java.lang.Object, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static java.lang.String getProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public static void setProperty(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static void setProperty(java.lang.Object, java.lang.String, java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
}
```

## `com.feilong.lib.beanutils.locale.LocaleBeanUtilsBean`

```java
public class com.feilong.lib.beanutils.locale.LocaleBeanUtilsBean extends com.feilong.lib.beanutils.BeanUtilsBean {
  public static com.feilong.lib.beanutils.locale.LocaleBeanUtilsBean getLocaleBeanUtilsInstance();
  public static void setInstance(com.feilong.lib.beanutils.locale.LocaleBeanUtilsBean);
  public com.feilong.lib.beanutils.locale.LocaleBeanUtilsBean();
  public com.feilong.lib.beanutils.locale.LocaleBeanUtilsBean(com.feilong.lib.beanutils.locale.LocaleConvertUtilsBean, com.feilong.lib.beanutils.ConvertUtilsBean, com.feilong.lib.beanutils.PropertyUtilsBean);
  public com.feilong.lib.beanutils.locale.LocaleBeanUtilsBean(com.feilong.lib.beanutils.locale.LocaleConvertUtilsBean);
  public com.feilong.lib.beanutils.locale.LocaleConvertUtilsBean getLocaleConvertUtils();
  public java.util.Locale getDefaultLocale();
  public void setDefaultLocale(java.util.Locale);
  public boolean getApplyLocalized();
  public void setApplyLocalized(boolean);
  public java.lang.String getIndexedProperty(java.lang.Object, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getIndexedProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getIndexedProperty(java.lang.Object, java.lang.String, int, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getIndexedProperty(java.lang.Object, java.lang.String, int) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getSimpleProperty(java.lang.Object, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getSimpleProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getMappedProperty(java.lang.Object, java.lang.String, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getMappedProperty(java.lang.Object, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getMappedPropertyLocale(java.lang.Object, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getMappedProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getNestedProperty(java.lang.Object, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getNestedProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getProperty(java.lang.Object, java.lang.String, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public java.lang.String getProperty(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.NoSuchMethodException;
  public void setProperty(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public void setProperty(java.lang.Object, java.lang.String, java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
}
```

## `com.feilong.lib.beanutils.locale.LocaleBeanUtilsBean$Descriptor`

```java
public class com.feilong.lib.beanutils.locale.LocaleBeanUtilsBean$Descriptor {
  public com.feilong.lib.beanutils.locale.LocaleBeanUtilsBean$Descriptor(com.feilong.lib.beanutils.locale.LocaleBeanUtilsBean, java.lang.Object, java.lang.String, java.lang.String, java.lang.String, int);
  public java.lang.Object getTarget();
  public void setTarget(java.lang.Object);
  public java.lang.String getKey();
  public void setKey(java.lang.String);
  public int getIndex();
  public void setIndex(int);
  public java.lang.String getName();
  public void setName(java.lang.String);
  public java.lang.String getPropName();
  public void setPropName(java.lang.String);
}
```

## `com.feilong.lib.beanutils.locale.LocaleConvertUtils`

```java
public class com.feilong.lib.beanutils.locale.LocaleConvertUtils {
  public com.feilong.lib.beanutils.locale.LocaleConvertUtils();
  public static java.util.Locale getDefaultLocale();
  public static void setDefaultLocale(java.util.Locale);
  public static boolean getApplyLocalized();
  public static void setApplyLocalized(boolean);
  public static java.lang.String convert(java.lang.Object);
  public static java.lang.String convert(java.lang.Object, java.lang.String);
  public static java.lang.String convert(java.lang.Object, java.util.Locale, java.lang.String);
  public static java.lang.Object convert(java.lang.String, java.lang.Class<?>);
  public static java.lang.Object convert(java.lang.String, java.lang.Class<?>, java.lang.String);
  public static java.lang.Object convert(java.lang.String, java.lang.Class<?>, java.util.Locale, java.lang.String);
  public static java.lang.Object convert(java.lang.String[], java.lang.Class<?>, java.lang.String);
  public static java.lang.Object convert(java.lang.String[], java.lang.Class<?>);
  public static java.lang.Object convert(java.lang.String[], java.lang.Class<?>, java.util.Locale, java.lang.String);
  public static void register(com.feilong.lib.beanutils.locale.LocaleConverter, java.lang.Class<?>, java.util.Locale);
  public static void deregister();
  public static void deregister(java.util.Locale);
  public static void deregister(java.lang.Class<?>, java.util.Locale);
  public static com.feilong.lib.beanutils.locale.LocaleConverter lookup(java.lang.Class<?>, java.util.Locale);
}
```

## `com.feilong.lib.beanutils.locale.LocaleConvertUtilsBean`

```java
public class com.feilong.lib.beanutils.locale.LocaleConvertUtilsBean {
  public static com.feilong.lib.beanutils.locale.LocaleConvertUtilsBean getInstance();
  public com.feilong.lib.beanutils.locale.LocaleConvertUtilsBean();
  public java.util.Locale getDefaultLocale();
  public void setDefaultLocale(java.util.Locale);
  public boolean getApplyLocalized();
  public void setApplyLocalized(boolean);
  public java.lang.String convert(java.lang.Object);
  public java.lang.String convert(java.lang.Object, java.lang.String);
  public java.lang.String convert(java.lang.Object, java.util.Locale, java.lang.String);
  public java.lang.Object convert(java.lang.String, java.lang.Class<?>);
  public java.lang.Object convert(java.lang.String, java.lang.Class<?>, java.lang.String);
  public java.lang.Object convert(java.lang.String, java.lang.Class<?>, java.util.Locale, java.lang.String);
  public java.lang.Object convert(java.lang.String[], java.lang.Class<?>, java.lang.String);
  public java.lang.Object convert(java.lang.String[], java.lang.Class<?>);
  public java.lang.Object convert(java.lang.String[], java.lang.Class<?>, java.util.Locale, java.lang.String);
  public void register(com.feilong.lib.beanutils.locale.LocaleConverter, java.lang.Class<?>, java.util.Locale);
  public void deregister();
  public void deregister(java.util.Locale);
  public void deregister(java.lang.Class<?>, java.util.Locale);
  public com.feilong.lib.beanutils.locale.LocaleConverter lookup(java.lang.Class<?>, java.util.Locale);
}
```

## `com.feilong.lib.beanutils.locale.LocaleConverter`

```java
public interface com.feilong.lib.beanutils.locale.LocaleConverter extends com.feilong.lib.beanutils.Converter {
  public abstract <T> T convert(java.lang.Class<T>, java.lang.Object, java.lang.String);
}
```
