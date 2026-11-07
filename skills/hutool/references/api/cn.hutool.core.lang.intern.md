# cn.hutool.core.lang.intern

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.lang.intern.InternUtil`

```java
public class cn.hutool.core.lang.intern.InternUtil {
  public cn.hutool.core.lang.intern.InternUtil();
  public static <T> cn.hutool.core.lang.intern.Interner<T> createWeakInterner();
  public static cn.hutool.core.lang.intern.Interner<java.lang.String> createJdkInterner();
  public static cn.hutool.core.lang.intern.Interner<java.lang.String> createStringInterner(boolean);
}
```

## `cn.hutool.core.lang.intern.Interner`

```java
public interface cn.hutool.core.lang.intern.Interner<T> {
  public abstract T intern(T);
}
```

## `cn.hutool.core.lang.intern.JdkStringInterner`

```java
public class cn.hutool.core.lang.intern.JdkStringInterner implements cn.hutool.core.lang.intern.Interner<java.lang.String> {
  public cn.hutool.core.lang.intern.JdkStringInterner();
  public java.lang.String intern(java.lang.String);
  public java.lang.Object intern(java.lang.Object);
}
```

## `cn.hutool.core.lang.intern.WeakInterner`

```java
public class cn.hutool.core.lang.intern.WeakInterner<T> implements cn.hutool.core.lang.intern.Interner<T> {
  public cn.hutool.core.lang.intern.WeakInterner();
  public T intern(T);
}
```
