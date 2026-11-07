# cn.hutool.cron.listener

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.cron.listener.SimpleTaskListener` | `void onFailed(TaskExecutor executor,Throwable exception)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.listener.SimpleTaskListener` | `void onStart(TaskExecutor executor)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.listener.SimpleTaskListener` | `void onSucceeded(TaskExecutor executor)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.listener.TaskListener` | `void onFailed(TaskExecutor executor,Throwable exception)` | 任务启动失败时触发 |
| `cn.hutool.cron.listener.TaskListener` | `void onStart(TaskExecutor executor)` | 定时任务启动时触发 |
| `cn.hutool.cron.listener.TaskListener` | `void onSucceeded(TaskExecutor executor)` | 任务成功结束时触发 |
| `cn.hutool.cron.listener.TaskListenerManager` | `TaskListenerManager addListener(TaskListener listener)` | 增加监听器 |
| `cn.hutool.cron.listener.TaskListenerManager` | `TaskListenerManager removeListener(TaskListener listener)` | 移除监听器 |
| `cn.hutool.cron.listener.TaskListenerManager` | `void notifyTaskFailed(TaskExecutor executor,Throwable exception)` | 通知所有监听任务启动器结束并失败 无监听将打印堆栈到命令行 |
| `cn.hutool.cron.listener.TaskListenerManager` | `void notifyTaskStart(TaskExecutor executor)` | 通知所有监听任务启动器启动 |
| `cn.hutool.cron.listener.TaskListenerManager` | `void notifyTaskSucceeded(TaskExecutor executor)` | 通知所有监听任务启动器成功结束 |
