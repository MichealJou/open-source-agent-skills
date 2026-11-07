# cn.hutool.aop

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.aop.ProxyUtil`

```java
public final class cn.hutool.aop.ProxyUtil {
  public cn.hutool.aop.ProxyUtil();
  public static <T> T proxy(T, java.lang.Class<? extends cn.hutool.aop.aspects.Aspect>);
  public static <T> T proxy(T, cn.hutool.aop.aspects.Aspect);
  public static <T> T newProxyInstance(java.lang.ClassLoader, java.lang.reflect.InvocationHandler, java.lang.Class<?>...);
  public static <T> T newProxyInstance(java.lang.reflect.InvocationHandler, java.lang.Class<?>...);
}
```
