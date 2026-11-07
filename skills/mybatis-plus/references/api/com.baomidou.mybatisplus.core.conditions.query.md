# com.baomidou.mybatisplus.core.conditions.query

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper`

```java
public class com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T> extends com.baomidou.mybatisplus.core.conditions.AbstractLambdaWrapper<T, com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T>> implements com.baomidou.mybatisplus.core.conditions.query.Query<com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T>, T, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>> {
  public com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper();
  public com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper(T);
  public com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper(java.lang.Class<T>);
  public com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T> select(boolean, java.util.List<com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>>);
  public com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T> select(java.lang.Class<T>, java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public final com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T> select(com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>...);
  public final com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T> select(boolean, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>...);
  public java.lang.String getSqlSelect();
  public void clear();
  public java.lang.Object select(java.lang.Class, java.util.function.Predicate);
  public java.lang.Object select(boolean, java.util.List);
  public java.lang.Object select(boolean, java.lang.Object[]);
  public java.lang.Object select(java.lang.Object[]);
}
```

## `com.baomidou.mybatisplus.core.conditions.query.Query`

```java
public interface com.baomidou.mybatisplus.core.conditions.query.Query<Children, T, R> extends java.io.Serializable {
  public default Children select(R...);
  public default Children select(boolean, R...);
  public default Children select(java.util.List<R>);
  public abstract Children select(boolean, java.util.List<R>);
  public default Children select(java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public abstract Children select(java.lang.Class<T>, java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public abstract java.lang.String getSqlSelect();
}
```

## `com.baomidou.mybatisplus.core.conditions.query.QueryWrapper`

```java
public class com.baomidou.mybatisplus.core.conditions.query.QueryWrapper<T> extends com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, java.lang.String, com.baomidou.mybatisplus.core.conditions.query.QueryWrapper<T>> implements com.baomidou.mybatisplus.core.conditions.query.Query<com.baomidou.mybatisplus.core.conditions.query.QueryWrapper<T>, T, java.lang.String> {
  public com.baomidou.mybatisplus.core.conditions.query.QueryWrapper();
  public com.baomidou.mybatisplus.core.conditions.query.QueryWrapper(T);
  public com.baomidou.mybatisplus.core.conditions.query.QueryWrapper(java.lang.Class<T>);
  public com.baomidou.mybatisplus.core.conditions.query.QueryWrapper(T, java.lang.String...);
  public com.baomidou.mybatisplus.core.conditions.query.QueryWrapper<T> checkSqlInjection();
  public com.baomidou.mybatisplus.core.conditions.query.QueryWrapper<T> select(boolean, java.util.List<java.lang.String>);
  public com.baomidou.mybatisplus.core.conditions.query.QueryWrapper<T> select(java.lang.Class<T>, java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public java.lang.String getSqlSelect();
  public com.baomidou.mybatisplus.core.conditions.query.LambdaQueryWrapper<T> lambda();
  public void clear();
  public java.lang.Object select(java.lang.Class, java.util.function.Predicate);
  public java.lang.Object select(boolean, java.util.List);
}
```
