# com.baomidou.mybatisplus.core.toolkit.support

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.toolkit.support.BiIntFunction`

```java
public interface com.baomidou.mybatisplus.core.toolkit.support.BiIntFunction<T, R> {
  public abstract R apply(T, int);
}
```

## `com.baomidou.mybatisplus.core.toolkit.support.ColumnCache`

```java
public class com.baomidou.mybatisplus.core.toolkit.support.ColumnCache implements java.io.Serializable {
  public com.baomidou.mybatisplus.core.toolkit.support.ColumnCache(java.lang.String, java.lang.String);
  public java.lang.String getColumn();
  public java.lang.String getColumnSelect();
  public java.lang.String getMapping();
  public void setColumn(java.lang.String);
  public void setColumnSelect(java.lang.String);
  public void setMapping(java.lang.String);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public com.baomidou.mybatisplus.core.toolkit.support.ColumnCache(java.lang.String, java.lang.String, java.lang.String);
}
```

## `com.baomidou.mybatisplus.core.toolkit.support.IdeaProxyLambdaMeta`

```java
public class com.baomidou.mybatisplus.core.toolkit.support.IdeaProxyLambdaMeta implements com.baomidou.mybatisplus.core.toolkit.support.LambdaMeta {
  public com.baomidou.mybatisplus.core.toolkit.support.IdeaProxyLambdaMeta(java.lang.reflect.Proxy);
  public java.lang.String getImplMethodName();
  public java.lang.Class<?> getInstantiatedClass();
  public java.lang.String toString();
}
```

## `com.baomidou.mybatisplus.core.toolkit.support.LambdaMeta`

```java
public interface com.baomidou.mybatisplus.core.toolkit.support.LambdaMeta {
  public abstract java.lang.String getImplMethodName();
  public abstract java.lang.Class<?> getInstantiatedClass();
}
```

## `com.baomidou.mybatisplus.core.toolkit.support.ReflectLambdaMeta`

```java
public class com.baomidou.mybatisplus.core.toolkit.support.ReflectLambdaMeta implements com.baomidou.mybatisplus.core.toolkit.support.LambdaMeta {
  public com.baomidou.mybatisplus.core.toolkit.support.ReflectLambdaMeta(java.lang.invoke.SerializedLambda, java.lang.ClassLoader);
  public java.lang.String getImplMethodName();
  public java.lang.Class<?> getInstantiatedClass();
}
```

## `com.baomidou.mybatisplus.core.toolkit.support.SerializedLambda`

```java
public class com.baomidou.mybatisplus.core.toolkit.support.SerializedLambda implements java.io.Serializable {
  public com.baomidou.mybatisplus.core.toolkit.support.SerializedLambda();
  public static com.baomidou.mybatisplus.core.toolkit.support.SerializedLambda extract(java.io.Serializable);
  public java.lang.String getInstantiatedMethodType();
  public java.lang.Class<?> getCapturingClass();
  public java.lang.String getImplMethodName();
}
```

## `com.baomidou.mybatisplus.core.toolkit.support.ShadowLambdaMeta`

```java
public class com.baomidou.mybatisplus.core.toolkit.support.ShadowLambdaMeta implements com.baomidou.mybatisplus.core.toolkit.support.LambdaMeta {
  public com.baomidou.mybatisplus.core.toolkit.support.ShadowLambdaMeta(com.baomidou.mybatisplus.core.toolkit.support.SerializedLambda);
  public java.lang.String getImplMethodName();
  public java.lang.Class<?> getInstantiatedClass();
}
```
