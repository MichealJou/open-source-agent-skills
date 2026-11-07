# com.feilong.net.filetransfer

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.filetransfer.AbstractFileTransfer` | `Map<String, FileInfoEntity> getFileEntityMap(String remotePath,String... fileNames)` | 【原文待译】Gets the file entity map. |
| `com.feilong.net.filetransfer.AbstractFileTransfer` | `String getLogTraceContext()` | 获得 日志追踪上下文. |
| `com.feilong.net.filetransfer.AbstractFileTransfer` | `boolean delete(String... remoteAbsolutePaths)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.filetransfer.AbstractFileTransfer` | `boolean upload(String remoteDirectory,String... batchLocalFileFullPaths)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.filetransfer.AbstractFileTransfer` | `void download(String localAbsoluteDirectoryPath,String... remotePaths)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.net.filetransfer.AbstractFileTransfer` | `void setLogTraceContext(String logTraceContext)` | 设置 日志追踪上下文. |
| `com.feilong.net.filetransfer.AbstractFileTransferConfig` | `Integer getPort()` | 获得 端口号. |
| `com.feilong.net.filetransfer.AbstractFileTransferConfig` | `String getHostName()` | 获得 host name. |
| `com.feilong.net.filetransfer.AbstractFileTransferConfig` | `String getPassword()` | 获得 密码. |
| `com.feilong.net.filetransfer.AbstractFileTransferConfig` | `String getUserName()` | 获得 用户名. |
| `com.feilong.net.filetransfer.AbstractFileTransferConfig` | `void setHostName(String hostName)` | 设置 host name. |
| `com.feilong.net.filetransfer.AbstractFileTransferConfig` | `void setPassword(String password)` | 设置 密码. |
| `com.feilong.net.filetransfer.AbstractFileTransferConfig` | `void setPort(Integer port)` | 设置 端口号. |
| `com.feilong.net.filetransfer.AbstractFileTransferConfig` | `void setUserName(String userName)` | 设置 用户名. |
| `com.feilong.net.filetransfer.FileTransfer` | `Map<String, FileInfoEntity> getFileEntityMap(String remotePath,String... fileNames)` | 获得某特定文件夹下面指定文件名相关信息. 注意:该方法不支持级联, 只支持获取 remotePath 下面的一级目录或者文件 |
| `com.feilong.net.filetransfer.FileTransfer` | `boolean delete(String... remoteAbsolutePaths)` | 删除远程的一组文件 remoteAbsolutePaths . |
| `com.feilong.net.filetransfer.FileTransfer` | `boolean upload(String remoteDirectory,String... batchLocalFileFullPaths)` | 支持将多个不定路径文件 batchLocalFileFullPaths 上传到远程文件夹 remoteDirectory . |
| `com.feilong.net.filetransfer.FileTransfer` | `void download(String localAbsoluteDirectoryPath,String... remotePaths)` | 打开一次链接,将一批远程文件/文件夹 ( remotePaths )循环下载到本地目录 localAbsoluteDirectoryPath . |
