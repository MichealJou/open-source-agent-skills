# com.feilong.lib.lang3.time

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.lang3.time.DateFormatUtils`

```java
public class com.feilong.lib.lang3.time.DateFormatUtils {
  public com.feilong.lib.lang3.time.DateFormatUtils();
  public static java.lang.String formatUTC(long, java.lang.String);
  public static java.lang.String formatUTC(java.util.Date, java.lang.String);
  public static java.lang.String formatUTC(long, java.lang.String, java.util.Locale);
  public static java.lang.String formatUTC(java.util.Date, java.lang.String, java.util.Locale);
  public static java.lang.String format(long, java.lang.String);
  public static java.lang.String format(java.util.Date, java.lang.String);
  public static java.lang.String format(java.util.Calendar, java.lang.String);
  public static java.lang.String format(long, java.lang.String, java.util.TimeZone);
  public static java.lang.String format(java.util.Date, java.lang.String, java.util.TimeZone);
  public static java.lang.String format(java.util.Calendar, java.lang.String, java.util.TimeZone);
  public static java.lang.String format(long, java.lang.String, java.util.Locale);
  public static java.lang.String format(java.util.Date, java.lang.String, java.util.Locale);
  public static java.lang.String format(java.util.Calendar, java.lang.String, java.util.Locale);
  public static java.lang.String format(long, java.lang.String, java.util.TimeZone, java.util.Locale);
  public static java.lang.String format(java.util.Date, java.lang.String, java.util.TimeZone, java.util.Locale);
  public static java.lang.String format(java.util.Calendar, java.lang.String, java.util.TimeZone, java.util.Locale);
}
```

## `com.feilong.lib.lang3.time.DateParser`

```java
public interface com.feilong.lib.lang3.time.DateParser {
  public abstract java.util.Date parse(java.lang.String) throws java.text.ParseException;
  public abstract java.util.Date parse(java.lang.String, java.text.ParsePosition);
  public abstract boolean parse(java.lang.String, java.text.ParsePosition, java.util.Calendar);
  public abstract java.lang.String getPattern();
  public abstract java.util.TimeZone getTimeZone();
  public abstract java.util.Locale getLocale();
  public abstract java.lang.Object parseObject(java.lang.String) throws java.text.ParseException;
  public abstract java.lang.Object parseObject(java.lang.String, java.text.ParsePosition);
}
```

## `com.feilong.lib.lang3.time.DatePrinter`

```java
public interface com.feilong.lib.lang3.time.DatePrinter {
  public abstract java.lang.String format(long);
  public abstract java.lang.String format(java.util.Date);
  public abstract java.lang.String format(java.util.Calendar);
  public abstract java.lang.StringBuffer format(long, java.lang.StringBuffer);
  public abstract java.lang.StringBuffer format(java.util.Date, java.lang.StringBuffer);
  public abstract java.lang.StringBuffer format(java.util.Calendar, java.lang.StringBuffer);
  public abstract <B extends java.lang.Appendable> B format(long, B);
  public abstract <B extends java.lang.Appendable> B format(java.util.Date, B);
  public abstract <B extends java.lang.Appendable> B format(java.util.Calendar, B);
  public abstract java.lang.String getPattern();
  public abstract java.util.TimeZone getTimeZone();
  public abstract java.util.Locale getLocale();
  public abstract java.lang.StringBuffer format(java.lang.Object, java.lang.StringBuffer, java.text.FieldPosition);
}
```

## `com.feilong.lib.lang3.time.DateUtils`

```java
public class com.feilong.lib.lang3.time.DateUtils {
  public com.feilong.lib.lang3.time.DateUtils();
  public static boolean isSameDay(java.util.Date, java.util.Date);
  public static boolean isSameDay(java.util.Calendar, java.util.Calendar);
  public static boolean isSameInstant(java.util.Date, java.util.Date);
  public static boolean isSameInstant(java.util.Calendar, java.util.Calendar);
  public static boolean isSameLocalTime(java.util.Calendar, java.util.Calendar);
  public static java.util.Date parseDate(java.lang.String, java.lang.String...) throws java.text.ParseException;
  public static java.util.Date parseDate(java.lang.String, java.util.Locale, java.lang.String...) throws java.text.ParseException;
  public static java.util.Date parseDateStrictly(java.lang.String, java.lang.String...) throws java.text.ParseException;
  public static java.util.Date parseDateStrictly(java.lang.String, java.util.Locale, java.lang.String...) throws java.text.ParseException;
  public static java.util.Date addYears(java.util.Date, int);
  public static java.util.Date addMonths(java.util.Date, int);
  public static java.util.Date addWeeks(java.util.Date, int);
  public static java.util.Date addDays(java.util.Date, int);
  public static java.util.Date addHours(java.util.Date, int);
  public static java.util.Date addMinutes(java.util.Date, int);
  public static java.util.Date addSeconds(java.util.Date, int);
  public static java.util.Date addMilliseconds(java.util.Date, int);
  public static java.util.Date setYears(java.util.Date, int);
  public static java.util.Date setMonths(java.util.Date, int);
  public static java.util.Date setDays(java.util.Date, int);
  public static java.util.Date setHours(java.util.Date, int);
  public static java.util.Date setMinutes(java.util.Date, int);
  public static java.util.Date setSeconds(java.util.Date, int);
  public static java.util.Date setMilliseconds(java.util.Date, int);
  public static java.util.Calendar toCalendar(java.util.Date);
  public static java.util.Calendar toCalendar(java.util.Date, java.util.TimeZone);
  public static java.util.Date round(java.util.Date, int);
  public static java.util.Calendar round(java.util.Calendar, int);
  public static java.util.Date round(java.lang.Object, int);
  public static java.util.Date truncate(java.util.Date, int);
  public static java.util.Calendar truncate(java.util.Calendar, int);
  public static java.util.Date truncate(java.lang.Object, int);
  public static java.util.Date ceiling(java.util.Date, int);
  public static java.util.Calendar ceiling(java.util.Calendar, int);
  public static java.util.Date ceiling(java.lang.Object, int);
  public static java.util.Iterator<java.util.Calendar> iterator(java.util.Date, int);
  public static java.util.Iterator<java.util.Calendar> iterator(java.util.Calendar, int);
  public static java.util.Iterator<?> iterator(java.lang.Object, int);
  public static long getFragmentInMilliseconds(java.util.Date, int);
  public static long getFragmentInSeconds(java.util.Date, int);
  public static long getFragmentInMinutes(java.util.Date, int);
  public static long getFragmentInHours(java.util.Date, int);
  public static long getFragmentInDays(java.util.Date, int);
  public static long getFragmentInMilliseconds(java.util.Calendar, int);
  public static long getFragmentInSeconds(java.util.Calendar, int);
  public static long getFragmentInMinutes(java.util.Calendar, int);
  public static long getFragmentInHours(java.util.Calendar, int);
  public static long getFragmentInDays(java.util.Calendar, int);
  public static boolean truncatedEquals(java.util.Calendar, java.util.Calendar, int);
  public static boolean truncatedEquals(java.util.Date, java.util.Date, int);
  public static int truncatedCompareTo(java.util.Calendar, java.util.Calendar, int);
  public static int truncatedCompareTo(java.util.Date, java.util.Date, int);
}
```

## `com.feilong.lib.lang3.time.DurationFormatUtils`

```java
public class com.feilong.lib.lang3.time.DurationFormatUtils {
  public com.feilong.lib.lang3.time.DurationFormatUtils();
  public static java.lang.String formatDurationHMS(long);
  public static java.lang.String formatDurationISO(long);
  public static java.lang.String formatDuration(long, java.lang.String);
  public static java.lang.String formatDuration(long, java.lang.String, boolean);
  public static java.lang.String formatPeriodISO(long, long);
  public static java.lang.String formatPeriod(long, long, java.lang.String);
  public static java.lang.String formatPeriod(long, long, java.lang.String, boolean, java.util.TimeZone);
}
```

## `com.feilong.lib.lang3.time.FastDateFormat`

```java
public class com.feilong.lib.lang3.time.FastDateFormat extends java.text.Format implements com.feilong.lib.lang3.time.DateParser,com.feilong.lib.lang3.time.DatePrinter {
  public static com.feilong.lib.lang3.time.FastDateFormat getInstance();
  public static com.feilong.lib.lang3.time.FastDateFormat getInstance(java.lang.String);
  public static com.feilong.lib.lang3.time.FastDateFormat getInstance(java.lang.String, java.util.TimeZone);
  public static com.feilong.lib.lang3.time.FastDateFormat getInstance(java.lang.String, java.util.Locale);
  public static com.feilong.lib.lang3.time.FastDateFormat getInstance(java.lang.String, java.util.TimeZone, java.util.Locale);
  public static com.feilong.lib.lang3.time.FastDateFormat getDateInstance(int);
  public static com.feilong.lib.lang3.time.FastDateFormat getDateInstance(int, java.util.Locale);
  public static com.feilong.lib.lang3.time.FastDateFormat getDateInstance(int, java.util.TimeZone);
  public static com.feilong.lib.lang3.time.FastDateFormat getDateInstance(int, java.util.TimeZone, java.util.Locale);
  public static com.feilong.lib.lang3.time.FastDateFormat getTimeInstance(int);
  public static com.feilong.lib.lang3.time.FastDateFormat getTimeInstance(int, java.util.Locale);
  public static com.feilong.lib.lang3.time.FastDateFormat getTimeInstance(int, java.util.TimeZone);
  public static com.feilong.lib.lang3.time.FastDateFormat getTimeInstance(int, java.util.TimeZone, java.util.Locale);
  public static com.feilong.lib.lang3.time.FastDateFormat getDateTimeInstance(int, int);
  public static com.feilong.lib.lang3.time.FastDateFormat getDateTimeInstance(int, int, java.util.Locale);
  public static com.feilong.lib.lang3.time.FastDateFormat getDateTimeInstance(int, int, java.util.TimeZone);
  public static com.feilong.lib.lang3.time.FastDateFormat getDateTimeInstance(int, int, java.util.TimeZone, java.util.Locale);
  public java.lang.StringBuffer format(java.lang.Object, java.lang.StringBuffer, java.text.FieldPosition);
  public java.lang.String format(long);
  public java.lang.String format(java.util.Date);
  public java.lang.String format(java.util.Calendar);
  public java.lang.StringBuffer format(long, java.lang.StringBuffer);
  public java.lang.StringBuffer format(java.util.Date, java.lang.StringBuffer);
  public java.lang.StringBuffer format(java.util.Calendar, java.lang.StringBuffer);
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
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.feilong.lib.lang3.time.FastDateParser`

```java
public class com.feilong.lib.lang3.time.FastDateParser implements com.feilong.lib.lang3.time.DateParser,java.io.Serializable {
  public java.lang.String getPattern();
  public java.util.TimeZone getTimeZone();
  public java.util.Locale getLocale();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public java.lang.Object parseObject(java.lang.String) throws java.text.ParseException;
  public java.util.Date parse(java.lang.String) throws java.text.ParseException;
  public java.lang.Object parseObject(java.lang.String, java.text.ParsePosition);
  public java.util.Date parse(java.lang.String, java.text.ParsePosition);
  public boolean parse(java.lang.String, java.text.ParsePosition, java.util.Calendar);
}
```

## `com.feilong.lib.lang3.time.FastDatePrinter`

```java
public class com.feilong.lib.lang3.time.FastDatePrinter implements com.feilong.lib.lang3.time.DatePrinter,java.io.Serializable {
  public java.lang.StringBuffer format(java.lang.Object, java.lang.StringBuffer, java.text.FieldPosition);
  public java.lang.String format(long);
  public java.lang.String format(java.util.Date);
  public java.lang.String format(java.util.Calendar);
  public java.lang.StringBuffer format(long, java.lang.StringBuffer);
  public java.lang.StringBuffer format(java.util.Date, java.lang.StringBuffer);
  public java.lang.StringBuffer format(java.util.Calendar, java.lang.StringBuffer);
  public <B extends java.lang.Appendable> B format(long, B);
  public <B extends java.lang.Appendable> B format(java.util.Date, B);
  public <B extends java.lang.Appendable> B format(java.util.Calendar, B);
  public java.lang.String getPattern();
  public java.util.TimeZone getTimeZone();
  public java.util.Locale getLocale();
  public int getMaxLengthEstimate();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.feilong.lib.lang3.time.FastTimeZone`

```java
public class com.feilong.lib.lang3.time.FastTimeZone {
  public static java.util.TimeZone getGmtTimeZone();
  public static java.util.TimeZone getGmtTimeZone(java.lang.String);
  public static java.util.TimeZone getTimeZone(java.lang.String);
}
```

## `com.feilong.lib.lang3.time.StopWatch`

```java
public class com.feilong.lib.lang3.time.StopWatch {
  public static com.feilong.lib.lang3.time.StopWatch create();
  public static com.feilong.lib.lang3.time.StopWatch createStarted();
  public com.feilong.lib.lang3.time.StopWatch();
  public com.feilong.lib.lang3.time.StopWatch(java.lang.String);
  public java.lang.String formatSplitTime();
  public java.lang.String formatTime();
  public java.lang.String getMessage();
  public long getNanoTime();
  public long getSplitNanoTime();
  public long getSplitTime();
  public long getStartTime();
  public long getTime();
  public long getTime(java.util.concurrent.TimeUnit);
  public boolean isStarted();
  public boolean isStopped();
  public boolean isSuspended();
  public void reset();
  public void resume();
  public void split();
  public void start();
  public void stop();
  public void suspend();
  public java.lang.String toSplitString();
  public java.lang.String toString();
  public void unsplit();
}
```
