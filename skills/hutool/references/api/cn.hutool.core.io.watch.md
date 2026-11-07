# cn.hutool.core.io.watch

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.io.watch.SimpleWatcher`

```java
public class cn.hutool.core.io.watch.SimpleWatcher extends cn.hutool.core.io.watch.watchers.IgnoreWatcher {
  public cn.hutool.core.io.watch.SimpleWatcher();
}
```

## `cn.hutool.core.io.watch.WatchAction`

```java
public interface cn.hutool.core.io.watch.WatchAction {
  public abstract void doAction(java.nio.file.WatchEvent<?>, java.nio.file.Path);
}
```

## `cn.hutool.core.io.watch.WatchException`

```java
public class cn.hutool.core.io.watch.WatchException extends java.lang.RuntimeException {
  public cn.hutool.core.io.watch.WatchException(java.lang.Throwable);
  public cn.hutool.core.io.watch.WatchException(java.lang.String);
  public cn.hutool.core.io.watch.WatchException(java.lang.String, java.lang.Object...);
  public cn.hutool.core.io.watch.WatchException(java.lang.String, java.lang.Throwable);
  public cn.hutool.core.io.watch.WatchException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.core.io.watch.WatchKind`

```java
public final class cn.hutool.core.io.watch.WatchKind extends java.lang.Enum<cn.hutool.core.io.watch.WatchKind> {
  public static cn.hutool.core.io.watch.WatchKind[] values();
  public static cn.hutool.core.io.watch.WatchKind valueOf(java.lang.String);
  public java.nio.file.WatchEvent$Kind<?> getValue();
}
```

## `cn.hutool.core.io.watch.WatchMonitor`

```java
public class cn.hutool.core.io.watch.WatchMonitor extends cn.hutool.core.io.watch.WatchServer {
  public static cn.hutool.core.io.watch.WatchMonitor create(java.net.URL, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.net.URL, int, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.net.URI, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.net.URI, int, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.io.File, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.io.File, int, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.lang.String, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.lang.String, int, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.nio.file.Path, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.nio.file.Path, int, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.net.URI, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.net.URL, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.io.File, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.lang.String, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.nio.file.Path, cn.hutool.core.io.watch.Watcher);
  public cn.hutool.core.io.watch.WatchMonitor(java.io.File, java.nio.file.WatchEvent$Kind<?>...);
  public cn.hutool.core.io.watch.WatchMonitor(java.lang.String, java.nio.file.WatchEvent$Kind<?>...);
  public cn.hutool.core.io.watch.WatchMonitor(java.nio.file.Path, java.nio.file.WatchEvent$Kind<?>...);
  public cn.hutool.core.io.watch.WatchMonitor(java.nio.file.Path, int, java.nio.file.WatchEvent$Kind<?>...);
  public void init() throws cn.hutool.core.io.watch.WatchException;
  public cn.hutool.core.io.watch.WatchMonitor setWatcher(cn.hutool.core.io.watch.Watcher);
  public void run();
  public void watch();
  public void watch(cn.hutool.core.io.watch.Watcher) throws cn.hutool.core.io.watch.WatchException;
  public cn.hutool.core.io.watch.WatchMonitor setMaxDepth(int);
}
```

## `cn.hutool.core.io.watch.WatchServer`

```java
public class cn.hutool.core.io.watch.WatchServer extends java.lang.Thread implements java.io.Closeable,java.io.Serializable {
  public cn.hutool.core.io.watch.WatchServer();
  public void init() throws cn.hutool.core.io.watch.WatchException;
  public void setModifiers(java.nio.file.WatchEvent$Modifier[]);
  public void registerPath(java.nio.file.Path, int);
  public void watch(cn.hutool.core.io.watch.WatchAction, cn.hutool.core.lang.Filter<java.nio.file.WatchEvent<?>>);
  public void watch(cn.hutool.core.io.watch.Watcher, cn.hutool.core.lang.Filter<java.nio.file.WatchEvent<?>>);
  public java.nio.file.WatchKey getWatchKey(java.nio.file.Path);
  public void close();
}
```

## `cn.hutool.core.io.watch.WatchUtil`

```java
public class cn.hutool.core.io.watch.WatchUtil {
  public cn.hutool.core.io.watch.WatchUtil();
  public static cn.hutool.core.io.watch.WatchMonitor create(java.net.URL, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.net.URL, int, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.net.URI, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.net.URI, int, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.io.File, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.io.File, int, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.lang.String, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.lang.String, int, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.nio.file.Path, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor create(java.nio.file.Path, int, java.nio.file.WatchEvent$Kind<?>...);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.net.URL, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.net.URL, int, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.net.URI, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.net.URI, int, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.io.File, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.io.File, int, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.lang.String, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.lang.String, int, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.nio.file.Path, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createAll(java.nio.file.Path, int, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createModify(java.net.URL, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createModify(java.net.URL, int, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createModify(java.net.URI, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createModify(java.net.URI, int, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createModify(java.io.File, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createModify(java.io.File, int, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createModify(java.lang.String, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createModify(java.lang.String, int, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createModify(java.nio.file.Path, cn.hutool.core.io.watch.Watcher);
  public static cn.hutool.core.io.watch.WatchMonitor createModify(java.nio.file.Path, int, cn.hutool.core.io.watch.Watcher);
  public static java.nio.file.WatchKey register(java.nio.file.Watchable, java.nio.file.WatchService, java.nio.file.WatchEvent$Kind<?>...);
}
```

## `cn.hutool.core.io.watch.Watcher`

```java
public interface cn.hutool.core.io.watch.Watcher {
  public abstract void onCreate(java.nio.file.WatchEvent<?>, java.nio.file.Path);
  public abstract void onModify(java.nio.file.WatchEvent<?>, java.nio.file.Path);
  public abstract void onDelete(java.nio.file.WatchEvent<?>, java.nio.file.Path);
  public abstract void onOverflow(java.nio.file.WatchEvent<?>, java.nio.file.Path);
}
```
