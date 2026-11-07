# com.baomidou.mybatisplus.core.conditions.segments

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.conditions.segments.AbstractISegmentList`

```java
public abstract class com.baomidou.mybatisplus.core.conditions.segments.AbstractISegmentList extends java.util.ArrayList<com.baomidou.mybatisplus.core.conditions.ISqlSegment> implements com.baomidou.mybatisplus.core.conditions.ISqlSegment, com.baomidou.mybatisplus.core.toolkit.StringPool {
  public com.baomidou.mybatisplus.core.conditions.segments.AbstractISegmentList();
  public boolean addAll(java.util.Collection<? extends com.baomidou.mybatisplus.core.conditions.ISqlSegment>);
  public java.lang.String getSqlSegment();
  public void clear();
}
```

## `com.baomidou.mybatisplus.core.conditions.segments.GroupBySegmentList`

```java
public class com.baomidou.mybatisplus.core.conditions.segments.GroupBySegmentList extends com.baomidou.mybatisplus.core.conditions.segments.AbstractISegmentList {
  public com.baomidou.mybatisplus.core.conditions.segments.GroupBySegmentList();
}
```

## `com.baomidou.mybatisplus.core.conditions.segments.HavingSegmentList`

```java
public class com.baomidou.mybatisplus.core.conditions.segments.HavingSegmentList extends com.baomidou.mybatisplus.core.conditions.segments.AbstractISegmentList {
  public com.baomidou.mybatisplus.core.conditions.segments.HavingSegmentList();
}
```

## `com.baomidou.mybatisplus.core.conditions.segments.MatchSegment`

```java
public final class com.baomidou.mybatisplus.core.conditions.segments.MatchSegment extends java.lang.Enum<com.baomidou.mybatisplus.core.conditions.segments.MatchSegment> {
  public static com.baomidou.mybatisplus.core.conditions.segments.MatchSegment[] values();
  public static com.baomidou.mybatisplus.core.conditions.segments.MatchSegment valueOf(java.lang.String);
  public boolean match(com.baomidou.mybatisplus.core.conditions.ISqlSegment);
  public java.util.function.Predicate<com.baomidou.mybatisplus.core.conditions.ISqlSegment> getPredicate();
}
```

## `com.baomidou.mybatisplus.core.conditions.segments.MergeSegments`

```java
public class com.baomidou.mybatisplus.core.conditions.segments.MergeSegments implements com.baomidou.mybatisplus.core.conditions.ISqlSegment {
  public com.baomidou.mybatisplus.core.conditions.segments.MergeSegments();
  public void add(com.baomidou.mybatisplus.core.conditions.ISqlSegment...);
  public java.lang.String getSqlSegment();
  public void clear();
  public com.baomidou.mybatisplus.core.conditions.segments.NormalSegmentList getNormal();
  public com.baomidou.mybatisplus.core.conditions.segments.GroupBySegmentList getGroupBy();
  public com.baomidou.mybatisplus.core.conditions.segments.HavingSegmentList getHaving();
  public com.baomidou.mybatisplus.core.conditions.segments.OrderBySegmentList getOrderBy();
}
```

## `com.baomidou.mybatisplus.core.conditions.segments.NormalSegmentList`

```java
public class com.baomidou.mybatisplus.core.conditions.segments.NormalSegmentList extends com.baomidou.mybatisplus.core.conditions.segments.AbstractISegmentList {
  public void clear();
}
```

## `com.baomidou.mybatisplus.core.conditions.segments.OrderBySegmentList`

```java
public class com.baomidou.mybatisplus.core.conditions.segments.OrderBySegmentList extends com.baomidou.mybatisplus.core.conditions.segments.AbstractISegmentList {
  public com.baomidou.mybatisplus.core.conditions.segments.OrderBySegmentList();
}
```
