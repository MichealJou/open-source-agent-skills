# cn.hutool.extra.compress.extractor

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.compress.extractor.Extractor` | `String stripName(String name,int stripComponents)` | 剥离名称 |
| `cn.hutool.extra.compress.extractor.Extractor` | `void close()` | 无异常关闭 |
| `cn.hutool.extra.compress.extractor.Extractor` | `void extract(File targetDir)` | 释放（解压）到指定目录，结束后自动关闭流，此方法只能调用一次 |
| `cn.hutool.extra.compress.extractor.Extractor` | `void extract(File targetDir,Filter<ArchiveEntry> filter)` | 释放（解压）到指定目录，结束后自动关闭流，此方法只能调用一次 |
| `cn.hutool.extra.compress.extractor.Extractor` | `void extract(File targetDir,int stripComponents)` | 释放（解压）到指定目录，结束后自动关闭流，此方法只能调用一次 |
| `cn.hutool.extra.compress.extractor.Extractor` | `void extract(File targetDir,int stripComponents,Filter<ArchiveEntry> filter)` | 释放（解压）到指定目录，结束后自动关闭流，此方法只能调用一次 |
| `cn.hutool.extra.compress.extractor.Seven7EntryInputStream` | `int available()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.compress.extractor.Seven7EntryInputStream` | `int read()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.compress.extractor.Seven7EntryInputStream` | `long getReadSize()` | 获取读取的长度（字节数） |
| `cn.hutool.extra.compress.extractor.SevenZExtractor` | `InputStream get(String entryName)` | 获取指定名称的文件流 |
| `cn.hutool.extra.compress.extractor.SevenZExtractor` | `InputStream getFirst(Filter<ArchiveEntry> filter)` | 获取满足指定过滤要求的压缩包内的第一个文件流 |
| `cn.hutool.extra.compress.extractor.SevenZExtractor` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.compress.extractor.SevenZExtractor` | `void extract(File targetDir,int stripComponents,Filter<ArchiveEntry> filter)` | 释放（解压）到指定目录，结束后自动关闭流，此方法只能调用一次 |
| `cn.hutool.extra.compress.extractor.StreamExtractor` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.compress.extractor.StreamExtractor` | `void extract(File targetDir,int stripComponents,Filter<ArchiveEntry> filter)` | 释放（解压）到指定目录，结束后自动关闭流，此方法只能调用一次 |
