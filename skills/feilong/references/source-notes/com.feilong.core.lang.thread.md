# com.feilong.core.lang.thread

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.core.lang.thread.AbstractPartitionThreadExecutor` | `void execute(List<T> list,int eachSize,Map<String, ?> paramsMap,PartitionRunnableBuilder<T> partitionRunnableBuilder)` | 执行. |
| `com.feilong.core.lang.thread.AbstractPartitionThreadExecutor` | `void execute(List<T> list,int eachSize,PartitionRunnableBuilder<T> partitionRunnableBuilder)` | 【原文待译】Excute. |
| `com.feilong.core.lang.thread.DefaultPartitionPerHandler` | `void handle(List<T> perBatchList,PartitionThreadEntity partitionThreadEntity,Map<String, ?> paramsMap)` | 【原文待译】Handle. |
| `com.feilong.core.lang.thread.DefaultPartitionRunnableBuilder` | `Runnable build(final List<T> perBatchList,final PartitionThreadEntity partitionThreadEntity,final Map<String, ?> paramsMap)` | 【原文待译】Builds the. |
| `com.feilong.core.lang.thread.PartitionEachSizeBuilder` | `int build(int totalSize)` | 【原文待译】Builds the. |
| `com.feilong.core.lang.thread.PartitionEachSizeThreadConfigBuilder` | `int build(int totalSize)` | 构造每个分区大小. |
| `com.feilong.core.lang.thread.PartitionEachSizeThreadConfigBuilder` | `void setPartitionThreadConfig(PartitionThreadConfig partitionThreadConfig)` | 【原文待译】Sets the partition thread config. |
| `com.feilong.core.lang.thread.PartitionPerElementHandler` | `void handle(T element,PartitionThreadEntity partitionThreadEntity,Map<String, ?> paramsMap)` | 【原文待译】Handle. |
| `com.feilong.core.lang.thread.PartitionPerHandler` | `void handle(List<T> perBatchList,PartitionThreadEntity partitionThreadEntity,Map<String, ?> paramsMap)` | 【原文待译】Handle. |
| `com.feilong.core.lang.thread.PartitionRunnableBuilder` | `Runnable build(List<T> perBatchList,PartitionThreadEntity partitionThreadEntity,Map<String, ?> paramsMap)` | 构造Runnable. |
| `com.feilong.core.lang.thread.PartitionThreadConfig` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.core.lang.thread.PartitionThreadConfig` | `int getMaxThreadCount()` | 获得 启动最大线程数. |
| `com.feilong.core.lang.thread.PartitionThreadConfig` | `int getMinPerThreadHandlerCount()` | 获得 每个线程最少处理数量. |
| `com.feilong.core.lang.thread.PartitionThreadConfig` | `void setMaxThreadCount(int maxThreadCount)` | 设置 启动最大线程数. |
| `com.feilong.core.lang.thread.PartitionThreadConfig` | `void setMinPerThreadHandlerCount(int minPerThreadHandlerCount)` | 设置 每个线程最少处理数量. |
| `com.feilong.core.lang.thread.PartitionThreadEntity` | `String getName()` | 获得 线程的名字. |
| `com.feilong.core.lang.thread.PartitionThreadEntity` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.core.lang.thread.PartitionThreadEntity` | `int getBatchNumber()` | 获得 批次,当前线程序号,从0开始. |
| `com.feilong.core.lang.thread.PartitionThreadEntity` | `int getCurrentListSize()` | 获得 当前线程执行数量,=perBatchList size. |
| `com.feilong.core.lang.thread.PartitionThreadEntity` | `int getEachSize()` | 获得 分配大小. |
| `com.feilong.core.lang.thread.PartitionThreadEntity` | `int getTotalListCount()` | 获得 总数,list 的总size. |
| `com.feilong.core.lang.thread.PartitionThreadExecutor` | `void execute(List<T> list,int eachSize,Map<String, ?> paramsMap,PartitionRunnableBuilder<T> partitionRunnableBuilder)` | 给定一个待解析的 list ,设定每个线程执行多少条 eachSize ,传入一些额外的参数 paramsMap ,使用自定义的 partitionRunnableBuilder ,自动 构造多条线程 并运行. 如果 list 是null,抛出 NullPointerException 如果 list 是empty,抛出 IllegalArgumentException 如果 eachSize 如果 partitionRunnableBuilder 是null,抛出 NullPointerException |
| `com.feilong.core.lang.thread.PartitionThreadExecutor` | `void execute(List<T> list,int eachSize,PartitionRunnableBuilder<T> partitionRunnableBuilder)` | 给定一个待解析的 list ,设定每个线程执行多少条 eachSize ,使用自定义的 partitionRunnableBuilder ,自动 构造多条线程 并运行. 如果 list 是null,抛出 NullPointerException 如果 list 是empty,抛出 IllegalArgumentException 如果 eachSize 如果 partitionRunnableBuilder 是null,抛出 NullPointerException |
