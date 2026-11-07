# cn.hutool.core.lang.reflect

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.lang.reflect.ActualTypeMapperPool`

```java
public class cn.hutool.core.lang.reflect.ActualTypeMapperPool {
  public cn.hutool.core.lang.reflect.ActualTypeMapperPool();
  public static java.util.Map<java.lang.reflect.Type, java.lang.reflect.Type> get(java.lang.reflect.Type);
  public static java.util.Map<java.lang.String, java.lang.reflect.Type> getStrKeyMap(java.lang.reflect.Type);
  public static java.lang.reflect.Type getActualType(java.lang.reflect.Type, java.lang.reflect.TypeVariable<?>);
  public static java.lang.reflect.Type getActualType(java.lang.reflect.Type, java.lang.reflect.GenericArrayType);
  public static java.lang.reflect.Type[] getActualTypes(java.lang.reflect.Type, java.lang.reflect.Type...);
}
```

## `cn.hutool.core.lang.reflect.LookupFactory`

```java
public class cn.hutool.core.lang.reflect.LookupFactory {
  public cn.hutool.core.lang.reflect.LookupFactory();
  public static java.lang.invoke.MethodHandles$Lookup lookup(java.lang.Class<?>);
}
```

## `cn.hutool.core.lang.reflect.MethodHandleUtil`

```java
public class cn.hutool.core.lang.reflect.MethodHandleUtil {
  public cn.hutool.core.lang.reflect.MethodHandleUtil();
  public static java.lang.invoke.MethodHandles$Lookup lookup(java.lang.Class<?>);
  public static java.lang.invoke.MethodHandle findMethod(java.lang.Class<?>, java.lang.String, java.lang.invoke.MethodType);
  public static java.lang.invoke.MethodHandle findConstructor(java.lang.Class<?>, java.lang.Class<?>...);
  public static java.lang.invoke.MethodHandle findConstructor(java.lang.Class<?>, java.lang.invoke.MethodType);
  public static <T> T invokeSpecial(java.lang.Object, java.lang.String, java.lang.Object...);
  public static <T> T invoke(java.lang.Object, java.lang.reflect.Method, java.lang.Object...);
  public static <T> T invokeSpecial(java.lang.Object, java.lang.reflect.Method, java.lang.Object...);
  public static <T> T invoke(boolean, java.lang.Object, java.lang.reflect.Method, java.lang.Object...);
}
```
