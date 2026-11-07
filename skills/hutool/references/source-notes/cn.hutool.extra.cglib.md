# cn.hutool.extra.cglib

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.cglib.BeanCopierCache` | `BeanCopier get(Class<?> srcClass,Class<?> targetClass,Converter converter)` | 获得类与转换器生成的key在BeanCopier的Map中对应的元素 |
| `cn.hutool.extra.cglib.BeanCopierCache` | `BeanCopier get(Class<?> srcClass,Class<?> targetClass,boolean useConverter)` | 获得类与转换器生成的key在BeanCopier的Map中对应的元素 |
| `cn.hutool.extra.cglib.CglibUtil` | `BeanMap toMap(Object bean)` | 将Bean转换为Map |
| `cn.hutool.extra.cglib.CglibUtil` | `List<T> copyList(Collection<S> source,Supplier<T> target)` | 拷贝List Bean对象属性 |
| `cn.hutool.extra.cglib.CglibUtil` | `List<T> copyList(Collection<S> source,Supplier<T> target,BiConsumer<S, T> callback)` | 拷贝List Bean对象属性 |
| `cn.hutool.extra.cglib.CglibUtil` | `List<T> copyList(Collection<S> source,Supplier<T> target,Converter converter)` | 拷贝List Bean对象属性 |
| `cn.hutool.extra.cglib.CglibUtil` | `List<T> copyList(Collection<S> source,Supplier<T> target,Converter converter,BiConsumer<S, T> callback)` | 拷贝List Bean对象属性 |
| `cn.hutool.extra.cglib.CglibUtil` | `T copy(Object source,Class<T> targetClass)` | 拷贝Bean对象属性到目标类型 此方法通过指定目标类型自动创建之，然后拷贝属性 |
| `cn.hutool.extra.cglib.CglibUtil` | `T copy(Object source,Class<T> targetClass,Converter converter)` | 拷贝Bean对象属性 此方法通过指定目标类型自动创建之，然后拷贝属性 |
| `cn.hutool.extra.cglib.CglibUtil` | `T fillBean(Map map,T bean)` | 将Map中的内容填充至Bean中 |
| `cn.hutool.extra.cglib.CglibUtil` | `T toBean(Map map,Class<T> beanClass)` | 将Map转换为Bean |
| `cn.hutool.extra.cglib.CglibUtil` | `void copy(Object source,Object target)` | 拷贝Bean对象属性 |
| `cn.hutool.extra.cglib.CglibUtil` | `void copy(Object source,Object target,Converter converter)` | 拷贝Bean对象属性 |
