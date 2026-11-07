# cn.hutool.core.lang.loader

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.lang.loader.AtomicLoader` | `T get()` | 获取一个对象，第一次调用此方法时初始化对象然后返回，之后调用此方法直接返回原对象 |
| `cn.hutool.core.lang.loader.LazyFunLoader` | `LazyFunLoader<T> on(final Supplier<T> supplier)` | 静态工厂方法，提供语义性与编码便利性 |
| `cn.hutool.core.lang.loader.LazyFunLoader` | `boolean isInitialize()` | 是否已经初始化 |
| `cn.hutool.core.lang.loader.LazyFunLoader` | `void ifInitialized(Consumer<T> consumer)` | 如果已经初始化，就执行传入函数 |
| `cn.hutool.core.lang.loader.LazyLoader` | `T get()` | 获取一个对象，第一次调用此方法时初始化对象然后返回，之后调用此方法直接返回原对象 |
| `cn.hutool.core.lang.loader.Loader` | `T get()` | 获取一个准备好的对象 通过准备逻辑准备好被加载的对象，然后返回。在准备完毕之前此方法应该被阻塞 |
