# cn.hutool.core.lang.ansi

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.lang.ansi.Ansi8BitColor`

```java
public final class cn.hutool.core.lang.ansi.Ansi8BitColor implements cn.hutool.core.lang.ansi.AnsiElement {
  public static cn.hutool.core.lang.ansi.Ansi8BitColor foreground(int);
  public static cn.hutool.core.lang.ansi.Ansi8BitColor background(int);
  public int getCode();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `cn.hutool.core.lang.ansi.AnsiBackground`

```java
public final class cn.hutool.core.lang.ansi.AnsiBackground extends java.lang.Enum<cn.hutool.core.lang.ansi.AnsiBackground> implements cn.hutool.core.lang.ansi.AnsiElement {
  public static cn.hutool.core.lang.ansi.AnsiBackground[] values();
  public static cn.hutool.core.lang.ansi.AnsiBackground valueOf(java.lang.String);
  public int getCode();
  public java.lang.String toString();
}
```

## `cn.hutool.core.lang.ansi.AnsiColor`

```java
public final class cn.hutool.core.lang.ansi.AnsiColor extends java.lang.Enum<cn.hutool.core.lang.ansi.AnsiColor> implements cn.hutool.core.lang.ansi.AnsiElement {
  public static cn.hutool.core.lang.ansi.AnsiColor[] values();
  public static cn.hutool.core.lang.ansi.AnsiColor valueOf(java.lang.String);
  public int getCode();
  public java.lang.String toString();
}
```

## `cn.hutool.core.lang.ansi.AnsiColorWrapper`

```java
public class cn.hutool.core.lang.ansi.AnsiColorWrapper {
  public cn.hutool.core.lang.ansi.AnsiColorWrapper(int, cn.hutool.core.lang.ansi.AnsiColors$BitDepth);
  public cn.hutool.core.lang.ansi.AnsiElement toAnsiElement(cn.hutool.core.lang.ansi.ForeOrBack);
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `cn.hutool.core.lang.ansi.AnsiColors`

```java
public final class cn.hutool.core.lang.ansi.AnsiColors {
  public cn.hutool.core.lang.ansi.AnsiColors(cn.hutool.core.lang.ansi.AnsiColors$BitDepth);
  public cn.hutool.core.lang.ansi.AnsiColorWrapper findClosest(java.awt.Color);
}
```

## `cn.hutool.core.lang.ansi.AnsiColors$BitDepth`

```java
public final class cn.hutool.core.lang.ansi.AnsiColors$BitDepth extends java.lang.Enum<cn.hutool.core.lang.ansi.AnsiColors$BitDepth> {
  public static cn.hutool.core.lang.ansi.AnsiColors$BitDepth[] values();
  public static cn.hutool.core.lang.ansi.AnsiColors$BitDepth valueOf(java.lang.String);
  public static cn.hutool.core.lang.ansi.AnsiColors$BitDepth of(int);
}
```

## `cn.hutool.core.lang.ansi.AnsiElement`

```java
public interface cn.hutool.core.lang.ansi.AnsiElement {
  public abstract java.lang.String toString();
  public default int getCode();
}
```

## `cn.hutool.core.lang.ansi.AnsiEncoder`

```java
public abstract class cn.hutool.core.lang.ansi.AnsiEncoder {
  public cn.hutool.core.lang.ansi.AnsiEncoder();
  public static java.lang.String encode(java.lang.Object...);
}
```

## `cn.hutool.core.lang.ansi.AnsiStyle`

```java
public final class cn.hutool.core.lang.ansi.AnsiStyle extends java.lang.Enum<cn.hutool.core.lang.ansi.AnsiStyle> implements cn.hutool.core.lang.ansi.AnsiElement {
  public static cn.hutool.core.lang.ansi.AnsiStyle[] values();
  public static cn.hutool.core.lang.ansi.AnsiStyle valueOf(java.lang.String);
  public int getCode();
  public java.lang.String toString();
}
```

## `cn.hutool.core.lang.ansi.ForeOrBack`

```java
public final class cn.hutool.core.lang.ansi.ForeOrBack extends java.lang.Enum<cn.hutool.core.lang.ansi.ForeOrBack> {
  public static cn.hutool.core.lang.ansi.ForeOrBack[] values();
  public static cn.hutool.core.lang.ansi.ForeOrBack valueOf(java.lang.String);
}
```
