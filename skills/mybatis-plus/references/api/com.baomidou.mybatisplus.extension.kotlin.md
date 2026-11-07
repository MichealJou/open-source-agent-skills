# com.baomidou.mybatisplus.extension.kotlin

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.kotlin.AbstractKtWrapper`

```java
public abstract class com.baomidou.mybatisplus.extension.kotlin.AbstractKtWrapper<T, Children extends com.baomidou.mybatisplus.extension.kotlin.AbstractKtWrapper<T, Children>> extends com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, kotlin.reflect.KProperty1<? super T, ?>, Children> {
  public com.baomidou.mybatisplus.extension.kotlin.AbstractKtWrapper();
  public final java.lang.String columnsToString(boolean, kotlin.reflect.KProperty1<? super T, ?>...);
  public final java.lang.String columnsToString(boolean, java.util.List<kotlin.reflect.KProperty1<? super T, ?>>);
  public java.lang.String columnToString(java.lang.Object);
}
```

## `com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper`

```java
public class com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper<T> extends com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper<T, kotlin.reflect.KProperty1<? super T, ?>, com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper<T>, com.baomidou.mybatisplus.extension.kotlin.KtQueryWrapper<T>> implements com.baomidou.mybatisplus.extension.conditions.query.ChainQuery<T>, com.baomidou.mybatisplus.core.conditions.query.Query<com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper<T>, T, kotlin.reflect.KProperty1<? super T, ?>> {
  public com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>);
  public final com.baomidou.mybatisplus.core.mapper.BaseMapper<T> getBaseMapper$mybatis_plus_extension();
  public com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, java.lang.Class<T>);
  public com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, T);
  public com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper(java.lang.Class<T>);
  public com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper(T);
  public com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper<T> select(boolean, java.util.List<kotlin.reflect.KProperty1<? super T, ?>>);
  public com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper<T> select(java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public com.baomidou.mybatisplus.extension.kotlin.KtQueryChainWrapper<T> select(java.lang.Class<T>, java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public com.baomidou.mybatisplus.core.mapper.BaseMapper<T> getBaseMapper();
  public java.lang.Class<T> getEntityClass();
  public java.lang.Object select(boolean, java.util.List);
  public java.lang.Object select(java.util.function.Predicate);
  public java.lang.Object select(java.lang.Class, java.util.function.Predicate);
  public com.baomidou.mybatisplus.core.conditions.Wrapper getWrapper();
}
```

## `com.baomidou.mybatisplus.extension.kotlin.KtQueryWrapper`

```java
public class com.baomidou.mybatisplus.extension.kotlin.KtQueryWrapper<T> extends com.baomidou.mybatisplus.extension.kotlin.AbstractKtWrapper<T, com.baomidou.mybatisplus.extension.kotlin.KtQueryWrapper<T>> implements com.baomidou.mybatisplus.core.conditions.query.Query<com.baomidou.mybatisplus.extension.kotlin.KtQueryWrapper<T>, T, kotlin.reflect.KProperty1<? super T, ?>> {
  public com.baomidou.mybatisplus.extension.kotlin.KtQueryWrapper(T);
  public com.baomidou.mybatisplus.extension.kotlin.KtQueryWrapper(java.lang.Class<T>);
  public com.baomidou.mybatisplus.extension.kotlin.KtQueryWrapper(T, java.lang.Class<T>, com.baomidou.mybatisplus.core.conditions.SharedString, java.util.concurrent.atomic.AtomicInteger, java.util.Map<java.lang.String, ? extends java.lang.Object>, java.util.Map<java.lang.String, ? extends com.baomidou.mybatisplus.core.toolkit.support.ColumnCache>, com.baomidou.mybatisplus.core.conditions.SharedString, com.baomidou.mybatisplus.core.conditions.SharedString, com.baomidou.mybatisplus.core.conditions.SharedString);
  public com.baomidou.mybatisplus.extension.kotlin.KtQueryWrapper<T> select(boolean, java.util.List<kotlin.reflect.KProperty1<? super T, ?>>);
  public com.baomidou.mybatisplus.extension.kotlin.KtQueryWrapper<T> select(java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public com.baomidou.mybatisplus.extension.kotlin.KtQueryWrapper<T> select(java.lang.Class<T>, java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public java.lang.String getSqlSelect();
  public void clear();
  public java.lang.Object select(boolean, java.util.List);
  public java.lang.Object select(java.util.function.Predicate);
  public java.lang.Object select(java.lang.Class, java.util.function.Predicate);
  public com.baomidou.mybatisplus.core.conditions.AbstractWrapper instance();
}
```

## `com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper`

```java
public class com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper<T> extends com.baomidou.mybatisplus.extension.conditions.AbstractChainWrapper<T, kotlin.reflect.KProperty1<? super T, ?>, com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper<T>, com.baomidou.mybatisplus.extension.kotlin.KtUpdateWrapper<T>> implements com.baomidou.mybatisplus.extension.conditions.update.ChainUpdate<T>, com.baomidou.mybatisplus.core.conditions.update.Update<com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper<T>, kotlin.reflect.KProperty1<? super T, ?>> {
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>);
  public final com.baomidou.mybatisplus.core.mapper.BaseMapper<T> getBaseMapper$mybatis_plus_extension();
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, java.lang.Class<T>);
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper(com.baomidou.mybatisplus.core.mapper.BaseMapper<T>, T);
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper(java.lang.Class<T>);
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper(T);
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper<T> set(boolean, kotlin.reflect.KProperty1<? super T, ?>, java.lang.Object, java.lang.String);
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper<T> setSql(boolean, java.lang.String, java.lang.Object...);
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper<T> setDecrBy(boolean, kotlin.reflect.KProperty1<? super T, ?>, java.lang.Number);
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateChainWrapper<T> setIncrBy(boolean, kotlin.reflect.KProperty1<? super T, ?>, java.lang.Number);
  public com.baomidou.mybatisplus.core.mapper.BaseMapper<T> getBaseMapper();
  public java.lang.Class<T> getEntityClass();
  public java.lang.Object set(boolean, java.lang.Object, java.lang.Object, java.lang.String);
  public java.lang.Object setSql(boolean, java.lang.String, java.lang.Object[]);
  public java.lang.Object setDecrBy(boolean, java.lang.Object, java.lang.Number);
  public java.lang.Object setIncrBy(boolean, java.lang.Object, java.lang.Number);
  public com.baomidou.mybatisplus.core.conditions.Wrapper getWrapper();
}
```

## `com.baomidou.mybatisplus.extension.kotlin.KtUpdateWrapper`

```java
public class com.baomidou.mybatisplus.extension.kotlin.KtUpdateWrapper<T> extends com.baomidou.mybatisplus.extension.kotlin.AbstractKtWrapper<T, com.baomidou.mybatisplus.extension.kotlin.KtUpdateWrapper<T>> implements com.baomidou.mybatisplus.core.conditions.update.Update<com.baomidou.mybatisplus.extension.kotlin.KtUpdateWrapper<T>, kotlin.reflect.KProperty1<? super T, ?>> {
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateWrapper(T);
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateWrapper(java.lang.Class<T>);
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateWrapper(T, java.util.concurrent.atomic.AtomicInteger, java.util.Map<java.lang.String, ? extends java.lang.Object>, java.util.Map<java.lang.String, ? extends com.baomidou.mybatisplus.core.toolkit.support.ColumnCache>, com.baomidou.mybatisplus.core.conditions.SharedString, com.baomidou.mybatisplus.core.conditions.SharedString, com.baomidou.mybatisplus.core.conditions.SharedString);
  public java.lang.String getSqlSet();
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateWrapper<T> set(boolean, kotlin.reflect.KProperty1<? super T, ?>, java.lang.Object, java.lang.String);
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateWrapper<T> setSql(boolean, java.lang.String, java.lang.Object...);
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateWrapper<T> setIncrBy(boolean, kotlin.reflect.KProperty1<? super T, ?>, java.lang.Number);
  public com.baomidou.mybatisplus.extension.kotlin.KtUpdateWrapper<T> setDecrBy(boolean, kotlin.reflect.KProperty1<? super T, ?>, java.lang.Number);
  public void clear();
  public java.lang.Object set(boolean, java.lang.Object, java.lang.Object, java.lang.String);
  public java.lang.Object setSql(boolean, java.lang.String, java.lang.Object[]);
  public java.lang.Object setIncrBy(boolean, java.lang.Object, java.lang.Number);
  public java.lang.Object setDecrBy(boolean, java.lang.Object, java.lang.Number);
  public com.baomidou.mybatisplus.core.conditions.AbstractWrapper instance();
}
```
