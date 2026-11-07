# cn.hutool.extra.cglib

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.cglib.BeanCopierCache`

```java
public final class cn.hutool.extra.cglib.BeanCopierCache extends java.lang.Enum<cn.hutool.extra.cglib.BeanCopierCache> {
  public static cn.hutool.extra.cglib.BeanCopierCache[] values();
  public static cn.hutool.extra.cglib.BeanCopierCache valueOf(java.lang.String);
  public net.sf.cglib.beans.BeanCopier get(java.lang.Class<?>, java.lang.Class<?>, net.sf.cglib.core.Converter);
  public net.sf.cglib.beans.BeanCopier get(java.lang.Class<?>, java.lang.Class<?>, boolean);
}
```

## `cn.hutool.extra.cglib.CglibUtil`

```java
public class cn.hutool.extra.cglib.CglibUtil {
  public cn.hutool.extra.cglib.CglibUtil();
  public static <T> T copy(java.lang.Object, java.lang.Class<T>);
  public static <T> T copy(java.lang.Object, java.lang.Class<T>, net.sf.cglib.core.Converter);
  public static void copy(java.lang.Object, java.lang.Object);
  public static void copy(java.lang.Object, java.lang.Object, net.sf.cglib.core.Converter);
  public static <S, T> java.util.List<T> copyList(java.util.Collection<S>, java.util.function.Supplier<T>);
  public static <S, T> java.util.List<T> copyList(java.util.Collection<S>, java.util.function.Supplier<T>, net.sf.cglib.core.Converter);
  public static <S, T> java.util.List<T> copyList(java.util.Collection<S>, java.util.function.Supplier<T>, java.util.function.BiConsumer<S, T>);
  public static <S, T> java.util.List<T> copyList(java.util.Collection<S>, java.util.function.Supplier<T>, net.sf.cglib.core.Converter, java.util.function.BiConsumer<S, T>);
  public static net.sf.cglib.beans.BeanMap toMap(java.lang.Object);
  public static <T> T fillBean(java.util.Map, T);
  public static <T> T toBean(java.util.Map, java.lang.Class<T>);
}
```
