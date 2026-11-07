# cn.hutool.core.lang.loader

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.lang.loader.AtomicLoader`

```java
public abstract class cn.hutool.core.lang.loader.AtomicLoader<T> implements cn.hutool.core.lang.loader.Loader<T>, java.io.Serializable {
  public cn.hutool.core.lang.loader.AtomicLoader();
  public T get();
}
```

## `cn.hutool.core.lang.loader.LazyFunLoader`

```java
public class cn.hutool.core.lang.loader.LazyFunLoader<T> extends cn.hutool.core.lang.loader.LazyLoader<T> {
  public static <T> cn.hutool.core.lang.loader.LazyFunLoader<T> on(java.util.function.Supplier<T>);
  public cn.hutool.core.lang.loader.LazyFunLoader(java.util.function.Supplier<T>);
  public boolean isInitialize();
  public void ifInitialized(java.util.function.Consumer<T>);
}
```

## `cn.hutool.core.lang.loader.LazyLoader`

```java
public abstract class cn.hutool.core.lang.loader.LazyLoader<T> implements cn.hutool.core.lang.loader.Loader<T>, java.io.Serializable {
  public cn.hutool.core.lang.loader.LazyLoader();
  public T get();
}
```

## `cn.hutool.core.lang.loader.Loader`

```java
public interface cn.hutool.core.lang.loader.Loader<T> {
  public abstract T get();
}
```
