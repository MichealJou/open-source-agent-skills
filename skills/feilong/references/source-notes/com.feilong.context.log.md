# com.feilong.context.log

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.context.log.AutoLog` | `String autoLog(String messagePattern,Object... params)` | auto输出日志 |
| `com.feilong.context.log.ContextLogCreator` | `String getContextLog()` | 创建固定的上下文. 分为两部分, 第一部分会自动获取http请求参数和地址 (如果是http请求 比如controller ),第二部分支持获取自定义的上下文, 比如后台应用 获取登录用户id name ; rpc应用获取调用应用名字和ip等等. |
| `com.feilong.context.log.FixedContextLogCreator` | `String createContextLog()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.log.HttpSpringFixedContextLogCreator` | `String createContextLog()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.log.LogContextExecutor` | `T call(String logKey,Callable<T> callable)` | 核心功能是日志上下文管理. |
| `com.feilong.context.log.LogContextExecutor` | `T call(String logKey,Callable<T> callable,ThrowableCallback throwableCallback)` | 核心功能是日志上下文管理. 如果exceptionCallback 不是null, 那么会回调调用,比如可以发钉钉提醒 |
| `com.feilong.context.log.LogContextExecutor` | `void run(String logKey,Runnable runnable)` | 无返回值的场景 |
| `com.feilong.context.log.LogCounterThreadLocal` | `AtomicInteger getCounter()` | 获取计步器. |
| `com.feilong.context.log.LogCounterThreadLocal` | `void beginCounter()` | 开始计步器. |
| `com.feilong.context.log.LogCounterThreadLocal` | `void removeCounter()` | 删除计步器. |
| `com.feilong.context.log.LogCounterThreadLocal` | `void setCounter(AtomicInteger counter)` | 设置计步器. |
| `com.feilong.context.log.LogKeyThreadLocal` | `String getLogKey()` | 获取通用日志. |
| `com.feilong.context.log.LogKeyThreadLocal` | `void appendLogKey(String appendLogKey)` | 追加通用日志. |
| `com.feilong.context.log.LogKeyThreadLocal` | `void removeLogKey()` | 删除通用日志. |
| `com.feilong.context.log.LogKeyThreadLocal` | `void setLogKey(String logKey)` | 设置通用日志. |
| `com.feilong.context.log.MqInfo` | `String getMqContent()` | 【原文待译】@return the mqContent |
| `com.feilong.context.log.MqInfo` | `String getMqQueueOrConsumer()` | 【原文待译】@return the mqQueueOrConsumer |
| `com.feilong.context.log.MqInfo` | `String getMqType()` | 【原文待译】@return the mqType |
| `com.feilong.context.log.MqInfo` | `String getReceiverApplication()` | 【原文待译】@return the receiverApplication |
| `com.feilong.context.log.MqInfo` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.log.MqInfo` | `void setMqContent(String mqContent)` | 【原文待译】@param mqContent the mqContent to set |
| `com.feilong.context.log.MqInfo` | `void setMqQueueOrConsumer(String mqQueueOrConsumer)` | 【原文待译】@param mqQueueOrConsumer the mqQueueOrConsumer to set |
| `com.feilong.context.log.MqInfo` | `void setMqType(String mqType)` | 【原文待译】@param mqType the mqType to set |
| `com.feilong.context.log.MqInfo` | `void setReceiverApplication(String receiverApplication)` | 【原文待译】@param receiverApplication the receiverApplication to set |
| `com.feilong.context.log.MqInfoThreadLocal` | `MqInfo getMqInfo()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.log.MqInfoThreadLocal` | `void removeMqInfo()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.log.MqInfoThreadLocal` | `void setMqInfo(MqInfo mqInfo)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.log.RequestLogHelper` | `String autoRequestInfo(HttpServletRequest request,String messagePattern,Object... params)` | 显性传入HttpServletRequest参数, 自动追加request简单信息. 此方法非常适用于filter里面, 因为filter先于springmvc无法自动获取HttpServletRequest对象 自动获取请求的路径和请求参数,前置追加类似于这种字符串 api:[http://mpay.feilong.com/subscribe/h5],paramString:[app_key=876*******14ec5f3c&third_party_order_no=XML*******95315×tamp=1733******111&sig=145ad********f84013467 |
| `com.feilong.context.log.RequestLogHelper` | `String autoRequestInfo(String messagePattern,Object... params)` | 自动追加request简单信息. 自动获取请求的路径和请求参数,前置追加类似于这种字符串 api:[http://mpay.feilong.com/subscribe/h5],paramString:[app_key=876*******14ec5f3c&third_party_order_no=XML*******95315×tamp=1733******111&sig=145ad********f84013467 |
| `com.feilong.context.log.ThrowableCallback` | `void callback(Throwable e)` | 【原文待译】Callback. |
