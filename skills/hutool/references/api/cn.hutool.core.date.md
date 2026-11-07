# cn.hutool.core.date

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.date.BetweenFormatter`

```java
public class cn.hutool.core.date.BetweenFormatter implements java.io.Serializable {
  public cn.hutool.core.date.BetweenFormatter(long, cn.hutool.core.date.BetweenFormatter$Level);
  public cn.hutool.core.date.BetweenFormatter(long, cn.hutool.core.date.BetweenFormatter$Level, int);
  public java.lang.String format();
  public long getBetweenMs();
  public void setBetweenMs(long);
  public cn.hutool.core.date.BetweenFormatter$Level getLevel();
  public void setLevel(cn.hutool.core.date.BetweenFormatter$Level);
  public cn.hutool.core.date.BetweenFormatter setLevelFormatter(java.util.function.Function<cn.hutool.core.date.BetweenFormatter$Level, java.lang.String>);
  public cn.hutool.core.date.BetweenFormatter setSeparator(java.lang.String);
  public java.lang.String toString();
}
```

## `cn.hutool.core.date.BetweenFormatter$Level`

```java
public final class cn.hutool.core.date.BetweenFormatter$Level extends java.lang.Enum<cn.hutool.core.date.BetweenFormatter$Level> {
  public static cn.hutool.core.date.BetweenFormatter$Level[] values();
  public static cn.hutool.core.date.BetweenFormatter$Level valueOf(java.lang.String);
  public java.lang.String getName();
}
```

## `cn.hutool.core.date.CalendarUtil`

```java
public class cn.hutool.core.date.CalendarUtil {
  public cn.hutool.core.date.CalendarUtil();
  public static java.util.Calendar calendar();
  public static java.util.Calendar calendar(java.util.Date);
  public static java.util.Calendar calendar(long);
  public static java.util.Calendar calendar(long, java.util.TimeZone);
  public static java.util.Calendar calendar(java.util.Calendar, java.util.TimeZone);
  public static boolean isAM(java.util.Calendar);
  public static boolean isPM(java.util.Calendar);
  public static java.util.Calendar truncate(java.util.Calendar, cn.hutool.core.date.DateField);
  public static java.util.Calendar round(java.util.Calendar, cn.hutool.core.date.DateField);
  public static java.util.Calendar ceiling(java.util.Calendar, cn.hutool.core.date.DateField);
  public static java.util.Calendar ceiling(java.util.Calendar, cn.hutool.core.date.DateField, boolean);
  public static java.util.Calendar beginOfSecond(java.util.Calendar);
  public static java.util.Calendar endOfSecond(java.util.Calendar);
  public static java.util.Calendar beginOfHour(java.util.Calendar);
  public static java.util.Calendar endOfHour(java.util.Calendar);
  public static java.util.Calendar beginOfMinute(java.util.Calendar);
  public static java.util.Calendar endOfMinute(java.util.Calendar);
  public static java.util.Calendar beginOfDay(java.util.Calendar);
  public static java.util.Calendar endOfDay(java.util.Calendar);
  public static java.util.Calendar beginOfWeek(java.util.Calendar);
  public static java.util.Calendar beginOfWeek(java.util.Calendar, boolean);
  public static java.util.Calendar endOfWeek(java.util.Calendar);
  public static java.util.Calendar endOfWeek(java.util.Calendar, boolean);
  public static java.util.Calendar beginOfMonth(java.util.Calendar);
  public static java.util.Calendar endOfMonth(java.util.Calendar);
  public static java.util.Calendar beginOfQuarter(java.util.Calendar);
  public static java.util.Calendar endOfQuarter(java.util.Calendar);
  public static java.util.Calendar beginOfYear(java.util.Calendar);
  public static java.util.Calendar endOfYear(java.util.Calendar);
  public static boolean isSameDay(java.util.Calendar, java.util.Calendar);
  public static boolean isLastDayOfMonth(java.util.Calendar);
  public static boolean isSameWeek(java.util.Calendar, java.util.Calendar, boolean);
  public static boolean isSameMonth(java.util.Calendar, java.util.Calendar);
  public static boolean isSameYear(java.util.Calendar, java.util.Calendar);
  public static boolean isSameInstant(java.util.Calendar, java.util.Calendar);
  public static java.util.LinkedHashSet<java.lang.String> yearAndQuarter(long, long);
  public static java.lang.String yearAndQuarter(java.util.Calendar);
  public static int getBeginValue(java.util.Calendar, cn.hutool.core.date.DateField);
  public static int getBeginValue(java.util.Calendar, int);
  public static int getEndValue(java.util.Calendar, cn.hutool.core.date.DateField);
  public static int getEndValue(java.util.Calendar, int);
  public static java.time.Instant toInstant(java.util.Calendar);
  public static java.time.LocalDateTime toLocalDateTime(java.util.Calendar);
  public static int compare(java.util.Calendar, java.util.Calendar);
  public static int age(java.util.Calendar, java.util.Calendar);
  public static java.lang.String formatChineseDate(java.util.Calendar, boolean);
  public static java.util.Calendar parseByPatterns(java.lang.String, java.lang.String...) throws cn.hutool.core.date.DateException;
  public static java.util.Calendar parseByPatterns(java.lang.String, java.util.Locale, java.lang.String...) throws cn.hutool.core.date.DateException;
  public static java.util.Calendar parseByPatterns(java.lang.String, java.util.Locale, boolean, java.lang.String...) throws cn.hutool.core.date.DateException;
  public static java.util.Calendar parse(java.lang.CharSequence, boolean, cn.hutool.core.date.format.DateParser);
}
```

## `cn.hutool.core.date.ChineseDate`

```java
public class cn.hutool.core.date.ChineseDate {
  public cn.hutool.core.date.ChineseDate(java.util.Date);
  public cn.hutool.core.date.ChineseDate(java.time.LocalDate);
  public cn.hutool.core.date.ChineseDate(int, int, int);
  public cn.hutool.core.date.ChineseDate(int, int, int, boolean);
  public int getChineseYear();
  public int getGregorianYear();
  public int getMonth();
  public int getGregorianMonthBase1();
  public int getGregorianMonth();
  public boolean isLeapMonth();
  public java.lang.String getChineseMonth();
  public java.lang.String getChineseMonthName();
  public java.lang.String getChineseMonth(boolean);
  public int getDay();
  public int getGregorianDay();
  public java.lang.String getChineseDay();
  public java.util.Date getGregorianDate();
  public java.util.Calendar getGregorianCalendar();
  public java.lang.String getFestivals();
  public java.lang.String getChineseZodiac();
  public java.lang.String getCyclical();
  public java.lang.String getCyclicalYMD();
  public java.lang.String getTerm();
  public java.lang.String toStringNormal();
  public java.lang.String toString();
}
```

## `cn.hutool.core.date.DateBetween`

```java
public class cn.hutool.core.date.DateBetween implements java.io.Serializable {
  public static cn.hutool.core.date.DateBetween create(java.util.Date, java.util.Date);
  public static cn.hutool.core.date.DateBetween create(java.util.Date, java.util.Date, boolean);
  public cn.hutool.core.date.DateBetween(java.util.Date, java.util.Date);
  public cn.hutool.core.date.DateBetween(java.util.Date, java.util.Date, boolean);
  public long between(cn.hutool.core.date.DateUnit);
  public long betweenMonth(boolean);
  public long betweenYear(boolean);
  public java.lang.String toString(cn.hutool.core.date.DateUnit, cn.hutool.core.date.BetweenFormatter$Level);
  public java.lang.String toString(cn.hutool.core.date.BetweenFormatter$Level);
  public java.lang.String toString();
}
```

## `cn.hutool.core.date.DateException`

```java
public class cn.hutool.core.date.DateException extends java.lang.RuntimeException {
  public cn.hutool.core.date.DateException(java.lang.Throwable);
  public cn.hutool.core.date.DateException(java.lang.String);
  public cn.hutool.core.date.DateException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.date.DateException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.date.DateException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.core.date.DateField`

```java
public final class cn.hutool.core.date.DateField extends java.lang.Enum<cn.hutool.core.date.DateField> {
  public static cn.hutool.core.date.DateField[] values();
  public static cn.hutool.core.date.DateField valueOf(java.lang.String);
  public int getValue();
  public static cn.hutool.core.date.DateField of(int);
}
```

## `cn.hutool.core.date.DateModifier`

```java
public class cn.hutool.core.date.DateModifier {
  public cn.hutool.core.date.DateModifier();
  public static java.util.Calendar modify(java.util.Calendar, int, cn.hutool.core.date.DateModifier$ModifyType);
  public static java.util.Calendar modify(java.util.Calendar, int, cn.hutool.core.date.DateModifier$ModifyType, boolean);
}
```

## `cn.hutool.core.date.DateModifier$ModifyType`

```java
public final class cn.hutool.core.date.DateModifier$ModifyType extends java.lang.Enum<cn.hutool.core.date.DateModifier$ModifyType> {
  public static cn.hutool.core.date.DateModifier$ModifyType[] values();
  public static cn.hutool.core.date.DateModifier$ModifyType valueOf(java.lang.String);
}
```

## `cn.hutool.core.date.DatePattern`

```java
public class cn.hutool.core.date.DatePattern {
  public cn.hutool.core.date.DatePattern();
  public static java.time.format.DateTimeFormatter createFormatter(java.lang.String);
}
```

## `cn.hutool.core.date.DateRange`

```java
public class cn.hutool.core.date.DateRange extends cn.hutool.core.lang.Range<cn.hutool.core.date.DateTime> {
  public cn.hutool.core.date.DateRange(java.util.Date, java.util.Date, cn.hutool.core.date.DateField);
  public cn.hutool.core.date.DateRange(java.util.Date, java.util.Date, cn.hutool.core.date.DateField, int);
  public cn.hutool.core.date.DateRange(java.util.Date, java.util.Date, cn.hutool.core.date.DateField, int, boolean, boolean);
}
```

## `cn.hutool.core.date.DateTime`

```java
public class cn.hutool.core.date.DateTime extends java.util.Date {
  public static void setUseJdkToStringStyle(boolean);
  public static cn.hutool.core.date.DateTime of(long);
  public static cn.hutool.core.date.DateTime of(java.util.Date);
  public static cn.hutool.core.date.DateTime of(java.util.Calendar);
  public static cn.hutool.core.date.DateTime of(java.lang.String, java.lang.String);
  public static cn.hutool.core.date.DateTime now();
  public cn.hutool.core.date.DateTime();
  public cn.hutool.core.date.DateTime(java.util.TimeZone);
  public cn.hutool.core.date.DateTime(java.util.Date);
  public cn.hutool.core.date.DateTime(java.util.Date, java.util.TimeZone);
  public cn.hutool.core.date.DateTime(java.util.Calendar);
  public cn.hutool.core.date.DateTime(java.time.Instant);
  public cn.hutool.core.date.DateTime(java.time.Instant, java.time.ZoneId);
  public cn.hutool.core.date.DateTime(java.time.temporal.TemporalAccessor);
  public cn.hutool.core.date.DateTime(java.time.ZonedDateTime);
  public cn.hutool.core.date.DateTime(long);
  public cn.hutool.core.date.DateTime(long, java.util.TimeZone);
  public cn.hutool.core.date.DateTime(java.lang.CharSequence);
  public cn.hutool.core.date.DateTime(java.lang.CharSequence, java.lang.String);
  public cn.hutool.core.date.DateTime(java.lang.CharSequence, java.text.DateFormat);
  public cn.hutool.core.date.DateTime(java.lang.CharSequence, java.time.format.DateTimeFormatter);
  public cn.hutool.core.date.DateTime(java.lang.CharSequence, cn.hutool.core.date.format.DateParser);
  public cn.hutool.core.date.DateTime(java.lang.CharSequence, cn.hutool.core.date.format.DateParser, boolean);
  public cn.hutool.core.date.DateTime offset(cn.hutool.core.date.DateField, int);
  public cn.hutool.core.date.DateTime offsetNew(cn.hutool.core.date.DateField, int);
  public int getField(cn.hutool.core.date.DateField);
  public int getField(int);
  public cn.hutool.core.date.DateTime setField(cn.hutool.core.date.DateField, int);
  public cn.hutool.core.date.DateTime setField(int, int);
  public void setTime(long);
  public int year();
  public int quarter();
  public cn.hutool.core.date.Quarter quarterEnum();
  public int month();
  public int monthBaseOne();
  public int monthStartFromOne();
  public cn.hutool.core.date.Month monthEnum();
  public int weekOfYear();
  public int weekOfMonth();
  public int dayOfMonth();
  public int dayOfYear();
  public int dayOfWeek();
  public int dayOfWeekInMonth();
  public cn.hutool.core.date.Week dayOfWeekEnum();
  public int hour(boolean);
  public int minute();
  public int second();
  public int millisecond();
  public boolean isAM();
  public boolean isPM();
  public boolean isWeekend();
  public boolean isLeapYear();
  public java.util.Calendar toCalendar();
  public java.util.Calendar toCalendar(java.util.Locale);
  public java.util.Calendar toCalendar(java.util.TimeZone);
  public java.util.Calendar toCalendar(java.util.TimeZone, java.util.Locale);
  public java.util.Date toJdkDate();
  public java.sql.Timestamp toTimestamp();
  public java.sql.Date toSqlDate();
  public java.time.LocalDateTime toLocalDateTime();
  public cn.hutool.core.date.DateBetween between(java.util.Date);
  public long between(java.util.Date, cn.hutool.core.date.DateUnit);
  public java.lang.String between(java.util.Date, cn.hutool.core.date.DateUnit, cn.hutool.core.date.BetweenFormatter$Level);
  public boolean isIn(java.util.Date, java.util.Date);
  public boolean isBefore(java.util.Date);
  public boolean isBeforeOrEquals(java.util.Date);
  public boolean isAfter(java.util.Date);
  public boolean isAfterOrEquals(java.util.Date);
  public boolean isMutable();
  public cn.hutool.core.date.DateTime setMutable(boolean);
  public cn.hutool.core.date.Week getFirstDayOfWeek();
  public cn.hutool.core.date.DateTime setFirstDayOfWeek(cn.hutool.core.date.Week);
  public java.util.TimeZone getTimeZone();
  public java.time.ZoneId getZoneId();
  public cn.hutool.core.date.DateTime setTimeZone(java.util.TimeZone);
  public cn.hutool.core.date.DateTime setMinimalDaysInFirstWeek(int);
  public boolean isLastDayOfMonth();
  public int getLastDayOfMonth();
  public java.lang.String toString();
  public java.lang.String toStringDefaultTimeZone();
  public java.lang.String toString(java.util.TimeZone);
  public java.lang.String toDateStr();
  public java.lang.String toTimeStr();
  public java.lang.String toString(java.lang.String);
  public java.lang.String toString(cn.hutool.core.date.format.DatePrinter);
  public java.lang.String toString(java.text.DateFormat);
  public java.lang.String toMsStr();
}
```

## `cn.hutool.core.date.DateUnit`

```java
public final class cn.hutool.core.date.DateUnit extends java.lang.Enum<cn.hutool.core.date.DateUnit> {
  public static cn.hutool.core.date.DateUnit[] values();
  public static cn.hutool.core.date.DateUnit valueOf(java.lang.String);
  public long getMillis();
  public java.time.temporal.ChronoUnit toChronoUnit();
  public static cn.hutool.core.date.DateUnit of(java.time.temporal.ChronoUnit);
  public static java.time.temporal.ChronoUnit toChronoUnit(cn.hutool.core.date.DateUnit);
}
```

## `cn.hutool.core.date.DateUtil`

```java
public class cn.hutool.core.date.DateUtil extends cn.hutool.core.date.CalendarUtil {
  public cn.hutool.core.date.DateUtil();
  public static cn.hutool.core.date.DateTime date();
  public static cn.hutool.core.date.DateTime dateSecond();
  public static cn.hutool.core.date.DateTime date(java.util.Date);
  public static cn.hutool.core.date.DateTime dateNew(java.util.Date);
  public static cn.hutool.core.date.DateTime date(long);
  public static cn.hutool.core.date.DateTime date(java.util.Calendar);
  public static cn.hutool.core.date.DateTime date(java.time.temporal.TemporalAccessor);
  public static long current();
  public static long currentSeconds();
  public static java.lang.String now();
  public static java.lang.String today();
  public static int year(java.util.Date);
  public static int quarter(java.util.Date);
  public static cn.hutool.core.date.Quarter quarterEnum(java.util.Date);
  public static int month(java.util.Date);
  public static cn.hutool.core.date.Month monthEnum(java.util.Date);
  public static int weekOfYear(java.util.Date);
  public static int weekOfMonth(java.util.Date);
  public static int dayOfMonth(java.util.Date);
  public static int dayOfYear(java.util.Date);
  public static int dayOfWeek(java.util.Date);
  public static cn.hutool.core.date.Week dayOfWeekEnum(java.util.Date);
  public static boolean isWeekend(java.util.Date);
  public static int hour(java.util.Date, boolean);
  public static int minute(java.util.Date);
  public static int second(java.util.Date);
  public static int millisecond(java.util.Date);
  public static boolean isAM(java.util.Date);
  public static boolean isPM(java.util.Date);
  public static int thisYear();
  public static int thisMonth();
  public static cn.hutool.core.date.Month thisMonthEnum();
  public static int thisWeekOfYear();
  public static int thisWeekOfMonth();
  public static int thisDayOfMonth();
  public static int thisDayOfWeek();
  public static cn.hutool.core.date.Week thisDayOfWeekEnum();
  public static int thisHour(boolean);
  public static int thisMinute();
  public static int thisSecond();
  public static int thisMillisecond();
  public static java.lang.String yearAndQuarter(java.util.Date);
  public static java.util.LinkedHashSet<java.lang.String> yearAndQuarter(java.util.Date, java.util.Date);
  public static java.lang.String formatLocalDateTime(java.time.LocalDateTime);
  public static java.lang.String format(java.time.LocalDateTime, java.lang.String);
  public static java.lang.String format(java.util.Date, java.lang.String);
  public static java.lang.String format(java.util.Date, cn.hutool.core.date.format.DatePrinter);
  public static java.lang.String format(java.util.Date, java.text.DateFormat);
  public static java.lang.String format(java.util.Date, java.time.format.DateTimeFormatter);
  public static java.lang.String formatDateTime(java.util.Date);
  public static java.lang.String formatDate(java.util.Date);
  public static java.lang.String formatTime(java.util.Date);
  public static java.lang.String formatHttpDate(java.util.Date);
  public static java.lang.String formatChineseDate(java.util.Date, boolean, boolean);
  public static java.time.LocalDateTime parseLocalDateTime(java.lang.CharSequence);
  public static java.time.LocalDateTime parseLocalDateTime(java.lang.CharSequence, java.lang.String);
  public static cn.hutool.core.date.DateTime parse(java.lang.CharSequence, java.text.DateFormat);
  public static cn.hutool.core.date.DateTime parse(java.lang.CharSequence, cn.hutool.core.date.format.DateParser);
  public static cn.hutool.core.date.DateTime parse(java.lang.CharSequence, cn.hutool.core.date.format.DateParser, boolean);
  public static cn.hutool.core.date.DateTime parse(java.lang.CharSequence, java.time.format.DateTimeFormatter);
  public static cn.hutool.core.date.DateTime parse(java.lang.CharSequence, java.lang.String);
  public static cn.hutool.core.date.DateTime parse(java.lang.CharSequence, java.lang.String, java.util.Locale);
  public static cn.hutool.core.date.DateTime parse(java.lang.String, java.lang.String...) throws cn.hutool.core.date.DateException;
  public static cn.hutool.core.date.DateTime parseDateTime(java.lang.CharSequence);
  public static cn.hutool.core.date.DateTime parseDate(java.lang.CharSequence);
  public static cn.hutool.core.date.DateTime parseTime(java.lang.CharSequence);
  public static cn.hutool.core.date.DateTime parseTimeToday(java.lang.CharSequence);
  public static cn.hutool.core.date.DateTime parseUTC(java.lang.String);
  public static cn.hutool.core.date.DateTime parseISO8601(java.lang.String);
  public static cn.hutool.core.date.DateTime parseCST(java.lang.CharSequence);
  public static cn.hutool.core.date.DateTime parseRFC2822(java.lang.CharSequence);
  public static cn.hutool.core.date.DateTime parse(java.lang.CharSequence);
  public static cn.hutool.core.date.DateTime truncate(java.util.Date, cn.hutool.core.date.DateField);
  public static cn.hutool.core.date.DateTime round(java.util.Date, cn.hutool.core.date.DateField);
  public static cn.hutool.core.date.DateTime ceiling(java.util.Date, cn.hutool.core.date.DateField);
  public static cn.hutool.core.date.DateTime ceiling(java.util.Date, cn.hutool.core.date.DateField, boolean);
  public static cn.hutool.core.date.DateTime beginOfSecond(java.util.Date);
  public static cn.hutool.core.date.DateTime endOfSecond(java.util.Date);
  public static cn.hutool.core.date.DateTime beginOfHour(java.util.Date);
  public static cn.hutool.core.date.DateTime endOfHour(java.util.Date);
  public static cn.hutool.core.date.DateTime beginOfMinute(java.util.Date);
  public static cn.hutool.core.date.DateTime endOfMinute(java.util.Date);
  public static cn.hutool.core.date.DateTime beginOfDay(java.util.Date);
  public static cn.hutool.core.date.DateTime endOfDay(java.util.Date);
  public static cn.hutool.core.date.DateTime beginOfWeek(java.util.Date);
  public static cn.hutool.core.date.DateTime beginOfWeek(java.util.Date, boolean);
  public static cn.hutool.core.date.DateTime endOfWeek(java.util.Date);
  public static cn.hutool.core.date.DateTime endOfWeek(java.util.Date, boolean);
  public static cn.hutool.core.date.DateTime beginOfMonth(java.util.Date);
  public static cn.hutool.core.date.DateTime endOfMonth(java.util.Date);
  public static cn.hutool.core.date.DateTime beginOfQuarter(java.util.Date);
  public static cn.hutool.core.date.DateTime endOfQuarter(java.util.Date);
  public static cn.hutool.core.date.DateTime beginOfYear(java.util.Date);
  public static cn.hutool.core.date.DateTime endOfYear(java.util.Date);
  public static cn.hutool.core.date.DateTime yesterday();
  public static cn.hutool.core.date.DateTime tomorrow();
  public static cn.hutool.core.date.DateTime lastWeek();
  public static cn.hutool.core.date.DateTime nextWeek();
  public static cn.hutool.core.date.DateTime lastMonth();
  public static cn.hutool.core.date.DateTime nextMonth();
  public static cn.hutool.core.date.DateTime offsetMillisecond(java.util.Date, int);
  public static cn.hutool.core.date.DateTime offsetSecond(java.util.Date, int);
  public static cn.hutool.core.date.DateTime offsetMinute(java.util.Date, int);
  public static cn.hutool.core.date.DateTime offsetHour(java.util.Date, int);
  public static cn.hutool.core.date.DateTime offsetDay(java.util.Date, int);
  public static cn.hutool.core.date.DateTime offsetWeek(java.util.Date, int);
  public static cn.hutool.core.date.DateTime offsetMonth(java.util.Date, int);
  public static cn.hutool.core.date.DateTime offsetYear(java.util.Date, int);
  public static cn.hutool.core.date.DateTime offset(java.util.Date, cn.hutool.core.date.DateField, int);
  public static long between(java.util.Date, java.util.Date, cn.hutool.core.date.DateUnit);
  public static long between(java.util.Date, java.util.Date, cn.hutool.core.date.DateUnit, boolean);
  public static long betweenMs(java.util.Date, java.util.Date);
  public static long betweenDay(java.util.Date, java.util.Date, boolean);
  public static long betweenWeek(java.util.Date, java.util.Date, boolean);
  public static long betweenMonth(java.util.Date, java.util.Date, boolean);
  public static long betweenYear(java.util.Date, java.util.Date, boolean);
  public static java.lang.String formatBetween(java.util.Date, java.util.Date, cn.hutool.core.date.BetweenFormatter$Level);
  public static java.lang.String formatBetween(java.util.Date, java.util.Date);
  public static java.lang.String formatBetween(long, cn.hutool.core.date.BetweenFormatter$Level);
  public static java.lang.String formatBetween(long);
  public static boolean isIn(java.util.Date, java.util.Date, java.util.Date);
  public static boolean isSameTime(java.util.Date, java.util.Date);
  public static boolean isSameDay(java.util.Date, java.util.Date);
  public static boolean isSameWeek(java.util.Date, java.util.Date, boolean);
  public static boolean isSameMonth(java.util.Date, java.util.Date);
  public static long spendNt(long);
  public static long spendMs(long);
  public static int toIntSecond(java.util.Date);
  public static cn.hutool.core.date.TimeInterval timer();
  public static cn.hutool.core.date.TimeInterval timer(boolean);
  public static cn.hutool.core.date.StopWatch createStopWatch();
  public static cn.hutool.core.date.StopWatch createStopWatch(java.lang.String);
  public static int ageOfNow(java.lang.String);
  public static int ageOfNow(java.util.Date);
  public static boolean isLeapYear(int);
  public static int age(java.util.Date, java.util.Date);
  public static boolean isExpired(java.util.Date, cn.hutool.core.date.DateField, int, java.util.Date);
  public static boolean isExpired(java.util.Date, java.util.Date, java.util.Date);
  public static int timeToSecond(java.lang.String);
  public static java.lang.String secondToTime(int);
  public static cn.hutool.core.date.DateRange range(java.util.Date, java.util.Date, cn.hutool.core.date.DateField);
  public static java.util.List<cn.hutool.core.date.DateTime> rangeContains(cn.hutool.core.date.DateRange, cn.hutool.core.date.DateRange);
  public static java.util.List<cn.hutool.core.date.DateTime> rangeNotContains(cn.hutool.core.date.DateRange, cn.hutool.core.date.DateRange);
  public static <T> java.util.List<T> rangeFunc(java.util.Date, java.util.Date, cn.hutool.core.date.DateField, java.util.function.Function<java.util.Date, T>);
  public static void rangeConsume(java.util.Date, java.util.Date, cn.hutool.core.date.DateField, java.util.function.Consumer<java.util.Date>);
  public static java.util.List<cn.hutool.core.date.DateTime> rangeToList(java.util.Date, java.util.Date, cn.hutool.core.date.DateField);
  public static java.util.List<cn.hutool.core.date.DateTime> rangeToList(java.util.Date, java.util.Date, cn.hutool.core.date.DateField, int);
  public static java.lang.String getZodiac(int, int);
  public static java.lang.String getChineseZodiac(int);
  public static int compare(java.util.Date, java.util.Date);
  public static int compare(java.util.Date, java.util.Date, java.lang.String);
  public static long nanosToMillis(long);
  public static double nanosToSeconds(long);
  public static java.time.Instant toInstant(java.util.Date);
  public static java.time.Instant toInstant(java.time.temporal.TemporalAccessor);
  public static java.time.LocalDateTime toLocalDateTime(java.time.Instant);
  public static java.time.LocalDateTime toLocalDateTime(java.util.Date);
  public static cn.hutool.core.date.DateTime convertTimeZone(java.util.Date, java.time.ZoneId);
  public static cn.hutool.core.date.DateTime convertTimeZone(java.util.Date, java.util.TimeZone);
  public static int lengthOfYear(int);
  public static int lengthOfMonth(int, boolean);
  public static java.text.SimpleDateFormat newSimpleFormat(java.lang.String);
  public static java.text.SimpleDateFormat newSimpleFormat(java.lang.String, java.util.Locale, java.util.TimeZone);
  public static java.lang.String getShotName(java.util.concurrent.TimeUnit);
  public static boolean isOverlap(java.util.Date, java.util.Date, java.util.Date, java.util.Date);
  public static boolean isLastDayOfMonth(java.util.Date);
  public static int getLastDayOfMonth(java.util.Date);
}
```

## `cn.hutool.core.date.GroupTimeInterval`

```java
public class cn.hutool.core.date.GroupTimeInterval implements java.io.Serializable {
  public cn.hutool.core.date.GroupTimeInterval(boolean);
  public cn.hutool.core.date.GroupTimeInterval clear();
  public long start(java.lang.String);
  public long intervalRestart(java.lang.String);
  public long interval(java.lang.String);
  public long interval(java.lang.String, cn.hutool.core.date.DateUnit);
  public long intervalMs(java.lang.String);
  public long intervalSecond(java.lang.String);
  public long intervalMinute(java.lang.String);
  public long intervalHour(java.lang.String);
  public long intervalDay(java.lang.String);
  public long intervalWeek(java.lang.String);
  public java.lang.String intervalPretty(java.lang.String);
}
```

## `cn.hutool.core.date.LocalDateTimeUtil`

```java
public class cn.hutool.core.date.LocalDateTimeUtil {
  public cn.hutool.core.date.LocalDateTimeUtil();
  public static java.time.LocalDateTime now();
  public static java.time.LocalDateTime of(java.time.Instant);
  public static java.time.LocalDateTime ofUTC(java.time.Instant);
  public static java.time.LocalDateTime of(java.time.ZonedDateTime);
  public static java.time.LocalDateTime of(java.time.Instant, java.time.ZoneId);
  public static java.time.LocalDateTime of(java.time.Instant, java.util.TimeZone);
  public static java.time.LocalDateTime of(long);
  public static java.time.LocalDateTime ofUTC(long);
  public static java.time.LocalDateTime of(long, java.time.ZoneId);
  public static java.time.LocalDateTime of(long, java.util.TimeZone);
  public static java.time.LocalDateTime of(java.util.Date);
  public static java.time.LocalDateTime of(java.time.temporal.TemporalAccessor);
  public static java.time.LocalDate ofDate(java.time.temporal.TemporalAccessor);
  public static java.time.LocalDateTime parse(java.lang.CharSequence);
  public static java.time.LocalDateTime parse(java.lang.CharSequence, java.time.format.DateTimeFormatter);
  public static java.time.LocalDateTime parse(java.lang.CharSequence, java.lang.String);
  public static java.time.LocalDate parseDate(java.lang.CharSequence);
  public static java.time.LocalDate parseDate(java.lang.CharSequence, java.time.format.DateTimeFormatter);
  public static java.time.LocalDate parseDate(java.lang.CharSequence, java.lang.String);
  public static java.lang.String formatNormal(java.time.LocalDateTime);
  public static java.lang.String format(java.time.LocalDateTime, java.time.format.DateTimeFormatter);
  public static java.lang.String format(java.time.LocalDateTime, java.lang.String);
  public static java.lang.String formatNormal(java.time.LocalDate);
  public static java.lang.String format(java.time.LocalDate, java.time.format.DateTimeFormatter);
  public static java.lang.String format(java.time.LocalDate, java.lang.String);
  public static java.time.LocalDateTime offset(java.time.LocalDateTime, long, java.time.temporal.TemporalUnit);
  public static java.time.Duration between(java.time.LocalDateTime, java.time.LocalDateTime);
  public static long between(java.time.LocalDateTime, java.time.LocalDateTime, java.time.temporal.ChronoUnit);
  public static java.time.Period betweenPeriod(java.time.LocalDate, java.time.LocalDate);
  public static java.time.LocalDateTime beginOfDay(java.time.LocalDateTime);
  public static java.time.LocalDateTime beginOfDay(java.time.LocalDate);
  public static java.time.LocalDateTime endOfDay(java.time.LocalDateTime);
  public static java.time.LocalDateTime endOfDay(java.time.LocalDate);
  public static java.time.LocalDateTime endOfDay(java.time.LocalDateTime, boolean);
  public static java.time.LocalDateTime endOfDay(java.time.LocalDate, boolean);
  public static long toEpochMilli(java.time.temporal.TemporalAccessor);
  public static boolean isWeekend(java.time.LocalDateTime);
  public static boolean isWeekend(java.time.LocalDate);
  public static cn.hutool.core.date.Week dayOfWeek(java.time.LocalDate);
  public static boolean isOverlap(java.time.chrono.ChronoLocalDateTime<?>, java.time.chrono.ChronoLocalDateTime<?>, java.time.chrono.ChronoLocalDateTime<?>, java.time.chrono.ChronoLocalDateTime<?>);
  public static int weekOfYear(java.time.temporal.TemporalAccessor);
  public static boolean isSameDay(java.time.LocalDateTime, java.time.LocalDateTime);
  public static boolean isSameDay(java.time.LocalDate, java.time.LocalDate);
  public static boolean isIn(java.time.chrono.ChronoLocalDateTime<?>, java.time.chrono.ChronoLocalDateTime<?>, java.time.chrono.ChronoLocalDateTime<?>);
  public static boolean isIn(java.time.chrono.ChronoLocalDateTime<?>, java.time.chrono.ChronoLocalDateTime<?>, java.time.chrono.ChronoLocalDateTime<?>, boolean, boolean);
}
```

## `cn.hutool.core.date.Month`

```java
public final class cn.hutool.core.date.Month extends java.lang.Enum<cn.hutool.core.date.Month> {
  public static cn.hutool.core.date.Month[] values();
  public static cn.hutool.core.date.Month valueOf(java.lang.String);
  public int getValue();
  public int getValueBaseOne();
  public int getLastDay(boolean);
  public static cn.hutool.core.date.Month of(int);
  public static cn.hutool.core.date.Month of(java.lang.String) throws java.lang.IllegalArgumentException;
  public static cn.hutool.core.date.Month of(java.time.Month);
  public static int getLastDay(int, boolean);
  public java.time.Month toJdkMonth();
  public java.lang.String getDisplayName(java.time.format.TextStyle);
  public java.lang.String getDisplayName(java.time.format.TextStyle, java.util.Locale);
}
```

## `cn.hutool.core.date.Quarter`

```java
public final class cn.hutool.core.date.Quarter extends java.lang.Enum<cn.hutool.core.date.Quarter> {
  public static cn.hutool.core.date.Quarter[] values();
  public static cn.hutool.core.date.Quarter valueOf(java.lang.String);
  public int getValue();
  public static cn.hutool.core.date.Quarter of(int);
  public static cn.hutool.core.date.Quarter fromMonth(int);
  public static cn.hutool.core.date.Quarter fromMonth(cn.hutool.core.date.Month);
  public final cn.hutool.core.date.YearQuarter atYear(int);
  public cn.hutool.core.date.Quarter plus(int);
  public cn.hutool.core.date.Month firstMonth();
  public int firstMonthValue();
  public cn.hutool.core.date.Month lastMonth();
  public int lastMonthValue();
  public java.time.MonthDay firstMonthDay();
  public java.time.MonthDay lastMonthDay();
  public static int checkValidIntValue(int);
}
```

## `cn.hutool.core.date.StopWatch`

```java
public class cn.hutool.core.date.StopWatch {
  public static cn.hutool.core.date.StopWatch create(java.lang.String);
  public cn.hutool.core.date.StopWatch();
  public cn.hutool.core.date.StopWatch(java.lang.String);
  public cn.hutool.core.date.StopWatch(java.lang.String, boolean);
  public java.lang.String getId();
  public void setKeepTaskList(boolean);
  public void start() throws java.lang.IllegalStateException;
  public void start(java.lang.String) throws java.lang.IllegalStateException;
  public void stop() throws java.lang.IllegalStateException;
  public boolean isRunning();
  public java.lang.String currentTaskName();
  public long getLastTaskTimeNanos() throws java.lang.IllegalStateException;
  public long getLastTaskTimeMillis() throws java.lang.IllegalStateException;
  public java.lang.String getLastTaskName() throws java.lang.IllegalStateException;
  public cn.hutool.core.date.StopWatch$TaskInfo getLastTaskInfo() throws java.lang.IllegalStateException;
  public long getTotal(java.util.concurrent.TimeUnit);
  public long getTotalTimeNanos();
  public long getTotalTimeMillis();
  public double getTotalTimeSeconds();
  public int getTaskCount();
  public cn.hutool.core.date.StopWatch$TaskInfo[] getTaskInfo();
  public java.lang.String shortSummary();
  public java.lang.String shortSummary(java.util.concurrent.TimeUnit);
  public java.lang.String prettyPrint();
  public java.lang.String prettyPrint(java.util.concurrent.TimeUnit);
  public java.lang.String toString();
}
```

## `cn.hutool.core.date.StopWatch$TaskInfo`

```java
public final class cn.hutool.core.date.StopWatch$TaskInfo {
  public java.lang.String getTaskName();
  public long getTime(java.util.concurrent.TimeUnit);
  public long getTimeNanos();
  public long getTimeMillis();
  public double getTimeSeconds();
}
```

## `cn.hutool.core.date.SystemClock`

```java
public class cn.hutool.core.date.SystemClock {
  public cn.hutool.core.date.SystemClock(long);
  public static long now();
  public static java.lang.String nowDate();
}
```

## `cn.hutool.core.date.TemporalAccessorUtil`

```java
public class cn.hutool.core.date.TemporalAccessorUtil extends cn.hutool.core.date.TemporalUtil {
  public cn.hutool.core.date.TemporalAccessorUtil();
  public static int get(java.time.temporal.TemporalAccessor, java.time.temporal.TemporalField);
  public static java.lang.String format(java.time.temporal.TemporalAccessor, java.time.format.DateTimeFormatter);
  public static java.lang.String format(java.time.temporal.TemporalAccessor, java.lang.String);
  public static long toEpochMilli(java.time.temporal.TemporalAccessor);
  public static java.time.Instant toInstant(java.time.temporal.TemporalAccessor);
  public static boolean isIn(java.time.temporal.TemporalAccessor, java.time.temporal.TemporalAccessor, java.time.temporal.TemporalAccessor);
  public static boolean isIn(java.time.temporal.TemporalAccessor, java.time.temporal.TemporalAccessor, java.time.temporal.TemporalAccessor, boolean, boolean);
}
```

## `cn.hutool.core.date.TemporalUtil`

```java
public class cn.hutool.core.date.TemporalUtil {
  public cn.hutool.core.date.TemporalUtil();
  public static java.time.Duration between(java.time.temporal.Temporal, java.time.temporal.Temporal);
  public static long between(java.time.temporal.Temporal, java.time.temporal.Temporal, java.time.temporal.ChronoUnit);
  public static java.time.temporal.ChronoUnit toChronoUnit(java.util.concurrent.TimeUnit) throws java.lang.IllegalArgumentException;
  public static java.util.concurrent.TimeUnit toTimeUnit(java.time.temporal.ChronoUnit) throws java.lang.IllegalArgumentException;
  public static <T extends java.time.temporal.Temporal> T offset(T, long, java.time.temporal.TemporalUnit);
  public static <T extends java.time.temporal.Temporal> T offset(T, java.time.DayOfWeek, boolean);
}
```

## `cn.hutool.core.date.TimeInterval`

```java
public class cn.hutool.core.date.TimeInterval extends cn.hutool.core.date.GroupTimeInterval {
  public cn.hutool.core.date.TimeInterval();
  public cn.hutool.core.date.TimeInterval(boolean);
  public long start();
  public long intervalRestart();
  public cn.hutool.core.date.TimeInterval restart();
  public long interval();
  public java.lang.String intervalPretty();
  public long intervalMs();
  public long intervalSecond();
  public long intervalMinute();
  public long intervalHour();
  public long intervalDay();
  public long intervalWeek();
}
```

## `cn.hutool.core.date.TimeZoneUtil`

```java
public class cn.hutool.core.date.TimeZoneUtil {
  public cn.hutool.core.date.TimeZoneUtil();
  public static java.util.TimeZone getTimeZone(java.lang.String);
  public static java.util.TimeZone toTimeZone(java.util.TimeZone);
}
```

## `cn.hutool.core.date.Week`

```java
public final class cn.hutool.core.date.Week extends java.lang.Enum<cn.hutool.core.date.Week> {
  public static cn.hutool.core.date.Week[] values();
  public static cn.hutool.core.date.Week valueOf(java.lang.String);
  public int getValue();
  public int getIso8601Value();
  public java.lang.String toChinese();
  public java.lang.String toChinese(java.lang.String);
  public java.time.DayOfWeek toJdkDayOfWeek();
  public static cn.hutool.core.date.Week of(int);
  public static cn.hutool.core.date.Week of(java.lang.String) throws java.lang.IllegalArgumentException;
  public static cn.hutool.core.date.Week of(java.time.DayOfWeek);
}
```

## `cn.hutool.core.date.YearQuarter`

```java
public final class cn.hutool.core.date.YearQuarter implements java.lang.Comparable<cn.hutool.core.date.YearQuarter>, java.io.Serializable {
  public static cn.hutool.core.date.YearQuarter of(int, int);
  public static cn.hutool.core.date.YearQuarter of(int, cn.hutool.core.date.Quarter);
  public static cn.hutool.core.date.YearQuarter of(java.time.LocalDate);
  public static cn.hutool.core.date.YearQuarter of(java.util.Date);
  public static cn.hutool.core.date.YearQuarter of(java.util.Calendar);
  public static cn.hutool.core.date.YearQuarter of(java.time.YearMonth);
  public static cn.hutool.core.date.YearQuarter now();
  public int getYear();
  public cn.hutool.core.date.Quarter getQuarter();
  public int getQuarterValue();
  public java.time.YearMonth firstYearMonth();
  public cn.hutool.core.date.Month firstMonth();
  public int firstMonthValue();
  public java.time.YearMonth lastYearMonth();
  public cn.hutool.core.date.Month lastMonth();
  public int lastMonthValue();
  public java.time.LocalDate firstDate();
  public java.time.LocalDate lastDate();
  public cn.hutool.core.date.YearQuarter plusQuarters(long);
  public cn.hutool.core.date.YearQuarter minusQuarters(long);
  public cn.hutool.core.date.YearQuarter nextQuarter();
  public cn.hutool.core.date.YearQuarter lastQuarter();
  public cn.hutool.core.date.YearQuarter plusYears(long);
  public cn.hutool.core.date.YearQuarter minusYears(long);
  public cn.hutool.core.date.YearQuarter nextYear();
  public cn.hutool.core.date.YearQuarter lastYear();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public int compareTo(cn.hutool.core.date.YearQuarter);
  public boolean isBefore(cn.hutool.core.date.YearQuarter);
  public boolean isAfter(cn.hutool.core.date.YearQuarter);
  public java.lang.String toString();
  public int compareTo(java.lang.Object);
}
```

## `cn.hutool.core.date.Zodiac`

```java
public class cn.hutool.core.date.Zodiac {
  public cn.hutool.core.date.Zodiac();
  public static java.lang.String getZodiac(java.util.Date);
  public static java.lang.String getZodiac(java.util.Calendar);
  public static java.lang.String getZodiac(cn.hutool.core.date.Month, int);
  public static java.lang.String getZodiac(int, int);
  public static java.lang.String getChineseZodiac(java.util.Date);
  public static java.lang.String getChineseZodiac(java.util.Calendar);
  public static java.lang.String getChineseZodiac(int);
}
```

## `cn.hutool.core.date.ZoneUtil`

```java
public class cn.hutool.core.date.ZoneUtil {
  public cn.hutool.core.date.ZoneUtil();
  public static java.util.TimeZone toTimeZone(java.time.ZoneId);
  public static java.time.ZoneId toZoneId(java.util.TimeZone);
}
```
