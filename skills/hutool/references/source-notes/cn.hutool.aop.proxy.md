# cn.hutool.aop.proxy

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.aop.proxy.CglibProxyFactory` | `T proxy(T target,Aspect aspect)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.aop.proxy.JdkProxyFactory` | `T proxy(T target,Aspect aspect)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.aop.proxy.ProxyFactory` | `ProxyFactory create()` | 根据用户引入Cglib与否创建代理工厂 |
| `cn.hutool.aop.proxy.ProxyFactory` | `T createProxy(T target,Aspect aspect)` | 根据用户引入Cglib与否自动创建代理对象 |
| `cn.hutool.aop.proxy.ProxyFactory` | `T createProxy(T target,Class<? extends Aspect> aspectClass)` | 根据用户引入Cglib与否自动创建代理对象 |
| `cn.hutool.aop.proxy.ProxyFactory` | `T proxy(T target,Aspect aspect)` | 创建代理 |
| `cn.hutool.aop.proxy.ProxyFactory` | `T proxy(T target,Class<? extends Aspect> aspectClass)` | 创建代理 |
| `cn.hutool.aop.proxy.SpringCglibProxyFactory` | `T proxy(T target,Aspect aspect)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
