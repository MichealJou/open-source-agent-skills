# com.feilong.formatter

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.formatter.FormatterColumn`

```java
public interface com.feilong.formatter.FormatterColumn extends java.lang.annotation.Annotation {
  public abstract java.lang.String name();
  public abstract int order();
}
```

## `com.feilong.formatter.FormatterUtil`

```java
public final class com.feilong.formatter.FormatterUtil {
  public static final <T> java.lang.String formatToSimpleTable(java.lang.Iterable<T>);
  public static final <T> java.lang.String formatToSimpleTable(java.lang.Iterable<T>, com.feilong.formatter.entity.BeanFormatterConfig);
  public static final <T> java.lang.String formatToSimpleTable(java.lang.Iterable<T>, java.lang.String...);
  public static final <K, V> java.lang.String formatToSimpleTable(java.util.Map<K, V>);
  public static final <T> java.lang.String formatToSimpleTable(T);
}
```

## `com.feilong.formatter.SimpleTableFormatter`

```java
public class com.feilong.formatter.SimpleTableFormatter extends com.feilong.formatter.AbstractFormatter {
  public com.feilong.formatter.SimpleTableFormatter();
  public java.lang.String format(java.lang.String[], java.util.List<java.lang.Object[]>);
  public java.lang.String format(java.lang.Iterable, com.feilong.formatter.entity.BeanFormatterConfig);
  public java.lang.String format(java.lang.Iterable);
  public java.lang.String format(java.util.Map);
  public java.lang.String format(java.lang.Object);
}
```
