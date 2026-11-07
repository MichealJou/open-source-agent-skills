# cn.hutool.cache.file

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.cache.file.AbstractFileCache`

```java
public abstract class cn.hutool.cache.file.AbstractFileCache implements java.io.Serializable {
  public cn.hutool.cache.file.AbstractFileCache(int, int, long);
  public int capacity();
  public int getUsedSize();
  public int maxFileSize();
  public int getCachedFilesCount();
  public long timeout();
  public void clear();
  public byte[] getFileBytes(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public byte[] getFileBytes(java.io.File) throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.cache.file.LFUFileCache`

```java
public class cn.hutool.cache.file.LFUFileCache extends cn.hutool.cache.file.AbstractFileCache {
  public cn.hutool.cache.file.LFUFileCache(int);
  public cn.hutool.cache.file.LFUFileCache(int, int);
  public cn.hutool.cache.file.LFUFileCache(int, int, long);
}
```

## `cn.hutool.cache.file.LRUFileCache`

```java
public class cn.hutool.cache.file.LRUFileCache extends cn.hutool.cache.file.AbstractFileCache {
  public cn.hutool.cache.file.LRUFileCache(int);
  public cn.hutool.cache.file.LRUFileCache(int, int);
  public cn.hutool.cache.file.LRUFileCache(int, int, long);
}
```
