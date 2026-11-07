# cn.hutool.core.date.chinese

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.date.chinese.ChineseMonth` | `String getChineseMonthName(boolean isLeapMonth,int month,boolean isTraditional)` | 获得农历月称呼 当为传统表示时，表示为二月，腊月，或者润正月等 当为非传统表示时，二月，十二月，或者润一月等 |
| `cn.hutool.core.date.chinese.ChineseMonth` | `boolean isLeapMonth(int year,int month)` | 当前农历月份是否为闰月 |
| `cn.hutool.core.date.chinese.GanZhi` | `String cyclicalm(int num)` | 传入 月日的offset 传回干支, 0=甲子 |
| `cn.hutool.core.date.chinese.GanZhi` | `String getGanzhiOfDay(int year,int month,int day)` | 获取干支日 |
| `cn.hutool.core.date.chinese.GanZhi` | `String getGanzhiOfMonth(int year,int month,int day)` | 获取干支月 |
| `cn.hutool.core.date.chinese.GanZhi` | `String getGanzhiOfYear(int year)` | 传入年传回干支 |
| `cn.hutool.core.date.chinese.LunarFestival` | `List<String> getFestivals(int month,int day)` | 获得节日列表，此方法无法判断月是否为大月或小月 |
| `cn.hutool.core.date.chinese.LunarFestival` | `List<String> getFestivals(int year,int month,int day)` | 获得节日列表 |
| `cn.hutool.core.date.chinese.LunarInfo` | `int leapDays(int y)` | 传回农历 y年闰月的天数，如果本年无闰月，返回0，区分大小月 |
| `cn.hutool.core.date.chinese.LunarInfo` | `int leapMonth(int y)` | 传回农历 y年闰哪个月 1-12 , 没闰传回 0 此方法会返回润N月中的N，如二月、闰二月都返回2 |
| `cn.hutool.core.date.chinese.LunarInfo` | `int monthDays(int y,int m)` | 传回农历 y年m月的总天数，区分大小月 |
| `cn.hutool.core.date.chinese.LunarInfo` | `int yearDays(int y)` | 传回农历 y年的总天数 |
| `cn.hutool.core.date.chinese.SolarTerms` | `String getTerm(ChineseDate chineseDate)` | 根据农历日期获取节气 |
| `cn.hutool.core.date.chinese.SolarTerms` | `String getTerm(Date date)` | 根据日期获取节气 |
| `cn.hutool.core.date.chinese.SolarTerms` | `String getTerm(LocalDate date)` | 根据日期获取节气 |
| `cn.hutool.core.date.chinese.SolarTerms` | `String getTerm(int year,int mouth,int day)` | 根据年月日获取节气 |
| `cn.hutool.core.date.chinese.SolarTerms` | `int getTerm(int y,int n)` | 传入公历y年获得该年第n个节气的公历日期 |
