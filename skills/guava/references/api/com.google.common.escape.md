# com.google.common.escape

版本：33.4.8-jre。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.google.common.escape.ArrayBasedCharEscaper`

```java
public abstract class com.google.common.escape.ArrayBasedCharEscaper extends com.google.common.escape.CharEscaper {
  public final java.lang.String escape(java.lang.String);
}
```

## `com.google.common.escape.ArrayBasedEscaperMap`

```java
public final class com.google.common.escape.ArrayBasedEscaperMap {
  public static com.google.common.escape.ArrayBasedEscaperMap create(java.util.Map<java.lang.Character, java.lang.String>);
}
```

## `com.google.common.escape.ArrayBasedUnicodeEscaper`

```java
public abstract class com.google.common.escape.ArrayBasedUnicodeEscaper extends com.google.common.escape.UnicodeEscaper {
  public final java.lang.String escape(java.lang.String);
}
```

## `com.google.common.escape.CharEscaper`

```java
public abstract class com.google.common.escape.CharEscaper extends com.google.common.escape.Escaper {
  public java.lang.String escape(java.lang.String);
}
```

## `com.google.common.escape.CharEscaperBuilder`

```java
public final class com.google.common.escape.CharEscaperBuilder {
  public com.google.common.escape.CharEscaperBuilder();
  public com.google.common.escape.CharEscaperBuilder addEscape(char, java.lang.String);
  public com.google.common.escape.CharEscaperBuilder addEscapes(char[], java.lang.String);
  public char[][] toArray();
  public com.google.common.escape.Escaper toEscaper();
}
```

## `com.google.common.escape.Escaper`

```java
public abstract class com.google.common.escape.Escaper {
  public abstract java.lang.String escape(java.lang.String);
  public final com.google.common.base.Function<java.lang.String, java.lang.String> asFunction();
}
```

## `com.google.common.escape.Escapers`

```java
public final class com.google.common.escape.Escapers {
  public static com.google.common.escape.Escaper nullEscaper();
  public static com.google.common.escape.Escapers$Builder builder();
  public static java.lang.String computeReplacement(com.google.common.escape.CharEscaper, char);
  public static java.lang.String computeReplacement(com.google.common.escape.UnicodeEscaper, int);
}
```

## `com.google.common.escape.Escapers$Builder`

```java
public final class com.google.common.escape.Escapers$Builder {
  public com.google.common.escape.Escapers$Builder setSafeRange(char, char);
  public com.google.common.escape.Escapers$Builder setUnsafeReplacement(java.lang.String);
  public com.google.common.escape.Escapers$Builder addEscape(char, java.lang.String);
  public com.google.common.escape.Escaper build();
}
```

## `com.google.common.escape.UnicodeEscaper`

```java
public abstract class com.google.common.escape.UnicodeEscaper extends com.google.common.escape.Escaper {
  public java.lang.String escape(java.lang.String);
}
```
