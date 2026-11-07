# com.google.common.base.internal

版本 33.4.8-jre。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.google.common.base.internal.Finalizer` | `void run()` | 【原文待译】Loops continuously, pulling references off the queue and cleaning them up. |
| `com.google.common.base.internal.Finalizer` | `void startFinalizer(Class<?> finalizableReferenceClass,ReferenceQueue<Object> queue,PhantomReference<Object> frqReference)` | 【原文待译】Starts the Finalizer thread. FinalizableReferenceQueue calls this method reflectively. |
