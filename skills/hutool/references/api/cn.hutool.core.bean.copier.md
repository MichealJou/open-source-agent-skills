# cn.hutool.core.bean.copier

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.bean.copier.AbsCopier`

```java
public abstract class cn.hutool.core.bean.copier.AbsCopier<S, T> implements cn.hutool.core.lang.copier.Copier<T> {
  public cn.hutool.core.bean.copier.AbsCopier(S, T, cn.hutool.core.bean.copier.CopyOptions);
}
```

## `cn.hutool.core.bean.copier.BeanCopier`

```java
public class cn.hutool.core.bean.copier.BeanCopier<T> implements cn.hutool.core.lang.copier.Copier<T>, java.io.Serializable {
  public static <T> cn.hutool.core.bean.copier.BeanCopier<T> create(java.lang.Object, T, cn.hutool.core.bean.copier.CopyOptions);
  public static <T> cn.hutool.core.bean.copier.BeanCopier<T> create(java.lang.Object, T, java.lang.reflect.Type, cn.hutool.core.bean.copier.CopyOptions);
  public cn.hutool.core.bean.copier.BeanCopier(java.lang.Object, T, java.lang.reflect.Type, cn.hutool.core.bean.copier.CopyOptions);
  public T copy();
}
```

## `cn.hutool.core.bean.copier.BeanToBeanCopier`

```java
public class cn.hutool.core.bean.copier.BeanToBeanCopier<S, T> extends cn.hutool.core.bean.copier.AbsCopier<S, T> {
  public cn.hutool.core.bean.copier.BeanToBeanCopier(S, T, java.lang.reflect.Type, cn.hutool.core.bean.copier.CopyOptions);
  public T copy();
}
```

## `cn.hutool.core.bean.copier.BeanToMapCopier`

```java
public class cn.hutool.core.bean.copier.BeanToMapCopier extends cn.hutool.core.bean.copier.AbsCopier<java.lang.Object, java.util.Map> {
  public cn.hutool.core.bean.copier.BeanToMapCopier(java.lang.Object, java.util.Map, java.lang.reflect.Type, cn.hutool.core.bean.copier.CopyOptions);
  public java.util.Map copy();
  public java.lang.Object copy();
}
```

## `cn.hutool.core.bean.copier.CopyOptions`

```java
public class cn.hutool.core.bean.copier.CopyOptions implements java.io.Serializable {
  public static cn.hutool.core.bean.copier.CopyOptions create();
  public static cn.hutool.core.bean.copier.CopyOptions create(java.lang.Class<?>, boolean, java.lang.String...);
  public cn.hutool.core.bean.copier.CopyOptions();
  public cn.hutool.core.bean.copier.CopyOptions(java.lang.Class<?>, boolean, java.lang.String...);
  public cn.hutool.core.bean.copier.CopyOptions setEditable(java.lang.Class<?>);
  public cn.hutool.core.bean.copier.CopyOptions setIgnoreNullValue(boolean);
  public cn.hutool.core.bean.copier.CopyOptions ignoreNullValue();
  public cn.hutool.core.bean.copier.CopyOptions setPropertiesFilter(java.util.function.BiPredicate<java.lang.reflect.Field, java.lang.Object>);
  public cn.hutool.core.bean.copier.CopyOptions setIgnoreProperties(java.lang.String...);
  public <P, R> cn.hutool.core.bean.copier.CopyOptions setIgnoreProperties(cn.hutool.core.lang.func.Func1<P, R>...);
  public cn.hutool.core.bean.copier.CopyOptions setIgnoreError(boolean);
  public cn.hutool.core.bean.copier.CopyOptions ignoreError();
  public cn.hutool.core.bean.copier.CopyOptions setIgnoreCase(boolean);
  public cn.hutool.core.bean.copier.CopyOptions ignoreCase();
  public cn.hutool.core.bean.copier.CopyOptions setFieldMapping(java.util.Map<java.lang.String, java.lang.String>);
  public cn.hutool.core.bean.copier.CopyOptions setFieldNameEditor(cn.hutool.core.lang.Editor<java.lang.String>);
  public cn.hutool.core.bean.copier.CopyOptions setFieldValueEditor(java.util.function.BiFunction<java.lang.String, java.lang.Object, java.lang.Object>);
  public cn.hutool.core.bean.copier.CopyOptions setTransientSupport(boolean);
  public cn.hutool.core.bean.copier.CopyOptions setOverride(boolean);
  public cn.hutool.core.bean.copier.CopyOptions setAutoTransCamelCase(boolean);
  public cn.hutool.core.bean.copier.CopyOptions setConverter(cn.hutool.core.convert.TypeConverter);
  public java.lang.String getFormatIfDate();
  public cn.hutool.core.bean.copier.CopyOptions setFormatIfDate(java.lang.String);
}
```

## `cn.hutool.core.bean.copier.IJSONTypeConverter`

```java
public interface cn.hutool.core.bean.copier.IJSONTypeConverter {
  public abstract <T> T toBean(java.lang.reflect.Type);
}
```

## `cn.hutool.core.bean.copier.MapToBeanCopier`

```java
public class cn.hutool.core.bean.copier.MapToBeanCopier<T> extends cn.hutool.core.bean.copier.AbsCopier<java.util.Map<?, ?>, T> {
  public cn.hutool.core.bean.copier.MapToBeanCopier(java.util.Map<?, ?>, T, java.lang.reflect.Type, cn.hutool.core.bean.copier.CopyOptions);
  public T copy();
}
```

## `cn.hutool.core.bean.copier.MapToMapCopier`

```java
public class cn.hutool.core.bean.copier.MapToMapCopier extends cn.hutool.core.bean.copier.AbsCopier<java.util.Map, java.util.Map> {
  public cn.hutool.core.bean.copier.MapToMapCopier(java.util.Map, java.util.Map, java.lang.reflect.Type, cn.hutool.core.bean.copier.CopyOptions);
  public java.util.Map copy();
  public java.lang.Object copy();
}
```

## `cn.hutool.core.bean.copier.ValueProvider`

```java
public interface cn.hutool.core.bean.copier.ValueProvider<T> {
  public abstract java.lang.Object value(T, java.lang.reflect.Type);
  public abstract boolean containsKey(T);
}
```

## `cn.hutool.core.bean.copier.ValueProviderToBeanCopier`

```java
public class cn.hutool.core.bean.copier.ValueProviderToBeanCopier<T> extends cn.hutool.core.bean.copier.AbsCopier<cn.hutool.core.bean.copier.ValueProvider<java.lang.String>, T> {
  public cn.hutool.core.bean.copier.ValueProviderToBeanCopier(cn.hutool.core.bean.copier.ValueProvider<java.lang.String>, T, java.lang.reflect.Type, cn.hutool.core.bean.copier.CopyOptions);
  public T copy();
}
```
