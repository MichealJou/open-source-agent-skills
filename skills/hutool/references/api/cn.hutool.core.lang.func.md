# cn.hutool.core.lang.func

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.lang.func.Consumer3`

```java
public interface cn.hutool.core.lang.func.Consumer3<P1, P2, P3> {
  public abstract void accept(P1, P2, P3);
}
```

## `cn.hutool.core.lang.func.Func`

```java
public interface cn.hutool.core.lang.func.Func<P, R> extends java.io.Serializable {
  public abstract R call(P...) throws java.lang.Exception;
  public default R callWithRuntimeException(P...);
}
```

## `cn.hutool.core.lang.func.Func0`

```java
public interface cn.hutool.core.lang.func.Func0<R> extends java.io.Serializable {
  public abstract R call() throws java.lang.Exception;
  public default R callWithRuntimeException();
}
```

## `cn.hutool.core.lang.func.Func1`

```java
public interface cn.hutool.core.lang.func.Func1<P, R> extends java.io.Serializable {
  public abstract R call(P) throws java.lang.Exception;
  public default R callWithRuntimeException(P);
}
```

## `cn.hutool.core.lang.func.LambdaUtil`

```java
public class cn.hutool.core.lang.func.LambdaUtil {
  public cn.hutool.core.lang.func.LambdaUtil();
  public static <R> java.lang.Class<R> getRealClass(cn.hutool.core.lang.func.Func0<?>);
  public static <T> java.lang.invoke.SerializedLambda resolve(cn.hutool.core.lang.func.Func1<T, ?>);
  public static <R> java.lang.invoke.SerializedLambda resolve(cn.hutool.core.lang.func.Func0<R>);
  public static <P> java.lang.String getMethodName(cn.hutool.core.lang.func.Func1<P, ?>);
  public static <R> java.lang.String getMethodName(cn.hutool.core.lang.func.Func0<R>);
  public static <P, R> java.lang.Class<P> getRealClass(cn.hutool.core.lang.func.Func1<P, R>);
  public static <T> java.lang.String getFieldName(cn.hutool.core.lang.func.Func1<T, ?>) throws java.lang.IllegalArgumentException;
  public static <T> java.lang.String getFieldName(cn.hutool.core.lang.func.Func0<T>) throws java.lang.IllegalArgumentException;
}
```

## `cn.hutool.core.lang.func.Supplier1`

```java
public interface cn.hutool.core.lang.func.Supplier1<T, P1> {
  public abstract T get(P1);
  public default java.util.function.Supplier<T> toSupplier(P1);
}
```

## `cn.hutool.core.lang.func.Supplier2`

```java
public interface cn.hutool.core.lang.func.Supplier2<T, P1, P2> {
  public abstract T get(P1, P2);
  public default java.util.function.Supplier<T> toSupplier(P1, P2);
}
```

## `cn.hutool.core.lang.func.Supplier3`

```java
public interface cn.hutool.core.lang.func.Supplier3<T, P1, P2, P3> {
  public abstract T get(P1, P2, P3);
  public default java.util.function.Supplier<T> toSupplier(P1, P2, P3);
}
```

## `cn.hutool.core.lang.func.Supplier4`

```java
public interface cn.hutool.core.lang.func.Supplier4<T, P1, P2, P3, P4> {
  public abstract T get(P1, P2, P3, P4);
  public default java.util.function.Supplier<T> toSupplier(P1, P2, P3, P4);
}
```

## `cn.hutool.core.lang.func.Supplier5`

```java
public interface cn.hutool.core.lang.func.Supplier5<T, P1, P2, P3, P4, P5> {
  public abstract T get(P1, P2, P3, P4, P5);
  public default java.util.function.Supplier<T> toSupplier(P1, P2, P3, P4, P5);
}
```

## `cn.hutool.core.lang.func.VoidFunc`

```java
public interface cn.hutool.core.lang.func.VoidFunc<P> extends java.io.Serializable {
  public abstract void call(P...) throws java.lang.Exception;
  public default void callWithRuntimeException(P...);
}
```

## `cn.hutool.core.lang.func.VoidFunc0`

```java
public interface cn.hutool.core.lang.func.VoidFunc0 extends java.io.Serializable {
  public abstract void call() throws java.lang.Exception;
  public default void callWithRuntimeException();
}
```

## `cn.hutool.core.lang.func.VoidFunc1`

```java
public interface cn.hutool.core.lang.func.VoidFunc1<P> extends java.io.Serializable {
  public abstract void call(P) throws java.lang.Exception;
  public default void callWithRuntimeException(P);
}
```
