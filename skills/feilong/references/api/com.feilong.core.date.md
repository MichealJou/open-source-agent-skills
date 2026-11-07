# com.feilong.core.date

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.core.date.DateUtil`

```java
public final class com.feilong.core.date.DateUtil {
  public static java.util.Date now();
  public static java.lang.String nowString(java.lang.String);
  public static java.lang.String nowTimestamp();
  public static long nowTime();
  public static java.util.Date getFirstDateOfThisDay(java.util.Date);
  public static java.util.Date getFirstDateOfToday();
  public static java.util.Date getFirstDateOfYesterday();
  public static java.util.Date getFirstDateOfTomorrow();
  public static java.util.Date getLastDateOfThisDay(java.util.Date);
  public static java.util.Date getLastDateOfYesterday();
  public static java.util.Date getLastDateOfTomorrow();
  public static java.util.Date getLastDateOfToday();
  public static java.util.Date getFirstDateOfThisWeek(java.util.Date);
  public static java.util.Date getLastDateOfThisWeek(java.util.Date);
  public static java.util.Date getFirstDateOfThisMonth(java.util.Date);
  public static java.util.Date getLastDateOfThisMonth(java.util.Date);
  public static java.util.Date getFirstDateOfThisYear(java.util.Date);
  public static java.util.Date getLastDateOfThisYear(java.util.Date);
  public static java.util.Date addYear(java.util.Date, int);
  public static java.util.Date addMonth(java.util.Date, int);
  public static java.util.Date addDay(java.util.Date, int);
  public static java.util.Date addWeek(java.util.Date, int);
  public static java.util.Date addHour(java.util.Date, int);
  public static java.util.Date addMinute(java.util.Date, int);
  public static java.util.Date addSecond(java.util.Date, int);
  public static java.util.Date addMillisecond(java.util.Date, int);
  public static int getYear(java.util.Date);
  public static int getMonth(java.util.Date);
  public static int getWeekOfYear(java.util.Date);
  public static int getDayOfYear(java.util.Date);
  public static int getDayOfMonth(java.util.Date);
  public static int getDayOfWeek(java.util.Date);
  public static int getHourOfYear(java.util.Date);
  public static int getHourOfDay(java.util.Date);
  public static int getMinute(java.util.Date);
  public static int getSecond(java.util.Date);
  public static int getSecondOfDay(java.util.Date);
  public static int getSecondOfHour(java.util.Date);
  public static java.lang.Long getTime(java.util.Date);
  public static java.lang.String toString(java.util.Date, java.lang.String);
  public static java.lang.String toString(java.lang.String, java.lang.String, java.lang.String);
  public static java.util.Date toDate(java.lang.String, java.lang.String...);
  public static java.util.Date toDate(java.lang.Long);
  public static java.util.Date toDate(java.lang.String);
  public static boolean isBefore(java.util.Date, java.util.Date);
  public static boolean isAfter(java.util.Date, java.util.Date);
  public static boolean isInTime(java.lang.String, java.lang.String, java.lang.String);
  public static boolean isInTime(java.util.Date, java.lang.String, java.lang.String, java.lang.String);
  public static boolean isInTime(java.util.Date, java.util.Date, java.util.Date);
  public static boolean isNotInTime(java.lang.String, java.lang.String, java.lang.String);
  public static boolean isNotInTime(java.util.Date, java.lang.String, java.lang.String, java.lang.String);
  public static boolean isNotInTime(java.util.Date, java.util.Date, java.util.Date);
  public static boolean isToday(java.util.Date);
  public static boolean isEquals(java.util.Date, java.util.Date, java.lang.String);
  public static boolean isLeapYear(int);
  public static com.feilong.lib.lang3.tuple.Pair<java.util.Date, java.util.Date> getTodayStartAndEndPair();
  public static com.feilong.lib.lang3.tuple.Pair<java.util.Date, java.util.Date> getYesterdayStartAndEndPair();
  public static com.feilong.lib.lang3.tuple.Pair<java.util.Date, java.util.Date> getDayStartAndEndPair(java.util.Date);
  public static com.feilong.lib.lang3.tuple.Pair<java.util.Date, java.util.Date> getMonthStartAndEndPair();
  public static com.feilong.lib.lang3.tuple.Pair<java.util.Date, java.util.Date> getMonthStartAndEndPair(java.util.Date);
  public static com.feilong.lib.lang3.tuple.Pair<java.util.Date, java.util.Date> getYearStartAndEndPair();
  public static com.feilong.lib.lang3.tuple.Pair<java.util.Date, java.util.Date> getYearStartAndEndPair(java.util.Date);
  public static java.lang.String formatDurationUseBeginTimeMillis(long);
  public static java.lang.String formatElapsedTime(long);
  public static java.lang.String formatDuration(java.util.Date);
  public static java.lang.String formatDuration(java.util.Date, java.util.Date);
  public static java.lang.String formatDuration(long);
  public static int getIntervalMonth(java.util.Date, java.util.Date);
  public static int getIntervalWeek(java.util.Date, java.util.Date);
  public static int getIntervalDay(java.util.Date, java.util.Date);
  public static int getIntervalHour(java.util.Date, java.util.Date);
  public static int getIntervalMinute(java.util.Date, java.util.Date);
  public static int getIntervalSecond(java.util.Date, java.util.Date);
  public static long getIntervalTime(java.util.Date, java.util.Date);
}
```
