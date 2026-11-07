# com.feilong.core.date

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.core.date.DateUtil` | `Date addDay(Date date,int day)` | 指定日期 date 加减天数. |
| `com.feilong.core.date.DateUtil` | `Date addHour(Date date,int hour)` | 指定日期 date 加减小时. |
| `com.feilong.core.date.DateUtil` | `Date addMillisecond(Date date,int millisecond)` | 指定日期 date 加减毫秒. |
| `com.feilong.core.date.DateUtil` | `Date addMinute(Date date,int minute)` | 指定日期 date 加减分钟. |
| `com.feilong.core.date.DateUtil` | `Date addMonth(Date date,int month)` | 指定日期 date 加减月份. |
| `com.feilong.core.date.DateUtil` | `Date addSecond(Date date,int second)` | 指定日期 date 加减秒. |
| `com.feilong.core.date.DateUtil` | `Date addWeek(Date date,int week)` | 指定日期 date 加减星期 . |
| `com.feilong.core.date.DateUtil` | `Date addYear(Date date,int year)` | 指定日期 date ,加减年份. |
| `com.feilong.core.date.DateUtil` | `Date getFirstDateOfThisDay(Date date)` | 获得指定日期 date 的 00:00:00.000 时间. |
| `com.feilong.core.date.DateUtil` | `Date getFirstDateOfThisMonth(Date date)` | 获得指定日期 date 所在月的第一天, 00:00:00.000 到毫秒. |
| `com.feilong.core.date.DateUtil` | `Date getFirstDateOfThisWeek(Date date)` | 获得指定日期所在的 星期第一天(周日) 00:00:00.000 到毫秒. |
| `com.feilong.core.date.DateUtil` | `Date getFirstDateOfThisYear(Date date)` | 获得指定日期 date 所在年的第一天 , 00:00:00.000 到毫秒. |
| `com.feilong.core.date.DateUtil` | `Date getFirstDateOfToday()` | 获得今天的 00:00:00.000 时间. |
| `com.feilong.core.date.DateUtil` | `Date getFirstDateOfTomorrow()` | 获得明天的 00:00:00.000 时间. |
| `com.feilong.core.date.DateUtil` | `Date getFirstDateOfYesterday()` | 获得昨天的 00:00:00.000 时间. |
| `com.feilong.core.date.DateUtil` | `Date getLastDateOfThisDay(Date date)` | 获得指定日期 date 的 23:59:59.999 时间. |
| `com.feilong.core.date.DateUtil` | `Date getLastDateOfThisMonth(Date date)` | 获得指定日期 date 所在月的最后一天 , 23:59:59.999 到毫秒. 以指定日期 date 月的实际天数为准,也就是说,2月会 自动区分闰年 是28天还是29天 |
| `com.feilong.core.date.DateUtil` | `Date getLastDateOfThisWeek(Date date)` | 获得指定日期所在 星期的最后一天(周六) 23:59:59.999 到毫秒. |
| `com.feilong.core.date.DateUtil` | `Date getLastDateOfThisYear(Date date)` | 获得指定日期 date 所在年的最后一天 23:59:59.999 到毫秒. |
| `com.feilong.core.date.DateUtil` | `Date getLastDateOfToday()` | 获得今天的 23:59:59.999 时间. |
| `com.feilong.core.date.DateUtil` | `Date getLastDateOfTomorrow()` | 获得明天的 23:59:59.999 时间. |
| `com.feilong.core.date.DateUtil` | `Date getLastDateOfYesterday()` | 获得昨天的 23:59:59.999 时间. |
| `com.feilong.core.date.DateUtil` | `Date now()` | 此时此刻的 Date. 使用静态导入 static import,开发效率要高于自己写 new Date() |
| `com.feilong.core.date.DateUtil` | `Date toDate(Long time)` | 将 time 使用 new Date 成date类型. |
| `com.feilong.core.date.DateUtil` | `Date toDate(String dateString)` | 将时间字符串 dateString 使用 DatePattern#COMMON_DATE 默认模式转换成date类型. |
| `com.feilong.core.date.DateUtil` | `Date toDate(String dateString,String... datePatterns)` | 将时间字符串 dateString 使用 一个或者多个 不同的 datePattern 模式按照顺序转换成date类型. |
| `com.feilong.core.date.DateUtil` | `Long getTime(Date date)` | 返回自 1970年1月1 日 00:00:00 GMT 以来,此 Date 对象表示的 毫秒 数. |
| `com.feilong.core.date.DateUtil` | `Pair<Date, Date> getDayStartAndEndPair(Date date)` | 获得 指定日的开始时间 00:00:00.000 及指定日的结束时间 23:59:59.999 . 一般用于统计指定日期数据,between ... and ... |
| `com.feilong.core.date.DateUtil` | `Pair<Date, Date> getMonthStartAndEndPair()` | 获得 当前月的开始时间 00:00:00.000 及当前月结束时间 23:59:59.999 . 一般用于统计当前月的数据,between ... and ... |
| `com.feilong.core.date.DateUtil` | `Pair<Date, Date> getMonthStartAndEndPair(Date date)` | 获得 指定月的开始时间 00:00:00.000 及指定月的结束时间 23:59:59.999 . 一般用于统计指定月数据,between ... and ... |
| `com.feilong.core.date.DateUtil` | `Pair<Date, Date> getTodayStartAndEndPair()` | 获得 今天的开始时间 00:00:00.000 及今天的结束时间 23:59:59.999 . 一般用于统计当天数据,between ... and ... |
| `com.feilong.core.date.DateUtil` | `Pair<Date, Date> getYearStartAndEndPair()` | 获得 当前年的开始时间 00:00:00.000 及当前年的结束时间 23:59:59.999 . 一般用于统计当前年数据,between ... and ... |
| `com.feilong.core.date.DateUtil` | `Pair<Date, Date> getYearStartAndEndPair(Date date)` | 获得 指定年的开始时间 00:00:00.000 及指定年的结束时间 23:59:59.999 . 一般用于统计指定年数据,between ... and ... |
| `com.feilong.core.date.DateUtil` | `Pair<Date, Date> getYesterdayStartAndEndPair()` | 获得 昨天的开始时间 00:00:00.000 及昨天的结束时间 23:59:59.999 . 一般用于统计昨天数据,between ... and ... |
| `com.feilong.core.date.DateUtil` | `String formatDuration(Date beginDate)` | 将开始时间 beginDate 到当前时间 now() ,两日期之间的 绝对值 间隔,格式化成直观的表示方式. |
| `com.feilong.core.date.DateUtil` | `String formatDuration(Date beginDate,Date endDate)` | 将 beginDate 和 endDate 两日期之间的 绝对值 间隔,格式化成直观的表示方式. |
| `com.feilong.core.date.DateUtil` | `String formatDuration(long spaceMilliseconds)` | 将间隔毫秒数 spaceMilliseconds ,格式化成直观的表示方式. |
| `com.feilong.core.date.DateUtil` | `String formatDurationUseBeginTimeMillis(long beginTimeMillis)` | 将开始时间 beginTimeMillis 到当前时间 System.currentTimeMillis() ,两日期之间的 绝对值 间隔,格式化成直观的表示方式. |
| `com.feilong.core.date.DateUtil` | `String formatElapsedTime(long beginTimeMillis)` | 将开始时间 beginTimeMillis 到当前时间 System.currentTimeMillis() ,两日期之间的 绝对值 间隔,格式化成直观的表示方式. |
| `com.feilong.core.date.DateUtil` | `String nowString(String datePattern)` | 将此时此刻转成时间字符串. |
| `com.feilong.core.date.DateUtil` | `String nowTimestamp()` | 将此时此刻转成 TIMESTAMP 时间字符串,(常用于生成文件名字). |
| `com.feilong.core.date.DateUtil` | `String toString(Date date,String datePattern)` | 将指定日期 date 转换成特殊格式 datePattern 的字符串. |
| `com.feilong.core.date.DateUtil` | `String toString(String dateString,String oldPattern,String newPattern)` | 将一个 oldPattern 格式日期 dateString 字符串 使用新格式 newPattern 转成新的字符串. |
| `com.feilong.core.date.DateUtil` | `boolean isAfter(Date date,Date whenDate)` | 判断指定日期 date 是否在 whenDate 时间之后. |
| `com.feilong.core.date.DateUtil` | `boolean isBefore(Date date,Date whenDate)` | 判断指定日期 date 是否 在 whenDate 时间之前. |
| `com.feilong.core.date.DateUtil` | `boolean isEquals(Date date1,Date date2,String datePattern)` | 在相同格式下 datePattern ,将两个日期转成字符串判断是否相等. |
| `com.feilong.core.date.DateUtil` | `boolean isInTime(Date date,Date beginDate,Date endDate)` | 判断指定日期 date 是否在 beginDate 和 endDate 两个时间之间. 判断逻辑 date>=beginDate &&date |
| `com.feilong.core.date.DateUtil` | `boolean isInTime(Date date,String beginDateString,String endDateString,String datePattern)` | 判断指定时间 date , 是否在格式是 pattern 的 beginDate 和 endDate 两个时间之间. 判断逻辑 date>=beginDate &&date |
| `com.feilong.core.date.DateUtil` | `boolean isInTime(String beginDateString,String endDateString,String datePattern)` | 判断当前时间 是否在格式是 pattern 的 beginDate 和 endDate 两个时间之间. 判断逻辑 date>=beginDate &&date |
| `com.feilong.core.date.DateUtil` | `boolean isLeapYear(int year)` | 判断指定年 year 是否为闰年 . 规则: (year % 4 == 0 && year % 100 != 0) \|\| year % 400 == 0 |
| `com.feilong.core.date.DateUtil` | `boolean isNotInTime(Date date,Date beginDate,Date endDate)` | 判断指定日期 date 不在 beginDate 和 endDate 两个时间之间. |
| `com.feilong.core.date.DateUtil` | `boolean isNotInTime(Date date,String beginDateString,String endDateString,String datePattern)` | 判断指定时间 date , 不在格式是 pattern 的 beginDate 和 endDate 两个时间之间. |
| `com.feilong.core.date.DateUtil` | `boolean isNotInTime(String beginDateString,String endDateString,String datePattern)` | 判断当前时间 不在 pattern 的 beginDate 和 endDate 两个时间之间. |
| `com.feilong.core.date.DateUtil` | `boolean isToday(Date date)` | 判断指定的日期 date ,是不是今天的日期. |
| `com.feilong.core.date.DateUtil` | `int getDayOfMonth(Date date)` | 获得指定日期 date 是当前月的几号. |
| `com.feilong.core.date.DateUtil` | `int getDayOfWeek(Date date)` | 获得指定日期 date 在当前星期是星期几 . |
| `com.feilong.core.date.DateUtil` | `int getDayOfYear(Date date)` | 获得指定日期 date 是当年中的第几天. |
| `com.feilong.core.date.DateUtil` | `int getHourOfDay(Date date)` | 获得指定日期 date 中的 小时 (24小时制). |
| `com.feilong.core.date.DateUtil` | `int getHourOfYear(Date date)` | 获得指定日期 date 在它 一年中的小时数 . max value: 8784. |
| `com.feilong.core.date.DateUtil` | `int getIntervalDay(Date date1,Date date2)` | 计算两个时间相差的的天数( 绝对值 ). |
| `com.feilong.core.date.DateUtil` | `int getIntervalHour(Date date1,Date date2)` | 两个时间相差的的小时数( 绝对值 ). |
| `com.feilong.core.date.DateUtil` | `int getIntervalMinute(Date date1,Date date2)` | 两个时间相差的分钟( 绝对值 ). |
| `com.feilong.core.date.DateUtil` | `int getIntervalMonth(Date date1,Date date2)` | 获得相差的月数( 绝对值 ). |
| `com.feilong.core.date.DateUtil` | `int getIntervalSecond(Date date1,Date date2)` | 两个时间相差的秒数( 绝对值 ). |
| `com.feilong.core.date.DateUtil` | `int getIntervalWeek(Date date1,Date date2)` | 获得相差的星期数( 绝对值 ). |
| `com.feilong.core.date.DateUtil` | `int getMinute(Date date)` | 获得指定日期 date 中的 分钟 . |
| `com.feilong.core.date.DateUtil` | `int getMonth(Date date)` | 获得指定日期 date 中的 月份 (已经+1处理) . |
| `com.feilong.core.date.DateUtil` | `int getSecond(Date date)` | 获得指定日期 date 中的 秒 . |
| `com.feilong.core.date.DateUtil` | `int getSecondOfDay(Date date)` | 获得指定日期 date 在 当天中的秒数 ,最大值86400. |
| `com.feilong.core.date.DateUtil` | `int getSecondOfHour(Date date)` | 获得指定日期 date 在 当前小时中的秒数 ,最大值3600 TimeInterval#SECONDS_PER_HOUR. |
| `com.feilong.core.date.DateUtil` | `int getWeekOfYear(Date date)` | 指定日期 date 年中的 星期数 . |
| `com.feilong.core.date.DateUtil` | `int getYear(Date date)` | 获得指定日期 date 中的 年份 . |
| `com.feilong.core.date.DateUtil` | `long getIntervalTime(Date date1,Date date2)` | 两个时间相差的 毫秒数 ( 绝对值 ). |
| `com.feilong.core.date.DateUtil` | `long nowTime()` | 将 自 1970年1月1 日 00:00:00 GMT 以来,此 此时此刻 对象表示的毫秒数. |
