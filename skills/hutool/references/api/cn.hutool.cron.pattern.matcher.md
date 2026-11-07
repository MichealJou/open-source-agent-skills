# cn.hutool.cron.pattern.matcher

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.cron.pattern.matcher.AlwaysTrueMatcher`

```java
public class cn.hutool.cron.pattern.matcher.AlwaysTrueMatcher implements cn.hutool.cron.pattern.matcher.PartMatcher {
  public cn.hutool.cron.pattern.matcher.AlwaysTrueMatcher();
  public boolean match(java.lang.Integer);
  public int nextAfter(int);
  public java.lang.String toString();
  public boolean match(java.lang.Object);
}
```

## `cn.hutool.cron.pattern.matcher.BoolArrayMatcher`

```java
public class cn.hutool.cron.pattern.matcher.BoolArrayMatcher implements cn.hutool.cron.pattern.matcher.PartMatcher {
  public cn.hutool.cron.pattern.matcher.BoolArrayMatcher(java.util.List<java.lang.Integer>);
  public boolean match(java.lang.Integer);
  public int nextAfter(int);
  public int getMinValue();
  public int getMaxValue();
  public java.lang.String toString();
  public boolean match(java.lang.Object);
}
```

## `cn.hutool.cron.pattern.matcher.DayOfMonthMatcher`

```java
public class cn.hutool.cron.pattern.matcher.DayOfMonthMatcher extends cn.hutool.cron.pattern.matcher.BoolArrayMatcher {
  public cn.hutool.cron.pattern.matcher.DayOfMonthMatcher(java.util.List<java.lang.Integer>);
  public boolean match(int, int, boolean);
  public int nextAfter(int, int, boolean);
  public boolean isLast();
  public boolean isLastDay(java.lang.Integer, java.lang.Integer, boolean);
  public int getMinValue(int, boolean);
  public int getMaxValue(int, boolean);
}
```

## `cn.hutool.cron.pattern.matcher.PartMatcher`

```java
public interface cn.hutool.cron.pattern.matcher.PartMatcher extends cn.hutool.core.lang.Matcher<java.lang.Integer> {
  public abstract int nextAfter(int);
}
```

## `cn.hutool.cron.pattern.matcher.PatternMatcher`

```java
public class cn.hutool.cron.pattern.matcher.PatternMatcher {
  public cn.hutool.cron.pattern.matcher.PatternMatcher(cn.hutool.cron.pattern.matcher.PartMatcher, cn.hutool.cron.pattern.matcher.PartMatcher, cn.hutool.cron.pattern.matcher.PartMatcher, cn.hutool.cron.pattern.matcher.PartMatcher, cn.hutool.cron.pattern.matcher.PartMatcher, cn.hutool.cron.pattern.matcher.PartMatcher, cn.hutool.cron.pattern.matcher.PartMatcher);
  public cn.hutool.cron.pattern.matcher.PartMatcher get(cn.hutool.cron.pattern.Part);
  public boolean match(int[]);
  public boolean matchWeek(int);
  public java.util.Calendar nextMatchAfter(int[], java.util.TimeZone);
}
```

## `cn.hutool.cron.pattern.matcher.YearValueMatcher`

```java
public class cn.hutool.cron.pattern.matcher.YearValueMatcher implements cn.hutool.cron.pattern.matcher.PartMatcher {
  public cn.hutool.cron.pattern.matcher.YearValueMatcher(java.util.Collection<java.lang.Integer>);
  public boolean match(java.lang.Integer);
  public int nextAfter(int);
  public boolean match(java.lang.Object);
}
```
