# cn.hutool.aop

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.aop.ProxyUtil` | `T newProxyInstance(ClassLoader classloader,InvocationHandler invocationHandler,Class<?>... interfaces)` | 创建动态代理对象 动态代理对象的创建原理是： 假设创建的代理对象名为 $Proxy0 1、根据传入的interfaces动态生成一个类，实现interfaces中的接口 2、通过传入的classloder将刚生成的类加载到jvm中。即将$Proxy0类load 3、调用$Proxy0的$Proxy0(InvocationHandler)构造函数 创建$Proxy0的对象，并且用interfaces参数遍历其所有接口的方法，这些实现方法的实现本质上是通过反射调用被代理对象的方法 4、将$Proxy0的实例返回给客户端。 5、当调用代理类的相应方法时，相当于调用 InvocationHandler… |
| `cn.hutool.aop.ProxyUtil` | `T newProxyInstance(InvocationHandler invocationHandler,Class<?>... interfaces)` | 创建动态代理对象 |
| `cn.hutool.aop.ProxyUtil` | `T proxy(T target,Aspect aspect)` | 使用切面代理对象 |
| `cn.hutool.aop.ProxyUtil` | `T proxy(T target,Class<? extends Aspect> aspectClass)` | 使用切面代理对象 |
