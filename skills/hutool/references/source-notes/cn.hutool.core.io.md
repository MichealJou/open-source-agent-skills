# cn.hutool.core.io

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.io.AppendableWriter` | `Writer append(final CharSequence csq)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.AppendableWriter` | `Writer append(final CharSequence csq,final int start,final int end)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.AppendableWriter` | `Writer append(final char c)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.AppendableWriter` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.AppendableWriter` | `void flush()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.AppendableWriter` | `void write(final String str)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.AppendableWriter` | `void write(final String str,final int off,final int len)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.AppendableWriter` | `void write(final char[] cbuf)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.AppendableWriter` | `void write(final char[] cbuf,final int off,final int len)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.AppendableWriter` | `void write(final int c)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.BOMInputStream` | `String getCharset()` | 获取BOM头中的编码 |
| `cn.hutool.core.io.BOMInputStream` | `String getDefaultCharset()` | 获取默认编码 |
| `cn.hutool.core.io.BOMInputStream` | `int read()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.BOMInputStream` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.BomReader` | `int read(char[] cbuf,int off,int len)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.BomReader` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.BufferUtil` | `ByteBuffer copy(ByteBuffer src,ByteBuffer dest)` | 拷贝ByteBuffer |
| `cn.hutool.core.io.BufferUtil` | `ByteBuffer copy(ByteBuffer src,ByteBuffer dest,int length)` | 拷贝ByteBuffer |
| `cn.hutool.core.io.BufferUtil` | `ByteBuffer copy(ByteBuffer src,int srcStart,ByteBuffer dest,int destStart,int length)` | 拷贝ByteBuffer |
| `cn.hutool.core.io.BufferUtil` | `ByteBuffer copy(ByteBuffer src,int start,int end)` | 拷贝到一个新的ByteBuffer |
| `cn.hutool.core.io.BufferUtil` | `ByteBuffer create(CharSequence data,Charset charset)` | 从字符串创建新Buffer |
| `cn.hutool.core.io.BufferUtil` | `ByteBuffer create(byte[] data)` | 创建新Buffer |
| `cn.hutool.core.io.BufferUtil` | `ByteBuffer createUtf8(CharSequence data)` | 从字符串创建新Buffer，使用UTF-8编码 |
| `cn.hutool.core.io.BufferUtil` | `CharBuffer createCharBuffer(int capacity)` | 创建CharBuffer |
| `cn.hutool.core.io.BufferUtil` | `String readLine(ByteBuffer buffer,Charset charset)` | 读取一行，如果buffer中最后一部分并非完整一行，则返回null 支持的换行符如下： |
| `cn.hutool.core.io.BufferUtil` | `String readStr(ByteBuffer buffer,Charset charset)` | 读取剩余部分并转为字符串 |
| `cn.hutool.core.io.BufferUtil` | `String readUtf8Str(ByteBuffer buffer)` | 读取剩余部分并转为UTF-8编码字符串 |
| `cn.hutool.core.io.BufferUtil` | `byte[] readBytes(ByteBuffer buffer)` | 读取剩余部分bytes |
| `cn.hutool.core.io.BufferUtil` | `byte[] readBytes(ByteBuffer buffer,int maxLength)` | 读取指定长度的bytes 如果长度不足，则读取剩余部分，此时buffer必须为读模式 |
| `cn.hutool.core.io.BufferUtil` | `byte[] readBytes(ByteBuffer buffer,int start,int end)` | 读取指定区间的数据 |
| `cn.hutool.core.io.BufferUtil` | `int lineEnd(ByteBuffer buffer)` | 一行的末尾位置，查找位置时位移ByteBuffer到结束位置 |
| `cn.hutool.core.io.BufferUtil` | `int lineEnd(ByteBuffer buffer,int maxLength)` | 一行的末尾位置，查找位置时位移ByteBuffer到结束位置 支持的换行符如下： |
| `cn.hutool.core.io.CharsetDetector` | `Charset detect(File file,Charset... charsets)` | 探测文件编码 |
| `cn.hutool.core.io.CharsetDetector` | `Charset detect(InputStream in,Charset... charsets)` | 探测编码 注意：此方法会读取流的一部分，然后关闭流，如重复使用流，请使用支持reset方法的流 |
| `cn.hutool.core.io.CharsetDetector` | `Charset detect(int bufferSize,InputStream in,Charset... charsets)` | 探测编码 注意：此方法会读取流的一部分，然后关闭流，如重复使用流，请使用支持reset方法的流 |
| `cn.hutool.core.io.FastByteArrayOutputStream` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastByteArrayOutputStream` | `String toString(Charset charset)` | 转为字符串 |
| `cn.hutool.core.io.FastByteArrayOutputStream` | `String toString(String charsetName)` | 转为字符串 |
| `cn.hutool.core.io.FastByteArrayOutputStream` | `byte[] toByteArray()` | 转为Byte数组 |
| `cn.hutool.core.io.FastByteArrayOutputStream` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastByteArrayOutputStream` | `void close()` | 此方法无任何效果，当流被关闭后不会抛出IOException |
| `cn.hutool.core.io.FastByteArrayOutputStream` | `void reset()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastByteArrayOutputStream` | `void write(byte[] b,int off,int len)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastByteArrayOutputStream` | `void write(int b)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastByteArrayOutputStream` | `void writeTo(OutputStream out)` | 写出 |
| `cn.hutool.core.io.FastByteBuffer` | `FastByteBuffer append(FastByteBuffer buff)` | 将另一个快速缓冲加入到自身 |
| `cn.hutool.core.io.FastByteBuffer` | `FastByteBuffer append(byte element)` | 向快速缓冲加入一个字节 |
| `cn.hutool.core.io.FastByteBuffer` | `FastByteBuffer append(byte[] array)` | 向快速缓冲加入数据 |
| `cn.hutool.core.io.FastByteBuffer` | `FastByteBuffer append(byte[] array,int off,int len)` | 向快速缓冲加入数据 |
| `cn.hutool.core.io.FastByteBuffer` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastByteBuffer` | `byte get(int index)` | 根据索引位返回一个字节 |
| `cn.hutool.core.io.FastByteBuffer` | `byte[] array(int index)` | 根据索引位返回缓冲集中的缓冲 |
| `cn.hutool.core.io.FastByteBuffer` | `byte[] toArray()` | 返回快速缓冲中的数据 |
| `cn.hutool.core.io.FastByteBuffer` | `byte[] toArray(int start,int len)` | 返回快速缓冲中的数据 |
| `cn.hutool.core.io.FastByteBuffer` | `int index()` | 当前缓冲位于缓冲区的索引位 |
| `cn.hutool.core.io.FastByteBuffer` | `int offset()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastByteBuffer` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastByteBuffer` | `void reset()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastStringWriter` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastStringWriter` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastStringWriter` | `void flush()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastStringWriter` | `void write(final String str)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastStringWriter` | `void write(final String str,final int off,final int len)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastStringWriter` | `void write(final char[] cbuf)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastStringWriter` | `void write(final char[] cbuf,final int off,final int len)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FastStringWriter` | `void write(final int c)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FileMagicNumber` | `FileMagicNumber getMagicNumber(final byte[] bytes)` | 根据给定的bytes，获取对应识别到的FileMagicNumber |
| `cn.hutool.core.io.FileMagicNumber` | `String getExtension()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FileMagicNumber` | `String getMimeType()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FileMagicNumber` | `boolean match(byte[] bytes)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.FileTypeUtil` | `String getType(File file)` | 根据文件流的头部信息获得文件类型 |
| `cn.hutool.core.io.FileTypeUtil` | `String getType(File file,boolean isExact)` | 根据文件流的头部信息获得文件类型 |
| `cn.hutool.core.io.FileTypeUtil` | `String getType(InputStream in)` | 根据文件流的头部信息获得文件类型 注意此方法会读取头部64个bytes，造成此流接下来读取时缺少部分bytes 因此如果想复用此流，流需支持InputStream#reset()方法。 |
| `cn.hutool.core.io.FileTypeUtil` | `String getType(InputStream in,String filename)` | 根据文件流的头部信息获得文件类型 注意此方法会读取头部64个bytes，造成此流接下来读取时缺少部分bytes 因此如果想复用此流，流需支持InputStream#reset()方法。 |
| `cn.hutool.core.io.FileTypeUtil` | `String getType(InputStream in,String filename,boolean isExact)` | 根据文件流的头部信息获得文件类型 注意此方法会读取头部一些bytes，造成此流接下来读取时缺少部分bytes 因此如果想复用此流，流需支持InputStream#reset()方法。 |
| `cn.hutool.core.io.FileTypeUtil` | `String getType(InputStream in,boolean isExact)` | 根据文件流的头部信息获得文件类型 注意此方法会读取头部一些bytes，造成此流接下来读取时缺少部分bytes 因此如果想复用此流，流需支持InputStream#reset()方法。 |
| `cn.hutool.core.io.FileTypeUtil` | `String getType(InputStream in,int fileHeadSize)` | 根据文件流的头部信息获得文件类型 |
| `cn.hutool.core.io.FileTypeUtil` | `String getType(String fileStreamHexHead)` | 根据文件流的头部信息获得文件类型 |
| `cn.hutool.core.io.FileTypeUtil` | `String getTypeByPath(String path)` | 通过路径获得文件类型 |
| `cn.hutool.core.io.FileTypeUtil` | `String getTypeByPath(String path,boolean isExact)` | 通过路径获得文件类型 |
| `cn.hutool.core.io.FileTypeUtil` | `String putFileType(String fileStreamHexHead,String extName)` | 增加文件类型映射 如果已经存在将覆盖之前的映射 |
| `cn.hutool.core.io.FileTypeUtil` | `String removeFileType(String fileStreamHexHead)` | 移除文件类型映射 |
| `cn.hutool.core.io.FileUtil` | `BOMInputStream getBOMInputStream(File file)` | 获得BOM输入流，用于处理带BOM头的文件 |
| `cn.hutool.core.io.FileUtil` | `BufferedInputStream getInputStream(File file)` | 获得输入流 |
| `cn.hutool.core.io.FileUtil` | `BufferedInputStream getInputStream(String path)` | 获得输入流 |
| `cn.hutool.core.io.FileUtil` | `BufferedOutputStream getOutputStream(File file)` | 获得一个输出流对象 |
| `cn.hutool.core.io.FileUtil` | `BufferedOutputStream getOutputStream(String path)` | 获得一个输出流对象 |
| `cn.hutool.core.io.FileUtil` | `BufferedReader getBOMReader(File file)` | 读取带BOM头的文件为Reader |
| `cn.hutool.core.io.FileUtil` | `BufferedReader getReader(File file,Charset charset)` | 获得一个文件读取器 |
| `cn.hutool.core.io.FileUtil` | `BufferedReader getReader(File file,String charsetName)` | 获得一个文件读取器 |
| `cn.hutool.core.io.FileUtil` | `BufferedReader getReader(String path,Charset charset)` | 获得一个文件读取器 |
| `cn.hutool.core.io.FileUtil` | `BufferedReader getReader(String path,String charsetName)` | 获得一个文件读取器 |
| `cn.hutool.core.io.FileUtil` | `BufferedReader getUtf8Reader(File file)` | 获得一个文件读取器 |
| `cn.hutool.core.io.FileUtil` | `BufferedReader getUtf8Reader(String path)` | 获得一个文件读取器 |
| `cn.hutool.core.io.FileUtil` | `BufferedWriter getWriter(File file,Charset charset,boolean isAppend)` | 获得一个带缓存的写入对象 |
| `cn.hutool.core.io.FileUtil` | `BufferedWriter getWriter(File file,String charsetName,boolean isAppend)` | 获得一个带缓存的写入对象 |
| `cn.hutool.core.io.FileUtil` | `BufferedWriter getWriter(String path,Charset charset,boolean isAppend)` | 获得一个带缓存的写入对象 |
| `cn.hutool.core.io.FileUtil` | `BufferedWriter getWriter(String path,String charsetName,boolean isAppend)` | 获得一个带缓存的写入对象 |
| `cn.hutool.core.io.FileUtil` | `Checksum checksum(File file,Checksum checksum)` | 计算文件校验码 |
| `cn.hutool.core.io.FileUtil` | `Date lastModifiedTime(File file)` | 指定文件最后修改时间 |
| `cn.hutool.core.io.FileUtil` | `Date lastModifiedTime(String path)` | 指定路径文件最后修改时间 |
| `cn.hutool.core.io.FileUtil` | `File appendLines(Collection<T> list,File file,Charset charset)` | 将列表写入文件，追加模式，策略为： 当文件为空，从开头追加，尾部不加空行 当有内容，换行追加，尾部不加空行 当有内容，并末尾有空行，依旧换行追加 |
| `cn.hutool.core.io.FileUtil` | `File appendLines(Collection<T> list,File file,String charset)` | 将列表写入文件，追加模式 |
| `cn.hutool.core.io.FileUtil` | `File appendLines(Collection<T> list,String path,Charset charset)` | 将列表写入文件，追加模式 |
| `cn.hutool.core.io.FileUtil` | `File appendLines(Collection<T> list,String path,String charset)` | 将列表写入文件，追加模式 |
| `cn.hutool.core.io.FileUtil` | `File appendString(String content,File file,Charset charset)` | 将String写入文件，追加模式 |
| `cn.hutool.core.io.FileUtil` | `File appendString(String content,File file,String charset)` | 将String写入文件，追加模式 |
| `cn.hutool.core.io.FileUtil` | `File appendString(String content,String path,Charset charset)` | 将String写入文件，追加模式 |
| `cn.hutool.core.io.FileUtil` | `File appendString(String content,String path,String charset)` | 将String写入文件，追加模式 |
| `cn.hutool.core.io.FileUtil` | `File appendUtf8Lines(Collection<T> list,File file)` | 将列表写入文件，追加模式 |
| `cn.hutool.core.io.FileUtil` | `File appendUtf8Lines(Collection<T> list,String path)` | 将列表写入文件，追加模式 |
| `cn.hutool.core.io.FileUtil` | `File appendUtf8String(String content,File file)` | 将String写入文件，UTF-8编码追加模式 |
| `cn.hutool.core.io.FileUtil` | `File appendUtf8String(String content,String path)` | 将String写入文件，UTF-8编码追加模式 |
| `cn.hutool.core.io.FileUtil` | `File checkSlip(File parentFile,File file)` | 检查父完整路径是否为自路径的前半部分，如果不是说明不是子路径，可能存在slip注入。 见http://blog.nsfocus.net/zip-slip-2/ |
| `cn.hutool.core.io.FileUtil` | `File convertCharset(File file,Charset srcCharset,Charset destCharset)` | 转换文件编码 此方法用于转换文件编码，读取的文件实际编码必须与指定的srcCharset编码一致，否则导致乱码 |
| `cn.hutool.core.io.FileUtil` | `File convertLineSeparator(File file,Charset charset,LineSeparator lineSeparator)` | 转换换行符 将给定文件的换行符转换为指定换行符 |
| `cn.hutool.core.io.FileUtil` | `File copy(File src,File dest,boolean isOverride)` | 复制文件或目录 情况如下： |
| `cn.hutool.core.io.FileUtil` | `File copy(String srcPath,String destPath,boolean isOverride)` | 复制文件或目录 如果目标文件为目录，则将源文件以相同文件名拷贝到目标目录 |
| `cn.hutool.core.io.FileUtil` | `File copyContent(File src,File dest,boolean isOverride)` | 复制文件或目录 情况如下： |
| `cn.hutool.core.io.FileUtil` | `File copyFile(File src,File dest,StandardCopyOption... options)` | 通过JDK7+的 Files#copy(Path, Path, CopyOption...) 方法拷贝文件 |
| `cn.hutool.core.io.FileUtil` | `File copyFile(InputStream src,File dest,StandardCopyOption... options)` | 通过JDK7+的 Files#copy(InputStream, Path, CopyOption...) 方法拷贝文件 |
| `cn.hutool.core.io.FileUtil` | `File copyFile(Resource src,File dest,StandardCopyOption... options)` | 通过JDK7+的 Files#copy(InputStream, Path, CopyOption...) 方法拷贝文件 |
| `cn.hutool.core.io.FileUtil` | `File copyFile(String src,String dest,StandardCopyOption... options)` | 通过JDK7+的 Files#copy(Path, Path, CopyOption...) 方法拷贝文件 |
| `cn.hutool.core.io.FileUtil` | `File copyFilesFromDir(File src,File dest,boolean isOverride)` | 复制文件或目录 情况如下： |
| `cn.hutool.core.io.FileUtil` | `File createTempFile()` | 在默认临时文件目录下创建临时文件，创建后的文件名为 prefix[Random].tmp。 默认临时文件目录由系统属性 java.io.tmpdir 指定。 在 UNIX 系统上，此属性的默认值通常是 "tmp" 或 "vartmp"； 在 Microsoft Windows 系统上，它通常是 "C:\\WINNT\\TEMP"。 调用 Java 虚拟机时，可以为该系统属性赋予不同的值，但不保证对该属性的编程更改对该方法使用的临时目录有任何影响。 |
| `cn.hutool.core.io.FileUtil` | `File createTempFile(File dir)` | 创建临时文件 创建后的文件名为 prefix[Random.tmp |
| `cn.hutool.core.io.FileUtil` | `File createTempFile(File dir,boolean isReCreat)` | 创建临时文件 创建后的文件名为 prefix[Random].tmp |
| `cn.hutool.core.io.FileUtil` | `File createTempFile(String prefix,String suffix,File dir,boolean isReCreat)` | 创建临时文件 创建后的文件名为 prefix[Random].suffix From com.jodd.io.FileUtil |
| `cn.hutool.core.io.FileUtil` | `File createTempFile(String prefix,String suffix,boolean isReCreat)` | 在默认临时文件目录下创建临时文件，创建后的文件名为 prefix[Random].suffix。 默认临时文件目录由系统属性 java.io.tmpdir 指定。 在 UNIX 系统上，此属性的默认值通常是 "tmp" 或 "vartmp"； 在 Microsoft Windows 系统上，它通常是 "C:\\WINNT\\TEMP"。 调用 Java 虚拟机时，可以为该系统属性赋予不同的值，但不保证对该属性的编程更改对该方法使用的临时目录有任何影响。 |
| `cn.hutool.core.io.FileUtil` | `File createTempFile(String suffix,boolean isReCreat)` | 在默认临时文件目录下创建临时文件，创建后的文件名为 prefix[Random].suffix。 默认临时文件目录由系统属性 java.io.tmpdir 指定。 在 UNIX 系统上，此属性的默认值通常是 "tmp" 或 "vartmp"； 在 Microsoft Windows 系统上，它通常是 "C:\\WINNT\\TEMP"。 调用 Java 虚拟机时，可以为该系统属性赋予不同的值，但不保证对该属性的编程更改对该方法使用的临时目录有任何影响。 |
| `cn.hutool.core.io.FileUtil` | `File file(File directory,String... names)` | 通过多层目录参数创建文件 此方法会检查slip漏洞，漏洞说明见http://blog.nsfocus.net/zip-slip-2/ |
| `cn.hutool.core.io.FileUtil` | `File file(File parent,String path)` | 创建File对象 根据的路径构建文件，在Win下直接构建，在Linux下拆分路径单独构建 此方法会检查slip漏洞，漏洞说明见http://blog.nsfocus.net/zip-slip-2/ |
| `cn.hutool.core.io.FileUtil` | `File file(String parent,String path)` | 创建File对象 此方法会检查slip漏洞，漏洞说明见http://blog.nsfocus.net/zip-slip-2/ |
| `cn.hutool.core.io.FileUtil` | `File file(String path)` | 创建File对象，自动识别相对或绝对路径，相对路径将自动从ClassPath下寻找 |
| `cn.hutool.core.io.FileUtil` | `File file(String... names)` | 通过多层目录创建文件 元素名（多层目录名） |
| `cn.hutool.core.io.FileUtil` | `File file(URI uri)` | 创建File对象 |
| `cn.hutool.core.io.FileUtil` | `File file(URL url)` | 创建File对象 |
| `cn.hutool.core.io.FileUtil` | `File getParent(File file,int level)` | 获取指定层级的父路径 |
| `cn.hutool.core.io.FileUtil` | `File getTmpDir()` | 获取临时文件目录 |
| `cn.hutool.core.io.FileUtil` | `File getUserHomeDir()` | 获取用户目录 |
| `cn.hutool.core.io.FileUtil` | `File getWebRoot()` | 获取Web项目下的web root路径 原理是首先获取ClassPath路径，由于在web项目中ClassPath位于 WEB-INF/classes/下，故向上获取两级目录即可。 |
| `cn.hutool.core.io.FileUtil` | `File mkParentDirs(File file)` | 创建所给文件或目录的父目录 |
| `cn.hutool.core.io.FileUtil` | `File mkParentDirs(String path)` | 创建父文件夹，如果存在直接返回此文件夹 |
| `cn.hutool.core.io.FileUtil` | `File mkdir(File dir)` | 创建文件夹，会递归自动创建其不存在的父文件夹，如果存在直接返回此文件夹 此方法不对File对象类型做判断，如果File不存在，无法判断其类型 |
| `cn.hutool.core.io.FileUtil` | `File mkdir(String dirPath)` | 创建文件夹，如果存在直接返回此文件夹 此方法不对File对象类型做判断，如果File不存在，无法判断其类型 |
| `cn.hutool.core.io.FileUtil` | `File newFile(String path)` | 创建File对象，相当于调用new File()，不做任何处理 |
| `cn.hutool.core.io.FileUtil` | `File rename(File file,String newName,boolean isOverride)` | 修改文件或目录的文件名，不变更路径，只是简单修改文件名，不保留扩展名。 |
| `cn.hutool.core.io.FileUtil` | `File rename(File file,String newName,boolean isRetainExt,boolean isOverride)` | 修改文件或目录的文件名，不变更路径，只是简单修改文件名 重命名有两种模式： 1、isRetainExt为true时，保留原扩展名： |
| `cn.hutool.core.io.FileUtil` | `File touch(File file)` | 创建文件及其父目录，如果这个文件存在，直接返回这个文件 此方法不对File对象类型做判断，如果File不存在，无法判断其类型 |
| `cn.hutool.core.io.FileUtil` | `File touch(File parent,String path)` | 创建文件及其父目录，如果这个文件存在，直接返回这个文件 此方法不对File对象类型做判断，如果File不存在，无法判断其类型 |
| `cn.hutool.core.io.FileUtil` | `File touch(String parent,String path)` | 创建文件及其父目录，如果这个文件存在，直接返回这个文件 此方法不对File对象类型做判断，如果File不存在，无法判断其类型 |
| `cn.hutool.core.io.FileUtil` | `File touch(String path)` | 创建文件及其父目录，如果这个文件存在，直接返回这个文件 此方法不对File对象类型做判断，如果File不存在，无法判断其类型 |
| `cn.hutool.core.io.FileUtil` | `File writeBytes(byte[] data,File dest)` | 写数据到文件中 |
| `cn.hutool.core.io.FileUtil` | `File writeBytes(byte[] data,File dest,int off,int len,boolean isAppend)` | 写入数据到文件 |
| `cn.hutool.core.io.FileUtil` | `File writeBytes(byte[] data,String path)` | 写数据到文件中 文件路径如果是相对路径，则相对ClassPath |
| `cn.hutool.core.io.FileUtil` | `File writeFromStream(InputStream in,File dest)` | 将流的内容写入文件 此方法会自动关闭输入流 |
| `cn.hutool.core.io.FileUtil` | `File writeFromStream(InputStream in,File dest,boolean isCloseIn)` | 将流的内容写入文件 |
| `cn.hutool.core.io.FileUtil` | `File writeFromStream(InputStream in,String fullFilePath)` | 将流的内容写入文件 此方法会自动关闭输入流 |
| `cn.hutool.core.io.FileUtil` | `File writeLines(Collection<T> list,File file,Charset charset)` | 将列表写入文件，覆盖模式 |
| `cn.hutool.core.io.FileUtil` | `File writeLines(Collection<T> list,File file,Charset charset,boolean isAppend)` | 将列表写入文件 |
| `cn.hutool.core.io.FileUtil` | `File writeLines(Collection<T> list,File file,String charset)` | 将列表写入文件，覆盖模式 |
| `cn.hutool.core.io.FileUtil` | `File writeLines(Collection<T> list,File file,String charset,boolean isAppend)` | 将列表写入文件 |
| `cn.hutool.core.io.FileUtil` | `File writeLines(Collection<T> list,String path,Charset charset)` | 将列表写入文件，覆盖模式 |
| `cn.hutool.core.io.FileUtil` | `File writeLines(Collection<T> list,String path,Charset charset,boolean isAppend)` | 将列表写入文件 |
| `cn.hutool.core.io.FileUtil` | `File writeLines(Collection<T> list,String path,String charset)` | 将列表写入文件，覆盖模式 |
| `cn.hutool.core.io.FileUtil` | `File writeLines(Collection<T> list,String path,String charset,boolean isAppend)` | 将列表写入文件 |
| `cn.hutool.core.io.FileUtil` | `File writeMap(Map<?, ?> map,File file,Charset charset,String kvSeparator,boolean isAppend)` | 将Map写入文件，每个键值对为一行，一行中键与值之间使用kvSeparator分隔 |
| `cn.hutool.core.io.FileUtil` | `File writeString(String content,File file,Charset charset)` | 将String写入文件，覆盖模式 |
| `cn.hutool.core.io.FileUtil` | `File writeString(String content,File file,String charset)` | 将String写入文件，覆盖模式 |
| `cn.hutool.core.io.FileUtil` | `File writeString(String content,String path,Charset charset)` | 将String写入文件，覆盖模式 |
| `cn.hutool.core.io.FileUtil` | `File writeString(String content,String path,String charset)` | 将String写入文件，覆盖模式 |
| `cn.hutool.core.io.FileUtil` | `File writeUtf8Lines(Collection<T> list,File file)` | 将列表写入文件，覆盖模式，编码为UTF-8 |
| `cn.hutool.core.io.FileUtil` | `File writeUtf8Lines(Collection<T> list,String path)` | 将列表写入文件，覆盖模式，编码为UTF-8 |
| `cn.hutool.core.io.FileUtil` | `File writeUtf8Map(Map<?, ?> map,File file,String kvSeparator,boolean isAppend)` | 将Map写入文件，每个键值对为一行，一行中键与值之间使用kvSeparator分隔 |
| `cn.hutool.core.io.FileUtil` | `File writeUtf8String(String content,File file)` | 将String写入文件，覆盖模式，字符集为UTF-8 |
| `cn.hutool.core.io.FileUtil` | `File writeUtf8String(String content,String path)` | 将String写入文件，覆盖模式，字符集为UTF-8 |
| `cn.hutool.core.io.FileUtil` | `File[] ls(String path)` | 列出指定路径下的目录和文件 给定的绝对路径不能是压缩包中的路径 |
| `cn.hutool.core.io.FileUtil` | `List<File> loopFiles(File file)` | 递归遍历目录以及子目录中的所有文件 |
| `cn.hutool.core.io.FileUtil` | `List<File> loopFiles(File file,FileFilter fileFilter)` | 递归遍历目录以及子目录中的所有文件 如果提供file为文件，直接返回过滤结果 |
| `cn.hutool.core.io.FileUtil` | `List<File> loopFiles(File file,int maxDepth,FileFilter fileFilter)` | 递归遍历目录以及子目录中的所有文件 如果提供file为文件，直接返回过滤结果 |
| `cn.hutool.core.io.FileUtil` | `List<File> loopFiles(String path)` | 递归遍历目录以及子目录中的所有文件 如果用户传入相对路径，则是相对classpath的路径 如："test/aaa"表示"${classpath}/test/aaa" |
| `cn.hutool.core.io.FileUtil` | `List<File> loopFiles(String path,FileFilter fileFilter)` | 递归遍历目录以及子目录中的所有文件 如果提供file为文件，直接返回过滤结果 |
| `cn.hutool.core.io.FileUtil` | `List<String> listFileNames(String path)` | 获得指定目录下所有文件 不会扫描子目录 如果用户传入相对路径，则是相对classpath的路径 如："test/aaa"表示"${classpath}/test/aaa" |
| `cn.hutool.core.io.FileUtil` | `List<String> readLines(File file,Charset charset)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `List<String> readLines(File file,Charset charset,Predicate<String> filter)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `List<String> readLines(File file,String charset)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `List<String> readLines(String path,Charset charset)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `List<String> readLines(String path,String charset)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `List<String> readLines(URL url,Charset charset)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `List<String> readLines(URL url,String charsetName)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `List<String> readUtf8Lines(File file)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `List<String> readUtf8Lines(File file,Predicate<String> filter)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `List<String> readUtf8Lines(String path)` | 从文件中读取每一行数据，编码为UTF-8 |
| `cn.hutool.core.io.FileUtil` | `List<String> readUtf8Lines(URL url)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `PrintWriter getPrintWriter(File file,Charset charset,boolean isAppend)` | 获得一个打印写入对象，可以有print |
| `cn.hutool.core.io.FileUtil` | `PrintWriter getPrintWriter(File file,String charset,boolean isAppend)` | 获得一个打印写入对象，可以有print |
| `cn.hutool.core.io.FileUtil` | `PrintWriter getPrintWriter(String path,Charset charset,boolean isAppend)` | 获得一个打印写入对象，可以有print |
| `cn.hutool.core.io.FileUtil` | `PrintWriter getPrintWriter(String path,String charset,boolean isAppend)` | 获得一个打印写入对象，可以有print |
| `cn.hutool.core.io.FileUtil` | `RandomAccessFile createRandomAccessFile(File file,FileMode mode)` | 创建RandomAccessFile |
| `cn.hutool.core.io.FileUtil` | `RandomAccessFile createRandomAccessFile(Path path,FileMode mode)` | 创建RandomAccessFile |
| `cn.hutool.core.io.FileUtil` | `String cleanInvalid(String fileName)` | 清除文件名中的在Windows下不支持的非法字符，包括： \ / : * ? " < > \| |
| `cn.hutool.core.io.FileUtil` | `String extName(File file)` | 获取文件扩展名（后缀名），扩展名不带“.” |
| `cn.hutool.core.io.FileUtil` | `String extName(String fileName)` | 获得文件的扩展名（后缀名），扩展名不带“.” |
| `cn.hutool.core.io.FileUtil` | `String getAbsolutePath(File file)` | 获取标准的绝对路径 |
| `cn.hutool.core.io.FileUtil` | `String getAbsolutePath(String path)` | 获取绝对路径，相对于ClassPath的目录 如果给定就是绝对路径，则返回原路径，原路径把所有\替换为/ 兼容Spring风格的路径表示，例如：classpath:config/example.setting也会被识别后转换 |
| `cn.hutool.core.io.FileUtil` | `String getAbsolutePath(String path,Class<?> baseClass)` | 获取绝对路径 此方法不会判定给定路径是否有效（文件或目录存在） |
| `cn.hutool.core.io.FileUtil` | `String getCanonicalPath(File file)` | 获取规范的绝对路径 |
| `cn.hutool.core.io.FileUtil` | `String getLineSeparator()` | 获取当前系统的换行分隔符 |
| `cn.hutool.core.io.FileUtil` | `String getMimeType(String filePath)` | 根据文件扩展名获得MimeType |
| `cn.hutool.core.io.FileUtil` | `String getName(File file)` | 返回文件名 |
| `cn.hutool.core.io.FileUtil` | `String getName(String filePath)` | 返回文件名 |
| `cn.hutool.core.io.FileUtil` | `String getParent(String filePath,int level)` | 获取指定层级的父路径 |
| `cn.hutool.core.io.FileUtil` | `String getPrefix(File file)` | 返回主文件名 |
| `cn.hutool.core.io.FileUtil` | `String getPrefix(String fileName)` | 返回主文件名 |
| `cn.hutool.core.io.FileUtil` | `String getSuffix(File file)` | 获取文件后缀名，扩展名不带“.” |
| `cn.hutool.core.io.FileUtil` | `String getSuffix(String fileName)` | 获得文件后缀名，扩展名不带“.” |
| `cn.hutool.core.io.FileUtil` | `String getTmpDirPath()` | 获取临时文件路径（绝对路径） |
| `cn.hutool.core.io.FileUtil` | `String getType(File file)` | 根据文件流的头部信息获得文件类型 |
| `cn.hutool.core.io.FileUtil` | `String getUserHomePath()` | 获取用户路径（绝对路径） |
| `cn.hutool.core.io.FileUtil` | `String mainName(File file)` | 返回主文件名 |
| `cn.hutool.core.io.FileUtil` | `String mainName(String fileName)` | 返回主文件名 |
| `cn.hutool.core.io.FileUtil` | `String normalize(String path)` | 修复路径 如果原路径尾部有分隔符，则保留为标准分隔符（/），否则不保留 1. 统一用 / 2. 多个 / 转换为一个 / 3. 去除左边空格 4. .. 和 . 转换为绝对路径，当..多于已有路径时，直接返回根路径 栗子： |
| `cn.hutool.core.io.FileUtil` | `String readLine(RandomAccessFile file,Charset charset)` | 单行处理文件内容 |
| `cn.hutool.core.io.FileUtil` | `String readString(File file,Charset charset)` | 读取文件内容 |
| `cn.hutool.core.io.FileUtil` | `String readString(File file,String charsetName)` | 读取文件内容 |
| `cn.hutool.core.io.FileUtil` | `String readString(String path,Charset charset)` | 读取文件内容 |
| `cn.hutool.core.io.FileUtil` | `String readString(String path,String charsetName)` | 读取文件内容 |
| `cn.hutool.core.io.FileUtil` | `String readString(URL url,Charset charset)` | 读取文件内容 |
| `cn.hutool.core.io.FileUtil` | `String readString(URL url,String charsetName)` | 读取文件内容 |
| `cn.hutool.core.io.FileUtil` | `String readUtf8String(File file)` | 读取文件内容 |
| `cn.hutool.core.io.FileUtil` | `String readUtf8String(String path)` | 读取文件内容 |
| `cn.hutool.core.io.FileUtil` | `String readableFileSize(File file)` | 可读的文件大小 |
| `cn.hutool.core.io.FileUtil` | `String readableFileSize(long size)` | 可读的文件大小 参考 http://stackoverflow.com/questions/3263892/format-file-size-as-mb-gb-etc |
| `cn.hutool.core.io.FileUtil` | `String subPath(String dirPath,String filePath)` | 获得相对子路径，忽略大小写 栗子： |
| `cn.hutool.core.io.FileUtil` | `String subPath(String rootDir,File file)` | 获得相对子路径 栗子： |
| `cn.hutool.core.io.FileUtil` | `T load(File file,Charset charset,ReaderHandler<T> readerHandler)` | 按照给定的readerHandler读取文件中的数据 |
| `cn.hutool.core.io.FileUtil` | `T load(String path,Charset charset,ReaderHandler<T> readerHandler)` | 按照给定的readerHandler读取文件中的数据 |
| `cn.hutool.core.io.FileUtil` | `T load(String path,String charset,ReaderHandler<T> readerHandler)` | 按照给定的readerHandler读取文件中的数据 |
| `cn.hutool.core.io.FileUtil` | `T loadUtf8(File file,ReaderHandler<T> readerHandler)` | 按照给定的readerHandler读取文件中的数据 |
| `cn.hutool.core.io.FileUtil` | `T loadUtf8(String path,ReaderHandler<T> readerHandler)` | 按照给定的readerHandler读取文件中的数据 |
| `cn.hutool.core.io.FileUtil` | `T readLines(File file,Charset charset,T collection)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `T readLines(File file,String charset,T collection)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `T readLines(String path,Charset charset,T collection)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `T readLines(String path,String charset,T collection)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `T readLines(URL url,Charset charset,T collection)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `T readLines(URL url,String charsetName,T collection)` | 从文件中读取每一行数据 |
| `cn.hutool.core.io.FileUtil` | `T readUtf8Lines(File file,T collection)` | 从文件中读取每一行数据，数据编码为UTF-8 |
| `cn.hutool.core.io.FileUtil` | `T readUtf8Lines(String path,T collection)` | 从文件中读取每一行的UTF-8编码数据 |
| `cn.hutool.core.io.FileUtil` | `T readUtf8Lines(URL url,T collection)` | 从文件中读取每一行数据，编码为UTF-8 |
| `cn.hutool.core.io.FileUtil` | `boolean clean(File directory)` | 清空文件夹 注意：清空文件夹时不会判断文件夹是否为空，如果不空则递归删除子文件或文件夹 某个文件删除失败会终止删除操作 |
| `cn.hutool.core.io.FileUtil` | `boolean clean(String dirPath)` | 清空文件夹 注意：清空文件夹时不会判断文件夹是否为空，如果不空则递归删除子文件或文件夹 某个文件删除失败会终止删除操作 |
| `cn.hutool.core.io.FileUtil` | `boolean cleanEmpty(File directory)` | 清理空文件夹 此方法用于递归删除空的文件夹，不删除文件 如果传入的文件夹本身就是空的，删除这个文件夹 |
| `cn.hutool.core.io.FileUtil` | `boolean containsInvalid(String fileName)` | 文件名中是否包含在Windows下不支持的非法字符，包括： \ / : * ? " < > \| |
| `cn.hutool.core.io.FileUtil` | `boolean contentEquals(File file1,File file2)` | 比较两个文件内容是否相同 首先比较长度，长度一致再比较内容 此方法来自Apache Commons io |
| `cn.hutool.core.io.FileUtil` | `boolean contentEqualsIgnoreEOL(File file1,File file2,Charset charset)` | 比较两个文件内容是否相同 首先比较长度，长度一致再比较内容，比较内容采用按行读取，每行比较 此方法来自Apache Commons io |
| `cn.hutool.core.io.FileUtil` | `boolean del(File file)` | 删除文件或者文件夹 注意：删除文件夹时不会判断文件夹是否为空，如果不空则递归删除子文件或文件夹 某个文件删除失败会终止删除操作 从5.7.6开始，删除文件使用Files#delete(Path)代替 File#delete() 因为前者遇到文件被占用等原因时，抛出异常，而非返回false，异常会指明具体的失败原因。 |
| `cn.hutool.core.io.FileUtil` | `boolean del(String fullFileOrDirPath)` | 删除文件或者文件夹 路径如果为相对路径，会转换为ClassPath路径！ 注意：删除文件夹时不会判断文件夹是否为空，如果不空则递归删除子文件或文件夹 某个文件删除失败会终止删除操作 |
| `cn.hutool.core.io.FileUtil` | `boolean equals(File file1,File file2)` | 检查两个文件是否是同一个文件 所谓文件相同，是指File对象是否指向同一个文件或文件夹 |
| `cn.hutool.core.io.FileUtil` | `boolean exist(File file)` | 判断文件是否存在，如果file为null，则返回false |
| `cn.hutool.core.io.FileUtil` | `boolean exist(String directory,String regexp)` | 是否存在匹配文件 |
| `cn.hutool.core.io.FileUtil` | `boolean exist(String path)` | 判断文件是否存在，如果path为null，则返回false |
| `cn.hutool.core.io.FileUtil` | `boolean isAbsolutePath(String path)` | 给定路径已经是绝对路径 此方法并没有针对路径做标准化，建议先执行#normalize(String)方法标准化路径后判断 绝对路径判断条件是： 以/开头的路径 满足类似于 c:/xxxxx，其中祖母随意，不区分大小写 满足类似于 d:\xxxxx，其中祖母随意，不区分大小写 满足windows SMB协议格式，如: \\192.168.254.1\Share |
| `cn.hutool.core.io.FileUtil` | `boolean isDirEmpty(File dir)` | 目录是否为空 |
| `cn.hutool.core.io.FileUtil` | `boolean isDirectory(File file)` | 判断是否为目录，如果file为null，则返回false |
| `cn.hutool.core.io.FileUtil` | `boolean isDirectory(String path)` | 判断是否为目录，如果path为null，则返回false |
| `cn.hutool.core.io.FileUtil` | `boolean isEmpty(File file)` | 文件是否为空 目录：里面没有文件时为空 文件：文件大小为0时为空 |
| `cn.hutool.core.io.FileUtil` | `boolean isFile(File file)` | 判断是否为文件，如果file为null，则返回false |
| `cn.hutool.core.io.FileUtil` | `boolean isFile(String path)` | 判断是否为文件，如果path为null，则返回false |
| `cn.hutool.core.io.FileUtil` | `boolean isModifed(File file,long lastModifyTime)` | 判断文件是否被改动 如果文件对象为 null 或者文件不存在，被视为改动 |
| `cn.hutool.core.io.FileUtil` | `boolean isModified(File file,long lastModifyTime)` | 判断文件是否被改动 如果文件对象为 null 或者文件不存在，被视为改动 |
| `cn.hutool.core.io.FileUtil` | `boolean isNotEmpty(File file)` | 目录是否为空 |
| `cn.hutool.core.io.FileUtil` | `boolean isSub(File parent,File sub)` | 判断给定的目录是否为给定文件或文件夹的子目录 |
| `cn.hutool.core.io.FileUtil` | `boolean isSymlink(File file)` | 判断是否为符号链接文件 |
| `cn.hutool.core.io.FileUtil` | `boolean isWindows()` | 是否为Windows环境 |
| `cn.hutool.core.io.FileUtil` | `boolean mkdirsSafely(File dir,int tryCount,long sleepMillis)` | 安全地级联创建目录 (确保并发环境下能创建成功) |
| `cn.hutool.core.io.FileUtil` | `boolean newerThan(File file,File reference)` | 给定文件或目录的最后修改时间是否晚于给定时间 |
| `cn.hutool.core.io.FileUtil` | `boolean newerThan(File file,long timeMillis)` | 给定文件或目录的最后修改时间是否晚于给定时间 |
| `cn.hutool.core.io.FileUtil` | `boolean pathEndsWith(File file,String suffix)` | 判断文件路径是否有指定后缀，忽略大小写 常用语判断扩展名 |
| `cn.hutool.core.io.FileUtil` | `boolean pathEquals(File file1,File file2)` | 文件路径是否相同 取两个文件的绝对路径比较，在Windows下忽略大小写，在Linux下不忽略。 |
| `cn.hutool.core.io.FileUtil` | `byte[] readBytes(File file)` | 读取文件所有数据 文件的长度不能超过Integer.MAX_VALUE |
| `cn.hutool.core.io.FileUtil` | `byte[] readBytes(String filePath)` | 读取文件所有数据 文件的长度不能超过Integer.MAX_VALUE |
| `cn.hutool.core.io.FileUtil` | `int getTotalLines(File file)` | 计算文件的总行数 参考：https://stackoverflow.com/questions/453018/number-of-lines-in-a-file-in-java |
| `cn.hutool.core.io.FileUtil` | `int getTotalLines(File file,int bufferSize)` | 计算文件的总行数 参考：https://stackoverflow.com/questions/453018/number-of-lines-in-a-file-in-java 最后一行如果末尾带有换行符，则被当作为新行 |
| `cn.hutool.core.io.FileUtil` | `int getTotalLines(File file,int bufferSize,boolean lastLineSeparatorAsNewLine)` | 计算文件的总行数 参考：https://stackoverflow.com/questions/453018/number-of-lines-in-a-file-in-java |
| `cn.hutool.core.io.FileUtil` | `int lastIndexOfSeparator(String filePath)` | 获得最后一个文件路径分隔符的位置 |
| `cn.hutool.core.io.FileUtil` | `long checksumCRC32(File file)` | 计算文件CRC32校验码 |
| `cn.hutool.core.io.FileUtil` | `long size(File file)` | 计算目录或文件的总大小 当给定对象为文件时，直接调用 File#length() 当给定对象为目录时，遍历目录下的所有文件和目录，递归计算其大小，求和返回 此方法不包括目录本身的占用空间大小。 |
| `cn.hutool.core.io.FileUtil` | `long size(File file,boolean includeDirSize)` | 计算目录或文件的总大小 当给定对象为文件时，直接调用 File#length() 当给定对象为目录时，遍历目录下的所有文件和目录，递归计算其大小，求和返回 |
| `cn.hutool.core.io.FileUtil` | `long writeToStream(File file,OutputStream out)` | 将文件写入流中，此方法不会关闭输出流 |
| `cn.hutool.core.io.FileUtil` | `long writeToStream(String fullFilePath,OutputStream out)` | 将路径对应文件写入流中，此方法不会关闭输出流 |
| `cn.hutool.core.io.FileUtil` | `void move(File src,File target,boolean isOverride)` | 移动文件或者目录 |
| `cn.hutool.core.io.FileUtil` | `void moveContent(File src,File target,boolean isOverride)` | 移动文件或者目录 |
| `cn.hutool.core.io.FileUtil` | `void readLine(RandomAccessFile file,Charset charset,LineHandler lineHandler)` | 单行处理文件内容 |
| `cn.hutool.core.io.FileUtil` | `void readLines(File file,Charset charset,LineHandler lineHandler)` | 按行处理文件内容 |
| `cn.hutool.core.io.FileUtil` | `void readLines(RandomAccessFile file,Charset charset,LineHandler lineHandler)` | 按行处理文件内容 |
| `cn.hutool.core.io.FileUtil` | `void readUtf8Lines(File file,LineHandler lineHandler)` | 按行处理文件内容，编码为UTF-8 |
| `cn.hutool.core.io.FileUtil` | `void tail(File file,Charset charset)` | 文件内容跟随器，实现类似Linux下"tail -f"命令功能 此方法会阻塞当前线程 |
| `cn.hutool.core.io.FileUtil` | `void tail(File file,Charset charset,LineHandler handler)` | 文件内容跟随器，实现类似Linux下"tail -f"命令功能 此方法会阻塞当前线程 |
| `cn.hutool.core.io.FileUtil` | `void tail(File file,LineHandler handler)` | 文件内容跟随器，实现类似Linux下"tail -f"命令功能 此方法会阻塞当前线程 |
| `cn.hutool.core.io.FileUtil` | `void walkFiles(File file,Consumer<File> consumer)` | 递归遍历目录并处理目录下的文件，可以处理目录或文件： 非目录则直接调用Consumer处理 目录则递归调用此方法处理 |
| `cn.hutool.core.io.IORuntimeException` | `boolean causeInstanceOf(Class<? extends Throwable> clazz)` | 导致这个异常的异常是否是指定类型的异常 |
| `cn.hutool.core.io.IoUtil` | `BomReader getBomReader(InputStream in)` | 从InputStream中获取BomReader |
| `cn.hutool.core.io.IoUtil` | `BufferedInputStream toBuffered(InputStream in)` | 转换为BufferedInputStream |
| `cn.hutool.core.io.IoUtil` | `BufferedInputStream toBuffered(InputStream in,int bufferSize)` | 转换为BufferedInputStream |
| `cn.hutool.core.io.IoUtil` | `BufferedOutputStream toBuffered(OutputStream out)` | 转换为BufferedOutputStream |
| `cn.hutool.core.io.IoUtil` | `BufferedOutputStream toBuffered(OutputStream out,int bufferSize)` | 转换为BufferedOutputStream |
| `cn.hutool.core.io.IoUtil` | `BufferedReader getReader(BOMInputStream in)` | 从BOMInputStream中获取Reader |
| `cn.hutool.core.io.IoUtil` | `BufferedReader getReader(InputStream in,Charset charset)` | 获得一个Reader |
| `cn.hutool.core.io.IoUtil` | `BufferedReader getReader(InputStream in,String charsetName)` | 获得一个文件读取器 |
| `cn.hutool.core.io.IoUtil` | `BufferedReader getReader(Reader reader)` | 获得BufferedReader 如果是BufferedReader强转返回，否则新建。如果提供的Reader为null返回null |
| `cn.hutool.core.io.IoUtil` | `BufferedReader getUtf8Reader(InputStream in)` | 获得一个文件读取器，默认使用UTF-8编码 |
| `cn.hutool.core.io.IoUtil` | `BufferedReader toBuffered(Reader reader)` | 转换为BufferedReader |
| `cn.hutool.core.io.IoUtil` | `BufferedReader toBuffered(Reader reader,int bufferSize)` | 转换为BufferedReader |
| `cn.hutool.core.io.IoUtil` | `BufferedWriter toBuffered(Writer writer)` | 转换为BufferedWriter |
| `cn.hutool.core.io.IoUtil` | `BufferedWriter toBuffered(Writer writer,int bufferSize)` | 转换为BufferedWriter |
| `cn.hutool.core.io.IoUtil` | `ByteArrayInputStream toStream(ByteArrayOutputStream out)` | ByteArrayOutputStream转为ByteArrayInputStream |
| `cn.hutool.core.io.IoUtil` | `ByteArrayInputStream toStream(String content,Charset charset)` | String 转为流 |
| `cn.hutool.core.io.IoUtil` | `ByteArrayInputStream toStream(String content,String charsetName)` | String 转为流 |
| `cn.hutool.core.io.IoUtil` | `ByteArrayInputStream toStream(byte[] content)` | byte[] 转为ByteArrayInputStream |
| `cn.hutool.core.io.IoUtil` | `ByteArrayInputStream toUtf8Stream(String content)` | String 转为UTF-8编码的字节流流 |
| `cn.hutool.core.io.IoUtil` | `Checksum checksum(InputStream in,Checksum checksum)` | 计算流的校验码，计算后关闭流 |
| `cn.hutool.core.io.IoUtil` | `FastByteArrayOutputStream read(InputStream in)` | 从流中读取内容，读到输出流中，读取完毕后关闭流 |
| `cn.hutool.core.io.IoUtil` | `FastByteArrayOutputStream read(InputStream in,boolean isClose)` | 从流中读取内容，读到输出流中，读取完毕后可选是否关闭流 |
| `cn.hutool.core.io.IoUtil` | `FileInputStream toStream(File file)` | 文件转为FileInputStream |
| `cn.hutool.core.io.IoUtil` | `InputStream toAvailableStream(InputStream in)` | 将指定InputStream 转换为InputStream#available()方法可用的流。 在Socket通信流中，服务端未返回数据情况下InputStream#available()方法始终为0 因此，在读取前需要调用InputStream#read()读取一个字节（未返回会阻塞），一旦读取到了，InputStream#available()方法就正常了。 需要注意的是，在网络流中，是按照块来传输的，所以 InputStream#available() 读取到的并非最终长度，而是此次块的长度。 此方法返回对象的规则为： FileInputStream 返回原对象，因为文件流的avail… |
| `cn.hutool.core.io.IoUtil` | `InputStream toMarkSupportStream(InputStream in)` | 将InputStream转换为支持mark标记的流 若原流支持mark标记，则返回原流，否则使用BufferedInputStream 包装之 |
| `cn.hutool.core.io.IoUtil` | `LineIter lineIter(InputStream in,Charset charset)` | 返回行遍历器 |
| `cn.hutool.core.io.IoUtil` | `LineIter lineIter(Reader reader)` | 返回行遍历器 |
| `cn.hutool.core.io.IoUtil` | `OutputStreamWriter getUtf8Writer(OutputStream out)` | 获得一个Writer，默认编码UTF-8 |
| `cn.hutool.core.io.IoUtil` | `OutputStreamWriter getWriter(OutputStream out,Charset charset)` | 获得一个Writer |
| `cn.hutool.core.io.IoUtil` | `OutputStreamWriter getWriter(OutputStream out,String charsetName)` | 获得一个Writer |
| `cn.hutool.core.io.IoUtil` | `PushbackInputStream toPushbackStream(InputStream in,int pushBackSize)` | 转换为PushbackInputStream 如果传入的输入流已经是PushbackInputStream，强转返回，否则新建一个 |
| `cn.hutool.core.io.IoUtil` | `PushbackReader getPushBackReader(Reader reader,int pushBackSize)` | 获得PushbackReader 如果是PushbackReader强转返回，否则新建 |
| `cn.hutool.core.io.IoUtil` | `String read(InputStream in,Charset charset)` | 从流中读取内容，读取完毕后关闭流 |
| `cn.hutool.core.io.IoUtil` | `String read(InputStream in,String charsetName)` | 从流中读取内容，读取完成后关闭流 |
| `cn.hutool.core.io.IoUtil` | `String read(Reader reader)` | 从Reader中读取String，读取完毕后关闭Reader |
| `cn.hutool.core.io.IoUtil` | `String read(Reader reader,boolean isClose)` | 从Reader中读取String |
| `cn.hutool.core.io.IoUtil` | `String readHex(InputStream in,int length,boolean toLowerCase)` | 读取16进制字符串 |
| `cn.hutool.core.io.IoUtil` | `String readHex64Lower(InputStream in)` | 从流中读取前64个byte并转换为16进制，字母部分使用小写 |
| `cn.hutool.core.io.IoUtil` | `String readHex64Upper(InputStream in)` | 从流中读取前64个byte并转换为16进制，字母部分使用大写 |
| `cn.hutool.core.io.IoUtil` | `String readHex8192Upper(InputStream in)` | 从流中读取前8192个byte并转换为16进制，字母部分使用大写 |
| `cn.hutool.core.io.IoUtil` | `String readUtf8(InputStream in)` | 从流中读取UTF8编码的内容 |
| `cn.hutool.core.io.IoUtil` | `String toStr(ByteArrayOutputStream out,Charset charset)` | ByteArrayOutputStream 转换为String |
| `cn.hutool.core.io.IoUtil` | `T readLines(InputStream in,Charset charset,T collection)` | 从流中读取内容 |
| `cn.hutool.core.io.IoUtil` | `T readLines(InputStream in,String charsetName,T collection)` | 从流中读取内容 |
| `cn.hutool.core.io.IoUtil` | `T readLines(Reader reader,T collection)` | 从Reader中读取内容 |
| `cn.hutool.core.io.IoUtil` | `T readObj(InputStream in)` | 从流中读取对象，即对象的反序列化 注意！！！ 此方法不会检查反序列化安全，可能存在反序列化漏洞风险！！！ |
| `cn.hutool.core.io.IoUtil` | `T readObj(InputStream in,Class<T> clazz)` | 从流中读取对象，即对象的反序列化，读取后不关闭流 注意！！！ 此方法不会检查反序列化安全，可能存在反序列化漏洞风险！！！ |
| `cn.hutool.core.io.IoUtil` | `T readObj(ValidateObjectInputStream in,Class<T> clazz)` | 从流中读取对象，即对象的反序列化，读取后不关闭流 此方法使用了ValidateObjectInputStream中的黑白名单方式过滤类，用于避免反序列化漏洞 通过构造ValidateObjectInputStream，调用ValidateObjectInputStream#accept(Class[]) 或者ValidateObjectInputStream#refuse(Class[])方法添加可以被序列化的类或者禁止序列化的类。 |
| `cn.hutool.core.io.IoUtil` | `T readUtf8Lines(InputStream in,T collection)` | 从流中读取内容，使用UTF-8编码 |
| `cn.hutool.core.io.IoUtil` | `boolean contentEquals(InputStream input1,InputStream input2)` | 对比两个流内容是否相同 内部会转换流为 BufferedInputStream |
| `cn.hutool.core.io.IoUtil` | `boolean contentEquals(Reader input1,Reader input2)` | 对比两个Reader的内容是否一致 内部会转换流为 BufferedInputStream |
| `cn.hutool.core.io.IoUtil` | `boolean contentEqualsIgnoreEOL(Reader input1,Reader input2)` | 对比两个流内容是否相同，忽略EOL字符 内部会转换流为 BufferedInputStream |
| `cn.hutool.core.io.IoUtil` | `byte[] readBytes(InputStream in)` | 从流中读取bytes，读取完毕后关闭流 |
| `cn.hutool.core.io.IoUtil` | `byte[] readBytes(InputStream in,boolean isClose)` | 从流中读取bytes |
| `cn.hutool.core.io.IoUtil` | `byte[] readBytes(InputStream in,int length)` | 读取指定长度的byte数组，不关闭流 |
| `cn.hutool.core.io.IoUtil` | `long checksumCRC32(InputStream in)` | 计算流CRC32校验码，计算后关闭流 |
| `cn.hutool.core.io.IoUtil` | `long checksumValue(InputStream in,Checksum checksum)` | 计算流的校验码，计算后关闭流 |
| `cn.hutool.core.io.IoUtil` | `long copy(FileInputStream in,FileOutputStream out)` | 拷贝文件流，使用NIO |
| `cn.hutool.core.io.IoUtil` | `long copy(InputStream in,OutputStream out)` | 拷贝流，使用默认Buffer大小，拷贝后不关闭流 |
| `cn.hutool.core.io.IoUtil` | `long copy(InputStream in,OutputStream out,int bufferSize)` | 拷贝流，拷贝后不关闭流 |
| `cn.hutool.core.io.IoUtil` | `long copy(InputStream in,OutputStream out,int bufferSize,StreamProgress streamProgress)` | 拷贝流，拷贝后不关闭流 |
| `cn.hutool.core.io.IoUtil` | `long copy(InputStream in,OutputStream out,int bufferSize,long count,StreamProgress streamProgress)` | 拷贝流，拷贝后不关闭流 |
| `cn.hutool.core.io.IoUtil` | `long copy(Reader reader,Writer writer)` | 将Reader中的内容复制到Writer中 使用默认缓存大小，拷贝后不关闭Reader |
| `cn.hutool.core.io.IoUtil` | `long copy(Reader reader,Writer writer,int bufferSize)` | 将Reader中的内容复制到Writer中，拷贝后不关闭Reader |
| `cn.hutool.core.io.IoUtil` | `long copy(Reader reader,Writer writer,int bufferSize,StreamProgress streamProgress)` | 将Reader中的内容复制到Writer中，拷贝后不关闭Reader |
| `cn.hutool.core.io.IoUtil` | `long copy(Reader reader,Writer writer,int bufferSize,long count,StreamProgress streamProgress)` | 将Reader中的内容复制到Writer中，拷贝后不关闭Reader |
| `cn.hutool.core.io.IoUtil` | `void close(Closeable closeable)` | 关闭 关闭失败不会抛出异常 |
| `cn.hutool.core.io.IoUtil` | `void closeIfPosible(Object obj)` | 尝试关闭指定对象 判断对象如果实现了AutoCloseable，则调用之 |
| `cn.hutool.core.io.IoUtil` | `void closeIfPossible(Object obj)` | 尝试关闭指定对象 判断对象如果实现了AutoCloseable，则调用之 |
| `cn.hutool.core.io.IoUtil` | `void flush(Flushable flushable)` | 从缓存中刷出数据 |
| `cn.hutool.core.io.IoUtil` | `void readLines(InputStream in,Charset charset,LineHandler lineHandler)` | 按行读取数据，针对每行的数据做处理 |
| `cn.hutool.core.io.IoUtil` | `void readLines(Reader reader,LineHandler lineHandler)` | 按行读取数据，针对每行的数据做处理 Reader自带编码定义，因此读取数据的编码跟随其编码。 此方法不会关闭流，除非抛出异常 |
| `cn.hutool.core.io.IoUtil` | `void readUtf8Lines(InputStream in,LineHandler lineHandler)` | 按行读取UTF-8编码数据，针对每行的数据做处理 |
| `cn.hutool.core.io.IoUtil` | `void write(OutputStream out,Charset charset,boolean isCloseOut,Object... contents)` | 将多部分内容写到流中，自动转换为字符串 |
| `cn.hutool.core.io.IoUtil` | `void write(OutputStream out,String charsetName,boolean isCloseOut,Object... contents)` | 将多部分内容写到流中，自动转换为字符串 |
| `cn.hutool.core.io.IoUtil` | `void write(OutputStream out,boolean isCloseOut,byte[] content)` | 将byte[]写到流中 |
| `cn.hutool.core.io.IoUtil` | `void writeObj(OutputStream out,boolean isCloseOut,Serializable obj)` | 将多部分内容写到流中 |
| `cn.hutool.core.io.IoUtil` | `void writeObjects(OutputStream out,boolean isCloseOut,Serializable... contents)` | 将多部分内容写到流中 |
| `cn.hutool.core.io.IoUtil` | `void writeUtf8(OutputStream out,boolean isCloseOut,Object... contents)` | 将多部分内容写到流中，自动转换为UTF-8字符串 |
| `cn.hutool.core.io.LimitedInputStream` | `int read()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.LimitedInputStream` | `int read(byte[] b,int off,int len)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.LimitedInputStream` | `long skip(long n)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.io.LineHandler` | `void handle(String line)` | 处理一行数据，可以编辑后存入指定地方 |
| `cn.hutool.core.io.ManifestUtil` | `Manifest getManifest(Class<?> cls)` | 根据 class 获取 所在 jar 包文件的 Manifest 此方法主要利用class定位jar包，如引入hutool-all，则传入hutool中任意一个类即可获取这个jar的Manifest信息 如果这个类不在jar包中，返回null |
| `cn.hutool.core.io.ManifestUtil` | `Manifest getManifest(File classpathItem)` | 获取 jar 包文件或项目目录下的 Manifest |
| `cn.hutool.core.io.ManifestUtil` | `Manifest getManifest(JarFile jarFile)` | 根据 JarURLConnection 获取 jar 包文件的 Manifest |
| `cn.hutool.core.io.ManifestUtil` | `Manifest getManifest(JarURLConnection connection)` | 根据 JarURLConnection 获取 jar 包文件的 Manifest |
| `cn.hutool.core.io.NioUtil` | `FastByteArrayOutputStream read(ReadableByteChannel channel)` | 从流中读取内容，读到输出流中 |
| `cn.hutool.core.io.NioUtil` | `String read(FileChannel fileChannel,Charset charset)` | 从FileChannel中读取内容 |
| `cn.hutool.core.io.NioUtil` | `String read(FileChannel fileChannel,String charsetName)` | 从FileChannel中读取内容，读取完毕后并不关闭Channel |
| `cn.hutool.core.io.NioUtil` | `String read(ReadableByteChannel channel,Charset charset)` | 从流中读取内容，读取完毕后并不关闭流 |
| `cn.hutool.core.io.NioUtil` | `String readUtf8(FileChannel fileChannel)` | 从FileChannel中读取UTF-8编码内容 |
| `cn.hutool.core.io.NioUtil` | `long copy(FileChannel inChannel,FileChannel outChannel)` | 拷贝文件Channel，使用NIO，拷贝后不会关闭channel |
| `cn.hutool.core.io.NioUtil` | `long copy(ReadableByteChannel in,WritableByteChannel out)` | 拷贝流，使用NIO，不会关闭channel |
| `cn.hutool.core.io.NioUtil` | `long copy(ReadableByteChannel in,WritableByteChannel out,int bufferSize)` | 拷贝流，使用NIO，不会关闭channel |
| `cn.hutool.core.io.NioUtil` | `long copy(ReadableByteChannel in,WritableByteChannel out,int bufferSize,StreamProgress streamProgress)` | 拷贝流，使用NIO，不会关闭channel |
| `cn.hutool.core.io.NioUtil` | `long copy(ReadableByteChannel in,WritableByteChannel out,int bufferSize,long count,StreamProgress streamProgress)` | 拷贝流，使用NIO，不会关闭channel |
| `cn.hutool.core.io.NioUtil` | `long copyByNIO(InputStream in,OutputStream out,int bufferSize,StreamProgress streamProgress)` | 拷贝流 thanks to: https://github.com/venusdrogon/feilong-io/blob/master/src/main/java/com/feilong/io/IOWriteUtil.java 本方法不会关闭流 |
| `cn.hutool.core.io.NioUtil` | `long copyByNIO(InputStream in,OutputStream out,int bufferSize,long count,StreamProgress streamProgress)` | 拷贝流 本方法不会关闭流 |
| `cn.hutool.core.io.NioUtil` | `void close(AutoCloseable closeable)` | 关闭 关闭失败不会抛出异常 |
| `cn.hutool.core.io.NullOutputStream` | `void write(byte[] b)` | 什么也不做，写出到 /dev/null . |
| `cn.hutool.core.io.NullOutputStream` | `void write(byte[] b,int off,int len)` | 什么也不做，写出到 /dev/null . |
| `cn.hutool.core.io.NullOutputStream` | `void write(int b)` | 什么也不做，写出到 /dev/null . |
| `cn.hutool.core.io.StreamProgress` | `void finish()` | 结束 |
| `cn.hutool.core.io.StreamProgress` | `void progress(long total,long progressSize)` | 进行中 |
| `cn.hutool.core.io.StreamProgress` | `void start()` | 开始 |
| `cn.hutool.core.io.ValidateObjectInputStream` | `void accept(Class<?>... acceptClasses)` | 接受反序列化的类，用于反序列化验证 |
| `cn.hutool.core.io.ValidateObjectInputStream` | `void refuse(Class<?>... refuseClasses)` | 禁止反序列化的类，用于反序列化验证 |
