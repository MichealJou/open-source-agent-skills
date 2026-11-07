# cn.hutool.cron

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.cron.CronConfig` | `CronConfig setMatchSecond(boolean isMatchSecond)` | 设置是否支持秒匹配，默认不使用 |
| `cn.hutool.cron.CronConfig` | `CronConfig setTimeZone(TimeZone timezone)` | 设置时区 |
| `cn.hutool.cron.CronConfig` | `TimeZone getTimeZone()` | 获得时区，默认为 TimeZone#getDefault() |
| `cn.hutool.cron.CronConfig` | `boolean isMatchSecond()` | 是否支持秒匹配 |
| `cn.hutool.cron.CronTimer` | `void run()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.CronTimer` | `void stopTimer()` | 关闭定时器 |
| `cn.hutool.cron.CronUtil` | `Scheduler getScheduler()` | @return 获得Scheduler对象 |
| `cn.hutool.cron.CronUtil` | `String schedule(String id,String schedulingPattern,Task task)` | 加入定时任务 |
| `cn.hutool.cron.CronUtil` | `String schedule(String schedulingPattern,Runnable task)` | 加入定时任务 |
| `cn.hutool.cron.CronUtil` | `String schedule(String schedulingPattern,Task task)` | 加入定时任务 |
| `cn.hutool.cron.CronUtil` | `boolean remove(String schedulerId)` | 移除任务 |
| `cn.hutool.cron.CronUtil` | `void restart()` | 重新启动定时任务 此方法会清除动态加载的任务，重新启动后，守护线程与否与之前保持一致 |
| `cn.hutool.cron.CronUtil` | `void schedule(Setting cronSetting)` | 批量加入配置文件中的定时任务 |
| `cn.hutool.cron.CronUtil` | `void setCronSetting(Setting cronSetting)` | 自定义定时任务配置文件 |
| `cn.hutool.cron.CronUtil` | `void setCronSetting(String cronSettingPath)` | 自定义定时任务配置文件路径 |
| `cn.hutool.cron.CronUtil` | `void setMatchSecond(boolean isMatchSecond)` | 设置是否支持秒匹配 此方法用于定义是否使用秒匹配模式，如果为true，则定时任务表达式中的第一位为秒，否则为分，默认是分 |
| `cn.hutool.cron.CronUtil` | `void start()` | 开始，非守护线程模式 |
| `cn.hutool.cron.CronUtil` | `void start(boolean isDaemon)` | 开始 |
| `cn.hutool.cron.CronUtil` | `void stop()` | 停止 |
| `cn.hutool.cron.CronUtil` | `void updatePattern(String id,CronPattern pattern)` | 更新Task的执行时间规则 |
| `cn.hutool.cron.Scheduler` | `CronPattern getPattern(String id)` | 获得指定id的CronPattern |
| `cn.hutool.cron.Scheduler` | `Scheduler addListener(TaskListener listener)` | 增加监听器 |
| `cn.hutool.cron.Scheduler` | `Scheduler clear()` | 清空任务表 |
| `cn.hutool.cron.Scheduler` | `Scheduler deschedule(String id)` | 移除Task |
| `cn.hutool.cron.Scheduler` | `Scheduler removeListener(TaskListener listener)` | 移除监听器 |
| `cn.hutool.cron.Scheduler` | `Scheduler schedule(Setting cronSetting)` | 批量加入配置文件中的定时任务 配置文件格式为： xxx.xxx.xxx.Class.method = * * * * * |
| `cn.hutool.cron.Scheduler` | `Scheduler schedule(String id,CronPattern pattern,Task task)` | 新增Task，如果任务ID已经存在，抛出异常 |
| `cn.hutool.cron.Scheduler` | `Scheduler schedule(String id,String pattern,Runnable task)` | 新增Task，如果任务ID已经存在，抛出异常 |
| `cn.hutool.cron.Scheduler` | `Scheduler schedule(String id,String pattern,Task task)` | 新增Task，如果任务ID已经存在，抛出异常 |
| `cn.hutool.cron.Scheduler` | `Scheduler setDaemon(boolean on)` | 设置是否为守护线程 如果为true，则在调用#stop()方法后执行的定时任务立即结束，否则等待执行完毕才结束。默认非守护线程 如果用户调用#setThreadExecutor(ExecutorService)自定义线程池则此参数无效 |
| `cn.hutool.cron.Scheduler` | `Scheduler setMatchSecond(boolean isMatchSecond)` | 设置是否支持秒匹配，默认不使用 |
| `cn.hutool.cron.Scheduler` | `Scheduler setThreadExecutor(ExecutorService threadExecutor)` | 设置自定义线程池 自定义线程池时须考虑方法执行的线程是否为守护线程 |
| `cn.hutool.cron.Scheduler` | `Scheduler setTimeZone(TimeZone timeZone)` | 设置时区 |
| `cn.hutool.cron.Scheduler` | `Scheduler start()` | 启动 |
| `cn.hutool.cron.Scheduler` | `Scheduler start(boolean isDaemon)` | 启动 |
| `cn.hutool.cron.Scheduler` | `Scheduler stop()` | 停止定时任务 此方法调用后会将定时器进程立即结束，如果为守护线程模式，则正在执行的作业也会自动结束，否则作业线程将在执行完成后结束。 此方法并不会清除任务表中的任务，请调用#clear() 方法清空任务或者使用#stop(boolean)方法可选是否清空 |
| `cn.hutool.cron.Scheduler` | `Scheduler stop(boolean clearTasks)` | 停止定时任务 此方法调用后会将定时器进程立即结束，如果为守护线程模式，则正在执行的作业也会自动结束，否则作业线程将在执行完成后结束。 |
| `cn.hutool.cron.Scheduler` | `Scheduler updatePattern(String id,CronPattern pattern)` | 更新Task执行的时间规则 |
| `cn.hutool.cron.Scheduler` | `String schedule(String pattern,Runnable task)` | 新增Task，使用随机UUID |
| `cn.hutool.cron.Scheduler` | `String schedule(String pattern,Task task)` | 新增Task，使用随机UUID |
| `cn.hutool.cron.Scheduler` | `Task getTask(String id)` | 获得指定id的Task |
| `cn.hutool.cron.Scheduler` | `TaskTable getTaskTable()` | 获取定时任务表，注意此方法返回非复制对象，对返回对象的修改将影响已有定时任务 |
| `cn.hutool.cron.Scheduler` | `TimeZone getTimeZone()` | 获得时区，默认为 TimeZone#getDefault() |
| `cn.hutool.cron.Scheduler` | `boolean descheduleWithStatus(String id)` | 移除Task，并返回是否移除成功 |
| `cn.hutool.cron.Scheduler` | `boolean isDaemon()` | 是否为守护线程 |
| `cn.hutool.cron.Scheduler` | `boolean isEmpty()` | 是否无任务 |
| `cn.hutool.cron.Scheduler` | `boolean isMatchSecond()` | 是否支持秒匹配 |
| `cn.hutool.cron.Scheduler` | `boolean isStarted()` | @return 是否已经启动 |
| `cn.hutool.cron.Scheduler` | `int size()` | 当前任务数 |
| `cn.hutool.cron.TaskExecutor` | `CronTask getCronTask()` | 获得原始任务对象 |
| `cn.hutool.cron.TaskExecutor` | `Task getTask()` | 获得原始任务对象 |
| `cn.hutool.cron.TaskExecutor` | `void run()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.TaskExecutorManager` | `List<TaskExecutor> getExecutors()` | 获取所有正在执行的任务调度执行器 |
| `cn.hutool.cron.TaskExecutorManager` | `TaskExecutor spawnExecutor(CronTask task)` | 启动 执行器TaskExecutor，即启动作业 |
| `cn.hutool.cron.TaskExecutorManager` | `TaskExecutorManager notifyExecutorCompleted(TaskExecutor executor)` | 执行器执行完毕调用此方法，将执行器从执行器列表移除，此方法由TaskExecutor对象调用，用于通知管理器自身已完成执行 |
| `cn.hutool.cron.TaskLauncher` | `void run()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.TaskTable` | `CronPattern getPattern(String id)` | 获得指定id的CronPattern |
| `cn.hutool.cron.TaskTable` | `CronPattern getPattern(int index)` | 获得指定位置的CronPattern |
| `cn.hutool.cron.TaskTable` | `List<CronPattern> getPatterns()` | 获取所有定时任务表达式，返回不可变列表，即列表不可修改 |
| `cn.hutool.cron.TaskTable` | `List<String> getIds()` | 获取所有ID，返回不可变列表，即列表不可修改 |
| `cn.hutool.cron.TaskTable` | `List<Task> getTasks()` | 获取所有定时任务，返回不可变列表，即列表不可修改 |
| `cn.hutool.cron.TaskTable` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.TaskTable` | `Task getTask(String id)` | 获得指定id的Task |
| `cn.hutool.cron.TaskTable` | `Task getTask(int index)` | 获得指定位置的Task |
| `cn.hutool.cron.TaskTable` | `TaskTable add(String id,CronPattern pattern,Task task)` | 新增Task |
| `cn.hutool.cron.TaskTable` | `boolean isEmpty()` | 任务表是否为空 |
| `cn.hutool.cron.TaskTable` | `boolean remove(String id)` | 移除Task |
| `cn.hutool.cron.TaskTable` | `boolean updatePattern(String id,CronPattern pattern)` | 更新某个Task的定时规则 |
| `cn.hutool.cron.TaskTable` | `int size()` | 任务表大小，加入的任务数 |
| `cn.hutool.cron.TaskTable` | `void executeTaskIfMatch(Scheduler scheduler,long millis)` | 如果时间匹配则执行相应的Task，带读锁 |
