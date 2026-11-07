# cn.hutool.cron.timingwheel

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.cron.timingwheel.SystemTimer` | `SystemTimer setDelayQueueTimeout(long delayQueueTimeout)` | 设置执行队列取元素超时时长，单位毫秒 |
| `cn.hutool.cron.timingwheel.SystemTimer` | `SystemTimer start()` | 启动，异步 |
| `cn.hutool.cron.timingwheel.SystemTimer` | `void addTask(TimerTask timerTask)` | 添加任务 |
| `cn.hutool.cron.timingwheel.SystemTimer` | `void stop()` | 强制结束 |
| `cn.hutool.cron.timingwheel.TimerTask` | `Runnable getTask()` | 获取任务 |
| `cn.hutool.cron.timingwheel.TimerTask` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.timingwheel.TimerTask` | `long getDelayMs()` | 获取延迟时间点，即创建时间+延迟时长（单位毫秒） |
| `cn.hutool.cron.timingwheel.TimerTaskList` | `boolean setExpiration(long expire)` | 设置过期时间 |
| `cn.hutool.cron.timingwheel.TimerTaskList` | `int compareTo(Delayed o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.timingwheel.TimerTaskList` | `long getDelay(TimeUnit unit)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.cron.timingwheel.TimerTaskList` | `long getExpire()` | 获取过期时间 |
| `cn.hutool.cron.timingwheel.TimerTaskList` | `void addTask(TimerTask timerTask)` | 新增任务，将任务加入到双向链表的头部 |
| `cn.hutool.cron.timingwheel.TimerTaskList` | `void flush(Consumer<TimerTask> flush)` | 重新分配，即将列表中的任务全部处理 |
| `cn.hutool.cron.timingwheel.TimerTaskList` | `void removeTask(TimerTask timerTask)` | 移除任务 |
| `cn.hutool.cron.timingwheel.TimingWheel` | `boolean addTask(TimerTask timerTask)` | 添加任务到时间轮 |
| `cn.hutool.cron.timingwheel.TimingWheel` | `void advanceClock(long timestamp)` | 推进时间 |
