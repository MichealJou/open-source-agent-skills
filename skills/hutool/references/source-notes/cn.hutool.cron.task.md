# cn.hutool.cron.task

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.cron.task.CronTask` | `CronPattern getPattern()` | 获取表达式 |
| `cn.hutool.cron.task.CronTask` | `CronTask setPattern(CronPattern pattern)` | 设置新的定时表达式 |
| `cn.hutool.cron.task.CronTask` | `String getId()` | 获取作业ID |
| `cn.hutool.cron.task.CronTask` | `Task getRaw()` | 获取原始作业 |
| `cn.hutool.cron.task.CronTask` | `void execute()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.task.InvokeTask` | `void execute()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.task.RunnableTask` | `void execute()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.task.Task` | `void execute()` | 执行作业 作业的具体实现需考虑异常情况，默认情况下任务异常在监听中统一监听处理，如果不加入监听，异常会被忽略 因此最好自行捕获异常后处理 |
