# com.baomidou.mybatisplus.core.toolkit.reflect

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.toolkit.reflect.GenericTypeUtils`

```java
public class com.baomidou.mybatisplus.core.toolkit.reflect.GenericTypeUtils {
  public com.baomidou.mybatisplus.core.toolkit.reflect.GenericTypeUtils();
  public static java.lang.Class<?>[] resolveTypeArguments(java.lang.Class<?>, java.lang.Class<?>);
  public static void setGenericTypeResolver(com.baomidou.mybatisplus.core.toolkit.reflect.IGenericTypeResolver);
  public static boolean hasGenericTypeResolver();
}
```

## `com.baomidou.mybatisplus.core.toolkit.reflect.IGenericTypeResolver`

```java
public interface com.baomidou.mybatisplus.core.toolkit.reflect.IGenericTypeResolver {
  public abstract java.lang.Class<?>[] resolveTypeArguments(java.lang.Class<?>, java.lang.Class<?>);
}
```

## `com.baomidou.mybatisplus.core.toolkit.reflect.SpringReflectionHelper`

```java
public class com.baomidou.mybatisplus.core.toolkit.reflect.SpringReflectionHelper {
  public com.baomidou.mybatisplus.core.toolkit.reflect.SpringReflectionHelper();
  public static java.lang.Class<?>[] resolveTypeArguments(java.lang.Class<?>, java.lang.Class<?>);
}
```

## `com.baomidou.mybatisplus.core.toolkit.reflect.TypeParameterResolver`

```java
public class com.baomidou.mybatisplus.core.toolkit.reflect.TypeParameterResolver {
  public static java.lang.reflect.Type resolveClassIndexedParameter(java.lang.reflect.Type, java.lang.Class<?>, int);
  public static java.lang.reflect.Type calculateParameterValue(java.util.Map<java.lang.reflect.TypeVariable<?>, java.lang.reflect.Type>, java.lang.reflect.TypeVariable<?>);
  public static java.util.Map<java.lang.reflect.TypeVariable<?>, java.lang.reflect.Type> resolveParameterValues(java.lang.reflect.Type);
  public void visitType(java.lang.reflect.Type);
}
```
