# cn.hutool.aop.proxy

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.aop.proxy.CglibProxyFactory`

```java
public class cn.hutool.aop.proxy.CglibProxyFactory extends cn.hutool.aop.proxy.ProxyFactory {
  public cn.hutool.aop.proxy.CglibProxyFactory();
  public <T> T proxy(T, cn.hutool.aop.aspects.Aspect);
}
```

## `cn.hutool.aop.proxy.JdkProxyFactory`

```java
public class cn.hutool.aop.proxy.JdkProxyFactory extends cn.hutool.aop.proxy.ProxyFactory {
  public cn.hutool.aop.proxy.JdkProxyFactory();
  public <T> T proxy(T, cn.hutool.aop.aspects.Aspect);
}
```

## `cn.hutool.aop.proxy.ProxyFactory`

```java
public abstract class cn.hutool.aop.proxy.ProxyFactory implements java.io.Serializable {
  public cn.hutool.aop.proxy.ProxyFactory();
  public <T> T proxy(T, java.lang.Class<? extends cn.hutool.aop.aspects.Aspect>);
  public abstract <T> T proxy(T, cn.hutool.aop.aspects.Aspect);
  public static <T> T createProxy(T, java.lang.Class<? extends cn.hutool.aop.aspects.Aspect>);
  public static <T> T createProxy(T, cn.hutool.aop.aspects.Aspect);
  public static cn.hutool.aop.proxy.ProxyFactory create();
}
```

## `cn.hutool.aop.proxy.SpringCglibProxyFactory`

```java
public class cn.hutool.aop.proxy.SpringCglibProxyFactory extends cn.hutool.aop.proxy.ProxyFactory {
  public cn.hutool.aop.proxy.SpringCglibProxyFactory();
  public <T> T proxy(T, cn.hutool.aop.aspects.Aspect);
}
```
