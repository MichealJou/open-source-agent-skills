# cn.hutool.cron.pattern.matcher

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.cron.pattern.matcher.AlwaysTrueMatcher` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.pattern.matcher.AlwaysTrueMatcher` | `boolean match(Integer t)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.pattern.matcher.AlwaysTrueMatcher` | `int nextAfter(int value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.pattern.matcher.BoolArrayMatcher` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.pattern.matcher.BoolArrayMatcher` | `boolean match(Integer value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.pattern.matcher.BoolArrayMatcher` | `int getMaxValue()` | 获取表达式定义的最大值 |
| `cn.hutool.cron.pattern.matcher.BoolArrayMatcher` | `int getMinValue()` | 获取表达式定义的最小值 |
| `cn.hutool.cron.pattern.matcher.BoolArrayMatcher` | `int nextAfter(int value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.pattern.matcher.DayOfMonthMatcher` | `boolean isLast()` | 是否包含最后一天 |
| `cn.hutool.cron.pattern.matcher.DayOfMonthMatcher` | `boolean isLastDay(Integer value,Integer month,boolean isLeapYear)` | 检查value是这个月的最后一天 |
| `cn.hutool.cron.pattern.matcher.DayOfMonthMatcher` | `boolean match(int dayValue,int month,boolean isLeapYear)` | 给定的日期是否匹配当前匹配器 |
| `cn.hutool.cron.pattern.matcher.DayOfMonthMatcher` | `int getMaxValue(final int month,final boolean isLeapYear)` | 获取表达式定义中指定月的最大日的值 首先获取表达式定义的最大值，如果这个值大于本月最后一天，则返回最后一天，否则返回用户定义的最大值 注意最后一天可能不是表达式中定义的有效值 |
| `cn.hutool.cron.pattern.matcher.DayOfMonthMatcher` | `int getMinValue(final int month,final boolean isLeapYear)` | 获取表达式定义中指定月的最小日的值 |
| `cn.hutool.cron.pattern.matcher.DayOfMonthMatcher` | `int nextAfter(int dayValue,final int month,final boolean isLeapYear)` | 获取指定日之后的匹配值，也可以是其本身 如果表达式中存在最后一天（如使用"L"），则： 4月、6月、9月、11月最多匹配到30日 4月闰年匹配到29日，非闰年28日 |
| `cn.hutool.cron.pattern.matcher.PartMatcher` | `int nextAfter(int value)` | 获取指定值之后的匹配值，也可以是指定值本身 |
| `cn.hutool.cron.pattern.matcher.PatternMatcher` | `Calendar nextMatchAfter(int[] values,TimeZone zone)` | 获取下一个匹配日期时间 获取方法是，先从年开始查找对应部分的下一个值： 如果此部分下个值不变，获取下一个部分 如果此部分下个值大于给定值，以下所有值置为最小值 如果此部分下个值小于给定值，回退到上一个值获取下一个新值，之后的值置为最小值 |
| `cn.hutool.cron.pattern.matcher.PatternMatcher` | `PartMatcher get(Part part)` | 根据表达式位置，获取对应的PartMatcher |
| `cn.hutool.cron.pattern.matcher.PatternMatcher` | `boolean match(int[] fields)` | 给定时间是否匹配定时任务表达式 |
| `cn.hutool.cron.pattern.matcher.PatternMatcher` | `boolean matchWeek(int dayOfWeekValue)` | 给定周的值是否匹配定时任务表达式对应部分 |
| `cn.hutool.cron.pattern.matcher.YearValueMatcher` | `boolean match(Integer t)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.pattern.matcher.YearValueMatcher` | `int nextAfter(int value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
