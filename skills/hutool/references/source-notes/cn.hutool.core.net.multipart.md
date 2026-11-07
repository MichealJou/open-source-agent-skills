# cn.hutool.core.net.multipart

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.net.multipart.MultipartFormData` | `List<String> getListParam(String paramName)` | 获得集合表单值 |
| `cn.hutool.core.net.multipart.MultipartFormData` | `List<UploadFile> getFileList(String paramName)` | 获得某个属性名的所有文件 当表单中两个文件使用同一个name的时候 |
| `cn.hutool.core.net.multipart.MultipartFormData` | `ListValueMap<String, String> getParamListMap()` | 获取所有属性的集合 |
| `cn.hutool.core.net.multipart.MultipartFormData` | `ListValueMap<String, UploadFile> getFileListValueMap()` | 获取文件映射 |
| `cn.hutool.core.net.multipart.MultipartFormData` | `Map<String, String[]> getParamMap()` | 获取所有属性的集合 |
| `cn.hutool.core.net.multipart.MultipartFormData` | `Map<String, UploadFile[]> getFileMap()` | 获取文件映射 |
| `cn.hutool.core.net.multipart.MultipartFormData` | `Set<String> getFileParamNames()` | 获取上传的文件属性名集合 |
| `cn.hutool.core.net.multipart.MultipartFormData` | `Set<String> getParamNames()` | @return 获得参数名集合 |
| `cn.hutool.core.net.multipart.MultipartFormData` | `String getParam(String paramName)` | 返回单一参数值，如果有多个只返回第一个 |
| `cn.hutool.core.net.multipart.MultipartFormData` | `String[] getArrayParam(String paramName)` | 获得数组表单值 |
| `cn.hutool.core.net.multipart.MultipartFormData` | `UploadFile getFile(String paramName)` | 获取上传的文件 |
| `cn.hutool.core.net.multipart.MultipartFormData` | `UploadFile[] getFiles(String paramName)` | 获得某个属性名的所有文件 当表单中两个文件使用同一个name的时候 |
| `cn.hutool.core.net.multipart.MultipartFormData` | `boolean isLoaded()` | 是否已被解析 |
| `cn.hutool.core.net.multipart.MultipartFormData` | `void parseRequestStream(InputStream inputStream,Charset charset)` | 提取上传的文件和表单数据 |
| `cn.hutool.core.net.multipart.MultipartRequestInputStream` | `String readString(Charset charset)` | 读取字节流，直到下一个boundary |
| `cn.hutool.core.net.multipart.MultipartRequestInputStream` | `UploadFileHeader getLastHeader()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.multipart.MultipartRequestInputStream` | `UploadFileHeader readDataHeader(Charset encoding)` | 从流中读取文件头部信息， 如果达到末尾则返回null |
| `cn.hutool.core.net.multipart.MultipartRequestInputStream` | `boolean isBoundary(byte b)` | 【原文待译】@param b byte |
| `cn.hutool.core.net.multipart.MultipartRequestInputStream` | `byte readByte()` | 读取byte字节流，在末尾抛出异常 |
| `cn.hutool.core.net.multipart.MultipartRequestInputStream` | `byte[] readBoundary()` | 输入流中读取边界 |
| `cn.hutool.core.net.multipart.MultipartRequestInputStream` | `long copy(OutputStream out)` | 字节流复制到out，直到下一个boundary |
| `cn.hutool.core.net.multipart.MultipartRequestInputStream` | `long copy(OutputStream out,long limit)` | 复制字节流到out， 大于maxBytes或者文件末尾停止 |
| `cn.hutool.core.net.multipart.MultipartRequestInputStream` | `long skipToBoundary()` | 跳过边界表示 |
| `cn.hutool.core.net.multipart.MultipartRequestInputStream` | `void skipBytes(long i)` | 跳过指定位数的 bytes. |
| `cn.hutool.core.net.multipart.UploadFile` | `File write(File destination)` | 将上传的文件写入目标文件 写入后原临时文件会被删除 |
| `cn.hutool.core.net.multipart.UploadFile` | `File write(String destPath)` | 将上传的文件写入指定的目标文件路径，自动创建文件 写入后原临时文件会被删除 |
| `cn.hutool.core.net.multipart.UploadFile` | `InputStream getFileInputStream()` | @return 获得文件流 |
| `cn.hutool.core.net.multipart.UploadFile` | `String getFileName()` | @return 文件名 |
| `cn.hutool.core.net.multipart.UploadFile` | `UploadFileHeader getHeader()` | @return 上传文件头部信息 |
| `cn.hutool.core.net.multipart.UploadFile` | `boolean isInMemory()` | @return 文件是否在内存中 |
| `cn.hutool.core.net.multipart.UploadFile` | `boolean isUploaded()` | @return 是否上传成功 |
| `cn.hutool.core.net.multipart.UploadFile` | `byte[] getFileContent()` | @return 获得文件字节流 |
| `cn.hutool.core.net.multipart.UploadFile` | `long size()` | @return 上传文件的大小，> 0 表示未上传 |
| `cn.hutool.core.net.multipart.UploadFile` | `void delete()` | 从磁盘或者内存中删除这个文件 |
| `cn.hutool.core.net.multipart.UploadFileHeader` | `String getContentDisposition()` | 【原文待译】Returns content disposition. Usually it is 'form-data'. |
| `cn.hutool.core.net.multipart.UploadFileHeader` | `String getContentType()` | 【原文待译】Returns uploaded content type. It is usually in the following form: mime_type/mime_subtype. |
| `cn.hutool.core.net.multipart.UploadFileHeader` | `String getFileName()` | 获取文件名，不包括路径 |
| `cn.hutool.core.net.multipart.UploadFileHeader` | `String getFormFieldName()` | 返回表单字段名 |
| `cn.hutool.core.net.multipart.UploadFileHeader` | `String getFormFileName()` | 返回表单中的文件名，来自客户端传入 |
| `cn.hutool.core.net.multipart.UploadFileHeader` | `String getMimeSubtype()` | 【原文待译】Returns file sub type MIME. |
| `cn.hutool.core.net.multipart.UploadFileHeader` | `String getMimeType()` | 【原文待译】Returns file types MIME. |
| `cn.hutool.core.net.multipart.UploadFileHeader` | `boolean isFile()` | 【原文待译】Returns true if uploaded data are correctly marked as a file. This is true if header contains string 'filename'. |
| `cn.hutool.core.net.multipart.UploadSetting` | `String getTmpUploadPath()` | @return 上传文件的临时目录，若为空，使用系统目录 |
| `cn.hutool.core.net.multipart.UploadSetting` | `String[] getFileExts()` | @return 文件扩展名限定列表 |
| `cn.hutool.core.net.multipart.UploadSetting` | `boolean isAllowFileExts()` | 是否允许文件扩展名 |
| `cn.hutool.core.net.multipart.UploadSetting` | `int getMemoryThreshold()` | @return 文件保存到内存的边界 |
| `cn.hutool.core.net.multipart.UploadSetting` | `long getMaxFileSize()` | @return 获得最大文件大小，-1表示无限制 |
| `cn.hutool.core.net.multipart.UploadSetting` | `void setAllowFileExts(boolean isAllowFileExts)` | 设定是否允许扩展名 |
| `cn.hutool.core.net.multipart.UploadSetting` | `void setFileExts(String[] fileExts)` | 设定文件扩展名限定里列表 禁止列表还是允许列表取决于isAllowFileExts |
| `cn.hutool.core.net.multipart.UploadSetting` | `void setMaxFileSize(long maxFileSize)` | 设定最大文件大小，-1表示无限制 |
| `cn.hutool.core.net.multipart.UploadSetting` | `void setMemoryThreshold(int memoryThreshold)` | 设定文件保存到内存的边界 如果文件大小小于这个边界，将保存于内存中，否则保存至临时目录中 |
| `cn.hutool.core.net.multipart.UploadSetting` | `void setTmpUploadPath(String tmpUploadPath)` | 设定上传文件的临时目录，null表示使用系统临时目录 |
