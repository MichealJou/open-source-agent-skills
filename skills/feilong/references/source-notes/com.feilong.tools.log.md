# com.feilong.tools.log

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.tools.log.LogHelper` | `String getProcessLog(ProcessLogParamEntity processLogParamEntity)` | 用来渲染进度日志的. |
| `com.feilong.tools.log.ProcessLogParamEntity` | `Long getAllBeginTimeMillis()` | 获得 所有开始执行的开始时间. |
| `com.feilong.tools.log.ProcessLogParamEntity` | `Long getCurrentBeginTimeMillis()` | 获得 当前执行的开始时间. |
| `com.feilong.tools.log.ProcessLogParamEntity` | `Number getAll()` | 获得 需要执行的总数. |
| `com.feilong.tools.log.ProcessLogParamEntity` | `Number getCurrent()` | 获得 当前执行到哪个位置. |
| `com.feilong.tools.log.ProcessLogParamEntity` | `void setAll(Number all)` | 设置 需要执行的总数. |
| `com.feilong.tools.log.ProcessLogParamEntity` | `void setAllBeginTimeMillis(Long allBeginTimeMillis)` | 设置 所有开始执行的开始时间. |
| `com.feilong.tools.log.ProcessLogParamEntity` | `void setCurrent(Number current)` | 设置 当前执行到哪个位置. |
| `com.feilong.tools.log.ProcessLogParamEntity` | `void setCurrentBeginTimeMillis(Long currentBeginTimeMillis)` | 设置 当前执行的开始时间. |
