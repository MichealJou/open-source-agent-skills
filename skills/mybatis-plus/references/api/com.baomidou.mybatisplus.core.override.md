# com.baomidou.mybatisplus.core.override

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.override.MybatisMapperMethod`

```java
public class com.baomidou.mybatisplus.core.override.MybatisMapperMethod {
  public com.baomidou.mybatisplus.core.override.MybatisMapperMethod(java.lang.Class<?>, java.lang.reflect.Method, org.apache.ibatis.session.Configuration);
  public java.lang.Object execute(org.apache.ibatis.session.SqlSession, java.lang.Object[]);
}
```

## `com.baomidou.mybatisplus.core.override.MybatisMapperProxy`

```java
public class com.baomidou.mybatisplus.core.override.MybatisMapperProxy<T> implements java.lang.reflect.InvocationHandler, java.io.Serializable {
  public com.baomidou.mybatisplus.core.override.MybatisMapperProxy(org.apache.ibatis.session.SqlSession, java.lang.Class<T>, java.util.Map<java.lang.reflect.Method, com.baomidou.mybatisplus.core.override.MybatisMapperProxy$MapperMethodInvoker>);
  public java.lang.Object invoke(java.lang.Object, java.lang.reflect.Method, java.lang.Object[]) throws java.lang.Throwable;
  public org.apache.ibatis.session.SqlSession getSqlSession();
  public java.lang.Class<T> getMapperInterface();
}
```

## `com.baomidou.mybatisplus.core.override.MybatisMapperProxyFactory`

```java
public class com.baomidou.mybatisplus.core.override.MybatisMapperProxyFactory<T> {
  public com.baomidou.mybatisplus.core.override.MybatisMapperProxyFactory(java.lang.Class<T>);
  public T newInstance(org.apache.ibatis.session.SqlSession);
  public java.lang.Class<T> getMapperInterface();
  public java.util.Map<java.lang.reflect.Method, com.baomidou.mybatisplus.core.override.MybatisMapperProxy$MapperMethodInvoker> getMethodCache();
}
```
