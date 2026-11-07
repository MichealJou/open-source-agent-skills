# cn.hutool.cron.pattern

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.cron.pattern.CronPattern` | `Calendar nextMatch(final Calendar calendar)` | 返回匹配到的下一个时间，如果给定时间匹配，直接返回 |
| `cn.hutool.cron.pattern.CronPattern` | `Calendar nextMatchAfter(Calendar calendar)` | 返回匹配到的下一个时间 |
| `cn.hutool.cron.pattern.CronPattern` | `CronPattern of(String pattern)` | 解析表达式为 CronPattern |
| `cn.hutool.cron.pattern.CronPattern` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.pattern.CronPattern` | `boolean match(Calendar calendar,boolean isMatchSecond)` | 给定时间是否匹配定时任务表达式 |
| `cn.hutool.cron.pattern.CronPattern` | `boolean match(LocalDateTime dateTime,boolean isMatchSecond)` | 给定时间是否匹配定时任务表达式 |
| `cn.hutool.cron.pattern.CronPattern` | `boolean match(TimeZone timezone,long millis,boolean isMatchSecond)` | 给定时间是否匹配定时任务表达式 |
| `cn.hutool.cron.pattern.CronPattern` | `boolean match(long millis,boolean isMatchSecond)` | 给定时间是否匹配定时任务表达式 |
| `cn.hutool.cron.pattern.CronPatternBuilder` | `CronPatternBuilder of()` | 创建构建器 |
| `cn.hutool.cron.pattern.CronPatternBuilder` | `CronPatternBuilder set(Part part,String value)` | 设置对应部分的定时任务值 |
| `cn.hutool.cron.pattern.CronPatternBuilder` | `CronPatternBuilder setRange(Part part,int begin,int end)` | 设置区间 |
| `cn.hutool.cron.pattern.CronPatternBuilder` | `CronPatternBuilder setValues(Part part,int... values)` | 设置值 |
| `cn.hutool.cron.pattern.CronPatternBuilder` | `String build()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.pattern.CronPatternUtil` | `Date nextDateAfter(CronPattern pattern,Date start)` | 列举指定日期之后内第一个匹配表达式的日期 |
| `cn.hutool.cron.pattern.CronPatternUtil` | `Date nextDateAfter(CronPattern pattern,Date start,boolean isMatchSecond)` | 列举指定日期之后内第一个匹配表达式的日期 |
| `cn.hutool.cron.pattern.CronPatternUtil` | `List<Date> matchedDates(CronPattern pattern,long start,long end,int count,boolean isMatchSecond)` | 列举指定日期范围内所有匹配表达式的日期 |
| `cn.hutool.cron.pattern.CronPatternUtil` | `List<Date> matchedDates(String patternStr,Date start,Date end,int count,boolean isMatchSecond)` | 列举指定日期范围内所有匹配表达式的日期 |
| `cn.hutool.cron.pattern.CronPatternUtil` | `List<Date> matchedDates(String patternStr,Date start,int count,boolean isMatchSecond)` | 列举指定日期之后（到开始日期对应年年底）内所有匹配表达式的日期 |
| `cn.hutool.cron.pattern.CronPatternUtil` | `List<Date> matchedDates(String patternStr,long start,long end,int count,boolean isMatchSecond)` | 列举指定日期范围内所有匹配表达式的日期 |
| `cn.hutool.cron.pattern.Part` | `Part of(int i)` | 根据位置获取Part |
| `cn.hutool.cron.pattern.Part` | `int checkValue(int value)` | 检查单个值是否有效 |
| `cn.hutool.cron.pattern.Part` | `int getCalendarField()` | 获取Calendar中对应字段项 |
| `cn.hutool.cron.pattern.Part` | `int getMax()` | 获取最大值 |
| `cn.hutool.cron.pattern.Part` | `int getMin()` | 获取最小值 |
