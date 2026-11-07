# com.feilong.context

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.context.AbstractDataListTask` | `Void run()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.AbstractDataListTask` | `void setDataListQuery(DataListQuery<T> dataListQuery)` | 设置 需要被处理的数据查询器. |
| `com.feilong.context.BeanLogMessageBuilder` | `String buildFieldsMessage(Object obj)` | 生成对象字段相关日志信息. |
| `com.feilong.context.BeanLogMessageBuilder` | `String buildFieldsSimpleMessage(Object obj)` | 生成对象字段相关日志信息. |
| `com.feilong.context.Condition` | `boolean canRun()` | 是否可以执行. |
| `com.feilong.context.ConditionableTask` | `T run()` | 【原文待译】Run. |
| `com.feilong.context.ConditionableTask` | `void setCondition(Condition condition)` | 设置 执行条件. |
| `com.feilong.context.ConditionableTask` | `void setTask(Task<T> task)` | 设置 task. |
| `com.feilong.context.DataHandler` | `void handle(Map<String, Object> data)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.DataListQuery` | `List<T> query()` | 查询数据. |
| `com.feilong.context.FileReworker` | `String rework(String filePath)` | 【原文待译】Rework. |
| `com.feilong.context.MapBuilder` | `Map<String, Object> build(T bean)` | 构造. |
| `com.feilong.context.MemberIdBuilder` | `T build(HttpServletRequest request)` | 基于request得到当前用户的id. 支持构造游客的member Id,比如有些商城固定member id 是 1 |
| `com.feilong.context.ObjectValidator` | `void validate(T input)` | 校验. 如果校验不通过,请直接抛出异常 |
| `com.feilong.context.Rebuilder` | `T rebuild(T t)` | 重新加工. |
| `com.feilong.context.RequestDataBuilder` | `Map<String, Object> build(HttpServletRequest request)` | 【原文待译】Builds the. |
| `com.feilong.context.ReturnResult` | `String getStatusCode()` | 返回状态码（可选值）. 通常操作失败了 isSuccess为false 的时候,会设置值 |
| `com.feilong.context.ReturnResult` | `T getReturnData()` | 对应返回的数据对象（可选值）. 比如,成功了可以放一个bean返回回去以便调用,失败了也可以放一段字符串 等等. |
| `com.feilong.context.ReturnResult` | `boolean getIsSuccess()` | 操作是否成功,默认成功. |
| `com.feilong.context.ReturnResult` | `void setIsSuccess(boolean isSuccess)` | 操作是否成功,默认成功. |
| `com.feilong.context.ReturnResult` | `void setReturnData(T returnData)` | 对应返回的数据对象（可选值）. 比如,成功了可以放一个bean返回回去以便调用,失败了也可以放一段字符串 等等. |
| `com.feilong.context.ReturnResult` | `void setStatusCode(String statusCode)` | 返回状态码（可选值）. 通常操作失败了 isSuccess为false 的时候,会设置值 |
| `com.feilong.context.ReturnResultBuilder` | `ReturnResult<Object> buildFailureResult(String statusCode)` | 构造带statusCode 的失败结果. |
| `com.feilong.context.SimpleParamNameConfigCondition` | `boolean canRun()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.SimpleParamNameConfigCondition` | `void setSimpleParamNameValueLoader(SimpleParamNameValueLoader<Boolean> simpleParamNameValueLoader)` | 【原文待译】Sets the simple param name value loader. |
| `com.feilong.context.SimpleParamNameValueLoader` | `V load()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.SimpleParamNameValueLoader` | `void setIfNullDefaultValue(V ifNullDefaultValue)` | 设置 如果是 null 默认值. |
| `com.feilong.context.SimpleParamNameValueLoader` | `void setParamName(String paramName)` | 设置 参数名字. |
| `com.feilong.context.SimpleParamNameValueLoader` | `void setStringValueParamLoader(StringValueParamLoader<V> stringValueParamLoader)` | 设置 value param loader. |
| `com.feilong.context.SimpleParamNameValueLoader` | `void setTargetTypeClass(Class<V> targetTypeClass)` | 设置 target type class. |
| `com.feilong.context.SimpleValueLoader` | `V load()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.context.SimpleValueLoader` | `void setV(V v)` | 【原文待译】Sets the v. |
| `com.feilong.context.Task` | `T run()` | 【原文待译】run. |
| `com.feilong.context.ValidatorHandler` | `ValidatorHandlerResult validate(T t)` | 【原文待译】Validate. |
| `com.feilong.context.ValueLoader` | `V load()` | 【原文待译】Load. |
| `com.feilong.context.ValueParamLoader` | `V load(T t)` | 【原文待译】Load. |
