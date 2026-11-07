# cn.hutool.core.io.copy

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.io.copy.ChannelCopier` | `long copy(ReadableByteChannel source,WritableByteChannel target)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.copy.IoCopier` | `IoCopier<S, T> setFlushEveryBuffer(boolean flushEveryBuffer)` | 设置是否每次写出一个buffer内容就执行flush |
| `cn.hutool.core.io.copy.IoCopier` | `long copy(S source,T target)` | 执行拷贝 |
| `cn.hutool.core.io.copy.ReaderWriterCopier` | `long copy(Reader source,Writer target)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.copy.StreamCopier` | `long copy(InputStream source,OutputStream target)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
