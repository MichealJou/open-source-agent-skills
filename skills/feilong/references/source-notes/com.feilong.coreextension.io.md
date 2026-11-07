# com.feilong.coreextension.io

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.coreextension.io.SerializableUtil` | `String toString(Serializable serializable)` | 【原文待译】To string. |
| `com.feilong.coreextension.io.SerializableUtil` | `T deserialize(byte[] objectData)` | 【原文待译】Deserialize. |
| `com.feilong.coreextension.io.SerializableUtil` | `T toObject(String serializableString)` | 【原文待译】To object. |
| `com.feilong.coreextension.io.SerializableUtil` | `byte[] serialize(Serializable serializable)` | 【原文待译】To byte array. |
| `com.feilong.coreextension.io.SerializableUtil` | `int size(Serializable serializable)` | 返回对象内存大小. 只有支持 java.io.Serializable Serializable或 java.io.Externalizable Externalizable 接口的对象才能被 java.io.ObjectInputStream ObjectInputStream/java.io.ObjectOutputStream ObjectOutputStream所操作！ |
