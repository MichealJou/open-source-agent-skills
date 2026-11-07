# cn.hutool.core.io.file

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.io.file.FileAppender` | `FileAppender append(String line)` | 追加 |
| `cn.hutool.core.io.file.FileAppender` | `FileAppender flush()` | 刷入到文件 |
| `cn.hutool.core.io.file.FileCopier` | `File copy()` | 执行拷贝 拷贝规则为： |
| `cn.hutool.core.io.file.FileCopier` | `FileCopier create(File src,File dest)` | 新建一个文件复制器 |
| `cn.hutool.core.io.file.FileCopier` | `FileCopier create(String srcPath,String destPath)` | 新建一个文件复制器 |
| `cn.hutool.core.io.file.FileCopier` | `FileCopier setCopyAttributes(boolean isCopyAttributes)` | 设置是否拷贝所有属性 |
| `cn.hutool.core.io.file.FileCopier` | `FileCopier setCopyContentIfDir(boolean isCopyContentIfDir)` | 当拷贝来源是目录时是否只拷贝目录下的内容 |
| `cn.hutool.core.io.file.FileCopier` | `FileCopier setOnlyCopyFile(boolean isOnlyCopyFile)` | 设置当拷贝来源是目录时是否只拷贝文件而忽略子目录 |
| `cn.hutool.core.io.file.FileCopier` | `FileCopier setOverride(boolean isOverride)` | 设置是否覆盖目标文件 |
| `cn.hutool.core.io.file.FileCopier` | `boolean isCopyAttributes()` | 是否拷贝所有属性 |
| `cn.hutool.core.io.file.FileCopier` | `boolean isCopyContentIfDir()` | 当拷贝来源是目录时是否只拷贝目录下的内容 |
| `cn.hutool.core.io.file.FileCopier` | `boolean isOnlyCopyFile()` | 当拷贝来源是目录时是否只拷贝文件而忽略子目录 |
| `cn.hutool.core.io.file.FileCopier` | `boolean isOverride()` | 是否覆盖目标文件 |
| `cn.hutool.core.io.file.FileNameUtil` | `String cleanInvalid(String fileName)` | 清除文件名中的在Windows下不支持的非法字符，包括： \ / : * ? " < > \| |
| `cn.hutool.core.io.file.FileNameUtil` | `String extName(File file)` | 获取文件扩展名（后缀名），扩展名不带“.” |
| `cn.hutool.core.io.file.FileNameUtil` | `String extName(String fileName)` | 获得文件的扩展名（后缀名），扩展名不带“.” |
| `cn.hutool.core.io.file.FileNameUtil` | `String getName(File file)` | 返回文件名 |
| `cn.hutool.core.io.file.FileNameUtil` | `String getName(String filePath)` | 返回文件名 |
| `cn.hutool.core.io.file.FileNameUtil` | `String getPrefix(File file)` | 返回主文件名 |
| `cn.hutool.core.io.file.FileNameUtil` | `String getPrefix(String fileName)` | 返回主文件名 |
| `cn.hutool.core.io.file.FileNameUtil` | `String getSuffix(File file)` | 获取文件后缀名，扩展名不带“.” |
| `cn.hutool.core.io.file.FileNameUtil` | `String getSuffix(String fileName)` | 获得文件后缀名，扩展名不带“.” |
| `cn.hutool.core.io.file.FileNameUtil` | `String mainName(File file)` | 返回主文件名 |
| `cn.hutool.core.io.file.FileNameUtil` | `String mainName(String fileName)` | 返回主文件名 |
| `cn.hutool.core.io.file.FileNameUtil` | `boolean containsInvalid(String fileName)` | 文件名中是否包含在Windows下不支持的非法字符，包括： \ / : * ? " < > \| |
| `cn.hutool.core.io.file.FileNameUtil` | `boolean isType(String fileName,String... extNames)` | 根据文件名检查文件类型，忽略大小写 |
| `cn.hutool.core.io.file.FileReader` | `BufferedInputStream getInputStream()` | 获得输入流 |
| `cn.hutool.core.io.file.FileReader` | `BufferedReader getReader()` | 获得一个文件读取器 |
| `cn.hutool.core.io.file.FileReader` | `FileReader create(File file)` | 创建 FileReader, 编码：FileWrapper#DEFAULT_CHARSET |
| `cn.hutool.core.io.file.FileReader` | `FileReader create(File file,Charset charset)` | 创建 FileReader |
| `cn.hutool.core.io.file.FileReader` | `List<String> readLines()` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.file.FileReader` | `String readString()` | 读取文件内容 |
| `cn.hutool.core.io.file.FileReader` | `T read(ReaderHandler<T> readerHandler)` | 按照给定的readerHandler读取文件中的数据 |
| `cn.hutool.core.io.file.FileReader` | `T readLines(T collection)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.file.FileReader` | `byte[] readBytes()` | 读取文件所有数据 文件的长度不能超过 Integer#MAX_VALUE |
| `cn.hutool.core.io.file.FileReader` | `long writeToStream(OutputStream out)` | 将文件写入流中，此方法不会关闭比输出流 |
| `cn.hutool.core.io.file.FileReader` | `long writeToStream(OutputStream out,boolean isCloseOut)` | 将文件写入流中 |
| `cn.hutool.core.io.file.FileReader` | `void readLines(LineHandler lineHandler)` | 按照行处理文件内容 |
| `cn.hutool.core.io.file.FileReader$ReaderHandler` | `T handle(BufferedReader reader)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.file.FileSystemUtil` | `FileSystem create(String path)` | 创建 FileSystem |
| `cn.hutool.core.io.file.FileSystemUtil` | `FileSystem createZip(String path)` | 创建 Zip的FileSystem，默认UTF-8编码 |
| `cn.hutool.core.io.file.FileSystemUtil` | `FileSystem createZip(String path,Charset charset)` | 创建 Zip的FileSystem |
| `cn.hutool.core.io.file.FileSystemUtil` | `Path getRoot(FileSystem fileSystem)` | 获取目录的根路径，或Zip文件中的根路径 |
| `cn.hutool.core.io.file.FileWrapper` | `Charset getCharset()` | 获得字符集编码 |
| `cn.hutool.core.io.file.FileWrapper` | `File getFile()` | 获得文件 |
| `cn.hutool.core.io.file.FileWrapper` | `FileWrapper setCharset(Charset charset)` | 设置字符集编码 |
| `cn.hutool.core.io.file.FileWrapper` | `FileWrapper setFile(File file)` | 设置文件 |
| `cn.hutool.core.io.file.FileWrapper` | `String readableFileSize()` | 可读的文件大小 |
| `cn.hutool.core.io.file.FileWriter` | `BufferedOutputStream getOutputStream()` | 获得一个输出流对象 |
| `cn.hutool.core.io.file.FileWriter` | `BufferedWriter getWriter(boolean isAppend)` | 获得一个带缓存的写入对象 |
| `cn.hutool.core.io.file.FileWriter` | `File append(String content)` | 将String写入文件，追加模式 |
| `cn.hutool.core.io.file.FileWriter` | `File append(byte[] data,int off,int len)` | 追加数据到文件 |
| `cn.hutool.core.io.file.FileWriter` | `File appendLines(Iterable<T> list)` | 将列表写入文件，追加模式，最后一行末尾不追加换行符 |
| `cn.hutool.core.io.file.FileWriter` | `File write(String content)` | 将String写入文件，覆盖模式 |
| `cn.hutool.core.io.file.FileWriter` | `File write(String content,boolean isAppend)` | 将String写入文件 |
| `cn.hutool.core.io.file.FileWriter` | `File write(byte[] data,int off,int len)` | 写入数据到文件 |
| `cn.hutool.core.io.file.FileWriter` | `File write(byte[] data,int off,int len,boolean isAppend)` | 写入数据到文件 |
| `cn.hutool.core.io.file.FileWriter` | `File writeFromStream(InputStream in)` | 将流的内容写入文件 此方法会自动关闭输入流 |
| `cn.hutool.core.io.file.FileWriter` | `File writeFromStream(InputStream in,boolean isCloseIn)` | 将流的内容写入文件 |
| `cn.hutool.core.io.file.FileWriter` | `File writeLines(Iterable<T> list)` | 将列表写入文件，覆盖模式，最后一行末尾不追加换行符 |
| `cn.hutool.core.io.file.FileWriter` | `File writeLines(Iterable<T> list,LineSeparator lineSeparator,boolean isAppend)` | 将列表写入文件，最后一行末尾不追加换行符 |
| `cn.hutool.core.io.file.FileWriter` | `File writeLines(Iterable<T> list,LineSeparator lineSeparator,boolean isAppend,boolean appendLineSeparator)` | 将列表写入文件 |
| `cn.hutool.core.io.file.FileWriter` | `File writeLines(Iterable<T> list,boolean isAppend)` | 将列表写入文件，最后一行末尾不追加换行符 |
| `cn.hutool.core.io.file.FileWriter` | `File writeMap(Map<?, ?> map,LineSeparator lineSeparator,String kvSeparator,boolean isAppend)` | 将Map写入文件，每个键值对为一行，一行中键与值之间使用kvSeparator分隔 |
| `cn.hutool.core.io.file.FileWriter` | `File writeMap(Map<?, ?> map,String kvSeparator,boolean isAppend)` | 将Map写入文件，每个键值对为一行，一行中键与值之间使用kvSeparator分隔 |
| `cn.hutool.core.io.file.FileWriter` | `FileWriter create(File file)` | 创建 FileWriter, 编码：FileWrapper#DEFAULT_CHARSET |
| `cn.hutool.core.io.file.FileWriter` | `FileWriter create(File file,Charset charset)` | 创建 FileWriter |
| `cn.hutool.core.io.file.FileWriter` | `PrintWriter getPrintWriter(boolean isAppend)` | 获得一个打印写入对象，可以有print |
| `cn.hutool.core.io.file.LineReadWatcher` | `void onModify(WatchEvent<?> event,Path currentPath)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.file.LineReadWatcher` | `void run()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.file.LineSeparator` | `String getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.file.PathMover` | `Path move()` | 移动文件或目录到目标中，例如： 如果src和target为同一文件或目录，直接返回target。 如果src为文件，target为目录，则移动到目标目录下，存在同名文件则按照是否覆盖参数执行。 如果src为文件，target为文件，则按照是否覆盖参数执行。 如果src为文件，target为不存在的路径，则重命名源文件到目标指定的文件，如move("/a/b", "/c/d"), d不存在，则b变成d。 如果src为目录，target为文件，抛出IllegalArgumentException 如果src为目录，target为目录，则将源目录及其内容移动到目标路径目录中，如move("/a/b"… |
| `cn.hutool.core.io.file.PathMover` | `Path moveContent()` | 移动文件或目录内容到目标中，例如： 如果src为文件，target为目录，则移动到目标目录下，存在同名文件则按照是否覆盖参数执行。 如果src为文件，target为文件，则按照是否覆盖参数执行。 如果src为文件，target为不存在的路径，则重命名源文件到目标指定的文件，如moveContent("/a/b", "/c/d"), d不存在，则b变成d。 如果src为目录，target为文件，抛出IllegalArgumentException 如果src为目录，target为目录，则将源目录下的内容移动到目标路径目录中，源目录不删除。 如果src为目录，target为不存在的路径，则创建目标… |
| `cn.hutool.core.io.file.PathMover` | `PathMover of(final Path src,final Path target,final CopyOption[] options)` | 创建文件或目录移动器 |
| `cn.hutool.core.io.file.PathMover` | `PathMover of(final Path src,final Path target,final boolean isOverride)` | 创建文件或目录移动器 |
| `cn.hutool.core.io.file.PathUtil` | `BasicFileAttributes getAttributes(Path path,boolean isFollowLinks)` | 获取文件属性 |
| `cn.hutool.core.io.file.PathUtil` | `BufferedInputStream getInputStream(Path path)` | 获得输入流 |
| `cn.hutool.core.io.file.PathUtil` | `BufferedOutputStream getOutputStream(Path path)` | 获得输出流 |
| `cn.hutool.core.io.file.PathUtil` | `BufferedReader getReader(Path path,Charset charset)` | 获得一个文件读取器 |
| `cn.hutool.core.io.file.PathUtil` | `BufferedReader getUtf8Reader(Path path)` | 获得一个文件读取器 |
| `cn.hutool.core.io.file.PathUtil` | `LinkOption[] getLinkOptions(final boolean isFollowLinks)` | 构建是否追踪软链的选项 |
| `cn.hutool.core.io.file.PathUtil` | `List<File> loopFiles(Path path,FileFilter fileFilter)` | 递归遍历目录以及子目录中的所有文件 如果提供path为文件，直接返回过滤结果 |
| `cn.hutool.core.io.file.PathUtil` | `List<File> loopFiles(Path path,int maxDepth,FileFilter fileFilter)` | 递归遍历目录以及子目录中的所有文件 如果提供path为文件，直接返回过滤结果 |
| `cn.hutool.core.io.file.PathUtil` | `List<File> loopFiles(final Path path,final int maxDepth,final boolean isFollowLinks,final FileFilter fileFilter)` | 递归遍历目录以及子目录中的所有文件 如果提供path为文件，直接返回过滤结果 |
| `cn.hutool.core.io.file.PathUtil` | `Path copy(Path src,Path target,CopyOption... options)` | 拷贝文件或目录，拷贝规则为： 源文件为目录，目标也为目录或不存在，则拷贝整个目录到目标目录下 源文件为文件，目标为目录或不存在，则拷贝文件到目标目录下 源文件为文件，目标也为文件，则在StandardCopyOption#REPLACE_EXISTING情况下覆盖之 |
| `cn.hutool.core.io.file.PathUtil` | `Path copyContent(Path src,Path target,CopyOption... options)` | 拷贝目录下的所有文件或目录到目标目录中，此方法不支持文件对文件的拷贝。 源文件为目录，目标也为目录或不存在，则拷贝目录下所有文件和目录到目标目录下 源文件为文件，目标为目录或不存在，则拷贝文件到目标目录下 |
| `cn.hutool.core.io.file.PathUtil` | `Path copyFile(InputStream src,Path target,CopyOption... options)` | 通过JDK7+的 Files#copy(InputStream, Path, CopyOption...) 方法拷贝文件 |
| `cn.hutool.core.io.file.PathUtil` | `Path copyFile(Path src,Path dest,StandardCopyOption... options)` | 通过JDK7+的 Files#copy(Path, Path, CopyOption...) 方法拷贝文件 此方法不支持递归拷贝目录，如果src传入是目录，只会在目标目录中创建空目录 |
| `cn.hutool.core.io.file.PathUtil` | `Path copyFile(Path src,Path target,CopyOption... options)` | 通过JDK7+的 Files#copy(Path, Path, CopyOption...) 方法拷贝文件 此方法不支持递归拷贝目录，如果src传入是目录，只会在目标目录中创建空目录 |
| `cn.hutool.core.io.file.PathUtil` | `Path copyFile(Resource src,Path target,CopyOption... options)` | 通过JDK7+的 Files#copy(InputStream, Path, CopyOption...) 方法拷贝文件 |
| `cn.hutool.core.io.file.PathUtil` | `Path createTempFile(final String prefix,final String suffix,final Path dir)` | 创建临时文件 创建后的文件名为 prefix[Random].suffix From com.jodd.io.FileUtil |
| `cn.hutool.core.io.file.PathUtil` | `Path getLastPathEle(Path path)` | 获取指定位置的最后一个子路径部分 |
| `cn.hutool.core.io.file.PathUtil` | `Path getPathEle(Path path,int index)` | 获取指定位置的子路径部分，支持负数，例如index为-1表示从后数第一个节点位置 |
| `cn.hutool.core.io.file.PathUtil` | `Path mkParentDirs(Path path)` | 创建所给文件或目录的父目录 |
| `cn.hutool.core.io.file.PathUtil` | `Path mkdir(Path dir)` | 创建所给目录及其父目录 |
| `cn.hutool.core.io.file.PathUtil` | `Path move(Path src,Path target,boolean isOverride)` | 移动文件或目录到目标中，例如： 如果src和target为同一文件或目录，直接返回target。 如果src为文件，target为目录，则移动到目标目录下，存在同名文件则按照是否覆盖参数执行。 如果src为文件，target为文件，则按照是否覆盖参数执行。 如果src为文件，target为不存在的路径，则重命名源文件到目标指定的文件，如moveContent("/a/b", "/c/d"), d不存在，则b变成d。 如果src为目录，target为文件，抛出IllegalArgumentException 如果src为目录，target为目录，则将源目录及其内容移动到目标路径目录中，如move… |
| `cn.hutool.core.io.file.PathUtil` | `Path moveContent(Path src,Path target,boolean isOverride)` | 移动文件或目录内容到目标中，例如： 如果src为文件，target为目录，则移动到目标目录下，存在同名文件则按照是否覆盖参数执行。 如果src为文件，target为文件，则按照是否覆盖参数执行。 如果src为文件，target为不存在的路径，则重命名源文件到目标指定的文件，如moveContent("/a/b", "/c/d"), d不存在，则b变成d。 如果src为目录，target为文件，抛出IllegalArgumentException 如果src为目录，target为目录，则将源目录下的内容移动到目标路径目录中，源目录不删除。 如果src为目录，target为不存在的路径，则创建目标… |
| `cn.hutool.core.io.file.PathUtil` | `Path rename(Path path,String newName,boolean isOverride)` | 修改文件或目录的文件名，不变更路径，只是简单修改文件名 |
| `cn.hutool.core.io.file.PathUtil` | `Path subPath(Path path,int fromIndex,int toIndex)` | 获取指定位置的子路径部分，支持负数，例如起始为-1表示从后数第一个节点位置 |
| `cn.hutool.core.io.file.PathUtil` | `Path toAbsNormal(Path path)` | 将Path路径转换为标准的绝对路径 |
| `cn.hutool.core.io.file.PathUtil` | `Set<FileVisitOption> getFileVisitOption(final boolean isFollowLinks)` | 构建是否追踪软链的选项 |
| `cn.hutool.core.io.file.PathUtil` | `String getMimeType(Path file)` | 获得文件的MimeType |
| `cn.hutool.core.io.file.PathUtil` | `String getName(Path path)` | 获取Path文件名 |
| `cn.hutool.core.io.file.PathUtil` | `boolean del(Path path)` | 删除文件或者文件夹，不追踪软链 注意：删除文件夹时不会判断文件夹是否为空，如果不空则递归删除子文件或文件夹 某个文件删除失败会终止删除操作 |
| `cn.hutool.core.io.file.PathUtil` | `boolean equals(Path file1,Path file2)` | 检查两个文件是否是同一个文件 所谓文件相同，是指Path对象是否指向同一个文件或文件夹 |
| `cn.hutool.core.io.file.PathUtil` | `boolean exists(Path path,boolean isFollowLinks)` | 判断文件或目录是否存在 |
| `cn.hutool.core.io.file.PathUtil` | `boolean isDirEmpty(Path dirPath)` | 目录是否为空 |
| `cn.hutool.core.io.file.PathUtil` | `boolean isDirectory(Path path)` | 判断是否为目录，如果file为null，则返回false 此方法不会追踪到软链对应的真实地址，即软链被当作文件 |
| `cn.hutool.core.io.file.PathUtil` | `boolean isDirectory(Path path,boolean isFollowLinks)` | 判断是否为目录，如果file为null，则返回false |
| `cn.hutool.core.io.file.PathUtil` | `boolean isExistsAndNotDirectory(final Path path,final boolean isFollowLinks)` | 判断是否存在且为非目录 如果path为null，返回false 如果path不存在，返回false |
| `cn.hutool.core.io.file.PathUtil` | `boolean isFile(Path path,boolean isFollowLinks)` | 判断是否为文件，如果file为null，则返回false |
| `cn.hutool.core.io.file.PathUtil` | `boolean isSub(Path parent,Path sub)` | 判断给定的目录是否为给定文件或文件夹的子目录 |
| `cn.hutool.core.io.file.PathUtil` | `boolean isSymlink(Path path)` | 判断是否为符号链接文件 |
| `cn.hutool.core.io.file.PathUtil` | `byte[] readBytes(Path path)` | 读取文件的所有内容为byte数组 |
| `cn.hutool.core.io.file.PathUtil` | `void walkFiles(Path start,FileVisitor<? super Path> visitor)` | 遍历指定path下的文件并做处理 |
| `cn.hutool.core.io.file.PathUtil` | `void walkFiles(Path start,int maxDepth,FileVisitor<? super Path> visitor)` | 遍历指定path下的文件并做处理 |
| `cn.hutool.core.io.file.PathUtil` | `void walkFiles(final Path start,int maxDepth,final boolean isFollowLinks,final FileVisitor<? super Path> visitor)` | 遍历指定path下的文件并做处理 |
| `cn.hutool.core.io.file.Tailer` | `void setStopOnDelete(final boolean stopOnDelete)` | 设置删除文件后是否退出并抛出异常 |
| `cn.hutool.core.io.file.Tailer` | `void start()` | 开始监听 |
| `cn.hutool.core.io.file.Tailer` | `void start(boolean async)` | 开始监听 |
| `cn.hutool.core.io.file.Tailer` | `void stop()` | 结束，此方法需在异步模式或 |
| `cn.hutool.core.io.file.Tailer$ConsoleLineHandler` | `void handle(String line)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
