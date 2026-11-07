# com.baomidou.mybatisplus.core.conditions.update

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper`

```java
public class com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper<T> extends com.baomidou.mybatisplus.core.conditions.AbstractLambdaWrapper<T, com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper<T>> implements com.baomidou.mybatisplus.core.conditions.update.Update<com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper<T>, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>> {
  public com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper();
  public com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper(T);
  public com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper(java.lang.Class<T>);
  public com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper<T> set(boolean, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, java.lang.Object, java.lang.String);
  public com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper<T> setSql(boolean, java.lang.String, java.lang.Object...);
  public com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper<T> setIncrBy(boolean, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, java.lang.Number);
  public com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper<T> setDecrBy(boolean, com.baomidou.mybatisplus.core.toolkit.support.SFunction<T, ?>, java.lang.Number);
  public java.lang.String getSqlSet();
  public void clear();
  public java.lang.Object setDecrBy(boolean, java.lang.Object, java.lang.Number);
  public java.lang.Object setIncrBy(boolean, java.lang.Object, java.lang.Number);
  public java.lang.Object setSql(boolean, java.lang.String, java.lang.Object[]);
  public java.lang.Object set(boolean, java.lang.Object, java.lang.Object, java.lang.String);
}
```

## `com.baomidou.mybatisplus.core.conditions.update.Update`

```java
public interface com.baomidou.mybatisplus.core.conditions.update.Update<Children, R> extends java.io.Serializable {
  public default Children set(R, java.lang.Object);
  public default Children set(boolean, R, java.lang.Object);
  public default Children set(R, java.lang.Object, java.lang.String);
  public abstract Children set(boolean, R, java.lang.Object, java.lang.String);
  public default Children setSql(java.lang.String, java.lang.Object...);
  public abstract Children setSql(boolean, java.lang.String, java.lang.Object...);
  public default Children setIncrBy(R, java.lang.Number);
  public abstract Children setIncrBy(boolean, R, java.lang.Number);
  public default Children setDecrBy(R, java.lang.Number);
  public abstract Children setDecrBy(boolean, R, java.lang.Number);
  public abstract java.lang.String getSqlSet();
}
```

## `com.baomidou.mybatisplus.core.conditions.update.UpdateWrapper`

```java
public class com.baomidou.mybatisplus.core.conditions.update.UpdateWrapper<T> extends com.baomidou.mybatisplus.core.conditions.AbstractWrapper<T, java.lang.String, com.baomidou.mybatisplus.core.conditions.update.UpdateWrapper<T>> implements com.baomidou.mybatisplus.core.conditions.update.Update<com.baomidou.mybatisplus.core.conditions.update.UpdateWrapper<T>, java.lang.String> {
  public com.baomidou.mybatisplus.core.conditions.update.UpdateWrapper();
  public com.baomidou.mybatisplus.core.conditions.update.UpdateWrapper(T);
  public com.baomidou.mybatisplus.core.conditions.update.UpdateWrapper<T> checkSqlInjection();
  public java.lang.String getSqlSet();
  public com.baomidou.mybatisplus.core.conditions.update.UpdateWrapper<T> set(boolean, java.lang.String, java.lang.Object, java.lang.String);
  public com.baomidou.mybatisplus.core.conditions.update.UpdateWrapper<T> setSql(boolean, java.lang.String, java.lang.Object...);
  public com.baomidou.mybatisplus.core.conditions.update.UpdateWrapper<T> setIncrBy(boolean, java.lang.String, java.lang.Number);
  public com.baomidou.mybatisplus.core.conditions.update.UpdateWrapper<T> setDecrBy(boolean, java.lang.String, java.lang.Number);
  public com.baomidou.mybatisplus.core.conditions.update.LambdaUpdateWrapper<T> lambda();
  public void clear();
  public java.lang.Object setDecrBy(boolean, java.lang.Object, java.lang.Number);
  public java.lang.Object setIncrBy(boolean, java.lang.Object, java.lang.Number);
  public java.lang.Object setSql(boolean, java.lang.String, java.lang.Object[]);
  public java.lang.Object set(boolean, java.lang.Object, java.lang.Object, java.lang.String);
}
```
