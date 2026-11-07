# cn.hutool.extra.compress.archiver

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.compress.archiver.Archiver` | `Archiver add(File file)` | 将文件或目录加入归档，目录采取递归读取方式按照层级加入 |
| `cn.hutool.extra.compress.archiver.Archiver` | `Archiver add(File file,Filter<File> filter)` | 将文件或目录加入归档，目录采取递归读取方式按照层级加入 |
| `cn.hutool.extra.compress.archiver.Archiver` | `Archiver add(File file,String path,Filter<File> filter)` | 将文件或目录加入归档包，目录采取递归读取方式按照层级加入 |
| `cn.hutool.extra.compress.archiver.Archiver` | `Archiver finish()` | 结束已经增加的文件归档，此方法不会关闭归档流，可以继续添加文件 |
| `cn.hutool.extra.compress.archiver.Archiver` | `void close()` | 无异常关闭 |
| `cn.hutool.extra.compress.archiver.SevenZArchiver` | `SevenZArchiver add(File file,String path,Filter<File> filter)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.compress.archiver.SevenZArchiver` | `SevenZArchiver finish()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.compress.archiver.SevenZArchiver` | `SevenZOutputFile getSevenZOutputFile()` | 获取SevenZOutputFile以便自定义相关设置 |
| `cn.hutool.extra.compress.archiver.SevenZArchiver` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.compress.archiver.StreamArchiver` | `StreamArchiver add(File file,String path,Filter<File> filter)` | 将文件或目录加入归档包，目录采取递归读取方式按照层级加入 |
| `cn.hutool.extra.compress.archiver.StreamArchiver` | `StreamArchiver create(Charset charset,String archiverName,File file)` | 创建归档器 |
| `cn.hutool.extra.compress.archiver.StreamArchiver` | `StreamArchiver create(Charset charset,String archiverName,OutputStream out)` | 创建归档器 |
| `cn.hutool.extra.compress.archiver.StreamArchiver` | `StreamArchiver finish()` | 结束已经增加的文件归档，此方法不会关闭归档流，可以继续添加文件 |
| `cn.hutool.extra.compress.archiver.StreamArchiver` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
