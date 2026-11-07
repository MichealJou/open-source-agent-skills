# cn.hutool.core.date.format

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.date.format.AbstractDateBasic`

```java
public abstract class cn.hutool.core.date.format.AbstractDateBasic implements cn.hutool.core.date.format.DateBasic,java.io.Serializable {
  public java.lang.String getPattern();
  public java.util.TimeZone getTimeZone();
  public java.util.Locale getLocale();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `cn.hutool.core.date.format.DateBasic`

```java
public interface cn.hutool.core.date.format.DateBasic {
  public abstract java.lang.String getPattern();
  public abstract java.util.TimeZone getTimeZone();
  public abstract java.util.Locale getLocale();
}
```

## `cn.hutool.core.date.format.DateParser`

```java
public interface cn.hutool.core.date.format.DateParser extends cn.hutool.core.date.format.DateBasic {
  public abstract java.util.Date parse(java.lang.String) throws java.text.ParseException;
  public abstract java.util.Date parse(java.lang.String, java.text.ParsePosition);
  public abstract boolean parse(java.lang.String, java.text.ParsePosition, java.util.Calendar);
  public default java.lang.Object parseObject(java.lang.String) throws java.text.ParseException;
  public default java.lang.Object parseObject(java.lang.String, java.text.ParsePosition);
}
```

## `cn.hutool.core.date.format.DatePrinter`

```java
public interface cn.hutool.core.date.format.DatePrinter extends cn.hutool.core.date.format.DateBasic {
  public abstract java.lang.String format(long);
  public abstract java.lang.String format(java.util.Date);
  public abstract java.lang.String format(java.util.Calendar);
  public abstract <B extends java.lang.Appendable> B format(long, B);
  public abstract <B extends java.lang.Appendable> B format(java.util.Date, B);
  public abstract <B extends java.lang.Appendable> B format(java.util.Calendar, B);
}
```

## `cn.hutool.core.date.format.FastDateFormat`

```java
public class cn.hutool.core.date.format.FastDateFormat extends java.text.Format implements cn.hutool.core.date.format.DateParser,cn.hutool.core.date.format.DatePrinter {
  public static cn.hutool.core.date.format.FastDateFormat getInstance();
  public static cn.hutool.core.date.format.FastDateFormat getInstance(java.lang.String);
  public static cn.hutool.core.date.format.FastDateFormat getInstance(java.lang.String, java.util.TimeZone);
  public static cn.hutool.core.date.format.FastDateFormat getInstance(java.lang.String, java.util.Locale);
  public static cn.hutool.core.date.format.FastDateFormat getInstance(java.lang.String, java.util.TimeZone, java.util.Locale);
  public static cn.hutool.core.date.format.FastDateFormat getDateInstance(int);
  public static cn.hutool.core.date.format.FastDateFormat getDateInstance(int, java.util.Locale);
  public static cn.hutool.core.date.format.FastDateFormat getDateInstance(int, java.util.TimeZone);
  public static cn.hutool.core.date.format.FastDateFormat getDateInstance(int, java.util.TimeZone, java.util.Locale);
  public static cn.hutool.core.date.format.FastDateFormat getTimeInstance(int);
  public static cn.hutool.core.date.format.FastDateFormat getTimeInstance(int, java.util.Locale);
  public static cn.hutool.core.date.format.FastDateFormat getTimeInstance(int, java.util.TimeZone);
  public static cn.hutool.core.date.format.FastDateFormat getTimeInstance(int, java.util.TimeZone, java.util.Locale);
  public static cn.hutool.core.date.format.FastDateFormat getDateTimeInstance(int, int);
  public static cn.hutool.core.date.format.FastDateFormat getDateTimeInstance(int, int, java.util.Locale);
  public static cn.hutool.core.date.format.FastDateFormat getDateTimeInstance(int, int, java.util.TimeZone);
  public static cn.hutool.core.date.format.FastDateFormat getDateTimeInstance(int, int, java.util.TimeZone, java.util.Locale);
  public java.lang.StringBuffer format(java.lang.Object, java.lang.StringBuffer, java.text.FieldPosition);
  public java.lang.String format(long);
  public java.lang.String format(java.util.Date);
  public java.lang.String format(java.util.Calendar);
  public <B extends java.lang.Appendable> B format(long, B);
  public <B extends java.lang.Appendable> B format(java.util.Date, B);
  public <B extends java.lang.Appendable> B format(java.util.Calendar, B);
  public java.util.Date parse(java.lang.String) throws java.text.ParseException;
  public java.util.Date parse(java.lang.String, java.text.ParsePosition);
  public boolean parse(java.lang.String, java.text.ParsePosition, java.util.Calendar);
  public java.lang.Object parseObject(java.lang.String, java.text.ParsePosition);
  public java.lang.String getPattern();
  public java.util.TimeZone getTimeZone();
  public java.util.Locale getLocale();
  public int getMaxLengthEstimate();
  public java.time.format.DateTimeFormatter getDateTimeFormatter();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `cn.hutool.core.date.format.FastDateParser`

```java
public class cn.hutool.core.date.format.FastDateParser extends cn.hutool.core.date.format.AbstractDateBasic implements cn.hutool.core.date.format.DateParser {
  public cn.hutool.core.date.format.FastDateParser(java.lang.String, java.util.TimeZone, java.util.Locale);
  public cn.hutool.core.date.format.FastDateParser(java.lang.String, java.util.TimeZone, java.util.Locale, java.util.Date);
  public java.util.Date parse(java.lang.String) throws java.text.ParseException;
  public java.util.Date parse(java.lang.String, java.text.ParsePosition);
  public boolean parse(java.lang.String, java.text.ParsePosition, java.util.Calendar);
}
```

## `cn.hutool.core.date.format.FastDatePrinter`

```java
public class cn.hutool.core.date.format.FastDatePrinter extends cn.hutool.core.date.format.AbstractDateBasic implements cn.hutool.core.date.format.DatePrinter {
  public cn.hutool.core.date.format.FastDatePrinter(java.lang.String, java.util.TimeZone, java.util.Locale);
  public java.lang.String format(long);
  public java.lang.String format(java.util.Date);
  public java.lang.String format(java.util.Calendar);
  public <B extends java.lang.Appendable> B format(long, B);
  public <B extends java.lang.Appendable> B format(java.util.Date, B);
  public <B extends java.lang.Appendable> B format(java.util.Calendar, B);
  public int getMaxLengthEstimate();
}
```

## `cn.hutool.core.date.format.GlobalCustomFormat`

```java
public class cn.hutool.core.date.format.GlobalCustomFormat {
  public cn.hutool.core.date.format.GlobalCustomFormat();
  public static void putFormatter(java.lang.String, java.util.function.Function<java.util.Date, java.lang.String>);
  public static void putParser(java.lang.String, java.util.function.Function<java.lang.CharSequence, java.util.Date>);
  public static boolean isCustomFormat(java.lang.String);
  public static java.lang.String format(java.util.Date, java.lang.CharSequence);
  public static java.lang.String format(java.time.temporal.TemporalAccessor, java.lang.CharSequence);
  public static java.util.Date parse(java.lang.CharSequence, java.lang.String);
}
```
