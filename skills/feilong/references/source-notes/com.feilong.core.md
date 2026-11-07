# com.feilong.core

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.core.Validate` | `T noNullElements(final T iterable,final String message,final Object... values)` | 【原文待译】Validate that the specified argument iterable is neither null nor contains any elements that are null; otherwise throwing an exception with the specified message. |
| `com.feilong.core.Validate` | `T notBlank(final T chars,final String message,final Object... values)` | 【原文待译】Validate that the specified argument character sequence is neither null, a length of zero (no characters), empty nor whitespace; otherwise throwing an exception with the specified message. |
| `com.feilong.core.Validate` | `T notEmpty(final T chars,final String message,final Object... values)` | 【原文待译】Validate that the specified argument character sequence is neither null nor a length of zero (no characters); otherwise throwing an exception with the specified message. |
| `com.feilong.core.Validate` | `T notEmpty(final T collection,final String message,final Object... values)` | 【原文待译】Validate that the specified argument collection is neither null nor a size of zero (no elements); otherwise throwing an exception with the specified message. |
| `com.feilong.core.Validate` | `T notEmpty(final T map,final String message,final Object... values)` | 【原文待译】Validate that the specified argument map is neither null nor a size of zero (no elements); otherwise throwing an exception with the specified message. |
| `com.feilong.core.Validate` | `T notNull(final T object,final String message,final Object... values)` | 【原文待译】Validate that the specified argument is not null; otherwise throwing an exception with the specified message. |
| `com.feilong.core.Validate` | `T[] noNullElements(final T[] array,final String message,final Object... values)` | 【原文待译】Validate that the specified argument array is neither null nor contains any elements that are null; otherwise throwing an exception with the specified message. |
| `com.feilong.core.Validate` | `T[] notEmpty(final T[] array,final String message,final Object... values)` | 【原文待译】Validate that the specified argument array is neither null nor a length of zero (no elements); otherwise throwing an exception with the specified message. |
| `com.feilong.core.Validate` | `void isTrue(final boolean expression,final String message,final Object... values)` | 【原文待译】Validate that the argument condition is true; otherwise throwing an exception with the specified message. This method is useful when validating according to an arbitrary boolean expression, such as validating a primitive number or using your own custom validation expression. |
| `com.feilong.core.Validate` | `void validState(final boolean expression,final String message,final Object... values)` | 【原文待译】Validate that the stateful condition is true; otherwise throwing an exception with the specified message. This method is useful when validating according to an arbitrary boolean expression, such as validating a primitive number or using your own custom validation expression. |
| `com.feilong.core.Validator` | `boolean isAllNullOrEmpty(Object... values)` | 判断所有元素 values 都是 null或者empty. |
| `com.feilong.core.Validator` | `boolean isAnyNullOrEmpty(Object... values)` | 判断内部任何对象 values 是不是 null或者empty. |
| `com.feilong.core.Validator` | `boolean isNotNullOrEmpty(Object value)` | 判断对象 value 是否不是null或者empty,调用 !#isNullOrEmpty(Object) 方法 . 示例参考 #isNullOrEmpty(Object) 方法 |
| `com.feilong.core.Validator` | `boolean isNotNullOrZero(Number value)` | 判断对象 value 是否不是null且不是0.,调用 !#isNullOrZero(Number) 方法 . |
| `com.feilong.core.Validator` | `boolean isNullOrEmpty(Object value)` | 判断对象 value 是不是 null或者empty. |
| `com.feilong.core.Validator` | `boolean isNullOrZero(Number value)` | 判断对象 value 是否是null或者是0. |
