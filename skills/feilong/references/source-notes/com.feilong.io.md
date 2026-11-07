# com.feilong.io

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.io.FileUtil` | `FileInputStream getFileInputStream(File file)` | 从文件系统中的文件 file 中获得输入字节. java.io.FileInputStream 用于读取诸如图像数据之类的原始字节流. 要读取字符流,请考虑使用 java.io.FileReader 如果指定文件不存在;或者它是一个目录,而不是一个常规文件;亦或因为其他某些原因而无法打开进行读取,则抛出 FileNotFoundException |
| `com.feilong.io.FileUtil` | `FileInputStream getFileInputStream(String filePath)` | 从文件系统中的文件 filePath 中获得输入字节. java.io.FileInputStream 用于读取诸如图像数据之类的原始字节流. 要读取字符流,请考虑使用 java.io.FileReader |
| `com.feilong.io.FileUtil` | `FileOutputStream getFileOutputStream(String filePath)` | 获得 java.io.FileOutputStream FileOutputStream 文件输出流. 该方法输出是使用 覆盖模式, 如果要使用追加模式, 请调用 #getFileOutputStream(String, FileWriteMode) java.io.FileOutputStream FileOutputStream 用于写入诸如图像数据之类的原始字节的流. 如果要写入字符流,请考虑使用 java.io.FileWriter. |
| `com.feilong.io.FileUtil` | `FileOutputStream getFileOutputStream(String filePath,FileWriteMode fileWriteMode)` | 获得 java.io.FileOutputStream FileOutputStream 文件输出流. java.io.FileOutputStream FileOutputStream 用于写入诸如图像数据之类的原始字节的流. 如果要写入字符流,请考虑使用 java.io.FileWriter. |
| `com.feilong.io.FileUtil` | `String formatSize(long fileSize)` | 文件大小 fileSize 格式化. 目前支持单位有TB GB MB KB以及最小单位 Bytes |
| `com.feilong.io.FileUtil` | `String getFileFormatSize(File file)` | 获得文件 file 格式化大小. 比如文件3834字节,格式化大小 3.74KB 比如文件36830335 字节, 格式化大小:35.12MB 比如文件2613122669 字节, 格式化大小 : 2.43GB 目前支持单位有TB GB MB KB以及最小单位 Bytes |
| `com.feilong.io.FileUtil` | `String getParent(String filePath)` | 返回此路径 filePath 父目录的路径名字符串. |
| `com.feilong.io.FileUtil` | `URL[] toURLs(List<String> filePathList)` | 将 filePathList 转成 URL 数组. |
| `com.feilong.io.FileUtil` | `URL[] toURLs(String... filePaths)` | 将 filePaths 转成 URL 数组. |
| `com.feilong.io.FileUtil` | `boolean deleteFileOrDirectory(File file)` | 删除文件或者文件夹,如果是文件夹 ,递归深层次删除. Deletes a file, never throwing an exception. If file is a directory, delete it and all sub-directories. |
| `com.feilong.io.FileUtil` | `boolean deleteFileOrDirectory(String filePath)` | 删除文件或者文件夹,如果是文件夹 ,递归深层次 删除. Deletes a file, never throwing an exception. If file is a directory, delete it and all sub-directories. |
| `com.feilong.io.FileUtil` | `boolean isEmptyDirectory(String directory)` | 判断一个目录是否是空目录 (判断的原则:里面没有文件) . |
| `com.feilong.io.FileUtil` | `boolean isExistFile(String filePath)` | 判断文件 filePath 是否存在. |
| `com.feilong.io.FileUtil` | `boolean isNotExistFile(String filePath)` | 判断文件 filePath 不存在. |
| `com.feilong.io.FileUtil` | `byte[] toByteArray(File file)` | 将文件转成 byte[] bytes . |
| `com.feilong.io.FileUtil` | `byte[] toByteArray(String filePath)` | 将文件 filePath 转成 byte[] bytes . |
| `com.feilong.io.FileUtil` | `long getFileSize(File file)` | 返回指定的文件或目录 file 的大小, 取得文件大小(单位字节). 返回指定的文件或目录的大小。 如果提供的文件是一个常规文件,那么文件的长度将被返回。 如果参数是一个目录,那么目录的大小是递归计算的。 |
| `com.feilong.io.FileUtil` | `void createDirectory(String directory)` | 创建文件夹,支持 级联创建 . |
| `com.feilong.io.FileUtil` | `void createDirectoryByFilePath(String filePath)` | 创建文件夹,by文件路径 filePath ,支持级联创建. |
| `com.feilong.io.FilenameUtil` | `List<String> getParentPathList(String path)` | 获得路径的所有 parent路径. 目前的使用场景有, 创建远程sftp目录地址 |
| `com.feilong.io.FilenameUtil` | `String getExtension(String fileName)` | 获得文件后缀名(不带. 的后缀),并返回原样字母. 如果文件没有后缀名 返回 "" (EMPTY) |
| `com.feilong.io.FilenameUtil` | `String getExtensionLowerCase(String fileName)` | 获得文件后缀名,并返回 小写字母 . |
| `com.feilong.io.FilenameUtil` | `String getFileName(String fileName)` | 获得带后缀的文件纯名称. 如:F:/pie2.png,返回 pie2.png |
| `com.feilong.io.FilenameUtil` | `String getFilePreName(String fileName)` | 获得文件的不带后缀名的名称. |
| `com.feilong.io.FilenameUtil` | `String getFileTopParentName(File file)` | 获得文件的最顶层父文件夹名称. |
| `com.feilong.io.FilenameUtil` | `String getFileTopParentName(String pathname)` | 获得文件的最顶层 父文件夹名称. |
| `com.feilong.io.FilenameUtil` | `String getFormatFileName(final String fileName)` | 不同的操作系统 对系统文件名称有要求,此方法的作用就是处理这些文件名称. |
| `com.feilong.io.FilenameUtil` | `String getNewFileName(String fileName,String newPostfixName)` | 将一个文件使用新的文件后缀,其余部分不变. 如果一个文件没有后缀,将会添加 .+newPostfixName |
| `com.feilong.io.FilenameUtil` | `boolean isExtensionIgnoreCase(String filename,String... extensions)` | 判断文件的扩展名是不是指定的扩展名中间的一个(忽略大小写比较). This method obtains the extension as the textual part of the filename after the last dot. There must be no directory separator after the dot. |
| `com.feilong.io.IOReaderUtil` | `List<String> readToList(File file,ReaderConfig readerConfig)` | 使用 ReaderConfig解析 Reader. |
| `com.feilong.io.IOReaderUtil` | `List<String> readToList(Reader reader,ReaderConfig readerConfig)` | 使用 ReaderConfig解析 Reader. |
| `com.feilong.io.IOReaderUtil` | `List<String> readToList(String location)` | 直接解析 location 成 List. |
| `com.feilong.io.IOReaderUtil` | `List<String> readToList(String location,ReaderConfig readerConfig)` | 使用 ReaderConfig解析 Reader. |
| `com.feilong.io.IOReaderUtil` | `Set<String> readToSet(File file,ReaderConfig readerConfig)` | 使用 ReaderConfig解析 Reader. |
| `com.feilong.io.IOReaderUtil` | `Set<String> readToSet(Reader reader,ReaderConfig readerConfig)` | 使用 ReaderConfig解析 Reader. |
| `com.feilong.io.IOReaderUtil` | `Set<String> readToSet(String location)` | 直接解析 location 成 Set. |
| `com.feilong.io.IOReaderUtil` | `Set<String> readToSet(String location,ReaderConfig readerConfig)` | 使用 ReaderConfig解析 Reader. |
| `com.feilong.io.IOReaderUtil` | `String readToString(File file,String charsetName)` | 获得文件内容直接转成字符串. 方法内部已经关闭了相关流 |
| `com.feilong.io.IOReaderUtil` | `String readToString(FileInputStream fileInputStream,String charsetName)` | 读取文件内容. 方法内部已经关闭了相关流 |
| `com.feilong.io.IOReaderUtil` | `String readToString(InputStream inputStream,String charsetName)` | 读取 InputStream 内容. 方法内部已经关闭了相关流 |
| `com.feilong.io.IOReaderUtil` | `String readToString(String location)` | 获得文件内容直接转成字符串. 方法内部已经关闭了相关流 |
| `com.feilong.io.IOReaderUtil` | `String readToString(String location,String charsetName)` | 获得文件内容直接转成字符串. 方法内部已经关闭了相关流 |
| `com.feilong.io.IOReaderUtil` | `T readToCollection(Reader reader,ReaderConfig readerConfig,T collection)` | 使用 ReaderConfig解析 Reader. |
| `com.feilong.io.IOReaderUtil` | `byte[] readToByteArray(String location)` | 获得内容直接转成字节数组. 方法内部已经关闭了相关流 |
| `com.feilong.io.IOReaderUtil` | `void resolverFile(File file,LineNumberReaderResolver lineNumberReaderResolver)` | 使用 LineNumberReaderResolver解析文件. 如果 file 是null,抛出 NullPointerException 如果 lineNumberReaderResolver 是null,抛出 NullPointerException |
| `com.feilong.io.IOReaderUtil` | `void resolverFile(Reader reader,LineNumberReaderResolver lineNumberReaderResolver)` | 使用 LineNumberReaderResolver解析 Reader. |
| `com.feilong.io.IOReaderUtil` | `void resolverFile(String location,LineNumberReaderResolver lineNumberReaderResolver)` | 使用 LineNumberReaderResolver解析文件. 如果 location 是null,抛出 NullPointerException 如果 location 是blank,抛出 IllegalArgumentException 如果 lineNumberReaderResolver 是null,抛出 NullPointerException |
| `com.feilong.io.IOUtil` | `int copy(final InputStream input,final OutputStream output)` | 【原文待译】Copies bytes from an InputStream to an OutputStream . This method buffers the input internally, so there is no need to use a BufferedInputStream . Large streams (over 2GB) will return a bytes copied value of -1 after the copy has completed since the correct number of bytes cannot be returned as an i… |
| `com.feilong.io.IOUtil` | `void closeQuietly(final Closeable... closeables)` | 【原文待译】Closes a Closeable unconditionally. Equivalent to Closeable#close(), except any exceptions will be ignored. This is typically used in finally blocks to ensure that the closeable is closed even if an Exception was thrown before the normal close statement was reached. It should not be used to replace … |
| `com.feilong.io.IOWriteUtil` | `String write(InputStream inputStream,String directoryPath,String fileName)` | 将inputStream 写到某个文件夹 directoryPath ,名字为 fileName . (注意,本方法最终会关闭 inputStream 以及 outputStream ). 如果拼接完的文件路径,父路径不存在,则自动创建 (支持级联创建文件夹) |
| `com.feilong.io.IOWriteUtil` | `void write(InputStream inputStream,OutputStream outputStream)` | 写资源,速度最快的方法,速度比较请看 电脑资料 >. (注意,本方法最终会关闭 inputStream 以及 outputStream ). Just write in blocks instead of copying it entirely into Java's memory first. The below basic example writes it in blocks of 10KB. This way you end up with a consistent memory usage of only 10KB instead of the complete content le… |
| `com.feilong.io.IOWriteUtil` | `void write(InputStream inputStream,OutputStream outputStream,int bufferLength)` | 写资源,速度最快的方法,速度比较请看电脑资料 > . (注意,本方法最终会关闭 inputStream 以及 outputStream ). 如果 inputStream 是null,抛出 NullPointerException 如果 outputStream 是null,抛出 NullPointerException |
| `com.feilong.io.IOWriteUtil` | `void writeStringToFile(String filePath,String content)` | 将字符串/文字写到文件中. |
| `com.feilong.io.IOWriteUtil` | `void writeStringToFile(String filePath,String content,String charsetType)` | 将字符串/文字写到文件中. |
| `com.feilong.io.IOWriteUtil` | `void writeStringToFile(String filePath,String content,String charsetType,FileWriteMode fileWriteMode)` | 将字符串写到文件中. (注意,本方法最终会关闭 inputStream 以及 outputStream ). |
| `com.feilong.io.InputStreamUtil` | `BufferedReader toBufferedReader(InputStream inputStream,String charsetName)` | 将 java.io.InputStream 转成 java.io.BufferedReader (java.io.BufferedReader 缓冲 高效读取). |
| `com.feilong.io.InputStreamUtil` | `InputStream getInputStream(String location)` | Return a Resource handle for the 指定的资源路径. The handle should always be a reusable resource descriptor,allowing for multiple Resource#getInputStream() calls. Note that a Resource handle does not imply an existing resource; you need to invoke Resource#exists to check for existence. |
| `com.feilong.io.InputStreamUtil` | `InputStream newByteArrayInputStream(String str,String charsetType)` | 构造一个 ByteArrayInputStream. |
| `com.feilong.io.InputStreamUtil` | `String toString(InputStream inputStream)` | 使用默认的编码集 Charset#defaultCharset() 将 java.io.InputStream 转成string. 如果需要将 String 转成 InputStream 可以调用 IOUtils#toInputStream(String, Charset) |
| `com.feilong.io.InputStreamUtil` | `String toString(InputStream inputStream,String charsetName)` | 将 java.io.InputStream 转成string. 读取cmd命令结果时候, 有时候读取的是乱码,需要传递 charsetName 字符集. 如果需要将 String 转成 InputStream 可以调用 IOUtils#toInputStream(String, Charset) |
| `com.feilong.io.LineNumberReaderResolver` | `boolean resolve(int lineNumber,String line)` | 每行读取的时候的操作. |
| `com.feilong.io.MimeTypeUtil` | `String getContentTypeByFileName(String fileName)` | 获得 content type by file name. Very incomplete function. As of Java 7, html, pdf and jpeg extensions 返回正确的 mime-type,但是js 和 css 返回 null! I tried Apache Tika but it is huge with tons of dependencies, URLConnection doesn't use the bytes of the files, javax.activation.MimetypesFileTypeMap also just look… |
| `com.feilong.io.ReaderConfig` | `String getRegexPattern()` | 获得 符合正则的内容才抓取,不符合的跳过. |
| `com.feilong.io.ReaderConfig` | `boolean getIgnoreBlankLine()` | 获得 是否忽略空白行. |
| `com.feilong.io.ReaderConfig` | `boolean getIsTrim()` | 获得 是否去空格. |
| `com.feilong.io.ReaderConfig` | `void setIgnoreBlankLine(boolean ignoreBlankLine)` | 设置 是否忽略空白行. |
| `com.feilong.io.ReaderConfig` | `void setIsTrim(boolean isTrim)` | 设置 是否去空格. |
| `com.feilong.io.ReaderConfig` | `void setRegexPattern(String regexPattern)` | 设置 符合正则的内容才抓取,不符合的跳过. |
| `com.feilong.io.ReaderUtil` | `String readLine(Reader reader)` | 读取 java.io.Reader 第一行内容. |
| `com.feilong.io.ReaderUtil` | `String toString(Reader reader)` | 将 java.io.Reader 转成 java.lang.String. |
| `com.feilong.io.ReaderUtil` | `StringReader newStringReader(String str)` | 构造一个 StringReader. |
