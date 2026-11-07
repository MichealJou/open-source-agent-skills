# cn.hutool.core.date.chinese

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.date.chinese.ChineseMonth`

```java
public class cn.hutool.core.date.chinese.ChineseMonth {
  public cn.hutool.core.date.chinese.ChineseMonth();
  public static boolean isLeapMonth(int, int);
  public static java.lang.String getChineseMonthName(boolean, int, boolean);
}
```

## `cn.hutool.core.date.chinese.GanZhi`

```java
public class cn.hutool.core.date.chinese.GanZhi {
  public cn.hutool.core.date.chinese.GanZhi();
  public static java.lang.String cyclicalm(int);
  public static java.lang.String getGanzhiOfYear(int);
  public static java.lang.String getGanzhiOfMonth(int, int, int);
  public static java.lang.String getGanzhiOfDay(int, int, int);
}
```

## `cn.hutool.core.date.chinese.LunarFestival`

```java
public class cn.hutool.core.date.chinese.LunarFestival {
  public cn.hutool.core.date.chinese.LunarFestival();
  public static java.util.List<java.lang.String> getFestivals(int, int, int);
  public static java.util.List<java.lang.String> getFestivals(int, int);
}
```

## `cn.hutool.core.date.chinese.LunarInfo`

```java
public class cn.hutool.core.date.chinese.LunarInfo {
  public cn.hutool.core.date.chinese.LunarInfo();
  public static int yearDays(int);
  public static int leapDays(int);
  public static int monthDays(int, int);
  public static int leapMonth(int);
}
```

## `cn.hutool.core.date.chinese.SolarTerms`

```java
public class cn.hutool.core.date.chinese.SolarTerms {
  public cn.hutool.core.date.chinese.SolarTerms();
  public static int getTerm(int, int);
  public static java.lang.String getTerm(java.util.Date);
  public static java.lang.String getTerm(cn.hutool.core.date.ChineseDate);
  public static java.lang.String getTerm(java.time.LocalDate);
  public static java.lang.String getTerm(int, int, int);
}
```
