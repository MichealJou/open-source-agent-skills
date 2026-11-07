# com.feilong.core.lang.reflect

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.core.lang.reflect.ConstructorUtil`

```java
public final class com.feilong.core.lang.reflect.ConstructorUtil {
  public static <T> T newInstance(java.lang.Class<T>, java.lang.Object...);
  public static <T> T newInstance(java.lang.Class<T>, java.lang.Object[], java.lang.Class<?>[]);
}
```

## `com.feilong.core.lang.reflect.FieldUtil`

```java
public final class com.feilong.core.lang.reflect.FieldUtil {
  public static java.util.Map<java.lang.String, java.lang.Object> getAllFieldNameAndValueMap(java.lang.Object, java.lang.String...);
  public static java.util.List<java.lang.reflect.Field> getAllFieldList(java.lang.Class<?>, java.lang.String...);
}
```

## `com.feilong.core.lang.reflect.MethodUtil`

```java
public final class com.feilong.core.lang.reflect.MethodUtil {
  public static <T> T invokeMethod(java.lang.Object, java.lang.String, java.lang.Object...);
  public static <T> T invokeMethod(java.lang.Object, java.lang.String, java.lang.Object[], java.lang.Class<?>[]);
  public static <T> T invokeStaticMethod(java.lang.Class<?>, java.lang.String, java.lang.Object...);
  public static <T> T invokeStaticMethod(java.lang.Class<?>, java.lang.String, java.lang.Object[], java.lang.Class<?>[]);
}
```

## `com.feilong.core.lang.reflect.ReflectException`

```java
public final class com.feilong.core.lang.reflect.ReflectException extends com.feilong.core.DefaultRuntimeException {
  public com.feilong.core.lang.reflect.ReflectException(java.lang.String, java.lang.Throwable);
  public com.feilong.core.lang.reflect.ReflectException(java.lang.Throwable);
}
```

## `com.feilong.core.lang.reflect.TypeUtil`

```java
public final class com.feilong.core.lang.reflect.TypeUtil {
  public static java.lang.Class<?>[] getGenericSuperclassParameterizedRawTypes(java.lang.Class<?>);
  public static java.lang.Class<?>[] getGenericInterfacesParameterizedRawTypes(java.lang.Class<?>, java.lang.Class<?>);
}
```
