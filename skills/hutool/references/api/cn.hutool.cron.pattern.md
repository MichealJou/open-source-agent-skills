# cn.hutool.cron.pattern

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.cron.pattern.CronPattern`

```java
public class cn.hutool.cron.pattern.CronPattern {
  public static cn.hutool.cron.pattern.CronPattern of(java.lang.String);
  public cn.hutool.cron.pattern.CronPattern(java.lang.String);
  public boolean match(long, boolean);
  public boolean match(java.util.TimeZone, long, boolean);
  public boolean match(java.util.Calendar, boolean);
  public boolean match(java.time.LocalDateTime, boolean);
  public java.util.Calendar nextMatchAfter(java.util.Calendar);
  public java.util.Calendar nextMatch(java.util.Calendar);
  public java.lang.String toString();
}
```

## `cn.hutool.cron.pattern.CronPatternBuilder`

```java
public class cn.hutool.cron.pattern.CronPatternBuilder implements cn.hutool.core.builder.Builder<java.lang.String> {
  public cn.hutool.cron.pattern.CronPatternBuilder();
  public static cn.hutool.cron.pattern.CronPatternBuilder of();
  public cn.hutool.cron.pattern.CronPatternBuilder setValues(cn.hutool.cron.pattern.Part, int...);
  public cn.hutool.cron.pattern.CronPatternBuilder setRange(cn.hutool.cron.pattern.Part, int, int);
  public cn.hutool.cron.pattern.CronPatternBuilder set(cn.hutool.cron.pattern.Part, java.lang.String);
  public java.lang.String build();
  public java.lang.Object build();
}
```

## `cn.hutool.cron.pattern.CronPatternUtil`

```java
public class cn.hutool.cron.pattern.CronPatternUtil {
  public cn.hutool.cron.pattern.CronPatternUtil();
  public static java.util.Date nextDateAfter(cn.hutool.cron.pattern.CronPattern, java.util.Date);
  public static java.util.Date nextDateAfter(cn.hutool.cron.pattern.CronPattern, java.util.Date, boolean);
  public static java.util.List<java.util.Date> matchedDates(java.lang.String, java.util.Date, int, boolean);
  public static java.util.List<java.util.Date> matchedDates(java.lang.String, java.util.Date, java.util.Date, int, boolean);
  public static java.util.List<java.util.Date> matchedDates(java.lang.String, long, long, int, boolean);
  public static java.util.List<java.util.Date> matchedDates(cn.hutool.cron.pattern.CronPattern, long, long, int, boolean);
}
```

## `cn.hutool.cron.pattern.Part`

```java
public final class cn.hutool.cron.pattern.Part extends java.lang.Enum<cn.hutool.cron.pattern.Part> {
  public static cn.hutool.cron.pattern.Part[] values();
  public static cn.hutool.cron.pattern.Part valueOf(java.lang.String);
  public int getCalendarField();
  public int getMin();
  public int getMax();
  public int checkValue(int) throws cn.hutool.cron.CronException;
  public static cn.hutool.cron.pattern.Part of(int);
}
```
