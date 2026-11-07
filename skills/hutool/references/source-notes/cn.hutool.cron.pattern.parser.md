# cn.hutool.cron.pattern.parser

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.cron.pattern.parser.PartParser` | `PartMatcher parse(String value)` | 将表达式解析为PartMatcher * 或者 ? 返回AlwaysTrueMatcher Part#DAY_OF_MONTH 返回DayOfMonthMatcher Part#YEAR 返回YearValueMatcher 其他 返回BoolArrayMatcher |
| `cn.hutool.cron.pattern.parser.PartParser` | `PartParser of(Part part)` | 创建解析器 |
| `cn.hutool.cron.pattern.parser.PatternParser` | `List<PatternMatcher> parse(String cronPattern)` | 解析表达式到匹配列表中 |
