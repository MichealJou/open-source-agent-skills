# com.google.common.annotations

版本 33.4.8-jre。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.google.common.annotations.GwtCompatible` | `boolean emulated()` | 【原文待译】When true, the annotated type is emulated in GWT. The emulated source (also known as super-source) is different from the implementation used by the JVM. |
| `com.google.common.annotations.GwtCompatible` | `boolean serializable()` | 【原文待译】When true, the annotated type or the type of the method return value is GWT serializable. |
| `com.google.common.annotations.GwtIncompatible` | `String value()` | 【原文待译】Describes why the annotated element is incompatible with GWT. Since this is generally due to a dependence on a type/method which GWT doesn't support, it is sufficient to simply reference the unsupported type/method. E.g. "Class.isInstance". As of Guava 20.0, this value is optional. We encourage auth… |
