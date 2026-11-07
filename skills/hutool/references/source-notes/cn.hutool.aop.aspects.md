# cn.hutool.aop.aspects

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.aop.aspects.Aspect` | `boolean after(Object target,Method method,Object[] args,Object returnVal)` | 目标方法执行后的操作 如果 target.method 抛出异常且 Aspect#afterException 返回true,则不会执行此操作 如果 Aspect#afterException 返回false,则无论target.method是否抛出异常，均会执行此操作 |
| `cn.hutool.aop.aspects.Aspect` | `boolean afterException(Object target,Method method,Object[] args,Throwable e)` | 目标方法抛出异常时的操作 |
| `cn.hutool.aop.aspects.Aspect` | `boolean before(Object target,Method method,Object[] args)` | 目标方法执行前的操作 |
| `cn.hutool.aop.aspects.SimpleAspect` | `boolean after(Object target,Method method,Object[] args,Object returnVal)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.aop.aspects.SimpleAspect` | `boolean afterException(Object target,Method method,Object[] args,Throwable e)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.aop.aspects.SimpleAspect` | `boolean before(Object target,Method method,Object[] args)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.aop.aspects.TimeIntervalAspect` | `boolean after(Object target,Method method,Object[] args,Object returnVal)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.aop.aspects.TimeIntervalAspect` | `boolean before(Object target,Method method,Object[] args)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
