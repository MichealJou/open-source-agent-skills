# cn.hutool.core.io.watch

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.io.watch.WatchAction` | `void doAction(WatchEvent<?> event,Path currentPath)` | 事件处理，通过实现此方法处理各种事件。 事件可以调用 WatchEvent#kind()获取，对应事件见WatchKind |
| `cn.hutool.core.io.watch.WatchKind` | `WatchEvent.Kind<?> getValue()` | 获取枚举对应的事件类型 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor create(File file,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor create(File file,int maxDepth,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor create(Path path,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor create(Path path,int maxDepth,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor create(String path,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor create(String path,int maxDepth,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor create(URI uri,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor create(URI uri,int maxDepth,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor create(URL url,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor create(URL url,int maxDepth,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor createAll(File file,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor createAll(Path path,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor createAll(String path,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor createAll(URI uri,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor createAll(URL url,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor setMaxDepth(int maxDepth)` | 当监听目录时，监听目录的最大深度 当设置值为1（或小于1）时，表示不递归监听子目录 例如设置： |
| `cn.hutool.core.io.watch.WatchMonitor` | `WatchMonitor setWatcher(Watcher watcher)` | 设置监听 多个监听请使用WatcherChain |
| `cn.hutool.core.io.watch.WatchMonitor` | `void init()` | 初始化 初始化包括： |
| `cn.hutool.core.io.watch.WatchMonitor` | `void run()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.watch.WatchMonitor` | `void watch()` | 开始监听事件，阻塞当前进程 |
| `cn.hutool.core.io.watch.WatchMonitor` | `void watch(Watcher watcher)` | 开始监听事件，阻塞当前进程 |
| `cn.hutool.core.io.watch.WatchServer` | `WatchKey getWatchKey(Path path)` | 通过 path 获取 watchKey |
| `cn.hutool.core.io.watch.WatchServer` | `void close()` | 关闭监听 |
| `cn.hutool.core.io.watch.WatchServer` | `void init()` | 初始化 初始化包括： |
| `cn.hutool.core.io.watch.WatchServer` | `void registerPath(Path path,int maxDepth)` | 将指定路径加入到监听中 |
| `cn.hutool.core.io.watch.WatchServer` | `void setModifiers(WatchEvent.Modifier[] modifiers)` | 设置监听选项，例如监听频率等，可设置项包括： |
| `cn.hutool.core.io.watch.WatchServer` | `void watch(WatchAction action,Filter<WatchEvent<?>> watchFilter)` | 执行事件获取并处理 |
| `cn.hutool.core.io.watch.WatchServer` | `void watch(Watcher watcher,Filter<WatchEvent<?>> watchFilter)` | 执行事件获取并处理 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchKey register(Watchable watchable,WatchService watcher,WatchEvent.Kind<?>... events)` | 注册Watchable对象到WatchService服务 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor create(File file,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor create(File file,int maxDepth,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor create(Path path,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor create(Path path,int maxDepth,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor create(String path,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor create(String path,int maxDepth,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor create(URI uri,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor create(URI uri,int maxDepth,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor create(URL url,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor create(URL url,int maxDepth,WatchEvent.Kind<?>... events)` | 创建并初始化监听 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createAll(File file,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createAll(File file,int maxDepth,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createAll(Path path,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createAll(Path path,int maxDepth,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createAll(String path,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createAll(String path,int maxDepth,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createAll(URI uri,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createAll(URI uri,int maxDepth,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createAll(URL url,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createAll(URL url,int maxDepth,Watcher watcher)` | 创建并初始化监听，监听所有事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createModify(File file,Watcher watcher)` | 创建并初始化监听，监听修改事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createModify(File file,int maxDepth,Watcher watcher)` | 创建并初始化监听，监听修改事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createModify(Path path,Watcher watcher)` | 创建并初始化监听，监听修改事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createModify(Path path,int maxDepth,Watcher watcher)` | 创建并初始化监听，监听修改事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createModify(String path,Watcher watcher)` | 创建并初始化监听，监听修改事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createModify(String path,int maxDepth,Watcher watcher)` | 创建并初始化监听，监听修改事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createModify(URI uri,Watcher watcher)` | 创建并初始化监听，监听修改事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createModify(URI uri,int maxDepth,Watcher watcher)` | 创建并初始化监听，监听修改事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createModify(URL url,Watcher watcher)` | 创建并初始化监听，监听修改事件 |
| `cn.hutool.core.io.watch.WatchUtil` | `WatchMonitor createModify(URL url,int maxDepth,Watcher watcher)` | 创建并初始化监听，监听修改事件 |
| `cn.hutool.core.io.watch.Watcher` | `void onCreate(WatchEvent<?> event,Path currentPath)` | 文件创建时执行的方法 |
| `cn.hutool.core.io.watch.Watcher` | `void onDelete(WatchEvent<?> event,Path currentPath)` | 文件删除时执行的方法 |
| `cn.hutool.core.io.watch.Watcher` | `void onModify(WatchEvent<?> event,Path currentPath)` | 文件修改时执行的方法 文件修改可能触发多次 |
| `cn.hutool.core.io.watch.Watcher` | `void onOverflow(WatchEvent<?> event,Path currentPath)` | 事件丢失或出错时执行的方法 |
