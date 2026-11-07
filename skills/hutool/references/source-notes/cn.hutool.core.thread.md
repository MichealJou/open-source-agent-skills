# cn.hutool.core.thread

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.thread.AsyncUtil` | `T get(CompletableFuture<T> task)` | 获取异步任务结果，包裹了异常 |
| `cn.hutool.core.thread.AsyncUtil` | `T waitAny(CompletableFuture<?>... tasks)` | 等待任意一个任务执行完毕，包裹了异常 |
| `cn.hutool.core.thread.AsyncUtil` | `void waitAll(CompletableFuture<?>... tasks)` | 等待所有任务执行完毕，包裹了异常 |
| `cn.hutool.core.thread.BlockPolicy` | `void rejectedExecution(Runnable r,ThreadPoolExecutor e)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.ConcurrencyTester` | `ConcurrencyTester reset()` | 重置测试器，重置包括： 清空worker 重置计时器 |
| `cn.hutool.core.thread.ConcurrencyTester` | `ConcurrencyTester test(Runnable runnable)` | 执行测试 执行测试后不会关闭线程池，可以调用#close()释放线程池 |
| `cn.hutool.core.thread.ConcurrencyTester` | `long getInterval()` | 获取执行时间 |
| `cn.hutool.core.thread.ConcurrencyTester` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.DelegatedExecutorService` | `Future<?> submit(Runnable task)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.DelegatedExecutorService` | `Future<T> submit(Callable<T> task)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.DelegatedExecutorService` | `Future<T> submit(Runnable task,T result)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.DelegatedExecutorService` | `List<Future<T>> invokeAll(Collection<? extends Callable<T>> tasks)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.DelegatedExecutorService` | `List<Future<T>> invokeAll(Collection<? extends Callable<T>> tasks,long timeout,TimeUnit unit)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.DelegatedExecutorService` | `List<Runnable> shutdownNow()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.DelegatedExecutorService` | `T invokeAny(Collection<? extends Callable<T>> tasks)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.DelegatedExecutorService` | `T invokeAny(Collection<? extends Callable<T>> tasks,long timeout,TimeUnit unit)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.DelegatedExecutorService` | `boolean awaitTermination(long timeout,TimeUnit unit)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.DelegatedExecutorService` | `boolean isShutdown()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.DelegatedExecutorService` | `boolean isTerminated()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.DelegatedExecutorService` | `void execute(Runnable command)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.DelegatedExecutorService` | `void shutdown()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.ExecutorBuilder` | `ExecutorBuilder create()` | 创建ExecutorBuilder，开始构建 |
| `cn.hutool.core.thread.ExecutorBuilder` | `ExecutorBuilder setAllowCoreThreadTimeOut(boolean allowCoreThreadTimeOut)` | 设置线程执行超时后是否回收线程 |
| `cn.hutool.core.thread.ExecutorBuilder` | `ExecutorBuilder setCorePoolSize(int corePoolSize)` | 设置初始池大小，默认0 |
| `cn.hutool.core.thread.ExecutorBuilder` | `ExecutorBuilder setHandler(RejectedExecutionHandler handler)` | 设置当线程阻塞（block）时的异常处理器，所谓线程阻塞即线程池和等待队列已满，无法处理线程时采取的策略 此处可以使用JDK预定义的几种策略，见RejectPolicy枚举 |
| `cn.hutool.core.thread.ExecutorBuilder` | `ExecutorBuilder setKeepAliveTime(long keepAliveTime)` | 设置线程存活时间，即当池中线程多于初始大小时，多出的线程保留的时长，单位纳秒 |
| `cn.hutool.core.thread.ExecutorBuilder` | `ExecutorBuilder setKeepAliveTime(long keepAliveTime,TimeUnit unit)` | 设置线程存活时间，即当池中线程多于初始大小时，多出的线程保留的时长 |
| `cn.hutool.core.thread.ExecutorBuilder` | `ExecutorBuilder setMaxPoolSize(int maxPoolSize)` | 设置最大池大小（允许同时执行的最大线程数） |
| `cn.hutool.core.thread.ExecutorBuilder` | `ExecutorBuilder setThreadFactory(ThreadFactory threadFactory)` | 设置线程工厂，用于自定义线程创建 |
| `cn.hutool.core.thread.ExecutorBuilder` | `ExecutorBuilder setWorkQueue(BlockingQueue<Runnable> workQueue)` | 设置队列，用于存在未执行的线程 可选队列有： |
| `cn.hutool.core.thread.ExecutorBuilder` | `ExecutorBuilder useArrayBlockingQueue(int capacity)` | 使用ArrayBlockingQueue 做为等待队列 有界队列，相对无界队列有利于控制队列大小，队列满时，运行线程小于maxPoolSize时会创建新线程，否则触发异常策略 |
| `cn.hutool.core.thread.ExecutorBuilder` | `ExecutorBuilder useSynchronousQueue()` | 使用SynchronousQueue 做为等待队列（非公平策略） 它将任务直接提交给线程而不保持它们。当运行线程小于maxPoolSize时会创建新线程，否则触发异常策略 |
| `cn.hutool.core.thread.ExecutorBuilder` | `ExecutorBuilder useSynchronousQueue(boolean fair)` | 使用SynchronousQueue 做为等待队列 它将任务直接提交给线程而不保持它们。当运行线程小于maxPoolSize时会创建新线程，否则触发异常策略 |
| `cn.hutool.core.thread.ExecutorBuilder` | `ExecutorService buildFinalizable()` | 创建有回收关闭功能的ExecutorService |
| `cn.hutool.core.thread.ExecutorBuilder` | `ThreadPoolExecutor build()` | 构建ThreadPoolExecutor |
| `cn.hutool.core.thread.GlobalThreadPool` | `ExecutorService getExecutor()` | 获得 ExecutorService |
| `cn.hutool.core.thread.GlobalThreadPool` | `Future<?> submit(Runnable runnable)` | 执行有返回值的异步方法 Future代表一个异步执行的操作，通过get()方法可以获得操作的结果，如果异步操作还没有完成，则，get()会使当前线程阻塞 |
| `cn.hutool.core.thread.GlobalThreadPool` | `Future<T> submit(Callable<T> task)` | 执行有返回值的异步方法 Future代表一个异步执行的操作，通过get()方法可以获得操作的结果，如果异步操作还没有完成，则，get()会使当前线程阻塞 |
| `cn.hutool.core.thread.GlobalThreadPool` | `void execute(Runnable runnable)` | 直接在公共线程池中执行线程 |
| `cn.hutool.core.thread.GlobalThreadPool` | `void init()` | 初始化全局线程池 |
| `cn.hutool.core.thread.GlobalThreadPool` | `void shutdown(boolean isNow)` | 关闭公共线程池 |
| `cn.hutool.core.thread.NamedThreadFactory` | `Thread newThread(Runnable r)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor` | `ExecutorService getExecutor()` | 获取线程池 |
| `cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor` | `List<R> process(List<T> data,int batchSize,Function<T, R> processor)` | 分批次处理数据 |
| `cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor` | `List<Warp<?>> processByWarp(List<Warp<?>> warps)` | 处理Warp集合 |
| `cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor` | `List<Warp<?>> processByWarp(Warp<?>... warps)` | 处理Warp数组 |
| `cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor` | `void shutdown()` | 关闭线程池 |
| `cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor$Warp` | `R get()` | 获取结果 |
| `cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor$Warp` | `Warp<R> execute()` | 执行 |
| `cn.hutool.core.thread.RecyclableBatchThreadPoolExecutor$Warp` | `Warp<R> of(Supplier<R> supplier)` | 创建Warp |
| `cn.hutool.core.thread.RejectPolicy` | `RejectedExecutionHandler getValue()` | 获取RejectedExecutionHandler枚举值 |
| `cn.hutool.core.thread.SemaphoreRunnable` | `Semaphore getSemaphore()` | 获得信号量 |
| `cn.hutool.core.thread.SemaphoreRunnable` | `void run()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.SyncFinisher` | `SyncFinisher addRepeatWorker(final Runnable runnable)` | 增加定义的线程数同等数量的worker |
| `cn.hutool.core.thread.SyncFinisher` | `SyncFinisher addWorker(Worker worker)` | 增加工作线程 |
| `cn.hutool.core.thread.SyncFinisher` | `SyncFinisher addWorker(final Runnable runnable)` | 增加工作线程 |
| `cn.hutool.core.thread.SyncFinisher` | `SyncFinisher setBeginAtSameTime(boolean isBeginAtSameTime)` | 设置是否所有worker线程同时开始 |
| `cn.hutool.core.thread.SyncFinisher` | `SyncFinisher setExceptionHandler(final Thread.UncaughtExceptionHandler exceptionHandler)` | 设置异常处理 |
| `cn.hutool.core.thread.SyncFinisher` | `SyncFinisher setExecutorService(ExecutorService executorService)` | 设置自定义线程池，默认为ExecutorBuilder创建的线程池 |
| `cn.hutool.core.thread.SyncFinisher` | `long count()` | 剩余任务数 |
| `cn.hutool.core.thread.SyncFinisher` | `void clearWorker()` | 清空工作线程对象 |
| `cn.hutool.core.thread.SyncFinisher` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.SyncFinisher` | `void start()` | 开始工作 执行此方法后如果不再重复使用此对象，需调用#stop()关闭回收资源。 |
| `cn.hutool.core.thread.SyncFinisher` | `void start(boolean sync)` | 开始工作 执行此方法后如果不再重复使用此对象，需调用#stop()关闭回收资源。 |
| `cn.hutool.core.thread.SyncFinisher` | `void stop()` | 结束线程池。此方法执行两种情况： 执行start(true)后，调用此方法结束线程池回收资源 执行start(false)后，用户自行判断结束点执行此方法 |
| `cn.hutool.core.thread.SyncFinisher` | `void stopNow()` | 立即结束线程池所有线程。此方法执行两种情况： 执行start(true)后，调用此方法结束线程池回收资源 执行start(false)后，用户自行判断结束点执行此方法 |
| `cn.hutool.core.thread.SyncFinisher$Worker` | `void run()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.thread.SyncFinisher$Worker` | `void work()` | 任务内容 |
| `cn.hutool.core.thread.ThreadFactoryBuilder` | `ThreadFactory build()` | 构建ThreadFactory |
| `cn.hutool.core.thread.ThreadFactoryBuilder` | `ThreadFactoryBuilder create()` | 创建ThreadFactoryBuilder |
| `cn.hutool.core.thread.ThreadFactoryBuilder` | `ThreadFactoryBuilder setDaemon(boolean daemon)` | 设置是否守护线程 |
| `cn.hutool.core.thread.ThreadFactoryBuilder` | `ThreadFactoryBuilder setNamePrefix(String namePrefix)` | 设置线程名前缀，例如设置前缀为hutool-thread-，则线程名为hutool-thread-1之类。 |
| `cn.hutool.core.thread.ThreadFactoryBuilder` | `ThreadFactoryBuilder setPriority(int priority)` | 设置线程优先级 |
| `cn.hutool.core.thread.ThreadFactoryBuilder` | `ThreadFactoryBuilder setThreadFactory(ThreadFactory backingThreadFactory)` | 设置用于创建基础线程的线程工厂 |
| `cn.hutool.core.thread.ThreadFactoryBuilder` | `ThreadFactoryBuilder setUncaughtExceptionHandler(UncaughtExceptionHandler uncaughtExceptionHandler)` | 设置未捕获异常的处理方式 |
| `cn.hutool.core.thread.ThreadUtil` | `CompletionService<T> newCompletionService()` | 新建一个CompletionService，调用其submit方法可以异步执行多个任务，最后调用take方法按照完成的顺序获得其结果。 若未完成，则会阻塞 |
| `cn.hutool.core.thread.ThreadUtil` | `CompletionService<T> newCompletionService(ExecutorService executor)` | 新建一个CompletionService，调用其submit方法可以异步执行多个任务，最后调用take方法按照完成的顺序获得其结果。 若未完成，则会阻塞 |
| `cn.hutool.core.thread.ThreadUtil` | `ConcurrencyTester concurrencyTest(int threadSize,Runnable runnable)` | 并发测试 此方法用于测试多线程下执行某些逻辑的并发性能 调用此方法会导致当前线程阻塞。 结束后可调用ConcurrencyTester#getInterval() 方法获取执行时间 |
| `cn.hutool.core.thread.ThreadUtil` | `CountDownLatch newCountDownLatch(int threadCount)` | 新建一个CountDownLatch，一个同步辅助类，在完成一组正在其他线程中执行的操作之前，它允许一个或多个线程一直等待。 |
| `cn.hutool.core.thread.ThreadUtil` | `ExecutorService newSingleExecutor()` | 获得一个新的线程池，只有单个线程，策略如下： |
| `cn.hutool.core.thread.ThreadUtil` | `Future<?> execAsync(Runnable runnable)` | 执行有返回值的异步方法 Future代表一个异步执行的操作，通过get()方法可以获得操作的结果，如果异步操作还没有完成，则，get()会使当前线程阻塞 |
| `cn.hutool.core.thread.ThreadUtil` | `Future<T> execAsync(Callable<T> task)` | 执行有返回值的异步方法 Future代表一个异步执行的操作，通过get()方法可以获得操作的结果，如果异步操作还没有完成，则，get()会使当前线程阻塞 |
| `cn.hutool.core.thread.ThreadUtil` | `Runnable execAsync(Runnable runnable,boolean isDaemon)` | 执行异步方法 |
| `cn.hutool.core.thread.ThreadUtil` | `ScheduledThreadPoolExecutor createScheduledExecutor(int corePoolSize)` | 创建ScheduledThreadPoolExecutor |
| `cn.hutool.core.thread.ThreadUtil` | `ScheduledThreadPoolExecutor schedule(ScheduledThreadPoolExecutor executor,Runnable command,long initialDelay,long period,TimeUnit timeUnit,boolean fixedRateOrFixedDelay)` | 开始执行一个定时任务，执行方式分fixedRate模式和fixedDelay模式。 fixedRate 模式：以固定的频率执行。每period的时刻检查，如果上个任务完成，启动下个任务，否则等待上个任务结束后立即启动。 fixedDelay模式：以固定的延时执行。上次任务结束后等待period再执行下个任务。 |
| `cn.hutool.core.thread.ThreadUtil` | `ScheduledThreadPoolExecutor schedule(ScheduledThreadPoolExecutor executor,Runnable command,long initialDelay,long period,boolean fixedRateOrFixedDelay)` | 开始执行一个定时任务，执行方式分fixedRate模式和fixedDelay模式。 注意：此方法的延迟和周期的单位均为毫秒。 fixedRate 模式：以固定的频率执行。每period的时刻检查，如果上个任务完成，启动下个任务，否则等待上个任务结束后立即启动。 fixedDelay模式：以固定的延时执行。上次任务结束后等待period再执行下个任务。 |
| `cn.hutool.core.thread.ThreadUtil` | `StackTraceElement getStackTraceElement(int i)` | 获得堆栈项 |
| `cn.hutool.core.thread.ThreadUtil` | `StackTraceElement[] getStackTrace()` | @return 获得堆栈列表 |
| `cn.hutool.core.thread.ThreadUtil` | `Thread getMainThread()` | 获取进程的主线程 from Voovan |
| `cn.hutool.core.thread.ThreadUtil` | `Thread newThread(Runnable runnable,String name)` | 创建新线程，非守护线程，正常优先级，线程组与当前线程的线程组一致 |
| `cn.hutool.core.thread.ThreadUtil` | `Thread newThread(Runnable runnable,String name,boolean isDaemon)` | 创建新线程 |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadFactory createThreadFactory(String threadNamePrefix)` | 创建自定义线程名称前缀的ThreadFactory |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadFactory newNamedThreadFactory(String prefix,ThreadGroup threadGroup,boolean isDaemon)` | 创建线程工厂 |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadFactory newNamedThreadFactory(String prefix,ThreadGroup threadGroup,boolean isDaemon,UncaughtExceptionHandler handler)` | 创建线程工厂 |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadFactory newNamedThreadFactory(String prefix,boolean isDaemon)` | 创建线程工厂 |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadFactoryBuilder createThreadFactoryBuilder()` | 创建ThreadFactoryBuilder |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadGroup currentThreadGroup()` | 获取当前线程的线程组 |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadLocal<T> createThreadLocal(Supplier<? extends T> supplier)` | 创建本地线程对象 |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadLocal<T> createThreadLocal(boolean isInheritable)` | 创建本地线程对象 |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadPoolExecutor newExecutor()` | 获得一个新的线程池，默认的策略如下： |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadPoolExecutor newExecutor(int corePoolSize)` | 新建一个线程池，默认的策略如下： |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadPoolExecutor newExecutor(int corePoolSize,int maximumPoolSize)` | 获得一个新的线程池 如果maximumPoolSize >= corePoolSize，在没有新任务加入的情况下，多出的线程将最多保留60s |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadPoolExecutor newExecutor(int corePoolSize,int maximumPoolSize,int maximumQueueSize)` | 获得一个新的线程池，并指定最大任务队列大小 如果maximumPoolSize >= corePoolSize，在没有新任务加入的情况下，多出的线程将最多保留60s |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadPoolExecutor newExecutorByBlockingCoefficient(float blockingCoefficient)` | 获得一个新的线程池 传入阻塞系数，线程池的大小计算公式为：CPU可用核心数 / (1 - 阻塞因子) Blocking Coefficient(阻塞系数) = 阻塞时间／（阻塞时间+使用CPU的时间） 计算密集型任务的阻塞系数为0，而IO密集型任务的阻塞系数则接近于1。 see: http://blog.csdn.net/partner4java/article/details/9417663 |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadPoolExecutor newFixedExecutor(int nThreads,String threadNamePrefix,boolean isBlocked)` | 获取一个新的线程池，默认的策略如下 |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadPoolExecutor newFixedExecutor(int nThreads,int maximumQueueSize,String threadNamePrefix,RejectedExecutionHandler handler)` | 获得一个新的线程池，默认策略如下 |
| `cn.hutool.core.thread.ThreadUtil` | `ThreadPoolExecutor newFixedExecutor(int nThreads,int maximumQueueSize,String threadNamePrefix,boolean isBlocked)` | 获取一个新的线程池，默认的策略如下 |
| `cn.hutool.core.thread.ThreadUtil` | `Thread[] getThreads()` | 获取JVM中与当前线程同组的所有线程 |
| `cn.hutool.core.thread.ThreadUtil` | `Thread[] getThreads(ThreadGroup group)` | 获取JVM中与当前线程同组的所有线程 使用数组二次拷贝方式，防止在线程列表获取过程中线程终止 from Voovan |
| `cn.hutool.core.thread.ThreadUtil` | `boolean safeSleep(Number millis)` | 考虑Thread#sleep(long)方法有可能时间不足给定毫秒数，此方法保证sleep时间不小于给定的毫秒数 |
| `cn.hutool.core.thread.ThreadUtil` | `boolean safeSleep(long millis)` | 考虑Thread#sleep(long)方法有可能时间不足给定毫秒数，此方法保证sleep时间不小于给定的毫秒数 |
| `cn.hutool.core.thread.ThreadUtil` | `boolean sleep(Number millis)` | 挂起当前线程 |
| `cn.hutool.core.thread.ThreadUtil` | `boolean sleep(Number timeout,TimeUnit timeUnit)` | 挂起当前线程 |
| `cn.hutool.core.thread.ThreadUtil` | `boolean sleep(long millis)` | 挂起当前线程 |
| `cn.hutool.core.thread.ThreadUtil` | `void execute(Runnable runnable)` | 直接在公共线程池中执行线程 |
| `cn.hutool.core.thread.ThreadUtil` | `void interrupt(Thread thread,boolean isJoin)` | 结束线程，调用此方法后，线程将抛出 InterruptedException异常 |
| `cn.hutool.core.thread.ThreadUtil` | `void sync(Object obj)` | 阻塞当前线程，保证在main方法中执行不被退出 |
| `cn.hutool.core.thread.ThreadUtil` | `void waitForDie()` | 等待当前线程结束. 调用 Thread#join() 并忽略 InterruptedException |
| `cn.hutool.core.thread.ThreadUtil` | `void waitForDie(Thread thread)` | 等待线程结束. 调用 Thread#join() 并忽略 InterruptedException |
