# cn.hutool.core.lang.intern

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.lang.intern.InternUtil` | `Interner<String> createJdkInterner()` | 创建JDK默认实现的字符串规范化器 |
| `cn.hutool.core.lang.intern.InternUtil` | `Interner<String> createStringInterner(boolean isWeak)` | 创建字符串规范化器 |
| `cn.hutool.core.lang.intern.InternUtil` | `Interner<T> createWeakInterner()` | 创建WeakHshMap实现的字符串规范化器 |
| `cn.hutool.core.lang.intern.Interner` | `T intern(T sample)` | 返回指定对象对应的规范化对象，sample对象可能有多个，但是这些对象如果都equals，则返回的是同一个对象 |
| `cn.hutool.core.lang.intern.JdkStringInterner` | `String intern(String sample)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.intern.WeakInterner` | `T intern(T sample)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
