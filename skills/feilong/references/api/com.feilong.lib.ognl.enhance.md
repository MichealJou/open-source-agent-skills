# com.feilong.lib.ognl.enhance

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.ognl.enhance.ContextClassLoader`

```java
public class com.feilong.lib.ognl.enhance.ContextClassLoader extends java.lang.ClassLoader {
  public com.feilong.lib.ognl.enhance.ContextClassLoader(java.lang.ClassLoader, com.feilong.lib.ognl.OgnlContext);
}
```

## `com.feilong.lib.ognl.enhance.EnhancedClassLoader`

```java
public class com.feilong.lib.ognl.enhance.EnhancedClassLoader extends java.lang.ClassLoader {
  public com.feilong.lib.ognl.enhance.EnhancedClassLoader(java.lang.ClassLoader);
  public java.lang.Class defineClass(java.lang.String, byte[]);
}
```

## `com.feilong.lib.ognl.enhance.ExpressionAccessor`

```java
public interface com.feilong.lib.ognl.enhance.ExpressionAccessor {
  public abstract java.lang.Object get(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public abstract void set(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.ognl.enhance.ExpressionCompiler`

```java
public class com.feilong.lib.ognl.enhance.ExpressionCompiler implements com.feilong.lib.ognl.enhance.OgnlExpressionCompiler {
  public com.feilong.lib.ognl.enhance.ExpressionCompiler();
  public static void addCastString(com.feilong.lib.ognl.OgnlContext, java.lang.String);
  public static java.lang.String getCastString(java.lang.Class);
  public static java.lang.String getRootExpression(com.feilong.lib.ognl.Node, java.lang.Object, com.feilong.lib.ognl.OgnlContext);
  public static boolean shouldCast(com.feilong.lib.ognl.Node);
  public java.lang.String castExpression(com.feilong.lib.ognl.OgnlContext, com.feilong.lib.ognl.Node, java.lang.String);
  public java.lang.String getClassName(java.lang.Class);
  public java.lang.Class getSuperOrInterfaceClass(java.lang.reflect.Method, java.lang.Class);
  public boolean containsMethod(java.lang.reflect.Method, java.lang.Class);
  public java.lang.Class getInterfaceClass(java.lang.Class);
  public java.lang.Class getRootExpressionClass(com.feilong.lib.ognl.Node, com.feilong.lib.ognl.OgnlContext);
  public java.lang.String createLocalReference(com.feilong.lib.ognl.OgnlContext, java.lang.String, java.lang.Class);
}
```

## `com.feilong.lib.ognl.enhance.LocalReference`

```java
public interface com.feilong.lib.ognl.enhance.LocalReference {
  public abstract java.lang.String getName();
  public abstract java.lang.String getExpression();
  public abstract java.lang.Class getType();
}
```

## `com.feilong.lib.ognl.enhance.LocalReferenceImpl`

```java
public class com.feilong.lib.ognl.enhance.LocalReferenceImpl implements com.feilong.lib.ognl.enhance.LocalReference {
  public com.feilong.lib.ognl.enhance.LocalReferenceImpl(java.lang.String, java.lang.String, java.lang.Class);
  public java.lang.String getName();
  public java.lang.String getExpression();
  public java.lang.Class getType();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.feilong.lib.ognl.enhance.OgnlExpressionCompiler`

```java
public interface com.feilong.lib.ognl.enhance.OgnlExpressionCompiler {
  public abstract java.lang.String getClassName(java.lang.Class);
  public abstract java.lang.Class getInterfaceClass(java.lang.Class);
  public abstract java.lang.Class getSuperOrInterfaceClass(java.lang.reflect.Method, java.lang.Class);
  public abstract java.lang.Class getRootExpressionClass(com.feilong.lib.ognl.Node, com.feilong.lib.ognl.OgnlContext);
  public abstract java.lang.String castExpression(com.feilong.lib.ognl.OgnlContext, com.feilong.lib.ognl.Node, java.lang.String);
  public abstract java.lang.String createLocalReference(com.feilong.lib.ognl.OgnlContext, java.lang.String, java.lang.Class);
}
```

## `com.feilong.lib.ognl.enhance.OrderedReturn`

```java
public interface com.feilong.lib.ognl.enhance.OrderedReturn {
  public abstract java.lang.String getCoreExpression();
  public abstract java.lang.String getLastExpression();
}
```

## `com.feilong.lib.ognl.enhance.UnsupportedCompilationException`

```java
public class com.feilong.lib.ognl.enhance.UnsupportedCompilationException extends java.lang.RuntimeException {
  public com.feilong.lib.ognl.enhance.UnsupportedCompilationException(java.lang.String);
  public com.feilong.lib.ognl.enhance.UnsupportedCompilationException(java.lang.String, java.lang.Throwable);
}
```
