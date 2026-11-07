# com.baomidou.mybatisplus.core.conditions

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.conditions.AbstractLambdaWrapper`

```java
public abstract class com.baomidou.mybatisplus.core.conditions.AbstractLambdaWrapper<T, Children extends com.baomidou.mybatisplus.core.conditions.AbstractLambdaWrapper<T, Children>> extends com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, Children> {
  public com.baomidou.mybatisplus.core.conditions.AbstractLambdaWrapper();
  public final Children groupBy(boolean, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>...);
  public final Children orderBy(boolean, boolean, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>...);
  public final Children groupBy(com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>...);
  public Children groupBy(boolean, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, java.util.List<com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>>);
  public final Children orderByAsc(com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>...);
  public final Children orderByAsc(boolean, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>...);
  public final Children orderByDesc(com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>...);
  public final Children orderByDesc(boolean, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>...);
  public com.baomidou.mybatisplus.core.conditions.AbstractWrapper orderBy(boolean, boolean, java.lang.Object, java.lang.Object[]);
  public com.baomidou.mybatisplus.core.conditions.AbstractWrapper groupBy(boolean, java.lang.Object, java.util.List);
  public com.baomidou.mybatisplus.core.conditions.AbstractWrapper groupBy(boolean, java.lang.Object, java.lang.Object[]);
  public java.lang.Object orderBy(boolean, boolean, java.lang.Object, java.lang.Object[]);
  public java.lang.Object orderByDesc(boolean, java.lang.Object, java.lang.Object[]);
  public java.lang.Object orderByDesc(java.lang.Object, java.lang.Object[]);
  public java.lang.Object orderByAsc(boolean, java.lang.Object, java.lang.Object[]);
  public java.lang.Object orderByAsc(java.lang.Object, java.lang.Object[]);
  public java.lang.Object groupBy(boolean, java.lang.Object, java.util.List);
  public java.lang.Object groupBy(boolean, java.lang.Object, java.lang.Object[]);
  public java.lang.Object groupBy(java.lang.Object, java.lang.Object[]);
}
```

## `com.baomidou.mybatisplus.core.conditions.AbstractWrapper`

```java
public abstract class com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, R, Children extends com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, R, Children>> extends com.baomidou.mybatisplus.core.conditions.Wrapper<T> implements com.baomidou.mybatisplus.core.conditions.interfaces.Compare<Children, R>, com.baomidou.mybatisplus.core.conditions.interfaces.Nested<Children, Children>, com.baomidou.mybatisplus.core.conditions.interfaces.Join<Children>, com.baomidou.mybatisplus.core.conditions.interfaces.Func<Children, R> {
  public com.baomidou.mybatisplus.core.conditions.AbstractWrapper();
  public T getEntity();
  public Children setEntity(T);
  public java.lang.Class<T> getEntityClass();
  public Children setEntityClass(java.lang.Class<T>);
  public <V> Children allEq(boolean, java.util.Map<R, V>, boolean);
  public <V> Children allEq(boolean, java.util.function.BiPredicate<R, V>, java.util.Map<R, V>, boolean);
  public Children eq(boolean, R, java.lang.Object);
  public Children ne(boolean, R, java.lang.Object);
  public Children gt(boolean, R, java.lang.Object);
  public Children ge(boolean, R, java.lang.Object);
  public Children lt(boolean, R, java.lang.Object);
  public Children le(boolean, R, java.lang.Object);
  public Children like(boolean, R, java.lang.Object);
  public Children notLike(boolean, R, java.lang.Object);
  public Children likeLeft(boolean, R, java.lang.Object);
  public Children likeRight(boolean, R, java.lang.Object);
  public Children notLikeLeft(boolean, R, java.lang.Object);
  public Children notLikeRight(boolean, R, java.lang.Object);
  public Children between(boolean, R, java.lang.Object, java.lang.Object);
  public Children notBetween(boolean, R, java.lang.Object, java.lang.Object);
  public Children and(boolean, java.util.function.Consumer<Children>);
  public Children or(boolean, java.util.function.Consumer<Children>);
  public Children nested(boolean, java.util.function.Consumer<Children>);
  public Children not(boolean, java.util.function.Consumer<Children>);
  public Children or(boolean);
  public Children apply(boolean, java.lang.String, java.lang.Object...);
  public Children last(boolean, java.lang.String);
  public Children comment(boolean, java.lang.String);
  public Children first(boolean, java.lang.String);
  public Children exists(boolean, java.lang.String, java.lang.Object...);
  public Children notExists(boolean, java.lang.String, java.lang.Object...);
  public Children isNull(boolean, R);
  public Children isNotNull(boolean, R);
  public Children in(boolean, R, java.util.Collection<?>);
  public Children in(boolean, R, java.lang.Object...);
  public Children notIn(boolean, R, java.util.Collection<?>);
  public Children notIn(boolean, R, java.lang.Object...);
  public Children eqSql(boolean, R, java.lang.String);
  public Children inSql(boolean, R, java.lang.String);
  public Children gtSql(boolean, R, java.lang.String);
  public Children geSql(boolean, R, java.lang.String);
  public Children ltSql(boolean, R, java.lang.String);
  public Children leSql(boolean, R, java.lang.String);
  public Children notInSql(boolean, R, java.lang.String);
  public Children groupBy(boolean, R, R...);
  public Children groupBy(boolean, R, java.util.List<R>);
  public Children doGroupBy(boolean, R, java.util.List<R>);
  public Children doOrderBy(boolean, boolean, R, java.util.List<R>);
  public Children orderBy(boolean, boolean, R, R...);
  public Children orderBy(boolean, boolean, R, java.util.List<R>);
  public Children groupBy(boolean, R);
  public Children groupBy(boolean, java.util.List<R>);
  public Children orderBy(boolean, boolean, R);
  public Children orderBy(boolean, boolean, java.util.List<R>);
  public Children having(boolean, java.lang.String, java.lang.Object...);
  public Children func(boolean, java.util.function.Consumer<Children>);
  public void clear();
  public boolean isUseAnnotationOrderBy();
  public java.lang.String getSqlSegment();
  public java.lang.String getSqlComment();
  public java.lang.String getSqlFirst();
  public com.baomidou.mybatisplus.core.conditions.segments.MergeSegments getExpression();
  public java.lang.String getParamAlias();
  public Children setParamAlias(java.lang.String);
  public Children clone();
  public java.util.Map<java.lang.String, java.lang.Object> getParamNameValuePairs();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
  public java.lang.Object likeRight(boolean, java.lang.Object, java.lang.Object);
  public java.lang.Object likeLeft(boolean, java.lang.Object, java.lang.Object);
  public java.lang.Object notLikeRight(boolean, java.lang.Object, java.lang.Object);
  public java.lang.Object notLikeLeft(boolean, java.lang.Object, java.lang.Object);
  public java.lang.Object notLike(boolean, java.lang.Object, java.lang.Object);
  public java.lang.Object like(boolean, java.lang.Object, java.lang.Object);
  public java.lang.Object notBetween(boolean, java.lang.Object, java.lang.Object, java.lang.Object);
  public java.lang.Object between(boolean, java.lang.Object, java.lang.Object, java.lang.Object);
  public java.lang.Object le(boolean, java.lang.Object, java.lang.Object);
  public java.lang.Object lt(boolean, java.lang.Object, java.lang.Object);
  public java.lang.Object ge(boolean, java.lang.Object, java.lang.Object);
  public java.lang.Object gt(boolean, java.lang.Object, java.lang.Object);
  public java.lang.Object ne(boolean, java.lang.Object, java.lang.Object);
  public java.lang.Object eq(boolean, java.lang.Object, java.lang.Object);
  public java.lang.Object allEq(boolean, java.util.function.BiPredicate, java.util.Map, boolean);
  public java.lang.Object allEq(boolean, java.util.Map, boolean);
  public java.lang.Object not(boolean, java.util.function.Consumer);
  public java.lang.Object nested(boolean, java.util.function.Consumer);
  public java.lang.Object or(boolean, java.util.function.Consumer);
  public java.lang.Object and(boolean, java.util.function.Consumer);
  public java.lang.Object notExists(boolean, java.lang.String, java.lang.Object[]);
  public java.lang.Object exists(boolean, java.lang.String, java.lang.Object[]);
  public java.lang.Object first(boolean, java.lang.String);
  public java.lang.Object comment(boolean, java.lang.String);
  public java.lang.Object last(boolean, java.lang.String);
  public java.lang.Object apply(boolean, java.lang.String, java.lang.Object[]);
  public java.lang.Object or(boolean);
  public java.lang.Object func(boolean, java.util.function.Consumer);
  public java.lang.Object having(boolean, java.lang.String, java.lang.Object[]);
  public java.lang.Object orderBy(boolean, boolean, java.lang.Object, java.util.List);
  public java.lang.Object orderBy(boolean, boolean, java.lang.Object, java.lang.Object[]);
  public java.lang.Object orderBy(boolean, boolean, java.util.List);
  public java.lang.Object orderBy(boolean, boolean, java.lang.Object);
  public java.lang.Object groupBy(boolean, java.lang.Object, java.util.List);
  public java.lang.Object groupBy(boolean, java.lang.Object, java.lang.Object[]);
  public java.lang.Object groupBy(boolean, java.util.List);
  public java.lang.Object groupBy(boolean, java.lang.Object);
  public java.lang.Object notInSql(boolean, java.lang.Object, java.lang.String);
  public java.lang.Object leSql(boolean, java.lang.Object, java.lang.String);
  public java.lang.Object ltSql(boolean, java.lang.Object, java.lang.String);
  public java.lang.Object geSql(boolean, java.lang.Object, java.lang.String);
  public java.lang.Object gtSql(boolean, java.lang.Object, java.lang.String);
  public java.lang.Object inSql(boolean, java.lang.Object, java.lang.String);
  public java.lang.Object eqSql(boolean, java.lang.Object, java.lang.String);
  public java.lang.Object notIn(boolean, java.lang.Object, java.lang.Object[]);
  public java.lang.Object notIn(boolean, java.lang.Object, java.util.Collection);
  public java.lang.Object in(boolean, java.lang.Object, java.lang.Object[]);
  public java.lang.Object in(boolean, java.lang.Object, java.util.Collection);
  public java.lang.Object isNotNull(boolean, java.lang.Object);
  public java.lang.Object isNull(boolean, java.lang.Object);
}
```

## `com.baomidou.mybatisplus.core.conditions.AbstractWrapper$DoSomething`

```java
public interface com.baomidou.mybatisplus.core.conditions.AbstractWrapper$DoSomething {
  public abstract void doIt();
}
```

## `com.baomidou.mybatisplus.core.conditions.ISqlSegment`

```java
public interface com.baomidou.mybatisplus.core.conditions.ISqlSegment extends java.io.Serializable {
  public abstract java.lang.String getSqlSegment();
}
```

## `com.baomidou.mybatisplus.core.conditions.SharedString`

```java
public class com.baomidou.mybatisplus.core.conditions.SharedString implements java.io.Serializable {
  public static com.baomidou.mybatisplus.core.conditions.SharedString emptyString();
  public void toEmpty();
  public void toNull();
  public java.lang.String getStringValue();
  public com.baomidou.mybatisplus.core.conditions.SharedString setStringValue(java.lang.String);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public com.baomidou.mybatisplus.core.conditions.SharedString();
  public com.baomidou.mybatisplus.core.conditions.SharedString(java.lang.String);
}
```

## `com.baomidou.mybatisplus.core.conditions.Wrapper`

```java
public abstract class com.baomidou.mybatisplus.core.conditions.Wrapper<T> implements com.baomidou.mybatisplus.core.conditions.ISqlSegment {
  public com.baomidou.mybatisplus.core.conditions.Wrapper();
  public abstract T getEntity();
  public java.lang.String getSqlSelect();
  public java.lang.String getSqlSet();
  public java.lang.String getSqlComment();
  public java.lang.String getSqlFirst();
  public abstract com.baomidou.mybatisplus.core.conditions.segments.MergeSegments getExpression();
  public java.lang.String getCustomSqlSegment();
  public boolean isEmptyOfWhere();
  public boolean isNonEmptyOfWhere();
  public boolean nonEmptyOfWhere();
  public boolean isEmptyOfNormal();
  public boolean isNonEmptyOfNormal();
  public boolean nonEmptyOfNormal();
  public boolean isNonEmptyOfEntity();
  public boolean nonEmptyOfEntity();
  public boolean isEmptyOfEntity();
  public java.lang.String getTargetSql();
  public abstract void clear();
}
```
