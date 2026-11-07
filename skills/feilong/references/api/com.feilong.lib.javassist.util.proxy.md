# com.feilong.lib.javassist.util.proxy

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.javassist.util.proxy.DefineClassHelper`

```java
public class com.feilong.lib.javassist.util.proxy.DefineClassHelper {
  public static java.lang.Class<?> toClass(java.lang.String, java.lang.Class<?>, java.lang.ClassLoader, java.security.ProtectionDomain, byte[]) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.util.proxy.DefinePackageHelper`

```java
public class com.feilong.lib.javassist.util.proxy.DefinePackageHelper {
  public static void definePackage(java.lang.String, java.lang.ClassLoader) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.util.proxy.FactoryHelper`

```java
public class com.feilong.lib.javassist.util.proxy.FactoryHelper {
  public com.feilong.lib.javassist.util.proxy.FactoryHelper();
  public static final int typeIndex(java.lang.Class<?>);
  public static java.lang.Class<?> toClass(com.feilong.lib.javassist.bytecode.ClassFile, java.lang.Class<?>, java.lang.ClassLoader, java.security.ProtectionDomain) throws com.feilong.lib.javassist.CannotCompileException;
  public static void writeFile(com.feilong.lib.javassist.bytecode.ClassFile, java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.util.proxy.MethodFilter`

```java
public interface com.feilong.lib.javassist.util.proxy.MethodFilter {
  public abstract boolean isHandled(java.lang.reflect.Method);
}
```

## `com.feilong.lib.javassist.util.proxy.MethodHandler`

```java
public interface com.feilong.lib.javassist.util.proxy.MethodHandler {
  public abstract java.lang.Object invoke(java.lang.Object, java.lang.reflect.Method, java.lang.reflect.Method, java.lang.Object[]) throws java.lang.Throwable;
}
```

## `com.feilong.lib.javassist.util.proxy.Proxy`

```java
public interface com.feilong.lib.javassist.util.proxy.Proxy {
  public abstract void setHandler(com.feilong.lib.javassist.util.proxy.MethodHandler);
}
```

## `com.feilong.lib.javassist.util.proxy.ProxyFactory`

```java
public class com.feilong.lib.javassist.util.proxy.ProxyFactory {
  public boolean isUseCache();
  public void setUseCache(boolean);
  public boolean isUseWriteReplace();
  public void setUseWriteReplace(boolean);
  public static boolean isProxyClass(java.lang.Class<?>);
  public com.feilong.lib.javassist.util.proxy.ProxyFactory();
  public void setSuperclass(java.lang.Class<?>);
  public java.lang.Class<?> getSuperclass();
  public void setInterfaces(java.lang.Class<?>[]);
  public java.lang.Class<?>[] getInterfaces();
  public void setFilter(com.feilong.lib.javassist.util.proxy.MethodFilter);
  public java.lang.Class<?> createClass();
  public java.lang.Class<?> createClass(com.feilong.lib.javassist.util.proxy.MethodFilter);
  public java.lang.Class<?> createClass(java.lang.invoke.MethodHandles$Lookup);
  public java.lang.Class<?> createClass(java.lang.invoke.MethodHandles$Lookup, com.feilong.lib.javassist.util.proxy.MethodFilter);
  public java.lang.String getKey(java.lang.Class<?>, java.lang.Class<?>[], byte[], boolean);
  public static com.feilong.lib.javassist.util.proxy.MethodHandler getHandler(com.feilong.lib.javassist.util.proxy.Proxy);
  public java.lang.Object create(java.lang.Class<?>[], java.lang.Object[], com.feilong.lib.javassist.util.proxy.MethodHandler) throws java.lang.NoSuchMethodException, java.lang.IllegalArgumentException, java.lang.InstantiationException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
  public java.lang.Object create(java.lang.Class<?>[], java.lang.Object[]) throws java.lang.NoSuchMethodException, java.lang.IllegalArgumentException, java.lang.InstantiationException, java.lang.IllegalAccessException, java.lang.reflect.InvocationTargetException;
}
```

## `com.feilong.lib.javassist.util.proxy.ProxyFactory$ClassLoaderProvider`

```java
public interface com.feilong.lib.javassist.util.proxy.ProxyFactory$ClassLoaderProvider {
  public abstract java.lang.ClassLoader get(com.feilong.lib.javassist.util.proxy.ProxyFactory);
}
```

## `com.feilong.lib.javassist.util.proxy.ProxyFactory$UniqueName`

```java
public interface com.feilong.lib.javassist.util.proxy.ProxyFactory$UniqueName {
  public abstract java.lang.String get(java.lang.String);
}
```

## `com.feilong.lib.javassist.util.proxy.ProxyObject`

```java
public interface com.feilong.lib.javassist.util.proxy.ProxyObject extends com.feilong.lib.javassist.util.proxy.Proxy {
  public abstract void setHandler(com.feilong.lib.javassist.util.proxy.MethodHandler);
  public abstract com.feilong.lib.javassist.util.proxy.MethodHandler getHandler();
}
```

## `com.feilong.lib.javassist.util.proxy.ProxyObjectInputStream`

```java
public class com.feilong.lib.javassist.util.proxy.ProxyObjectInputStream extends java.io.ObjectInputStream {
  public com.feilong.lib.javassist.util.proxy.ProxyObjectInputStream(java.io.InputStream) throws java.io.IOException;
  public void setClassLoader(java.lang.ClassLoader);
}
```

## `com.feilong.lib.javassist.util.proxy.ProxyObjectOutputStream`

```java
public class com.feilong.lib.javassist.util.proxy.ProxyObjectOutputStream extends java.io.ObjectOutputStream {
  public com.feilong.lib.javassist.util.proxy.ProxyObjectOutputStream(java.io.OutputStream) throws java.io.IOException;
}
```

## `com.feilong.lib.javassist.util.proxy.RuntimeSupport`

```java
public class com.feilong.lib.javassist.util.proxy.RuntimeSupport {
  public com.feilong.lib.javassist.util.proxy.RuntimeSupport();
  public static void find2Methods(java.lang.Class<?>, java.lang.String, java.lang.String, int, java.lang.String, java.lang.reflect.Method[]);
  public static java.lang.reflect.Method findMethod(java.lang.Class<?>, java.lang.String, java.lang.String);
  public static java.lang.reflect.Method findSuperMethod(java.lang.Object, java.lang.String, java.lang.String);
  public static java.lang.reflect.Method findSuperClassMethod(java.lang.Class<?>, java.lang.String, java.lang.String);
  public static java.lang.String makeDescriptor(java.lang.reflect.Method);
  public static java.lang.String makeDescriptor(java.lang.Class<?>[], java.lang.Class<?>);
  public static java.lang.String makeDescriptor(java.lang.String, java.lang.Class<?>);
  public static com.feilong.lib.javassist.util.proxy.SerializedProxy makeSerializedProxy(java.lang.Object) throws java.io.InvalidClassException;
}
```
