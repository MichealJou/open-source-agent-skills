# com.feilong.formatter.builder

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.formatter.builder.AbstractFormatterBuilder`

```java
public abstract class com.feilong.formatter.builder.AbstractFormatterBuilder implements com.feilong.formatter.builder.FormatterBuilder {
  public com.feilong.formatter.builder.AbstractFormatterBuilder();
  public <T> java.util.List<com.feilong.formatter.entity.FormatterColumnEntity> build(T, com.feilong.formatter.entity.BeanFormatterConfig);
}
```

## `com.feilong.formatter.builder.BeanTypeFormatterBuilder`

```java
public class com.feilong.formatter.builder.BeanTypeFormatterBuilder extends com.feilong.formatter.builder.AbstractFormatterBuilder {
  public com.feilong.formatter.builder.BeanTypeFormatterBuilder();
  public <T> java.lang.Object[] buildLineData(T, java.util.List<java.lang.String>, com.feilong.formatter.entity.BeanFormatterConfig);
}
```

## `com.feilong.formatter.builder.ColumnMaxWidthsBuilder`

```java
public final class com.feilong.formatter.builder.ColumnMaxWidthsBuilder {
  public static int[] build(java.util.List<java.lang.Object[]>);
}
```

## `com.feilong.formatter.builder.FormatterBuilder`

```java
public interface com.feilong.formatter.builder.FormatterBuilder {
  public abstract <T> java.util.List<com.feilong.formatter.entity.FormatterColumnEntity> build(T, com.feilong.formatter.entity.BeanFormatterConfig);
  public abstract <T> java.lang.Object[] buildLineData(T, java.util.List<java.lang.String>, com.feilong.formatter.entity.BeanFormatterConfig);
}
```

## `com.feilong.formatter.builder.FormatterBuilderFactory`

```java
public final class com.feilong.formatter.builder.FormatterBuilderFactory {
  public static <T> com.feilong.formatter.builder.FormatterBuilder create(T);
}
```

## `com.feilong.formatter.builder.MapTypeFormatterBuilder`

```java
public class com.feilong.formatter.builder.MapTypeFormatterBuilder extends com.feilong.formatter.builder.AbstractFormatterBuilder {
  public com.feilong.formatter.builder.MapTypeFormatterBuilder();
  public <T> java.lang.Object[] buildLineData(T, java.util.List<java.lang.String>, com.feilong.formatter.entity.BeanFormatterConfig);
}
```

## `com.feilong.formatter.builder.ValueHandler`

```java
public final class com.feilong.formatter.builder.ValueHandler {
  public static java.lang.String getValue(java.lang.String, java.lang.Object, com.feilong.formatter.entity.BeanFormatterConfig);
}
```
