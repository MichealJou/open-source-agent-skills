# com.feilong.core

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.core.DefaultRuntimeException`

```java
public class com.feilong.core.DefaultRuntimeException extends java.lang.RuntimeException {
  public com.feilong.core.DefaultRuntimeException(java.lang.String);
  public com.feilong.core.DefaultRuntimeException(java.lang.String, java.lang.Object...);
  public com.feilong.core.DefaultRuntimeException(java.lang.String, java.lang.Throwable);
  public com.feilong.core.DefaultRuntimeException(java.lang.Throwable);
}
```

## `com.feilong.core.Validate`

```java
public final class com.feilong.core.Validate {
  public static void isTrue(boolean, java.lang.String, java.lang.Object...);
  public static <T> T notNull(T, java.lang.String, java.lang.Object...);
  public static <T> T[] notEmpty(T[], java.lang.String, java.lang.Object...);
  public static <T extends java.util.Collection<?>> T notEmpty(T, java.lang.String, java.lang.Object...);
  public static <T extends java.util.Map<?, ?>> T notEmpty(T, java.lang.String, java.lang.Object...);
  public static <T extends java.lang.CharSequence> T notEmpty(T, java.lang.String, java.lang.Object...);
  public static <T extends java.lang.CharSequence> T notBlank(T, java.lang.String, java.lang.Object...);
  public static <T> T[] noNullElements(T[], java.lang.String, java.lang.Object...);
  public static <T extends java.lang.Iterable<?>> T noNullElements(T, java.lang.String, java.lang.Object...);
  public static void validState(boolean, java.lang.String, java.lang.Object...);
}
```

## `com.feilong.core.Validator`

```java
public final class com.feilong.core.Validator {
  public static boolean isAnyNullOrEmpty(java.lang.Object...);
  public static boolean isAllNullOrEmpty(java.lang.Object...);
  public static boolean isNullOrEmpty(java.lang.Object);
  public static boolean isNotNullOrEmpty(java.lang.Object);
  public static boolean isNullOrZero(java.lang.Number);
  public static boolean isNotNullOrZero(java.lang.Number);
}
```
