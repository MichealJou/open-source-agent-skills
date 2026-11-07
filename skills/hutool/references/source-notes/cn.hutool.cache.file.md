# cn.hutool.cache.file

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.cache.file.AbstractFileCache` | `byte[] getFileBytes(File file)` | 获得缓存过的文件bytes |
| `cn.hutool.cache.file.AbstractFileCache` | `byte[] getFileBytes(String path)` | 获得缓存过的文件bytes |
| `cn.hutool.cache.file.AbstractFileCache` | `int capacity()` | @return 缓存容量（byte数） |
| `cn.hutool.cache.file.AbstractFileCache` | `int getCachedFilesCount()` | @return 缓存的文件数 |
| `cn.hutool.cache.file.AbstractFileCache` | `int getUsedSize()` | @return 已使用空间大小（byte数） |
| `cn.hutool.cache.file.AbstractFileCache` | `int maxFileSize()` | @return 允许被缓存文件的最大byte数 |
| `cn.hutool.cache.file.AbstractFileCache` | `long timeout()` | @return 超时时间 |
| `cn.hutool.cache.file.AbstractFileCache` | `void clear()` | 清空缓存 |
