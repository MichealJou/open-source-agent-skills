# com.baomidou.mybatisplus.core.conditions.interfaces

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.conditions.interfaces.Compare`

```java
public interface com.baomidou.mybatisplus.core.conditions.interfaces.Compare<Children, R> extends java.io.Serializable {
  public default <V> Children allEq(java.util.Map<R, V>);
  public default <V> Children allEq(java.util.Map<R, V>, boolean);
  public abstract <V> Children allEq(boolean, java.util.Map<R, V>, boolean);
  public default <V> Children allEq(java.util.function.BiPredicate<R, V>, java.util.Map<R, V>);
  public default <V> Children allEq(java.util.function.BiPredicate<R, V>, java.util.Map<R, V>, boolean);
  public abstract <V> Children allEq(boolean, java.util.function.BiPredicate<R, V>, java.util.Map<R, V>, boolean);
  public default Children eq(R, java.lang.Object);
  public abstract Children eq(boolean, R, java.lang.Object);
  public default Children ne(R, java.lang.Object);
  public abstract Children ne(boolean, R, java.lang.Object);
  public default Children gt(R, java.lang.Object);
  public abstract Children gt(boolean, R, java.lang.Object);
  public default Children ge(R, java.lang.Object);
  public abstract Children ge(boolean, R, java.lang.Object);
  public default Children lt(R, java.lang.Object);
  public abstract Children lt(boolean, R, java.lang.Object);
  public default Children le(R, java.lang.Object);
  public abstract Children le(boolean, R, java.lang.Object);
  public default Children between(R, java.lang.Object, java.lang.Object);
  public abstract Children between(boolean, R, java.lang.Object, java.lang.Object);
  public default Children notBetween(R, java.lang.Object, java.lang.Object);
  public abstract Children notBetween(boolean, R, java.lang.Object, java.lang.Object);
  public default Children like(R, java.lang.Object);
  public abstract Children like(boolean, R, java.lang.Object);
  public default Children notLike(R, java.lang.Object);
  public abstract Children notLike(boolean, R, java.lang.Object);
  public default Children notLikeLeft(R, java.lang.Object);
  public abstract Children notLikeLeft(boolean, R, java.lang.Object);
  public default Children notLikeRight(R, java.lang.Object);
  public abstract Children notLikeRight(boolean, R, java.lang.Object);
  public default Children likeLeft(R, java.lang.Object);
  public abstract Children likeLeft(boolean, R, java.lang.Object);
  public default Children likeRight(R, java.lang.Object);
  public abstract Children likeRight(boolean, R, java.lang.Object);
}
```

## `com.baomidou.mybatisplus.core.conditions.interfaces.Func`

```java
public interface com.baomidou.mybatisplus.core.conditions.interfaces.Func<Children, R> extends java.io.Serializable {
  public default Children isNull(R);
  public abstract Children isNull(boolean, R);
  public default Children isNotNull(R);
  public abstract Children isNotNull(boolean, R);
  public default Children in(R, java.util.Collection<?>);
  public abstract Children in(boolean, R, java.util.Collection<?>);
  public default Children in(R, java.lang.Object...);
  public abstract Children in(boolean, R, java.lang.Object...);
  public default Children notIn(R, java.util.Collection<?>);
  public abstract Children notIn(boolean, R, java.util.Collection<?>);
  public default Children notIn(R, java.lang.Object...);
  public abstract Children notIn(boolean, R, java.lang.Object...);
  public default Children eqSql(R, java.lang.String);
  public abstract Children eqSql(boolean, R, java.lang.String);
  public default Children inSql(R, java.lang.String);
  public abstract Children inSql(boolean, R, java.lang.String);
  public abstract Children gtSql(boolean, R, java.lang.String);
  public default Children gtSql(R, java.lang.String);
  public abstract Children geSql(boolean, R, java.lang.String);
  public default Children geSql(R, java.lang.String);
  public abstract Children ltSql(boolean, R, java.lang.String);
  public default Children ltSql(R, java.lang.String);
  public abstract Children leSql(boolean, R, java.lang.String);
  public default Children leSql(R, java.lang.String);
  public default Children notInSql(R, java.lang.String);
  public abstract Children notInSql(boolean, R, java.lang.String);
  public abstract Children groupBy(boolean, R);
  public default Children groupBy(R);
  public abstract Children groupBy(boolean, java.util.List<R>);
  public default Children groupBy(java.util.List<R>);
  public default Children groupBy(R, R...);
  public abstract Children groupBy(boolean, R, R...);
  public abstract Children groupBy(boolean, R, java.util.List<R>);
  public default Children orderByAsc(boolean, R);
  public default Children orderByAsc(R);
  public default Children orderByAsc(boolean, java.util.List<R>);
  public default Children orderByAsc(java.util.List<R>);
  public default Children orderByAsc(R, R...);
  public default Children orderByAsc(boolean, R, R...);
  public default Children orderByAsc(boolean, R, java.util.List<R>);
  public default Children orderByDesc(boolean, R);
  public default Children orderByDesc(R);
  public default Children orderByDesc(boolean, java.util.List<R>);
  public default Children orderByDesc(java.util.List<R>);
  public default Children orderByDesc(R, R...);
  public default Children orderByDesc(boolean, R, R...);
  public default Children orderByDesc(boolean, R, java.util.List<R>);
  public abstract Children orderBy(boolean, boolean, R);
  public abstract Children orderBy(boolean, boolean, java.util.List<R>);
  public abstract Children orderBy(boolean, boolean, R, R...);
  public abstract Children orderBy(boolean, boolean, R, java.util.List<R>);
  public default Children having(java.lang.String, java.lang.Object...);
  public abstract Children having(boolean, java.lang.String, java.lang.Object...);
  public default Children func(java.util.function.Consumer<Children>);
  public abstract Children func(boolean, java.util.function.Consumer<Children>);
}
```

## `com.baomidou.mybatisplus.core.conditions.interfaces.Join`

```java
public interface com.baomidou.mybatisplus.core.conditions.interfaces.Join<Children> extends java.io.Serializable {
  public default Children or();
  public abstract Children or(boolean);
  public default Children apply(java.lang.String, java.lang.Object...);
  public abstract Children apply(boolean, java.lang.String, java.lang.Object...);
  public default Children last(java.lang.String);
  public abstract Children last(boolean, java.lang.String);
  public default Children comment(java.lang.String);
  public abstract Children comment(boolean, java.lang.String);
  public default Children first(java.lang.String);
  public abstract Children first(boolean, java.lang.String);
  public default Children exists(java.lang.String, java.lang.Object...);
  public abstract Children exists(boolean, java.lang.String, java.lang.Object...);
  public default Children notExists(java.lang.String, java.lang.Object...);
  public abstract Children notExists(boolean, java.lang.String, java.lang.Object...);
}
```

## `com.baomidou.mybatisplus.core.conditions.interfaces.Nested`

```java
public interface com.baomidou.mybatisplus.core.conditions.interfaces.Nested<Param, Children> extends java.io.Serializable {
  public default Children and(java.util.function.Consumer<Param>);
  public abstract Children and(boolean, java.util.function.Consumer<Param>);
  public default Children or(java.util.function.Consumer<Param>);
  public abstract Children or(boolean, java.util.function.Consumer<Param>);
  public default Children nested(java.util.function.Consumer<Param>);
  public abstract Children nested(boolean, java.util.function.Consumer<Param>);
  public default Children not(java.util.function.Consumer<Param>);
  public abstract Children not(boolean, java.util.function.Consumer<Param>);
}
```
