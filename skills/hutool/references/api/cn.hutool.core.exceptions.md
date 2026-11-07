# cn.hutool.core.exceptions

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.exceptions.CheckedUtil`

```java
public class cn.hutool.core.exceptions.CheckedUtil {
  public cn.hutool.core.exceptions.CheckedUtil();
  public static <P, R> cn.hutool.core.exceptions.CheckedUtil$FuncRt<P, R> uncheck(cn.hutool.core.lang.func.Func<P, R>);
  public static <R> cn.hutool.core.exceptions.CheckedUtil$Func0Rt<R> uncheck(cn.hutool.core.lang.func.Func0<R>);
  public static <P, R> cn.hutool.core.exceptions.CheckedUtil$Func1Rt<P, R> uncheck(cn.hutool.core.lang.func.Func1<P, R>);
  public static <P> cn.hutool.core.exceptions.CheckedUtil$VoidFuncRt<P> uncheck(cn.hutool.core.lang.func.VoidFunc<P>);
  public static cn.hutool.core.exceptions.CheckedUtil$VoidFunc0Rt uncheck(cn.hutool.core.lang.func.VoidFunc0);
  public static <P> cn.hutool.core.exceptions.CheckedUtil$VoidFunc1Rt<P> uncheck(cn.hutool.core.lang.func.VoidFunc1<P>);
  public static <P, R> cn.hutool.core.exceptions.CheckedUtil$FuncRt<P, R> uncheck(cn.hutool.core.lang.func.Func<P, R>, cn.hutool.core.lang.func.Supplier1<java.lang.RuntimeException, java.lang.Exception>);
  public static <R> cn.hutool.core.exceptions.CheckedUtil$Func0Rt<R> uncheck(cn.hutool.core.lang.func.Func0<R>, cn.hutool.core.lang.func.Supplier1<java.lang.RuntimeException, java.lang.Exception>);
  public static <P, R> cn.hutool.core.exceptions.CheckedUtil$Func1Rt<P, R> uncheck(cn.hutool.core.lang.func.Func1<P, R>, cn.hutool.core.lang.func.Supplier1<java.lang.RuntimeException, java.lang.Exception>);
  public static <P> cn.hutool.core.exceptions.CheckedUtil$VoidFuncRt<P> uncheck(cn.hutool.core.lang.func.VoidFunc<P>, cn.hutool.core.lang.func.Supplier1<java.lang.RuntimeException, java.lang.Exception>);
  public static cn.hutool.core.exceptions.CheckedUtil$VoidFunc0Rt uncheck(cn.hutool.core.lang.func.VoidFunc0, java.lang.RuntimeException);
  public static cn.hutool.core.exceptions.CheckedUtil$VoidFunc0Rt uncheck(cn.hutool.core.lang.func.VoidFunc0, cn.hutool.core.lang.func.Supplier1<java.lang.RuntimeException, java.lang.Exception>);
  public static <P> cn.hutool.core.exceptions.CheckedUtil$VoidFunc1Rt<P> uncheck(cn.hutool.core.lang.func.VoidFunc1<P>, cn.hutool.core.lang.func.Supplier1<java.lang.RuntimeException, java.lang.Exception>);
}
```

## `cn.hutool.core.exceptions.CheckedUtil$Func0Rt`

```java
public interface cn.hutool.core.exceptions.CheckedUtil$Func0Rt<R> extends cn.hutool.core.lang.func.Func0<R> {
  public abstract R call() throws java.lang.RuntimeException;
}
```

## `cn.hutool.core.exceptions.CheckedUtil$Func1Rt`

```java
public interface cn.hutool.core.exceptions.CheckedUtil$Func1Rt<P, R> extends cn.hutool.core.lang.func.Func1<P, R> {
  public abstract R call(P) throws java.lang.RuntimeException;
}
```

## `cn.hutool.core.exceptions.CheckedUtil$FuncRt`

```java
public interface cn.hutool.core.exceptions.CheckedUtil$FuncRt<P, R> extends cn.hutool.core.lang.func.Func<P, R> {
  public abstract R call(P...) throws java.lang.RuntimeException;
}
```

## `cn.hutool.core.exceptions.CheckedUtil$VoidFunc0Rt`

```java
public interface cn.hutool.core.exceptions.CheckedUtil$VoidFunc0Rt extends cn.hutool.core.lang.func.VoidFunc0 {
  public abstract void call() throws java.lang.RuntimeException;
}
```

## `cn.hutool.core.exceptions.CheckedUtil$VoidFunc1Rt`

```java
public interface cn.hutool.core.exceptions.CheckedUtil$VoidFunc1Rt<P> extends cn.hutool.core.lang.func.VoidFunc1<P> {
  public abstract void call(P) throws java.lang.RuntimeException;
}
```

## `cn.hutool.core.exceptions.CheckedUtil$VoidFuncRt`

```java
public interface cn.hutool.core.exceptions.CheckedUtil$VoidFuncRt<P> extends cn.hutool.core.lang.func.VoidFunc<P> {
  public abstract void call(P...) throws java.lang.RuntimeException;
}
```

## `cn.hutool.core.exceptions.DependencyException`

```java
public class cn.hutool.core.exceptions.DependencyException extends java.lang.RuntimeException {
  public cn.hutool.core.exceptions.DependencyException(java.lang.Throwable);
  public cn.hutool.core.exceptions.DependencyException(java.lang.String);
  public cn.hutool.core.exceptions.DependencyException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.exceptions.DependencyException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.exceptions.DependencyException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.core.exceptions.DependencyException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.core.exceptions.ExceptionUtil`

```java
public class cn.hutool.core.exceptions.ExceptionUtil {
  public cn.hutool.core.exceptions.ExceptionUtil();
  public static java.lang.String getMessage(java.lang.Throwable);
  public static java.lang.String getSimpleMessage(java.lang.Throwable);
  public static java.lang.RuntimeException wrapRuntime(java.lang.Throwable);
  public static java.lang.RuntimeException wrapRuntime(java.lang.String);
  public static <T extends java.lang.Throwable> T wrap(java.lang.Throwable, java.lang.Class<T>);
  public static void wrapAndThrow(java.lang.Throwable);
  public static void wrapRuntimeAndThrow(java.lang.String);
  public static java.lang.Throwable unwrap(java.lang.Throwable);
  public static java.lang.StackTraceElement[] getStackElements();
  public static java.lang.StackTraceElement getStackElement(int);
  public static java.lang.StackTraceElement getStackElement(java.lang.String, int);
  public static java.lang.StackTraceElement getRootStackElement();
  public static java.lang.String stacktraceToOneLineString(java.lang.Throwable);
  public static java.lang.String stacktraceToOneLineString(java.lang.Throwable, int);
  public static java.lang.String stacktraceToString(java.lang.Throwable);
  public static java.lang.String stacktraceToString(java.lang.Throwable, int);
  public static java.lang.String stacktraceToString(java.lang.Throwable, int, java.util.Map<java.lang.Character, java.lang.String>);
  public static boolean isCausedBy(java.lang.Throwable, java.lang.Class<? extends java.lang.Exception>...);
  public static java.lang.Throwable getCausedBy(java.lang.Throwable, java.lang.Class<? extends java.lang.Exception>...);
  public static boolean isFromOrSuppressedThrowable(java.lang.Throwable, java.lang.Class<? extends java.lang.Throwable>);
  public static boolean isFromOrSuppressedThrowable(java.lang.Throwable, java.lang.Class<? extends java.lang.Throwable>, boolean);
  public static <T extends java.lang.Throwable> T convertFromOrSuppressedThrowable(java.lang.Throwable, java.lang.Class<T>);
  public static <T extends java.lang.Throwable> T convertFromOrSuppressedThrowable(java.lang.Throwable, java.lang.Class<T>, boolean);
  public static java.util.List<java.lang.Throwable> getThrowableList(java.lang.Throwable);
  public static java.lang.Throwable getRootCause(java.lang.Throwable);
  public static java.lang.String getRootCauseMessage(java.lang.Throwable);
}
```

## `cn.hutool.core.exceptions.InvocationTargetRuntimeException`

```java
public class cn.hutool.core.exceptions.InvocationTargetRuntimeException extends cn.hutool.core.exceptions.UtilException {
  public cn.hutool.core.exceptions.InvocationTargetRuntimeException(java.lang.Throwable);
  public cn.hutool.core.exceptions.InvocationTargetRuntimeException(java.lang.String);
  public cn.hutool.core.exceptions.InvocationTargetRuntimeException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.exceptions.InvocationTargetRuntimeException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.exceptions.InvocationTargetRuntimeException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.core.exceptions.InvocationTargetRuntimeException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.core.exceptions.NotInitedException`

```java
public class cn.hutool.core.exceptions.NotInitedException extends java.lang.RuntimeException {
  public cn.hutool.core.exceptions.NotInitedException(java.lang.Throwable);
  public cn.hutool.core.exceptions.NotInitedException(java.lang.String);
  public cn.hutool.core.exceptions.NotInitedException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.exceptions.NotInitedException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.exceptions.NotInitedException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.core.exceptions.NotInitedException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.core.exceptions.StatefulException`

```java
public class cn.hutool.core.exceptions.StatefulException extends java.lang.RuntimeException {
  public cn.hutool.core.exceptions.StatefulException();
  public cn.hutool.core.exceptions.StatefulException(java.lang.String);
  public cn.hutool.core.exceptions.StatefulException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.exceptions.StatefulException(java.lang.Throwable);
  public cn.hutool.core.exceptions.StatefulException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.exceptions.StatefulException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.core.exceptions.StatefulException(int, java.lang.String);
  public cn.hutool.core.exceptions.StatefulException(int, java.lang.Throwable);
  public cn.hutool.core.exceptions.StatefulException(int, java.lang.String, java.lang.Throwable);
  public int getStatus();
}
```

## `cn.hutool.core.exceptions.UtilException`

```java
public class cn.hutool.core.exceptions.UtilException extends java.lang.RuntimeException {
  public cn.hutool.core.exceptions.UtilException(java.lang.Throwable);
  public cn.hutool.core.exceptions.UtilException(java.lang.String);
  public cn.hutool.core.exceptions.UtilException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.exceptions.UtilException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.exceptions.UtilException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.core.exceptions.UtilException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.core.exceptions.ValidateException`

```java
public class cn.hutool.core.exceptions.ValidateException extends cn.hutool.core.exceptions.StatefulException {
  public cn.hutool.core.exceptions.ValidateException();
  public cn.hutool.core.exceptions.ValidateException(java.lang.String);
  public cn.hutool.core.exceptions.ValidateException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.exceptions.ValidateException(java.lang.Throwable);
  public cn.hutool.core.exceptions.ValidateException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.exceptions.ValidateException(int, java.lang.String);
  public cn.hutool.core.exceptions.ValidateException(int, java.lang.Throwable);
  public cn.hutool.core.exceptions.ValidateException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.core.exceptions.ValidateException(int, java.lang.String, java.lang.Throwable);
}
```
