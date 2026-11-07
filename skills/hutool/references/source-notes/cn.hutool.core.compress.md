# cn.hutool.core.compress

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.compress.Deflate` | `Deflate deflater(int level)` | 将普通数据流压缩 |
| `cn.hutool.core.compress.Deflate` | `Deflate inflater()` | 将压缩流解压到target中 |
| `cn.hutool.core.compress.Deflate` | `Deflate of(InputStream source,OutputStream target,boolean nowrap)` | 创建Deflate |
| `cn.hutool.core.compress.Deflate` | `OutputStream getTarget()` | 获取目标流 |
| `cn.hutool.core.compress.Deflate` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.compress.Gzip` | `Gzip gzip()` | 将普通数据流压缩 |
| `cn.hutool.core.compress.Gzip` | `Gzip of(InputStream source,OutputStream target)` | 创建Gzip |
| `cn.hutool.core.compress.Gzip` | `Gzip unGzip()` | 将压缩流解压到target中 |
| `cn.hutool.core.compress.Gzip` | `OutputStream getTarget()` | 获取目标流 |
| `cn.hutool.core.compress.Gzip` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.compress.ZipCopyVisitor` | `FileVisitResult preVisitDirectory(Path dir,BasicFileAttributes attrs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.compress.ZipCopyVisitor` | `FileVisitResult visitFile(Path file,BasicFileAttributes attrs)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.compress.ZipReader` | `File readTo(File outFile)` | 解压到指定目录中 |
| `cn.hutool.core.compress.ZipReader` | `File readTo(File outFile,Filter<ZipEntry> entryFilter)` | 解压到指定目录中 |
| `cn.hutool.core.compress.ZipReader` | `InputStream get(String path)` | 获取指定路径的文件流 如果是文件模式，则直接获取Entry对应的流，如果是流模式，则遍历entry后，找到对应流返回 |
| `cn.hutool.core.compress.ZipReader` | `ZipReader of(File zipFile,Charset charset)` | 创建ZipReader |
| `cn.hutool.core.compress.ZipReader` | `ZipReader of(InputStream in,Charset charset)` | 创建ZipReader |
| `cn.hutool.core.compress.ZipReader` | `ZipReader read(Consumer<ZipEntry> consumer)` | 读取并处理Zip文件中的每一个ZipEntry |
| `cn.hutool.core.compress.ZipReader` | `ZipReader setMaxSizeDiff(final int maxSizeDiff)` | 设置检查ZipBomb文件差异倍数，-1表示不检查ZipBomb |
| `cn.hutool.core.compress.ZipReader` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.compress.ZipWriter` | `ZipOutputStream getOut()` | 获取原始的ZipOutputStream |
| `cn.hutool.core.compress.ZipWriter` | `ZipWriter add(Resource... resources)` | 添加资源到压缩包，添加后关闭资源流 |
| `cn.hutool.core.compress.ZipWriter` | `ZipWriter add(String path,InputStream in)` | 添加文件流到压缩包，添加后关闭输入文件流 如果输入流为null，则只创建空目录 |
| `cn.hutool.core.compress.ZipWriter` | `ZipWriter add(String[] paths,InputStream[] ins)` | 对流中的数据加入到压缩文件 路径列表和流列表长度必须一致 |
| `cn.hutool.core.compress.ZipWriter` | `ZipWriter add(boolean withSrcDir,FileFilter filter,File... files)` | 对文件或文件目录进行压缩 |
| `cn.hutool.core.compress.ZipWriter` | `ZipWriter of(File zipFile,Charset charset)` | 创建ZipWriter |
| `cn.hutool.core.compress.ZipWriter` | `ZipWriter of(OutputStream out,Charset charset)` | 创建ZipWriter |
| `cn.hutool.core.compress.ZipWriter` | `ZipWriter setComment(String comment)` | 设置注释 |
| `cn.hutool.core.compress.ZipWriter` | `ZipWriter setLevel(int level)` | 设置压缩级别，可选1~9，-1表示默认 |
| `cn.hutool.core.compress.ZipWriter` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
