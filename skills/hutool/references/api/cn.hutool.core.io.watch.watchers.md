# cn.hutool.core.io.watch.watchers

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.io.watch.watchers.DelayWatcher`

```java
public class cn.hutool.core.io.watch.watchers.DelayWatcher implements cn.hutool.core.io.watch.Watcher {
  public cn.hutool.core.io.watch.watchers.DelayWatcher(cn.hutool.core.io.watch.Watcher, long);
  public void onModify(java.nio.file.WatchEvent<?>, java.nio.file.Path);
  public void onCreate(java.nio.file.WatchEvent<?>, java.nio.file.Path);
  public void onDelete(java.nio.file.WatchEvent<?>, java.nio.file.Path);
  public void onOverflow(java.nio.file.WatchEvent<?>, java.nio.file.Path);
}
```

## `cn.hutool.core.io.watch.watchers.IgnoreWatcher`

```java
public class cn.hutool.core.io.watch.watchers.IgnoreWatcher implements cn.hutool.core.io.watch.Watcher {
  public cn.hutool.core.io.watch.watchers.IgnoreWatcher();
  public void onCreate(java.nio.file.WatchEvent<?>, java.nio.file.Path);
  public void onModify(java.nio.file.WatchEvent<?>, java.nio.file.Path);
  public void onDelete(java.nio.file.WatchEvent<?>, java.nio.file.Path);
  public void onOverflow(java.nio.file.WatchEvent<?>, java.nio.file.Path);
}
```

## `cn.hutool.core.io.watch.watchers.WatcherChain`

```java
public class cn.hutool.core.io.watch.watchers.WatcherChain implements cn.hutool.core.io.watch.Watcher, cn.hutool.core.lang.Chain<cn.hutool.core.io.watch.Watcher, cn.hutool.core.io.watch.watchers.WatcherChain> {
  public static cn.hutool.core.io.watch.watchers.WatcherChain create(cn.hutool.core.io.watch.Watcher...);
  public cn.hutool.core.io.watch.watchers.WatcherChain(cn.hutool.core.io.watch.Watcher...);
  public void onCreate(java.nio.file.WatchEvent<?>, java.nio.file.Path);
  public void onModify(java.nio.file.WatchEvent<?>, java.nio.file.Path);
  public void onDelete(java.nio.file.WatchEvent<?>, java.nio.file.Path);
  public void onOverflow(java.nio.file.WatchEvent<?>, java.nio.file.Path);
  public java.util.Iterator<cn.hutool.core.io.watch.Watcher> iterator();
  public cn.hutool.core.io.watch.watchers.WatcherChain addChain(cn.hutool.core.io.watch.Watcher);
  public java.lang.Object addChain(java.lang.Object);
}
```
