# com.feilong.lib.lang3.reflect

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.lang3.reflect.ConstructorUtils`

```java
public class com.feilong.lib.lang3.reflect.ConstructorUtils {
  public com.feilong.lib.lang3.reflect.ConstructorUtils();
  public static <T> T invokeConstructor(java.lang.Class<T>, java.lang.Object...) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.InstantiationException;
  public static <T> T invokeConstructor(java.lang.Class<T>, java.lang.Object[], java.lang.Class<?>[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.InstantiationException;
  public static <T> T invokeExactConstructor(java.lang.Class<T>, java.lang.Object...) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.InstantiationException;
  public static <T> T invokeExactConstructor(java.lang.Class<T>, java.lang.Object[], java.lang.Class<?>[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException, java.lang.InstantiationException;
  public static <T> java.lang.reflect.Constructor<T> getAccessibleConstructor(java.lang.Class<T>, java.lang.Class<?>...);
  public static <T> java.lang.reflect.Constructor<T> getAccessibleConstructor(java.lang.reflect.Constructor<T>);
  public static <T> java.lang.reflect.Constructor<T> getMatchingAccessibleConstructor(java.lang.Class<T>, java.lang.Class<?>...);
}
```

## `com.feilong.lib.lang3.reflect.FieldUtils`

```java
public class com.feilong.lib.lang3.reflect.FieldUtils {
  public com.feilong.lib.lang3.reflect.FieldUtils();
  public static java.lang.reflect.Field getField(java.lang.Class<?>, java.lang.String);
  public static java.lang.reflect.Field getField(java.lang.Class<?>, java.lang.String, boolean);
  public static java.lang.reflect.Field getDeclaredField(java.lang.Class<?>, java.lang.String);
  public static java.lang.reflect.Field getDeclaredField(java.lang.Class<?>, java.lang.String, boolean);
  public static java.lang.reflect.Field[] getAllFields(java.lang.Class<?>);
  public static java.util.List<java.lang.reflect.Field> getAllFieldsList(java.lang.Class<?>);
  public static java.lang.reflect.Field[] getFieldsWithAnnotation(java.lang.Class<?>, java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static java.util.List<java.lang.reflect.Field> getFieldsListWithAnnotation(java.lang.Class<?>, java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static java.lang.Object readStaticField(java.lang.reflect.Field) throws java.lang.IllegalAccessException;
  public static java.lang.Object readStaticField(java.lang.reflect.Field, boolean) throws java.lang.IllegalAccessException;
  public static java.lang.Object readStaticField(java.lang.Class<?>, java.lang.String) throws java.lang.IllegalAccessException;
  public static java.lang.Object readStaticField(java.lang.Class<?>, java.lang.String, boolean) throws java.lang.IllegalAccessException;
  public static java.lang.Object readDeclaredStaticField(java.lang.Class<?>, java.lang.String) throws java.lang.IllegalAccessException;
  public static java.lang.Object readDeclaredStaticField(java.lang.Class<?>, java.lang.String, boolean) throws java.lang.IllegalAccessException;
  public static java.lang.Object readField(java.lang.reflect.Field, java.lang.Object) throws java.lang.IllegalAccessException;
  public static java.lang.Object readField(java.lang.reflect.Field, java.lang.Object, boolean) throws java.lang.IllegalAccessException;
  public static java.lang.Object readField(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException;
  public static java.lang.Object readField(java.lang.Object, java.lang.String, boolean) throws java.lang.IllegalAccessException;
  public static java.lang.Object readDeclaredField(java.lang.Object, java.lang.String) throws java.lang.IllegalAccessException;
  public static java.lang.Object readDeclaredField(java.lang.Object, java.lang.String, boolean) throws java.lang.IllegalAccessException;
  public static void writeStaticField(java.lang.reflect.Field, java.lang.Object) throws java.lang.IllegalAccessException;
  public static void writeStaticField(java.lang.reflect.Field, java.lang.Object, boolean) throws java.lang.IllegalAccessException;
  public static void writeStaticField(java.lang.Class<?>, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException;
  public static void writeStaticField(java.lang.Class<?>, java.lang.String, java.lang.Object, boolean) throws java.lang.IllegalAccessException;
  public static void writeDeclaredStaticField(java.lang.Class<?>, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException;
  public static void writeDeclaredStaticField(java.lang.Class<?>, java.lang.String, java.lang.Object, boolean) throws java.lang.IllegalAccessException;
  public static void writeField(java.lang.reflect.Field, java.lang.Object, java.lang.Object) throws java.lang.IllegalAccessException;
  public static void writeField(java.lang.reflect.Field, java.lang.Object, java.lang.Object, boolean) throws java.lang.IllegalAccessException;
  public static void writeField(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException;
  public static void writeField(java.lang.Object, java.lang.String, java.lang.Object, boolean) throws java.lang.IllegalAccessException;
  public static void writeDeclaredField(java.lang.Object, java.lang.String, java.lang.Object) throws java.lang.IllegalAccessException;
  public static void writeDeclaredField(java.lang.Object, java.lang.String, java.lang.Object, boolean) throws java.lang.IllegalAccessException;
}
```

## `com.feilong.lib.lang3.reflect.MethodUtils`

```java
public class com.feilong.lib.lang3.reflect.MethodUtils {
  public com.feilong.lib.lang3.reflect.MethodUtils();
  public static java.lang.Object invokeMethod(java.lang.Object, java.lang.String) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeMethod(java.lang.Object, boolean, java.lang.String) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeMethod(java.lang.Object, java.lang.String, java.lang.Object...) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeMethod(java.lang.Object, boolean, java.lang.String, java.lang.Object...) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeMethod(java.lang.Object, boolean, java.lang.String, java.lang.Object[], java.lang.Class<?>[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeMethod(java.lang.Object, java.lang.String, java.lang.Object[], java.lang.Class<?>[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeExactMethod(java.lang.Object, java.lang.String) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeExactMethod(java.lang.Object, java.lang.String, java.lang.Object...) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeExactMethod(java.lang.Object, java.lang.String, java.lang.Object[], java.lang.Class<?>[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeExactStaticMethod(java.lang.Class<?>, java.lang.String, java.lang.Object[], java.lang.Class<?>[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeStaticMethod(java.lang.Class<?>, java.lang.String, java.lang.Object...) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeStaticMethod(java.lang.Class<?>, java.lang.String, java.lang.Object[], java.lang.Class<?>[]) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.Object invokeExactStaticMethod(java.lang.Class<?>, java.lang.String, java.lang.Object...) throws java.lang.NoSuchMethodException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public static java.lang.reflect.Method getAccessibleMethod(java.lang.Class<?>, java.lang.String, java.lang.Class<?>...);
  public static java.lang.reflect.Method getAccessibleMethod(java.lang.reflect.Method);
  public static java.lang.reflect.Method getMatchingAccessibleMethod(java.lang.Class<?>, java.lang.String, java.lang.Class<?>...);
  public static java.lang.reflect.Method getMatchingMethod(java.lang.Class<?>, java.lang.String, java.lang.Class<?>...);
  public static java.lang.reflect.Method[] getMethodsWithAnnotation(java.lang.Class<?>, java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static java.util.List<java.lang.reflect.Method> getMethodsListWithAnnotation(java.lang.Class<?>, java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static java.lang.reflect.Method[] getMethodsWithAnnotation(java.lang.Class<?>, java.lang.Class<? extends java.lang.annotation.Annotation>, boolean, boolean);
  public static java.util.List<java.lang.reflect.Method> getMethodsListWithAnnotation(java.lang.Class<?>, java.lang.Class<? extends java.lang.annotation.Annotation>, boolean, boolean);
  public static <A extends java.lang.annotation.Annotation> A getAnnotation(java.lang.reflect.Method, java.lang.Class<A>, boolean, boolean);
}
```
