# cn.hutool.aop.interceptor

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.aop.interceptor.CglibInterceptor`

```java
public class cn.hutool.aop.interceptor.CglibInterceptor implements net.sf.cglib.proxy.MethodInterceptor,java.io.Serializable {
  public cn.hutool.aop.interceptor.CglibInterceptor(java.lang.Object, cn.hutool.aop.aspects.Aspect);
  public java.lang.Object getTarget();
  public java.lang.Object intercept(java.lang.Object, java.lang.reflect.Method, java.lang.Object[], net.sf.cglib.proxy.MethodProxy) throws java.lang.Throwable;
}
```

## `cn.hutool.aop.interceptor.JdkInterceptor`

```java
public class cn.hutool.aop.interceptor.JdkInterceptor implements java.lang.reflect.InvocationHandler,java.io.Serializable {
  public cn.hutool.aop.interceptor.JdkInterceptor(java.lang.Object, cn.hutool.aop.aspects.Aspect);
  public java.lang.Object getTarget();
  public java.lang.Object invoke(java.lang.Object, java.lang.reflect.Method, java.lang.Object[]) throws java.lang.Throwable;
}
```

## `cn.hutool.aop.interceptor.SpringCglibInterceptor`

```java
public class cn.hutool.aop.interceptor.SpringCglibInterceptor implements org.springframework.cglib.proxy.MethodInterceptor,java.io.Serializable {
  public cn.hutool.aop.interceptor.SpringCglibInterceptor(java.lang.Object, cn.hutool.aop.aspects.Aspect);
  public java.lang.Object getTarget();
  public java.lang.Object intercept(java.lang.Object, java.lang.reflect.Method, java.lang.Object[], org.springframework.cglib.proxy.MethodProxy) throws java.lang.Throwable;
}
```
