# cn.hutool.core.date

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.date.BetweenFormatter` | `BetweenFormatter setLevelFormatter(Function<Level, String> levelFormatter)` | 设置级别格式化器 |
| `cn.hutool.core.date.BetweenFormatter` | `BetweenFormatter setSeparator(String separator)` | 设置分隔符 |
| `cn.hutool.core.date.BetweenFormatter` | `Level getLevel()` | 获得 格式化级别 |
| `cn.hutool.core.date.BetweenFormatter` | `String format()` | 格式化日期间隔输出 |
| `cn.hutool.core.date.BetweenFormatter` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.BetweenFormatter` | `long getBetweenMs()` | 获得 时长毫秒数 |
| `cn.hutool.core.date.BetweenFormatter` | `void setBetweenMs(long betweenMs)` | 设置 时长毫秒数 |
| `cn.hutool.core.date.BetweenFormatter` | `void setLevel(Level level)` | 设置格式化级别 |
| `cn.hutool.core.date.BetweenFormatter$Level` | `String getName()` | 获取级别名称 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar beginOfDay(Calendar calendar)` | 修改某天的开始时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar beginOfHour(Calendar calendar)` | 修改某小时的开始时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar beginOfMinute(Calendar calendar)` | 修改某分钟的开始时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar beginOfMonth(Calendar calendar)` | 修改某月的开始时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar beginOfQuarter(Calendar calendar)` | 修改某季度的开始时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar beginOfSecond(Calendar calendar)` | 修改秒级别的开始时间，即忽略毫秒部分 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar beginOfWeek(Calendar calendar)` | 修改给定日期当前周的开始时间，周一定为一周的开始时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar beginOfWeek(Calendar calendar,boolean isMondayAsFirstDay)` | 修改给定日期当前周的开始时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar beginOfYear(Calendar calendar)` | 修改某年的开始时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar calendar()` | 创建Calendar对象，时间为默认时区的当前时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar calendar(Calendar calendar,final TimeZone timeZone)` | 转换为指定时区的Calendar，返回新的Calendar |
| `cn.hutool.core.date.CalendarUtil` | `Calendar calendar(Date date)` | 转换为Calendar对象 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar calendar(long millis)` | 转换为Calendar对象，使用当前默认时区 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar calendar(long millis,TimeZone timeZone)` | 转换为Calendar对象 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar ceiling(Calendar calendar,DateField dateField)` | 修改日期为某个时间字段结束时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar ceiling(Calendar calendar,DateField dateField,boolean truncateMillisecond)` | 修改日期为某个时间字段结束时间 可选是否归零毫秒。 有时候由于毫秒部分必须为0（如MySQL数据库中），因此在此加上选项。 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar endOfDay(Calendar calendar)` | 修改某天的结束时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar endOfHour(Calendar calendar)` | 修改某小时的结束时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar endOfMinute(Calendar calendar)` | 修改某分钟的结束时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar endOfMonth(Calendar calendar)` | 修改某月的结束时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar endOfQuarter(Calendar calendar)` | 获取某季度的结束时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar endOfSecond(Calendar calendar)` | 修改秒级别的结束时间，即毫秒设置为999 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar endOfWeek(Calendar calendar)` | 修改某周的结束时间，周日定为一周的结束 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar endOfWeek(Calendar calendar,boolean isSundayAsLastDay)` | 修改某周的结束时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar endOfYear(Calendar calendar)` | 修改某年的结束时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar parse(CharSequence str,boolean lenient,DateParser parser)` | 使用指定DateParser解析字符串为Calendar |
| `cn.hutool.core.date.CalendarUtil` | `Calendar parseByPatterns(String str,Locale locale,String... parsePatterns)` | 通过给定的日期格式解析日期时间字符串。 传入的日期格式会逐个尝试，直到解析成功，返回Calendar对象，否则抛出DateException异常。 方法来自：Apache Commons-Lang3 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar parseByPatterns(String str,Locale locale,boolean lenient,String... parsePatterns)` | 通过给定的日期格式解析日期时间字符串。 传入的日期格式会逐个尝试，直到解析成功，返回Calendar对象，否则抛出DateException异常。 方法来自：Apache Commons-Lang3 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar parseByPatterns(String str,String... parsePatterns)` | 通过给定的日期格式解析日期时间字符串。 传入的日期格式会逐个尝试，直到解析成功，返回Calendar对象，否则抛出DateException异常。 方法来自：Apache Commons-Lang3 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar round(Calendar calendar,DateField dateField)` | 修改日期为某个时间字段四舍五入时间 |
| `cn.hutool.core.date.CalendarUtil` | `Calendar truncate(Calendar calendar,DateField dateField)` | 修改日期为某个时间字段起始时间 |
| `cn.hutool.core.date.CalendarUtil` | `Instant toInstant(Calendar calendar)` | CalendarInstant对象 |
| `cn.hutool.core.date.CalendarUtil` | `LinkedHashSet<String> yearAndQuarter(long startDate,long endDate)` | 获得指定日期区间内的年份和季度 |
| `cn.hutool.core.date.CalendarUtil` | `LocalDateTime toLocalDateTime(Calendar calendar)` | Calendar 转换为 LocalDateTime，使用系统默认时区 |
| `cn.hutool.core.date.CalendarUtil` | `String formatChineseDate(Calendar calendar,boolean withTime)` | 将指定Calendar时间格式化为纯中文形式，比如： |
| `cn.hutool.core.date.CalendarUtil` | `String yearAndQuarter(Calendar cal)` | 获得指定日期年份和季度 格式：[20131]表示2013年第一季度 |
| `cn.hutool.core.date.CalendarUtil` | `boolean isAM(Calendar calendar)` | 是否为上午 |
| `cn.hutool.core.date.CalendarUtil` | `boolean isLastDayOfMonth(Calendar calendar)` | 是否为本月最后一天 |
| `cn.hutool.core.date.CalendarUtil` | `boolean isPM(Calendar calendar)` | 是否为下午 |
| `cn.hutool.core.date.CalendarUtil` | `boolean isSameDay(Calendar cal1,Calendar cal2)` | 比较两个日期是否为同一天 |
| `cn.hutool.core.date.CalendarUtil` | `boolean isSameInstant(Calendar date1,Calendar date2)` | 检查两个Calendar时间戳是否相同。 此方法检查两个Calendar的毫秒数时间戳是否相同。 |
| `cn.hutool.core.date.CalendarUtil` | `boolean isSameMonth(Calendar cal1,Calendar cal2)` | 比较两个日期是否为同一月 同一个月的意思是：ERA（公元）、year（年）、month（月）都一致。 |
| `cn.hutool.core.date.CalendarUtil` | `boolean isSameWeek(Calendar cal1,Calendar cal2,boolean isMon)` | 比较两个日期是否为同一周 |
| `cn.hutool.core.date.CalendarUtil` | `boolean isSameYear(final Calendar cal1,Calendar cal2)` | 比较两个日期是否为同一年 同一个年的意思是：ERA（公元）、year（年）都一致。 |
| `cn.hutool.core.date.CalendarUtil` | `int age(Calendar birthday,Calendar dateToCompare)` | 计算相对于dateToCompare的年龄，长用于计算指定生日在某年的年龄 |
| `cn.hutool.core.date.CalendarUtil` | `int compare(Calendar calendar1,Calendar calendar2)` | null安全的Calendar比较，null小于任何日期 |
| `cn.hutool.core.date.CalendarUtil` | `int getBeginValue(Calendar calendar,DateField dateField)` | 获取指定日期字段的最小值，例如分钟的最小值是0 |
| `cn.hutool.core.date.CalendarUtil` | `int getBeginValue(Calendar calendar,int dateField)` | 获取指定日期字段的最小值，例如分钟的最小值是0 |
| `cn.hutool.core.date.CalendarUtil` | `int getEndValue(Calendar calendar,DateField dateField)` | 获取指定日期字段的最大值，例如分钟的最大值是59 |
| `cn.hutool.core.date.CalendarUtil` | `int getEndValue(Calendar calendar,int dateField)` | 获取指定日期字段的最大值，例如分钟的最大值是59 |
| `cn.hutool.core.date.ChineseDate` | `Calendar getGregorianCalendar()` | 获取公历的Calendar |
| `cn.hutool.core.date.ChineseDate` | `Date getGregorianDate()` | 获取公历的Date |
| `cn.hutool.core.date.ChineseDate` | `String getChineseDay()` | 获得农历日 |
| `cn.hutool.core.date.ChineseDate` | `String getChineseMonth()` | 获得农历月份（中文，例如二月，十二月，或者润一月） |
| `cn.hutool.core.date.ChineseDate` | `String getChineseMonth(boolean isTraditional)` | 获得农历月份（中文，例如二月，十二月，或者润一月） |
| `cn.hutool.core.date.ChineseDate` | `String getChineseMonthName()` | 获得农历月称呼（中文，例如二月，腊月，或者润正月） |
| `cn.hutool.core.date.ChineseDate` | `String getChineseZodiac()` | 获得年份生肖 |
| `cn.hutool.core.date.ChineseDate` | `String getCyclical()` | 获得年的天干地支 |
| `cn.hutool.core.date.ChineseDate` | `String getCyclicalYMD()` | 干支纪年信息 |
| `cn.hutool.core.date.ChineseDate` | `String getFestivals()` | 获得节日，闰月不计入节日中 |
| `cn.hutool.core.date.ChineseDate` | `String getTerm()` | 获得节气 |
| `cn.hutool.core.date.ChineseDate` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.ChineseDate` | `String toStringNormal()` | 转换为标准的日期格式来表示农历日期，例如2020-01-13 如果存在闰月，显示闰月月份，如润二月显示2 |
| `cn.hutool.core.date.ChineseDate` | `boolean isLeapMonth()` | 当前农历月份是否为闰月 |
| `cn.hutool.core.date.ChineseDate` | `int getChineseYear()` | 获得农历年份 |
| `cn.hutool.core.date.ChineseDate` | `int getDay()` | 获取农历的日，从1开始计数 |
| `cn.hutool.core.date.ChineseDate` | `int getGregorianDay()` | 获取公历的日 |
| `cn.hutool.core.date.ChineseDate` | `int getGregorianMonth()` | 获取公历的月，从0开始计数 |
| `cn.hutool.core.date.ChineseDate` | `int getGregorianMonthBase1()` | 获取公历的月，从1开始计数 |
| `cn.hutool.core.date.ChineseDate` | `int getGregorianYear()` | 获取公历的年 |
| `cn.hutool.core.date.ChineseDate` | `int getMonth()` | 获取农历的月，从1开始计数 此方法返回实际的月序号，如一月是闰月，则一月返回1，润一月返回2 |
| `cn.hutool.core.date.DateBetween` | `DateBetween create(Date begin,Date end)` | 创建 在前的日期做为起始时间，在后的做为结束时间，间隔只保留绝对值正数 |
| `cn.hutool.core.date.DateBetween` | `DateBetween create(Date begin,Date end,boolean isAbs)` | 创建 在前的日期做为起始时间，在后的做为结束时间，间隔只保留绝对值正数 |
| `cn.hutool.core.date.DateBetween` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.DateBetween` | `String toString(BetweenFormatter.Level level)` | 格式化输出时间差 |
| `cn.hutool.core.date.DateBetween` | `String toString(DateUnit unit,BetweenFormatter.Level level)` | 格式化输出时间差 |
| `cn.hutool.core.date.DateBetween` | `long between(DateUnit unit)` | 判断两个日期相差的时长 返回 给定单位的时长差 |
| `cn.hutool.core.date.DateBetween` | `long betweenMonth(boolean isReset)` | 计算两个日期相差月数 在非重置情况下，如果起始日期的天大于结束日期的天，月数要少算1（不足1个月） |
| `cn.hutool.core.date.DateBetween` | `long betweenYear(boolean isReset)` | 计算两个日期相差年数 在非重置情况下，如果起始日期的月大于结束日期的月，年数要少算1（不足1年） |
| `cn.hutool.core.date.DateField` | `DateField of(int calendarPartIntValue)` | 将 Calendar相关值转换为DatePart枚举对象 |
| `cn.hutool.core.date.DateField` | `int getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.DateModifier` | `Calendar modify(Calendar calendar,int dateField,ModifyType modifyType)` | 修改日期 |
| `cn.hutool.core.date.DateModifier` | `Calendar modify(Calendar calendar,int dateField,ModifyType modifyType,boolean truncateMillisecond)` | 修改日期，取起始值或者结束值 可选是否归零毫秒。 在ModifyType#TRUNCATE模式下，毫秒始终要归零, 但是在ModifyType#CEILING和ModifyType#ROUND模式下， 有时候由于毫秒部分必须为0（如MySQL数据库中），因此在此加上选项。 |
| `cn.hutool.core.date.DatePattern` | `DateTimeFormatter createFormatter(String pattern)` | 创建并为 DateTimeFormatter 赋予默认时区和位置信息，默认值为系统默认值。 |
| `cn.hutool.core.date.DateTime` | `Calendar toCalendar()` | 转换为Calendar, 默认 Locale |
| `cn.hutool.core.date.DateTime` | `Calendar toCalendar(Locale locale)` | 转换为Calendar |
| `cn.hutool.core.date.DateTime` | `Calendar toCalendar(TimeZone zone)` | 转换为Calendar |
| `cn.hutool.core.date.DateTime` | `Calendar toCalendar(TimeZone zone,Locale locale)` | 转换为Calendar |
| `cn.hutool.core.date.DateTime` | `Date toJdkDate()` | 转换为 Date 考虑到很多框架（例如Hibernate）的兼容性，提供此方法返回JDK原生的Date对象 |
| `cn.hutool.core.date.DateTime` | `DateBetween between(Date date)` | 计算相差时长 |
| `cn.hutool.core.date.DateTime` | `DateTime now()` | 现在的时间 |
| `cn.hutool.core.date.DateTime` | `DateTime of(Calendar calendar)` | 转换 Calendar 为 DateTime |
| `cn.hutool.core.date.DateTime` | `DateTime of(Date date)` | 转换JDK date为 DateTime |
| `cn.hutool.core.date.DateTime` | `DateTime of(String dateStr,String format)` | 构造 |
| `cn.hutool.core.date.DateTime` | `DateTime of(long timeMillis)` | 转换时间戳为 DateTime |
| `cn.hutool.core.date.DateTime` | `DateTime offset(DateField datePart,int offset)` | 调整日期和时间 如果此对象为可变对象，返回自身，否则返回新对象，设置是否可变对象见#setMutable(boolean) |
| `cn.hutool.core.date.DateTime` | `DateTime offsetNew(DateField datePart,int offset)` | 调整日期和时间 返回调整后的新DateTime，不影响原对象 |
| `cn.hutool.core.date.DateTime` | `DateTime setField(DateField field,int value)` | 设置日期的某个部分 如果此对象为可变对象，返回自身，否则返回新对象，设置是否可变对象见#setMutable(boolean) |
| `cn.hutool.core.date.DateTime` | `DateTime setField(int field,int value)` | 设置日期的某个部分 如果此对象为可变对象，返回自身，否则返回新对象，设置是否可变对象见#setMutable(boolean) |
| `cn.hutool.core.date.DateTime` | `DateTime setFirstDayOfWeek(Week firstDayOfWeek)` | 设置一周的第一天 JDK的Calendar中默认一周的第一天是周日，Hutool中将此默认值设置为周一 设置一周的第一天主要影响#weekOfMonth()和#weekOfYear() 两个方法 |
| `cn.hutool.core.date.DateTime` | `DateTime setMinimalDaysInFirstWeek(int minimalDaysInFirstWeek)` | 设置第一周最少天数 |
| `cn.hutool.core.date.DateTime` | `DateTime setMutable(boolean mutable)` | 设置对象是否可变 如果为不可变对象，以下方法将返回新方法： DateTime#offset(DateField, int) DateTime#setField(DateField, int) DateTime#setField(int, int) 如果为不可变对象，DateTime#setTime(long)将抛出异常 |
| `cn.hutool.core.date.DateTime` | `DateTime setTimeZone(TimeZone timeZone)` | 设置时区 |
| `cn.hutool.core.date.DateTime` | `LocalDateTime toLocalDateTime()` | 转换为 LocalDateTime |
| `cn.hutool.core.date.DateTime` | `Month monthEnum()` | 获得月份 |
| `cn.hutool.core.date.DateTime` | `Quarter quarterEnum()` | 获得当前日期所属季度 |
| `cn.hutool.core.date.DateTime` | `String between(Date date,DateUnit unit,BetweenFormatter.Level formatLevel)` | 计算相差时长 |
| `cn.hutool.core.date.DateTime` | `String toDateStr()` | 转为"yyyy-MM-dd" 格式字符串 |
| `cn.hutool.core.date.DateTime` | `String toMsStr()` | @return 输出精确到毫秒的标准日期形式 |
| `cn.hutool.core.date.DateTime` | `String toString()` | 转为字符串，如果时区被设置，会转换为其时区对应的时间，否则转换为当前地点对应的时区 可以调用DateTime#setUseJdkToStringStyle(boolean) 方法自定义默认的风格 如果#useJdkToStringStyle为true，返回"EEE MMM dd HH:mm:ss zzz yyyy"格式， 如果为false，则返回"yyyy-MM-dd HH:mm:ss" |
| `cn.hutool.core.date.DateTime` | `String toString(DateFormat format)` | 转为字符串 |
| `cn.hutool.core.date.DateTime` | `String toString(DatePrinter format)` | 转为字符串 |
| `cn.hutool.core.date.DateTime` | `String toString(String format)` | 转为字符串 |
| `cn.hutool.core.date.DateTime` | `String toString(TimeZone timeZone)` | 转为"yyyy-MM-dd HH:mm:ss" 格式字符串 如果时区不为null，会转换为其时区对应的时间，否则转换为当前时间对应的时区 |
| `cn.hutool.core.date.DateTime` | `String toStringDefaultTimeZone()` | 转为"yyyy-MM-dd HH:mm:ss" 格式字符串 时区使用当前地区的默认时区 |
| `cn.hutool.core.date.DateTime` | `String toTimeStr()` | 转为"HH:mm:ss" 格式字符串 |
| `cn.hutool.core.date.DateTime` | `TimeZone getTimeZone()` | 获取时区 |
| `cn.hutool.core.date.DateTime` | `Timestamp toTimestamp()` | 转为Timestamp |
| `cn.hutool.core.date.DateTime` | `Week dayOfWeekEnum()` | 获得指定日期是星期几 |
| `cn.hutool.core.date.DateTime` | `Week getFirstDayOfWeek()` | 获得一周的第一天，默认为周一 |
| `cn.hutool.core.date.DateTime` | `ZoneId getZoneId()` | 获取时区ID |
| `cn.hutool.core.date.DateTime` | `boolean isAM()` | 是否为上午 |
| `cn.hutool.core.date.DateTime` | `boolean isAfter(Date date)` | 是否在给定日期之后 |
| `cn.hutool.core.date.DateTime` | `boolean isAfterOrEquals(Date date)` | 是否在给定日期之后或与给定日期相等 |
| `cn.hutool.core.date.DateTime` | `boolean isBefore(Date date)` | 是否在给定日期之前 |
| `cn.hutool.core.date.DateTime` | `boolean isBeforeOrEquals(Date date)` | 是否在给定日期之前或与给定日期相等 |
| `cn.hutool.core.date.DateTime` | `boolean isIn(Date beginDate,Date endDate)` | 当前日期是否在日期指定范围内 起始日期和结束日期可以互换 |
| `cn.hutool.core.date.DateTime` | `boolean isLastDayOfMonth()` | 是否为本月最后一天 |
| `cn.hutool.core.date.DateTime` | `boolean isLeapYear()` | 是否闰年 |
| `cn.hutool.core.date.DateTime` | `boolean isMutable()` | 对象是否可变 如果为不可变对象，以下方法将返回新方法： DateTime#offset(DateField, int) DateTime#setField(DateField, int) DateTime#setField(int, int) 如果为不可变对象，DateTime#setTime(long)将抛出异常 |
| `cn.hutool.core.date.DateTime` | `boolean isPM()` | 是否为下午 |
| `cn.hutool.core.date.DateTime` | `boolean isWeekend()` | 是否为周末，周末指周六或者周日 |
| `cn.hutool.core.date.DateTime` | `int dayOfMonth()` | 获得指定日期是这个日期所在月份的第几天，从1开始 |
| `cn.hutool.core.date.DateTime` | `int dayOfWeek()` | 获得指定日期是星期几，1表示周日，2表示周一 |
| `cn.hutool.core.date.DateTime` | `int dayOfWeekInMonth()` | 获得天所在的周是这个月的第几周 |
| `cn.hutool.core.date.DateTime` | `int dayOfYear()` | 获得指定日期是这个日期所在年份的第几天，从1开始 |
| `cn.hutool.core.date.DateTime` | `int getField(DateField field)` | 获得日期的某个部分 例如获得年的部分，则使用 getField(DatePart.YEAR) |
| `cn.hutool.core.date.DateTime` | `int getField(int field)` | 获得日期的某个部分 例如获得年的部分，则使用 getField(Calendar.YEAR) |
| `cn.hutool.core.date.DateTime` | `int getLastDayOfMonth()` | 获得本月的最后一天 |
| `cn.hutool.core.date.DateTime` | `int hour(boolean is24HourClock)` | 获得指定日期的小时数部分 |
| `cn.hutool.core.date.DateTime` | `int millisecond()` | 获得指定日期的毫秒数部分 |
| `cn.hutool.core.date.DateTime` | `int minute()` | 获得指定日期的分钟数部分 例如：10:04:15.250 =》 4 |
| `cn.hutool.core.date.DateTime` | `int month()` | 获得月份，从0开始计数 |
| `cn.hutool.core.date.DateTime` | `int monthBaseOne()` | 获取月，从1开始计数 |
| `cn.hutool.core.date.DateTime` | `int monthStartFromOne()` | 获得月份，从1开始计数 由于Calendar 中的月份按照0开始计数，导致某些需求容易误解，因此如果想用1表示一月，2表示二月则调用此方法 |
| `cn.hutool.core.date.DateTime` | `int quarter()` | 获得当前日期所属季度，从1开始计数 |
| `cn.hutool.core.date.DateTime` | `int second()` | 获得指定日期的秒数部分 |
| `cn.hutool.core.date.DateTime` | `int weekOfMonth()` | 获得指定日期是所在月份的第几周 此方法返回值与一周的第一天有关，比如： 2016年1月3日为周日，如果一周的第一天为周日，那这天是第二周（返回2） 如果一周的第一天为周一，那这天是第一周（返回1） |
| `cn.hutool.core.date.DateTime` | `int weekOfYear()` | 获得指定日期是所在年份的第几周 此方法返回值与一周的第一天有关，比如： 2016年1月3日为周日，如果一周的第一天为周日，那这天是第二周（返回2） 如果一周的第一天为周一，那这天是第一周（返回1） 跨年的那个星期得到的结果总是1 |
| `cn.hutool.core.date.DateTime` | `int year()` | 获得年的部分 |
| `cn.hutool.core.date.DateTime` | `java.sql.Date toSqlDate()` | 转为 java.sql.Date |
| `cn.hutool.core.date.DateTime` | `long between(Date date,DateUnit unit)` | 计算相差时长 |
| `cn.hutool.core.date.DateTime` | `void setTime(long time)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.DateTime` | `void setUseJdkToStringStyle(boolean customUseJdkToStringStyle)` | 设置全局的，是否使用Date默认的toString()格式 如果为true，则调用toString()时返回"EEE MMM dd HH:mm:ss zzz yyyy"格式， 如果为false，则返回"yyyy-MM-dd HH:mm:ss"， 默认为false |
| `cn.hutool.core.date.DateUnit` | `ChronoUnit toChronoUnit()` | 单位兼容转换，将DateUnit转换为对应的ChronoUnit |
| `cn.hutool.core.date.DateUnit` | `ChronoUnit toChronoUnit(DateUnit unit)` | 单位兼容转换，将DateUnit转换为对应的ChronoUnit |
| `cn.hutool.core.date.DateUnit` | `DateUnit of(ChronoUnit unit)` | 单位兼容转换，将ChronoUnit转换为对应的DateUnit |
| `cn.hutool.core.date.DateUnit` | `long getMillis()` | @return 单位对应的毫秒数 |
| `cn.hutool.core.date.DateUtil` | `DateRange range(Date start,Date end,final DateField unit)` | 创建日期范围生成器 |
| `cn.hutool.core.date.DateUtil` | `DateTime beginOfDay(Date date)` | 获取某天的开始时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime beginOfHour(Date date)` | 获取某小时的开始时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime beginOfMinute(Date date)` | 获取某分钟的开始时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime beginOfMonth(Date date)` | 获取某月的开始时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime beginOfQuarter(Date date)` | 获取某季度的开始时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime beginOfSecond(Date date)` | 获取秒级别的开始时间，即毫秒部分设置为0 |
| `cn.hutool.core.date.DateUtil` | `DateTime beginOfWeek(Date date)` | 获取某周的开始时间，周一定为一周的开始时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime beginOfWeek(Date date,boolean isMondayAsFirstDay)` | 获取某周的开始时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime beginOfYear(Date date)` | 获取某年的开始时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime ceiling(Date date,DateField dateField)` | 修改日期为某个时间字段结束时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime ceiling(Date date,DateField dateField,boolean truncateMillisecond)` | 修改日期为某个时间字段结束时间 可选是否归零毫秒。 有时候由于毫秒部分必须为0（如MySQL数据库中），因此在此加上选项。 |
| `cn.hutool.core.date.DateUtil` | `DateTime convertTimeZone(Date date,TimeZone timeZone)` | Date 转换时区 |
| `cn.hutool.core.date.DateUtil` | `DateTime convertTimeZone(Date date,ZoneId zoneId)` | Date 转换时区 |
| `cn.hutool.core.date.DateUtil` | `DateTime date()` | 当前时间，转换为DateTime对象 |
| `cn.hutool.core.date.DateUtil` | `DateTime date(Calendar calendar)` | Calendar类型时间转为DateTime 始终根据已有Calendar 产生新的DateTime对象 |
| `cn.hutool.core.date.DateUtil` | `DateTime date(Date date)` | Date类型时间转为DateTime 如果date本身为DateTime对象，则返回强转后的对象，否则新建一个DateTime对象 |
| `cn.hutool.core.date.DateUtil` | `DateTime date(TemporalAccessor temporalAccessor)` | TemporalAccessor类型时间转为DateTime 始终根据已有TemporalAccessor 产生新的DateTime对象 |
| `cn.hutool.core.date.DateUtil` | `DateTime date(long date)` | Long类型时间转为DateTime 只支持毫秒级别时间戳，如果需要秒级别时间戳，请自行×1000 |
| `cn.hutool.core.date.DateUtil` | `DateTime dateNew(Date date)` | 根据已有Date 产生新的DateTime对象 |
| `cn.hutool.core.date.DateUtil` | `DateTime dateSecond()` | 当前时间，转换为DateTime对象，忽略毫秒部分 |
| `cn.hutool.core.date.DateUtil` | `DateTime endOfDay(Date date)` | 获取某天的结束时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime endOfHour(Date date)` | 获取某小时的结束时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime endOfMinute(Date date)` | 获取某分钟的结束时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime endOfMonth(Date date)` | 获取某月的结束时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime endOfQuarter(Date date)` | 获取某季度的结束时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime endOfSecond(Date date)` | 获取秒级别的结束时间，即毫秒设置为999 |
| `cn.hutool.core.date.DateUtil` | `DateTime endOfWeek(Date date)` | 获取某周的结束时间，周日定为一周的结束 |
| `cn.hutool.core.date.DateUtil` | `DateTime endOfWeek(Date date,boolean isSundayAsLastDay)` | 获取某周的结束时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime endOfYear(Date date)` | 获取某年的结束时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime lastMonth()` | 上个月 |
| `cn.hutool.core.date.DateUtil` | `DateTime lastWeek()` | 上周 |
| `cn.hutool.core.date.DateUtil` | `DateTime nextMonth()` | 下个月 |
| `cn.hutool.core.date.DateUtil` | `DateTime nextWeek()` | 下周 |
| `cn.hutool.core.date.DateUtil` | `DateTime offset(Date date,DateField dateField,int offset)` | 获取指定日期偏移指定时间后的时间，生成的偏移日期不影响原日期 |
| `cn.hutool.core.date.DateUtil` | `DateTime offsetDay(Date date,int offset)` | 偏移天 |
| `cn.hutool.core.date.DateUtil` | `DateTime offsetHour(Date date,int offset)` | 偏移小时 |
| `cn.hutool.core.date.DateUtil` | `DateTime offsetMillisecond(Date date,int offset)` | 偏移毫秒数 |
| `cn.hutool.core.date.DateUtil` | `DateTime offsetMinute(Date date,int offset)` | 偏移分钟 |
| `cn.hutool.core.date.DateUtil` | `DateTime offsetMonth(Date date,int offset)` | 偏移月 |
| `cn.hutool.core.date.DateUtil` | `DateTime offsetSecond(Date date,int offset)` | 偏移秒数 |
| `cn.hutool.core.date.DateUtil` | `DateTime offsetWeek(Date date,int offset)` | 偏移周 |
| `cn.hutool.core.date.DateUtil` | `DateTime offsetYear(final Date date,final int offset)` | 偏移年 |
| `cn.hutool.core.date.DateUtil` | `DateTime parse(CharSequence dateCharSequence)` | 将日期字符串转换为DateTime对象，格式： yyyy-MM-dd HH:mm:ss yyyy/MM/dd HH:mm:ss yyyy.MM.dd HH:mm:ss yyyy年MM月dd日 HH时mm分ss秒 yyyy-MM-dd yyyy/MM/dd yyyy.MM.dd HH:mm:ss HH时mm分ss秒 yyyy-MM-dd HH:mm yyyy-MM-dd HH:mm:ss.SSS yyyy-MM-dd HH:mm:ss.SSSSSS yyyyMMddHHmmss yyyyMMddHHmmssSSS yyyyMMdd EEE, dd MMM yyyy HH:mm:ss z EEE … |
| `cn.hutool.core.date.DateUtil` | `DateTime parse(CharSequence dateStr,DateFormat dateFormat)` | 构建DateTime对象 |
| `cn.hutool.core.date.DateUtil` | `DateTime parse(CharSequence dateStr,DateParser parser)` | 构建DateTime对象 |
| `cn.hutool.core.date.DateUtil` | `DateTime parse(CharSequence dateStr,DateParser parser,boolean lenient)` | 构建DateTime对象 |
| `cn.hutool.core.date.DateUtil` | `DateTime parse(CharSequence dateStr,DateTimeFormatter formatter)` | 构建DateTime对象 |
| `cn.hutool.core.date.DateUtil` | `DateTime parse(CharSequence dateStr,String format)` | 将特定格式的日期转换为Date对象 |
| `cn.hutool.core.date.DateUtil` | `DateTime parse(CharSequence dateStr,String format,Locale locale)` | 将特定格式的日期转换为Date对象 |
| `cn.hutool.core.date.DateUtil` | `DateTime parse(String str,String... parsePatterns)` | 通过给定的日期格式解析日期时间字符串。 传入的日期格式会逐个尝试，直到解析成功，返回DateTime对象，否则抛出DateException异常。 |
| `cn.hutool.core.date.DateUtil` | `DateTime parseCST(CharSequence cstString)` | 解析CST时间，格式： EEE MMM dd HH:mm:ss z yyyy（例如：Wed Aug 01 00:00:00 CST 2012） |
| `cn.hutool.core.date.DateUtil` | `DateTime parseDate(CharSequence dateString)` | 解析日期字符串，忽略时分秒，支持的格式包括： |
| `cn.hutool.core.date.DateUtil` | `DateTime parseDateTime(CharSequence dateString)` | 解析日期时间字符串，格式支持： |
| `cn.hutool.core.date.DateUtil` | `DateTime parseISO8601(String iso8601String)` | 解析ISO8601时间，格式： yyyy-MM-dd'T'HH:mm:ss'Z' yyyy-MM-dd'T'HH:mm:ss.SSS'Z' yyyy-MM-dd'T'HH:mm:ssZ yyyy-MM-dd'T'HH:mm:ss.SSSZ yyyy-MM-dd'T'HH:mm:ss+0800 yyyy-MM-dd'T'HH:mm:ss+08:00 |
| `cn.hutool.core.date.DateUtil` | `DateTime parseRFC2822(CharSequence source)` | 解析RFC2822时间，格式： EEE MMM dd HH:mm:ss z yyyy（例如：Wed Aug 01 00:00:00 CST 2012） |
| `cn.hutool.core.date.DateUtil` | `DateTime parseTime(CharSequence timeString)` | 解析时间，格式HH:mm:ss，日期部分默认为1970-01-01 |
| `cn.hutool.core.date.DateUtil` | `DateTime parseTimeToday(CharSequence timeString)` | 解析时间，格式HH:mm 或 HH:mm:ss，日期默认为今天 |
| `cn.hutool.core.date.DateUtil` | `DateTime parseUTC(String utcString)` | 解析UTC时间，格式： yyyy-MM-dd'T'HH:mm:ss'Z' yyyy-MM-dd'T'HH:mm:ss.SSS'Z' yyyy-MM-dd'T'HH:mm:ssZ yyyy-MM-dd'T'HH:mm:ss.SSSZ yyyy-MM-dd'T'HH:mm:ss+0800 yyyy-MM-dd'T'HH:mm:ss+08:00 |
| `cn.hutool.core.date.DateUtil` | `DateTime round(Date date,DateField dateField)` | 修改日期为某个时间字段四舍五入时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime tomorrow()` | 明天 |
| `cn.hutool.core.date.DateUtil` | `DateTime truncate(Date date,DateField dateField)` | 修改日期为某个时间字段起始时间 |
| `cn.hutool.core.date.DateUtil` | `DateTime yesterday()` | 昨天 |
| `cn.hutool.core.date.DateUtil` | `Instant toInstant(Date date)` | Date对象转换为Instant对象 |
| `cn.hutool.core.date.DateUtil` | `Instant toInstant(TemporalAccessor temporalAccessor)` | Date对象转换为Instant对象 |
| `cn.hutool.core.date.DateUtil` | `LinkedHashSet<String> yearAndQuarter(Date startDate,Date endDate)` | 获得指定日期区间内的年份和季节 |
| `cn.hutool.core.date.DateUtil` | `List<DateTime> rangeContains(DateRange start,DateRange end)` | 俩个时间区间取交集 |
| `cn.hutool.core.date.DateUtil` | `List<DateTime> rangeNotContains(DateRange start,DateRange end)` | 俩个时间区间取差集(end - start) |
| `cn.hutool.core.date.DateUtil` | `List<DateTime> rangeToList(Date start,Date end,DateField unit)` | 根据步进单位获取起始日期时间和结束日期时间的时间区间集合 |
| `cn.hutool.core.date.DateUtil` | `List<DateTime> rangeToList(Date start,Date end,final DateField unit,int step)` | 根据步进单位和步进获取起始日期时间和结束日期时间的时间区间集合 |
| `cn.hutool.core.date.DateUtil` | `List<T> rangeFunc(Date start,Date end,final DateField unit,Function<Date, T> func)` | 按日期范围遍历，执行 function |
| `cn.hutool.core.date.DateUtil` | `LocalDateTime parseLocalDateTime(CharSequence dateStr)` | 构建LocalDateTime对象 格式：yyyy-MM-dd HH:mm:ss |
| `cn.hutool.core.date.DateUtil` | `LocalDateTime parseLocalDateTime(CharSequence dateStr,String format)` | 构建LocalDateTime对象 |
| `cn.hutool.core.date.DateUtil` | `LocalDateTime toLocalDateTime(Date date)` | Date 转换为 LocalDateTime，使用系统默认时区 |
| `cn.hutool.core.date.DateUtil` | `LocalDateTime toLocalDateTime(Instant instant)` | Instant 转换为 LocalDateTime，使用系统默认时区 |
| `cn.hutool.core.date.DateUtil` | `Month monthEnum(Date date)` | 获得月份 |
| `cn.hutool.core.date.DateUtil` | `Month thisMonthEnum()` | @return 当前月份 Month |
| `cn.hutool.core.date.DateUtil` | `Quarter quarterEnum(Date date)` | 获得指定日期所属季度 |
| `cn.hutool.core.date.DateUtil` | `SimpleDateFormat newSimpleFormat(String pattern)` | 创建SimpleDateFormat，注意此对象非线程安全！ 此对象默认为严格格式模式，即parse时如果格式不正确会报错。 |
| `cn.hutool.core.date.DateUtil` | `SimpleDateFormat newSimpleFormat(String pattern,Locale locale,TimeZone timeZone)` | 创建SimpleDateFormat，注意此对象非线程安全！ 此对象默认为严格格式模式，即parse时如果格式不正确会报错。 |
| `cn.hutool.core.date.DateUtil` | `StopWatch createStopWatch()` | 创建秒表StopWatch，用于对代码块的执行时间计数 使用方法如下： |
| `cn.hutool.core.date.DateUtil` | `StopWatch createStopWatch(String id)` | 创建秒表StopWatch，用于对代码块的执行时间计数 使用方法如下： |
| `cn.hutool.core.date.DateUtil` | `String format(Date date,DateFormat format)` | 根据特定格式格式化日期 |
| `cn.hutool.core.date.DateUtil` | `String format(Date date,DatePrinter format)` | 根据特定格式格式化日期 |
| `cn.hutool.core.date.DateUtil` | `String format(Date date,DateTimeFormatter format)` | 根据特定格式格式化日期 |
| `cn.hutool.core.date.DateUtil` | `String format(Date date,String format)` | 根据特定格式格式化日期 |
| `cn.hutool.core.date.DateUtil` | `String format(LocalDateTime localDateTime,String format)` | 根据特定格式格式化日期 |
| `cn.hutool.core.date.DateUtil` | `String formatBetween(Date beginDate,Date endDate)` | 格式化日期间隔输出，精确到毫秒 |
| `cn.hutool.core.date.DateUtil` | `String formatBetween(Date beginDate,Date endDate,BetweenFormatter.Level level)` | 格式化日期间隔输出 |
| `cn.hutool.core.date.DateUtil` | `String formatBetween(long betweenMs)` | 格式化日期间隔输出，精确到毫秒 |
| `cn.hutool.core.date.DateUtil` | `String formatBetween(long betweenMs,BetweenFormatter.Level level)` | 格式化日期间隔输出 |
| `cn.hutool.core.date.DateUtil` | `String formatChineseDate(Date date,boolean isUppercase,boolean withTime)` | 格式化为中文日期格式，如果isUppercase为false，则返回类似：2018年10月24日，否则返回二〇一八年十月二十四日 |
| `cn.hutool.core.date.DateUtil` | `String formatDate(Date date)` | 格式化日期部分（不包括时间） 格式 yyyy-MM-dd |
| `cn.hutool.core.date.DateUtil` | `String formatDateTime(Date date)` | 格式化日期时间 格式 yyyy-MM-dd HH:mm:ss |
| `cn.hutool.core.date.DateUtil` | `String formatHttpDate(Date date)` | 格式化为Http的标准日期格式 标准日期格式遵循RFC 1123规范，格式类似于：Fri, 31 Dec 1999 23:59:59 GMT |
| `cn.hutool.core.date.DateUtil` | `String formatLocalDateTime(LocalDateTime localDateTime)` | 格式化日期时间 格式 yyyy-MM-dd HH:mm:ss |
| `cn.hutool.core.date.DateUtil` | `String formatTime(Date date)` | 格式化时间 格式 HH:mm:ss |
| `cn.hutool.core.date.DateUtil` | `String getChineseZodiac(int year)` | 计算生肖，只计算1900年后出生的人 |
| `cn.hutool.core.date.DateUtil` | `String getShotName(TimeUnit unit)` | 获取时长单位简写 |
| `cn.hutool.core.date.DateUtil` | `String getZodiac(int month,int day)` | 通过生日计算星座 |
| `cn.hutool.core.date.DateUtil` | `String now()` | 当前时间，格式 yyyy-MM-dd HH:mm:ss |
| `cn.hutool.core.date.DateUtil` | `String secondToTime(int seconds)` | 秒数转为时间格式(HH:mm:ss) 参考： https://github.com/iceroot |
| `cn.hutool.core.date.DateUtil` | `String today()` | 当前日期，格式 yyyy-MM-dd |
| `cn.hutool.core.date.DateUtil` | `String yearAndQuarter(Date date)` | 获得指定日期年份和季节 格式：[20131]表示2013年第一季度 |
| `cn.hutool.core.date.DateUtil` | `TimeInterval timer()` | 计时器 计算某个过程花费的时间，精确到毫秒 |
| `cn.hutool.core.date.DateUtil` | `TimeInterval timer(boolean isNano)` | 计时器 计算某个过程花费的时间，精确到毫秒 |
| `cn.hutool.core.date.DateUtil` | `Week dayOfWeekEnum(Date date)` | 获得指定日期是星期几 |
| `cn.hutool.core.date.DateUtil` | `Week thisDayOfWeekEnum()` | @return 当前日期是星期几 Week |
| `cn.hutool.core.date.DateUtil` | `boolean isAM(Date date)` | 是否为上午 |
| `cn.hutool.core.date.DateUtil` | `boolean isExpired(Date startDate,Date endDate,Date checkDate)` | 判定在指定检查时间是否过期。 以商品为例，startDate即生产日期，endDate即保质期的截止日期，checkDate表示在何时检查是否过期（一般为当前时间） endDate和startDate的差值即为保质期（按照毫秒计），checkDate和startDate的差值即为实际经过的时长，实际时长大于保质期表示超时。 |
| `cn.hutool.core.date.DateUtil` | `boolean isExpired(Date startDate,DateField dateField,int timeLength,Date endDate)` | 判定给定开始时间经过某段时间后是否过期 |
| `cn.hutool.core.date.DateUtil` | `boolean isIn(Date date,Date beginDate,Date endDate)` | 当前日期是否在日期指定范围内 起始日期和结束日期可以互换 |
| `cn.hutool.core.date.DateUtil` | `boolean isLastDayOfMonth(Date date)` | 是否为本月最后一天 |
| `cn.hutool.core.date.DateUtil` | `boolean isLeapYear(int year)` | 是否闰年 |
| `cn.hutool.core.date.DateUtil` | `boolean isOverlap(Date realStartTime,Date realEndTime,Date startTime,Date endTime)` | 检查两个时间段是否有时间重叠 重叠指两个时间段是否有交集，注意此方法时间段重合时如： 此方法未纠正开始时间小于结束时间 当realStartTime和realEndTime或startTime和endTime相等时,退化为判断区间是否包含点 当realStartTime和realEndTime和startTime和endTime相等时,退化为判断点与点是否相等 See 准确的区间关系参考:艾伦区间代数 |
| `cn.hutool.core.date.DateUtil` | `boolean isPM(Date date)` | 是否为下午 |
| `cn.hutool.core.date.DateUtil` | `boolean isSameDay(final Date date1,final Date date2)` | 比较两个日期是否为同一天 |
| `cn.hutool.core.date.DateUtil` | `boolean isSameMonth(final Date date1,final Date date2)` | 比较两个日期是否为同一月 |
| `cn.hutool.core.date.DateUtil` | `boolean isSameTime(Date date1,Date date2)` | 是否为相同时间 此方法比较两个日期的时间戳是否相同 |
| `cn.hutool.core.date.DateUtil` | `boolean isSameWeek(final Date date1,final Date date2,boolean isMon)` | 比较两个日期是否为同一周 |
| `cn.hutool.core.date.DateUtil` | `boolean isWeekend(Date date)` | 是否为周末（周六或周日） |
| `cn.hutool.core.date.DateUtil` | `double nanosToSeconds(long duration)` | 纳秒转秒，保留小数 |
| `cn.hutool.core.date.DateUtil` | `int age(Date birthday,Date dateToCompare)` | 计算相对于dateToCompare的年龄，常用于计算指定生日在某年的年龄 |
| `cn.hutool.core.date.DateUtil` | `int ageOfNow(Date birthDay)` | 生日转为年龄，计算法定年龄 |
| `cn.hutool.core.date.DateUtil` | `int ageOfNow(String birthDay)` | 生日转为年龄，计算法定年龄 |
| `cn.hutool.core.date.DateUtil` | `int compare(Date date1,Date date2)` | null安全的日期比较，null对象排在末尾 |
| `cn.hutool.core.date.DateUtil` | `int compare(Date date1,Date date2,String format)` | null安全的日期比较，并只比较指定格式； null对象排在末尾, 并指定日期格式； |
| `cn.hutool.core.date.DateUtil` | `int dayOfMonth(Date date)` | 获得指定日期是这个日期所在月份的第几天 |
| `cn.hutool.core.date.DateUtil` | `int dayOfWeek(Date date)` | 获得指定日期是星期几，1表示周日，2表示周一 |
| `cn.hutool.core.date.DateUtil` | `int dayOfYear(Date date)` | 获得指定日期是这个日期所在年的第几天 |
| `cn.hutool.core.date.DateUtil` | `int getLastDayOfMonth(Date date)` | 获得本月的最后一天 |
| `cn.hutool.core.date.DateUtil` | `int hour(Date date,boolean is24HourClock)` | 获得指定日期的小时数部分 |
| `cn.hutool.core.date.DateUtil` | `int lengthOfMonth(int month,boolean isLeapYear)` | 获得指定月份的总天数 |
| `cn.hutool.core.date.DateUtil` | `int lengthOfYear(int year)` | 获得指定年份的总天数 |
| `cn.hutool.core.date.DateUtil` | `int millisecond(Date date)` | 获得指定日期的毫秒数部分 |
| `cn.hutool.core.date.DateUtil` | `int minute(Date date)` | 获得指定日期的分钟数部分 例如：10:04:15.250 =》 4 |
| `cn.hutool.core.date.DateUtil` | `int month(Date date)` | 获得月份，从0开始计数 |
| `cn.hutool.core.date.DateUtil` | `int quarter(Date date)` | 获得指定日期所属季度，从1开始计数 |
| `cn.hutool.core.date.DateUtil` | `int second(Date date)` | 获得指定日期的秒数部分 |
| `cn.hutool.core.date.DateUtil` | `int thisDayOfMonth()` | @return 当前日期是这个日期所在月份的第几天 |
| `cn.hutool.core.date.DateUtil` | `int thisDayOfWeek()` | @return 当前日期是星期几 |
| `cn.hutool.core.date.DateUtil` | `int thisHour(boolean is24HourClock)` | @param is24HourClock 是否24小时制 |
| `cn.hutool.core.date.DateUtil` | `int thisMillisecond()` | @return 当前日期的毫秒数部分 |
| `cn.hutool.core.date.DateUtil` | `int thisMinute()` | @return 当前日期的分钟数部分 |
| `cn.hutool.core.date.DateUtil` | `int thisMonth()` | @return 当前月份，从0开始计数 |
| `cn.hutool.core.date.DateUtil` | `int thisSecond()` | @return 当前日期的秒数部分 |
| `cn.hutool.core.date.DateUtil` | `int thisWeekOfMonth()` | @return 当前日期所在月份的第几周 |
| `cn.hutool.core.date.DateUtil` | `int thisWeekOfYear()` | @return 当前日期所在年份的第几周 |
| `cn.hutool.core.date.DateUtil` | `int thisYear()` | @return 今年 |
| `cn.hutool.core.date.DateUtil` | `int timeToSecond(String timeStr)` | HH:mm:ss 时间格式字符串转为秒数 参考： https://github.com/iceroot |
| `cn.hutool.core.date.DateUtil` | `int toIntSecond(Date date)` | 格式化成yyMMddHHmm后转换为int型 |
| `cn.hutool.core.date.DateUtil` | `int weekOfMonth(Date date)` | 获得指定日期是所在月份的第几周 |
| `cn.hutool.core.date.DateUtil` | `int weekOfYear(Date date)` | 获得指定日期是所在年份的第几周 此方法返回值与一周的第一天有关，比如： 2016年1月3日为周日，如果一周的第一天为周日，那这天是第二周（返回2） 如果一周的第一天为周一，那这天是第一周（返回1） 跨年的那个星期得到的结果总是1 |
| `cn.hutool.core.date.DateUtil` | `int year(Date date)` | 获得年的部分 |
| `cn.hutool.core.date.DateUtil` | `long between(Date beginDate,Date endDate,DateUnit unit)` | 判断两个日期相差的时长，只保留绝对值 |
| `cn.hutool.core.date.DateUtil` | `long between(Date beginDate,Date endDate,DateUnit unit,boolean isAbs)` | 判断两个日期相差的时长 |
| `cn.hutool.core.date.DateUtil` | `long betweenDay(Date beginDate,Date endDate,boolean isReset)` | 判断两个日期相差的天数 |
| `cn.hutool.core.date.DateUtil` | `long betweenMonth(Date beginDate,Date endDate,boolean isReset)` | 计算两个日期相差月数 在非重置情况下，如果起始日期的天大于结束日期的天，月数要少算1（不足1个月） |
| `cn.hutool.core.date.DateUtil` | `long betweenMs(Date beginDate,Date endDate)` | 判断两个日期相差的毫秒数 |
| `cn.hutool.core.date.DateUtil` | `long betweenWeek(Date beginDate,Date endDate,boolean isReset)` | 计算指定时间区间内的周数 |
| `cn.hutool.core.date.DateUtil` | `long betweenYear(Date beginDate,Date endDate,boolean isReset)` | 计算两个日期相差年数 在非重置情况下，如果起始日期的月大于结束日期的月，年数要少算1（不足1年） |
| `cn.hutool.core.date.DateUtil` | `long current()` | 当前时间的时间戳 |
| `cn.hutool.core.date.DateUtil` | `long currentSeconds()` | 当前时间的时间戳（秒） |
| `cn.hutool.core.date.DateUtil` | `long nanosToMillis(long duration)` | 纳秒转毫秒 |
| `cn.hutool.core.date.DateUtil` | `long spendMs(long preTime)` | 计时，常用于记录某段代码的执行时间，单位：毫秒 |
| `cn.hutool.core.date.DateUtil` | `long spendNt(long preTime)` | 计时，常用于记录某段代码的执行时间，单位：纳秒 |
| `cn.hutool.core.date.DateUtil` | `void rangeConsume(Date start,Date end,final DateField unit,Consumer<Date> consumer)` | 按日期范围遍历，执行 consumer |
| `cn.hutool.core.date.GroupTimeInterval` | `GroupTimeInterval clear()` | 清空所有定时记录 |
| `cn.hutool.core.date.GroupTimeInterval` | `String intervalPretty(String id)` | 从开始到当前的间隔时间（毫秒数），返回XX天XX小时XX分XX秒XX毫秒 |
| `cn.hutool.core.date.GroupTimeInterval` | `long interval(String id)` | 从开始到当前的间隔时间（毫秒数） 如果使用纳秒计时，返回纳秒差，否则返回毫秒差 如果分组下没有开始时间，返回null |
| `cn.hutool.core.date.GroupTimeInterval` | `long interval(String id,DateUnit dateUnit)` | 从开始到当前的间隔时间 |
| `cn.hutool.core.date.GroupTimeInterval` | `long intervalDay(String id)` | 从开始到当前的间隔天数，取绝对值 |
| `cn.hutool.core.date.GroupTimeInterval` | `long intervalHour(String id)` | 从开始到当前的间隔小时数，取绝对值 |
| `cn.hutool.core.date.GroupTimeInterval` | `long intervalMinute(String id)` | 从开始到当前的间隔分钟数，取绝对值 |
| `cn.hutool.core.date.GroupTimeInterval` | `long intervalMs(String id)` | 从开始到当前的间隔时间（毫秒数） |
| `cn.hutool.core.date.GroupTimeInterval` | `long intervalRestart(String id)` | 重新计时并返回从开始到当前的持续时间秒 如果此分组下没有记录，则返回0; |
| `cn.hutool.core.date.GroupTimeInterval` | `long intervalSecond(String id)` | 从开始到当前的间隔秒数，取绝对值 |
| `cn.hutool.core.date.GroupTimeInterval` | `long intervalWeek(String id)` | 从开始到当前的间隔周数，取绝对值 |
| `cn.hutool.core.date.GroupTimeInterval` | `long start(String id)` | 开始计时并返回当前时间 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `Duration between(LocalDateTime startTimeInclude,LocalDateTime endTimeExclude)` | 获取两个日期的差，如果结束时间早于开始时间，获取结果为负。 返回结果为Duration对象，通过调用toXXX方法返回相差单位 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDate ofDate(TemporalAccessor temporalAccessor)` | TemporalAccessor转LocalDate，使用默认时区 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDate parseDate(CharSequence text)` | 解析日期时间字符串为LocalDate，仅支持yyyy-MM-dd格式，例如：2007-12-03 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDate parseDate(CharSequence text,DateTimeFormatter formatter)` | 解析日期时间字符串为LocalDate，格式支持日期 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDate parseDate(CharSequence text,String format)` | 解析日期字符串为LocalDate |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime beginOfDay(LocalDate date)` | 修改为一天的开始时间，例如：2020-02-02 00:00:00,000 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime beginOfDay(LocalDateTime time)` | 修改为一天的开始时间，例如：2020-02-02 00:00:00,000 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime endOfDay(LocalDate date)` | 修改为一天的结束时间，例如：2020-02-02 23:59:59,999 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime endOfDay(LocalDate date,boolean truncateMillisecond)` | 修改为一天的结束时间，例如： 毫秒不归零：2020-02-02 23:59:59,999 毫秒归零：2020-02-02 23:59:59,000 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime endOfDay(LocalDateTime time)` | 修改为一天的结束时间，例如：2020-02-02 23:59:59,999 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime endOfDay(LocalDateTime time,boolean truncateMillisecond)` | 修改为一天的结束时间，例如： 毫秒不归零：2020-02-02 23:59:59,999 毫秒归零：2020-02-02 23:59:59,000 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime now()` | 当前时间，默认时区 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime of(Date date)` | Date转LocalDateTime，使用默认时区 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime of(Instant instant)` | Instant转LocalDateTime，使用默认时区 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime of(Instant instant,TimeZone timeZone)` | Instant转LocalDateTime |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime of(Instant instant,ZoneId zoneId)` | Instant转LocalDateTime |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime of(TemporalAccessor temporalAccessor)` | TemporalAccessor转LocalDateTime，使用默认时区 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime of(ZonedDateTime zonedDateTime)` | ZonedDateTime转LocalDateTime |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime of(long epochMilli)` | 毫秒转LocalDateTime，使用默认时区 注意：此方法使用默认时区，如果非UTC，会产生时间偏移 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime of(long epochMilli,TimeZone timeZone)` | 毫秒转LocalDateTime，结果会产生时间偏移 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime of(long epochMilli,ZoneId zoneId)` | 毫秒转LocalDateTime，根据时区不同，结果会产生时间偏移 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime ofUTC(Instant instant)` | Instant转LocalDateTime，使用UTC时区 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime ofUTC(long epochMilli)` | 毫秒转LocalDateTime，使用UTC时区 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime offset(LocalDateTime time,long number,TemporalUnit field)` | 日期偏移,根据field不同加不同值（偏移会修改传入的对象） |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime parse(CharSequence text)` | 解析日期时间字符串为LocalDateTime，仅支持yyyy-MM-dd'T'HH:mm:ss格式，例如：2007-12-03T10:15:30 即DateTimeFormatter#ISO_LOCAL_DATE_TIME |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime parse(CharSequence text,DateTimeFormatter formatter)` | 解析日期时间字符串为LocalDateTime，格式支持日期时间、日期、时间 如果formatter为null，则使用DateTimeFormatter#ISO_LOCAL_DATE_TIME |
| `cn.hutool.core.date.LocalDateTimeUtil` | `LocalDateTime parse(CharSequence text,String format)` | 解析日期时间字符串为LocalDateTime |
| `cn.hutool.core.date.LocalDateTimeUtil` | `Period betweenPeriod(LocalDate startTimeInclude,LocalDate endTimeExclude)` | 获取两个日期的表象时间差，如果结束时间早于开始时间，获取结果为负。 比如2011年2月1日，和2021年8月11日，日相差了10天，月相差6月 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `String format(LocalDate date,DateTimeFormatter formatter)` | 格式化日期时间为指定格式 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `String format(LocalDate date,String format)` | 格式化日期时间为指定格式 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `String format(LocalDateTime time,DateTimeFormatter formatter)` | 格式化日期时间为指定格式 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `String format(LocalDateTime time,String format)` | 格式化日期时间为指定格式 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `String formatNormal(LocalDate date)` | 格式化日期时间为yyyy-MM-dd格式 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `String formatNormal(LocalDateTime time)` | 格式化日期时间为yyyy-MM-dd HH:mm:ss格式 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `Week dayOfWeek(LocalDate localDate)` | 获取LocalDate对应的星期值 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `boolean isIn(ChronoLocalDateTime<?> date,ChronoLocalDateTime<?> beginDate,ChronoLocalDateTime<?> endDate)` | 当前日期是否在日期指定范围内 起始日期和结束日期可以互换 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `boolean isIn(ChronoLocalDateTime<?> date,ChronoLocalDateTime<?> beginDate,ChronoLocalDateTime<?> endDate,boolean includeBegin,boolean includeEnd)` | 判断当前时间（默认时区）是否在指定范围内 起始时间和结束时间可以互换 通过includeBegin, includeEnd参数控制时间范围区间是否为开区间，例如：传入参数：includeBegin=true, includeEnd=false， 则本方法会判断 date ∈ (beginDate, endDate] 是否成立 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `boolean isOverlap(ChronoLocalDateTime<?> realStartTime,ChronoLocalDateTime<?> realEndTime,ChronoLocalDateTime<?> startTime,ChronoLocalDateTime<?> endTime)` | 检查两个时间段是否有时间重叠 重叠指两个时间段是否有交集，注意此方法时间段重合时如： 此方法未纠正开始时间小于结束时间 当realStartTime和realEndTime或startTime和endTime相等时,退化为判断区间是否包含点 当realStartTime和realEndTime和startTime和endTime相等时,退化为判断点与点是否相等 See 准确的区间关系参考:艾伦区间代数 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `boolean isSameDay(final LocalDate date1,final LocalDate date2)` | 比较两个日期是否为同一天 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `boolean isSameDay(final LocalDateTime date1,final LocalDateTime date2)` | 比较两个日期是否为同一天 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `boolean isWeekend(LocalDate localDate)` | 是否为周末（周六或周日） |
| `cn.hutool.core.date.LocalDateTimeUtil` | `boolean isWeekend(LocalDateTime localDateTime)` | 是否为周末（周六或周日） |
| `cn.hutool.core.date.LocalDateTimeUtil` | `int weekOfYear(TemporalAccessor date)` | 获得指定日期是所在年份的第几周，如： 如果一年的第一天是星期一，则第一周从第一天开始，没有零周 如果一年的第二天是星期一，则第一周从第二天开始，而第一天在零周 如果一年中的第4天是星期一，则第1周从第4周开始，第1至第3周在零周开始 如果一年中的第5天是星期一，则第二周从第5周开始，第1至第4周在第1周 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `long between(LocalDateTime startTimeInclude,LocalDateTime endTimeExclude,ChronoUnit unit)` | 获取两个日期的差，如果结束时间早于开始时间，获取结果为负。 返回结果为时间差的long值 |
| `cn.hutool.core.date.LocalDateTimeUtil` | `long toEpochMilli(TemporalAccessor temporalAccessor)` | TemporalAccessor转换为 时间戳（从1970-01-01T00:00:00Z开始的毫秒数） |
| `cn.hutool.core.date.Month` | `Month of(String name)` | 解析别名为Month对象，别名如：jan或者JANUARY，不区分大小写 |
| `cn.hutool.core.date.Month` | `Month of(int calendarMonthIntValue)` | 将 Calendar月份相关值转换为Month枚举对象 未找到返回null |
| `cn.hutool.core.date.Month` | `Month of(java.time.Month month)` | java.time.Month转换为Month对象 |
| `cn.hutool.core.date.Month` | `String getDisplayName(TextStyle style)` | 获取显示名称 |
| `cn.hutool.core.date.Month` | `String getDisplayName(TextStyle style,Locale locale)` | 获取显示名称 |
| `cn.hutool.core.date.Month` | `int getLastDay(boolean isLeapYear)` | 获取此月份最后一天的值，不支持的月份（例如UNDECIMBER）返回-1 |
| `cn.hutool.core.date.Month` | `int getLastDay(int month,boolean isLeapYear)` | 获得指定月的最后一天 |
| `cn.hutool.core.date.Month` | `int getValue()` | 获取Calendar中的对应值 此值从0开始，即0表示一月 |
| `cn.hutool.core.date.Month` | `int getValueBaseOne()` | 获取月份值，此值与java.time.Month对应 此值从1开始，即1表示一月 |
| `cn.hutool.core.date.Month` | `java.time.Month toJdkMonth()` | 转换为java.time.Month |
| `cn.hutool.core.date.Quarter` | `Month firstMonth()` | 该季度的第一个月 |
| `cn.hutool.core.date.Quarter` | `Month lastMonth()` | 该季度最后一个月 |
| `cn.hutool.core.date.Quarter` | `MonthDay firstMonthDay()` | 该季度的第一天 |
| `cn.hutool.core.date.Quarter` | `MonthDay lastMonthDay()` | 该季度的最后一天 |
| `cn.hutool.core.date.Quarter` | `Quarter fromMonth(Month month)` | 根据给定的月份返回对应的季度 |
| `cn.hutool.core.date.Quarter` | `Quarter fromMonth(int monthValue)` | 根据给定的月份值返回对应的季度 |
| `cn.hutool.core.date.Quarter` | `Quarter of(int intValue)` | 将 季度int转换为Season枚举对象 |
| `cn.hutool.core.date.Quarter` | `Quarter plus(int quarters)` | 加上指定数量的季度 |
| `cn.hutool.core.date.Quarter` | `YearQuarter atYear(int year)` | 根据指定的年份，获取一个新的 YearQuarter 实例 此方法允许在保持当前季度信息不变的情况下，更改年份 |
| `cn.hutool.core.date.Quarter` | `int checkValidIntValue(int value)` | 检查季度的值。（1~4） |
| `cn.hutool.core.date.Quarter` | `int firstMonthValue()` | 该季度的第一个月 |
| `cn.hutool.core.date.Quarter` | `int getValue()` | 获取季度值 |
| `cn.hutool.core.date.Quarter` | `int lastMonthValue()` | 该季度最后一个月 |
| `cn.hutool.core.date.StopWatch` | `StopWatch create(String id)` | 创建计时任务（秒表） |
| `cn.hutool.core.date.StopWatch` | `String currentTaskName()` | 获取当前任务名，null 表示无任务 |
| `cn.hutool.core.date.StopWatch` | `String getId()` | 获取StopWatch 的ID，用于多个秒表对象的区分 |
| `cn.hutool.core.date.StopWatch` | `String getLastTaskName()` | 获取最后的任务名 |
| `cn.hutool.core.date.StopWatch` | `String prettyPrint()` | 生成所有任务的一个任务花费时间表，单位纳秒 |
| `cn.hutool.core.date.StopWatch` | `String prettyPrint(TimeUnit unit)` | 生成所有任务的一个任务花费时间表 |
| `cn.hutool.core.date.StopWatch` | `String shortSummary()` | 获取任务信息，类似于： |
| `cn.hutool.core.date.StopWatch` | `String shortSummary(TimeUnit unit)` | 获取任务信息，类似于： |
| `cn.hutool.core.date.StopWatch` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.StopWatch` | `TaskInfo getLastTaskInfo()` | 获取最后的任务对象 |
| `cn.hutool.core.date.StopWatch` | `TaskInfo[] getTaskInfo()` | 获取任务列表 |
| `cn.hutool.core.date.StopWatch` | `boolean isRunning()` | 检查是否有正在运行的任务 |
| `cn.hutool.core.date.StopWatch` | `double getTotalTimeSeconds()` | 获取所有任务的总花费时间（秒） |
| `cn.hutool.core.date.StopWatch` | `int getTaskCount()` | 获取任务数 |
| `cn.hutool.core.date.StopWatch` | `long getLastTaskTimeMillis()` | 获取最后任务的花费时间（毫秒） |
| `cn.hutool.core.date.StopWatch` | `long getLastTaskTimeNanos()` | 获取最后任务的花费时间（纳秒） |
| `cn.hutool.core.date.StopWatch` | `long getTotal(TimeUnit unit)` | 获取所有任务的总花费时间 |
| `cn.hutool.core.date.StopWatch` | `long getTotalTimeMillis()` | 获取所有任务的总花费时间（毫秒） |
| `cn.hutool.core.date.StopWatch` | `long getTotalTimeNanos()` | 获取所有任务的总花费时间（纳秒） |
| `cn.hutool.core.date.StopWatch` | `void setKeepTaskList(boolean keepTaskList)` | 设置是否在停止后保留任务，false 表示停止运行后不保留任务 |
| `cn.hutool.core.date.StopWatch` | `void start()` | 开始默认的新任务 |
| `cn.hutool.core.date.StopWatch` | `void start(String taskName)` | 开始指定名称的新任务 |
| `cn.hutool.core.date.StopWatch` | `void stop()` | 停止当前任务 |
| `cn.hutool.core.date.StopWatch$TaskInfo` | `String getTaskName()` | 获取任务名 |
| `cn.hutool.core.date.StopWatch$TaskInfo` | `double getTimeSeconds()` | 获取任务花费时间（单位：秒） |
| `cn.hutool.core.date.StopWatch$TaskInfo` | `long getTime(TimeUnit unit)` | 获取指定单位的任务花费时间 |
| `cn.hutool.core.date.StopWatch$TaskInfo` | `long getTimeMillis()` | 获取任务花费时间（单位：毫秒） |
| `cn.hutool.core.date.StopWatch$TaskInfo` | `long getTimeNanos()` | 获取任务花费时间（单位：纳秒） |
| `cn.hutool.core.date.SystemClock` | `String nowDate()` | @return 当前时间字符串表现形式 |
| `cn.hutool.core.date.SystemClock` | `long now()` | @return 当前时间 |
| `cn.hutool.core.date.TemporalAccessorUtil` | `Instant toInstant(TemporalAccessor temporalAccessor)` | TemporalAccessor转换为 Instant对象 |
| `cn.hutool.core.date.TemporalAccessorUtil` | `String format(TemporalAccessor time,DateTimeFormatter formatter)` | 格式化日期时间为指定格式 如果为Month，调用Month#toString() |
| `cn.hutool.core.date.TemporalAccessorUtil` | `String format(TemporalAccessor time,String format)` | 格式化日期时间为指定格式 如果为Month，调用Month#toString() |
| `cn.hutool.core.date.TemporalAccessorUtil` | `boolean isIn(TemporalAccessor date,TemporalAccessor beginDate,TemporalAccessor endDate)` | 当前日期是否在日期指定范围内 起始日期和结束日期可以互换 |
| `cn.hutool.core.date.TemporalAccessorUtil` | `boolean isIn(TemporalAccessor date,TemporalAccessor beginDate,TemporalAccessor endDate,boolean includeBegin,boolean includeEnd)` | 当前日期是否在日期指定范围内 起始日期和结束日期可以互换 通过includeBegin, includeEnd参数控制日期范围区间是否为开区间，例如：传入参数：includeBegin=true, includeEnd=false， 则本方法会判断 date ∈ (beginDate, endDate] 是否成立 |
| `cn.hutool.core.date.TemporalAccessorUtil` | `int get(TemporalAccessor temporalAccessor,TemporalField field)` | 安全获取时间的某个属性，属性不存在返回最小值，一般为0 注意请谨慎使用此方法，某些TemporalAccessor#isSupported(TemporalField)为false的方法返回最小值 |
| `cn.hutool.core.date.TemporalAccessorUtil` | `long toEpochMilli(TemporalAccessor temporalAccessor)` | TemporalAccessor转换为 时间戳（从1970-01-01T00:00:00Z开始的毫秒数） 如果为Month，调用Month#getValue() |
| `cn.hutool.core.date.TemporalUtil` | `ChronoUnit toChronoUnit(TimeUnit unit)` | 将 TimeUnit 转换为 ChronoUnit. |
| `cn.hutool.core.date.TemporalUtil` | `Duration between(Temporal startTimeInclude,Temporal endTimeExclude)` | 获取两个日期的差，如果结束时间早于开始时间，获取结果为负。 返回结果为Duration对象，通过调用toXXX方法返回相差单位 |
| `cn.hutool.core.date.TemporalUtil` | `T offset(T temporal,DayOfWeek dayOfWeek,boolean isPrevious)` | 偏移到指定的周几 |
| `cn.hutool.core.date.TemporalUtil` | `T offset(T time,long number,TemporalUnit field)` | 日期偏移,根据field不同加不同值（偏移会修改传入的对象） |
| `cn.hutool.core.date.TemporalUtil` | `TimeUnit toTimeUnit(ChronoUnit unit)` | 转换 ChronoUnit 到 TimeUnit. |
| `cn.hutool.core.date.TemporalUtil` | `long between(Temporal startTimeInclude,Temporal endTimeExclude,ChronoUnit unit)` | 获取两个日期的差，如果结束时间早于开始时间，获取结果为负。 返回结果为时间差的long值 |
| `cn.hutool.core.date.TimeInterval` | `String intervalPretty()` | 从开始到当前的间隔时间（毫秒数），返回XX天XX小时XX分XX秒XX毫秒 |
| `cn.hutool.core.date.TimeInterval` | `TimeInterval restart()` | 重新开始计算时间（重置开始时间） |
| `cn.hutool.core.date.TimeInterval` | `long interval()` | 从开始到当前的间隔时间（毫秒数） 如果使用纳秒计时，返回纳秒差，否则返回毫秒差 |
| `cn.hutool.core.date.TimeInterval` | `long intervalDay()` | 从开始到当前的间隔天数，取绝对值 |
| `cn.hutool.core.date.TimeInterval` | `long intervalHour()` | 从开始到当前的间隔小时数，取绝对值 |
| `cn.hutool.core.date.TimeInterval` | `long intervalMinute()` | 从开始到当前的间隔分钟数，取绝对值 |
| `cn.hutool.core.date.TimeInterval` | `long intervalMs()` | 从开始到当前的间隔时间（毫秒数） |
| `cn.hutool.core.date.TimeInterval` | `long intervalRestart()` | @return 重新计时并返回从开始到当前的持续时间 |
| `cn.hutool.core.date.TimeInterval` | `long intervalSecond()` | 从开始到当前的间隔秒数，取绝对值 |
| `cn.hutool.core.date.TimeInterval` | `long intervalWeek()` | 从开始到当前的间隔周数，取绝对值 |
| `cn.hutool.core.date.TimeInterval` | `long start()` | @return 开始计时并返回当前时间 |
| `cn.hutool.core.date.TimeZoneUtil` | `TimeZone getTimeZone(final String id)` | 【原文待译】Delegates to TimeZone#getTimeZone(String) after mapping an ID if it's in ZoneId#SHORT_IDS. On Java 25, calling TimeZone#getTimeZone(String) with an ID in ZoneId#SHORT_IDS writes a message to System#err in the form: |
| `cn.hutool.core.date.TimeZoneUtil` | `TimeZone toTimeZone(final TimeZone timeZone)` | 【原文待译】Returns the given TimeZone if non-null, otherwise TimeZone#getDefault(). |
| `cn.hutool.core.date.Week` | `DayOfWeek toJdkDayOfWeek()` | 转换为DayOfWeek |
| `cn.hutool.core.date.Week` | `String toChinese()` | 转换为中文名 |
| `cn.hutool.core.date.Week` | `String toChinese(String weekNamePre)` | 转换为中文名 |
| `cn.hutool.core.date.Week` | `Week of(DayOfWeek dayOfWeek)` | 将 DayOfWeek星期相关值转换为Week枚举对象 |
| `cn.hutool.core.date.Week` | `Week of(String name)` | 解析别名为Week对象，别名如：sun或者SUNDAY，不区分大小写 |
| `cn.hutool.core.date.Week` | `Week of(int calendarWeekIntValue)` | 将 Calendar星期相关值转换为Week枚举对象 |
| `cn.hutool.core.date.Week` | `int getIso8601Value()` | 获取ISO8601规范的int值，from 1 (Monday) to 7 (Sunday). |
| `cn.hutool.core.date.Week` | `int getValue()` | 获得星期对应Calendar 中的Week值 |
| `cn.hutool.core.date.YearQuarter` | `LocalDate firstDate()` | 该季度的第一天 |
| `cn.hutool.core.date.YearQuarter` | `LocalDate lastDate()` | 该季度的最后一天 |
| `cn.hutool.core.date.YearQuarter` | `Month firstMonth()` | 该季度第一个月 |
| `cn.hutool.core.date.YearQuarter` | `Month lastMonth()` | 该季度的最后一个月 |
| `cn.hutool.core.date.YearQuarter` | `Quarter getQuarter()` | 季度 |
| `cn.hutool.core.date.YearQuarter` | `String toString()` | 返回 YearQuarter 的字符串表示形式，如 "2024 Q3" |
| `cn.hutool.core.date.YearQuarter` | `YearMonth firstYearMonth()` | 该季度第一个月 |
| `cn.hutool.core.date.YearQuarter` | `YearMonth lastYearMonth()` | 该季度的最后一个月 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter lastQuarter()` | 上一个季度 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter lastYear()` | 上一年同季度 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter minusQuarters(long quartersToMinus)` | 减去季度 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter minusYears(long yearsToMinus)` | 减去年份 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter nextQuarter()` | 下一个季度 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter nextYear()` | 下一年同季度 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter now()` | 当前年季 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter of(Calendar date)` | 根据指定日期，判断日期所在的年份与季度，创建 YearQuarter 实例 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter of(Date date)` | 根据指定日期，判断日期所在的年份与季度，创建 YearQuarter 实例 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter of(LocalDate date)` | 根据指定日期，判断日期所在的年份与季度，创建 YearQuarter 实例 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter of(YearMonth yearMonth)` | 根据指定年月，判断其所在的年份与季度，创建 YearQuarter 实例 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter of(int year,Quarter quarter)` | 根据指定年份与季度，创建 YearQuarter 实例 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter of(int year,int quarter)` | 根据指定年份与季度，创建 YearQuarter 实例 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter plusQuarters(long quartersToAdd)` | 添加季度 |
| `cn.hutool.core.date.YearQuarter` | `YearQuarter plusYears(long yearsToAdd)` | 添加年份 |
| `cn.hutool.core.date.YearQuarter` | `boolean equals(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.YearQuarter` | `boolean isAfter(YearQuarter other)` | 判断是否在指定年份季度之后 |
| `cn.hutool.core.date.YearQuarter` | `boolean isBefore(YearQuarter other)` | 判断是否在指定年份季度之前 |
| `cn.hutool.core.date.YearQuarter` | `int compareTo(YearQuarter other)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.YearQuarter` | `int firstMonthValue()` | 该季度的第一个月 |
| `cn.hutool.core.date.YearQuarter` | `int getQuarterValue()` | 季度值。从 1 开始。 |
| `cn.hutool.core.date.YearQuarter` | `int getYear()` | 年份 |
| `cn.hutool.core.date.YearQuarter` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.date.YearQuarter` | `int lastMonthValue()` | 该季度的最后一个月 |
| `cn.hutool.core.date.Zodiac` | `String getChineseZodiac(Calendar calendar)` | 通过生日计算生肖，只计算1900年后出生的人 |
| `cn.hutool.core.date.Zodiac` | `String getChineseZodiac(Date date)` | 通过生日计算生肖，只计算1900年后出生的人 |
| `cn.hutool.core.date.Zodiac` | `String getChineseZodiac(int year)` | 计算生肖，只计算1900年后出生的人 |
| `cn.hutool.core.date.Zodiac` | `String getZodiac(Calendar calendar)` | 通过生日计算星座 |
| `cn.hutool.core.date.Zodiac` | `String getZodiac(Date date)` | 通过生日计算星座 |
| `cn.hutool.core.date.Zodiac` | `String getZodiac(Month month,int day)` | 通过生日计算星座 |
| `cn.hutool.core.date.Zodiac` | `String getZodiac(int month,int day)` | 通过生日计算星座 |
| `cn.hutool.core.date.ZoneUtil` | `TimeZone toTimeZone(ZoneId zoneId)` | ZoneId转换为TimeZone，null则返回系统默认值 |
| `cn.hutool.core.date.ZoneUtil` | `ZoneId toZoneId(TimeZone timeZone)` | TimeZone转换为ZoneId，null则返回系统默认值 |
