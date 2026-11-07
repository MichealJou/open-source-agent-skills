# com.feilong.lib.javassist.tools.reflect

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.javassist.tools.reflect.CannotCreateException`

```java
public class com.feilong.lib.javassist.tools.reflect.CannotCreateException extends java.lang.Exception {
  public com.feilong.lib.javassist.tools.reflect.CannotCreateException(java.lang.String);
  public com.feilong.lib.javassist.tools.reflect.CannotCreateException(java.lang.Exception);
}
```

## `com.feilong.lib.javassist.tools.reflect.CannotInvokeException`

```java
public class com.feilong.lib.javassist.tools.reflect.CannotInvokeException extends java.lang.RuntimeException {
  public java.lang.Throwable getReason();
  public com.feilong.lib.javassist.tools.reflect.CannotInvokeException(java.lang.String);
  public com.feilong.lib.javassist.tools.reflect.CannotInvokeException(java.lang.reflect.InvocationTargetException);
  public com.feilong.lib.javassist.tools.reflect.CannotInvokeException(java.lang.IllegalAccessException);
  public com.feilong.lib.javassist.tools.reflect.CannotInvokeException(java.lang.ClassNotFoundException);
}
```

## `com.feilong.lib.javassist.tools.reflect.CannotReflectException`

```java
public class com.feilong.lib.javassist.tools.reflect.CannotReflectException extends com.feilong.lib.javassist.CannotCompileException {
  public com.feilong.lib.javassist.tools.reflect.CannotReflectException(java.lang.String);
}
```

## `com.feilong.lib.javassist.tools.reflect.ClassMetaobject`

```java
public class com.feilong.lib.javassist.tools.reflect.ClassMetaobject implements java.io.Serializable {
  public com.feilong.lib.javassist.tools.reflect.ClassMetaobject(java.lang.String[]);
  public final java.lang.Class<?> getJavaClass();
  public final java.lang.String getName();
  public final boolean isInstance(java.lang.Object);
  public final java.lang.Object newInstance(java.lang.Object[]) throws com.feilong.lib.javassist.tools.reflect.CannotCreateException;
  public java.lang.Object trapFieldRead(java.lang.String);
  public void trapFieldWrite(java.lang.String, java.lang.Object);
  public static java.lang.Object invoke(java.lang.Object, int, java.lang.Object[]) throws java.lang.Throwable;
  public java.lang.Object trapMethodcall(int, java.lang.Object[]) throws java.lang.Throwable;
  public final java.lang.reflect.Method[] getReflectiveMethods();
  public final java.lang.reflect.Method getMethod(int);
  public final java.lang.String getMethodName(int);
  public final java.lang.Class<?>[] getParameterTypes(int);
  public final java.lang.Class<?> getReturnType(int);
  public final int getMethodIndex(java.lang.String, java.lang.Class<?>[]) throws java.lang.NoSuchMethodException;
}
```

## `com.feilong.lib.javassist.tools.reflect.Loader`

```java
public class com.feilong.lib.javassist.tools.reflect.Loader extends com.feilong.lib.javassist.Loader {
  public static void main(java.lang.String[]) throws java.lang.Throwable;
  public com.feilong.lib.javassist.tools.reflect.Loader() throws com.feilong.lib.javassist.CannotCompileException, com.feilong.lib.javassist.NotFoundException;
  public boolean makeReflective(java.lang.String, java.lang.String, java.lang.String) throws com.feilong.lib.javassist.CannotCompileException, com.feilong.lib.javassist.NotFoundException;
}
```

## `com.feilong.lib.javassist.tools.reflect.Metalevel`

```java
public interface com.feilong.lib.javassist.tools.reflect.Metalevel {
  public abstract com.feilong.lib.javassist.tools.reflect.ClassMetaobject _getClass();
  public abstract com.feilong.lib.javassist.tools.reflect.Metaobject _getMetaobject();
  public abstract void _setMetaobject(com.feilong.lib.javassist.tools.reflect.Metaobject);
}
```

## `com.feilong.lib.javassist.tools.reflect.Metaobject`

```java
public class com.feilong.lib.javassist.tools.reflect.Metaobject implements java.io.Serializable {
  public com.feilong.lib.javassist.tools.reflect.Metaobject(java.lang.Object, java.lang.Object[]);
  public final com.feilong.lib.javassist.tools.reflect.ClassMetaobject getClassMetaobject();
  public final java.lang.Object getObject();
  public final void setObject(java.lang.Object);
  public final java.lang.String getMethodName(int);
  public final java.lang.Class<?>[] getParameterTypes(int);
  public final java.lang.Class<?> getReturnType(int);
  public java.lang.Object trapMethodcall(int, java.lang.Object[]) throws java.lang.Throwable;
}
```

## `com.feilong.lib.javassist.tools.reflect.Reflection`

```java
public class com.feilong.lib.javassist.tools.reflect.Reflection implements com.feilong.lib.javassist.Translator {
  public com.feilong.lib.javassist.tools.reflect.Reflection();
  public void start(com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.NotFoundException;
  public void onLoad(com.feilong.lib.javassist.ClassPool, java.lang.String) throws com.feilong.lib.javassist.CannotCompileException, com.feilong.lib.javassist.NotFoundException;
  public boolean makeReflective(java.lang.String, java.lang.String, java.lang.String) throws com.feilong.lib.javassist.CannotCompileException, com.feilong.lib.javassist.NotFoundException;
  public boolean makeReflective(java.lang.Class<?>, java.lang.Class<?>, java.lang.Class<?>) throws com.feilong.lib.javassist.CannotCompileException, com.feilong.lib.javassist.NotFoundException;
  public boolean makeReflective(com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException, com.feilong.lib.javassist.tools.reflect.CannotReflectException, com.feilong.lib.javassist.NotFoundException;
  public void rebuildClassFile(com.feilong.lib.javassist.bytecode.ClassFile) throws com.feilong.lib.javassist.bytecode.BadBytecode;
}
```
