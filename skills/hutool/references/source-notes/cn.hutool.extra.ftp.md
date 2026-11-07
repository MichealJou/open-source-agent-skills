# cn.hutool.extra.ftp

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.ftp.AbstractFtp` | `AbstractFtp reconnectIfTimeout()` | 如果连接超时的话，重新进行连接 |
| `cn.hutool.extra.ftp.AbstractFtp` | `List<String> ls(String path)` | 遍历某个目录下所有文件和目录，不会递归遍历 |
| `cn.hutool.extra.ftp.AbstractFtp` | `String pwd()` | 远程当前目录（工作目录） |
| `cn.hutool.extra.ftp.AbstractFtp` | `boolean cd(String directory)` | 打开指定目录，具体逻辑取决于实现，例如在FTP中，进入失败返回false， SFTP中则抛出异常 |
| `cn.hutool.extra.ftp.AbstractFtp` | `boolean delDir(String dirPath)` | 删除文件夹及其文件夹下的所有文件 |
| `cn.hutool.extra.ftp.AbstractFtp` | `boolean delFile(String path)` | 删除指定目录下的指定文件 |
| `cn.hutool.extra.ftp.AbstractFtp` | `boolean exist(String path)` | 文件或目录是否存在 |
| `cn.hutool.extra.ftp.AbstractFtp` | `boolean isDir(String dir)` | 判断给定路径是否为目录 |
| `cn.hutool.extra.ftp.AbstractFtp` | `boolean mkdir(String dir)` | 在当前远程目录（工作目录）下创建新的目录 |
| `cn.hutool.extra.ftp.AbstractFtp` | `boolean toParent()` | 打开上级目录 |
| `cn.hutool.extra.ftp.AbstractFtp` | `boolean upload(String destPath,File file)` | 将本地文件上传到目标服务器，目标文件名为destPath，若destPath为目录，则目标文件名将与file文件名相同。 覆盖模式 |
| `cn.hutool.extra.ftp.AbstractFtp` | `void download(String path,File outFile)` | 下载文件 |
| `cn.hutool.extra.ftp.AbstractFtp` | `void download(String path,File outFile,String tempFileSuffix)` | 下载文件-避免未完成的文件 来自：https://gitee.com/chinabugotech/hutool/pulls/407 此方法原理是先在目标文件同级目录下创建临时文件，下载之，等下载完毕后重命名，避免因下载错误导致的文件不完整。 |
| `cn.hutool.extra.ftp.AbstractFtp` | `void mkDirs(String dir)` | 创建指定文件夹及其父目录，从根目录开始创建，创建完成后回到默认的工作目录 |
| `cn.hutool.extra.ftp.AbstractFtp` | `void recursiveDownloadFolder(String sourcePath,File destDir)` | 递归下载FTP服务器上文件到本地(文件目录和服务器同步), 服务器上有新文件会覆盖本地文件 |
| `cn.hutool.extra.ftp.AbstractFtp` | `void rename(String from,String to)` | 重命名文件/目录 |
| `cn.hutool.extra.ftp.Ftp` | `FTPClient getClient()` | 获取FTPClient客户端对象 |
| `cn.hutool.extra.ftp.Ftp` | `FTPFile[] lsFiles(String path)` | 遍历某个目录下所有文件和目录，不会递归遍历 |
| `cn.hutool.extra.ftp.Ftp` | `Ftp init()` | 初始化连接 |
| `cn.hutool.extra.ftp.Ftp` | `Ftp init(FtpConfig config,FtpMode mode)` | 初始化连接 |
| `cn.hutool.extra.ftp.Ftp` | `Ftp init(String host,int port,String user,String password)` | 初始化连接 |
| `cn.hutool.extra.ftp.Ftp` | `Ftp init(String host,int port,String user,String password,FtpMode mode)` | 初始化连接 |
| `cn.hutool.extra.ftp.Ftp` | `Ftp reconnectIfTimeout()` | 如果连接超时的话，重新进行连接 经测试，当连接超时时，client.isConnected()仍然返回ture，无法判断是否连接超时 因此，通过发送pwd命令的方式，检查连接是否超时 |
| `cn.hutool.extra.ftp.Ftp` | `Ftp setBackToPwd(boolean backToPwd)` | 设置执行完操作是否返回当前目录 |
| `cn.hutool.extra.ftp.Ftp` | `Ftp setMode(FtpMode mode)` | 设置FTP连接模式，可选主动和被动模式 |
| `cn.hutool.extra.ftp.Ftp` | `List<FTPFile> lsFiles(String path,Filter<FTPFile> filter)` | 遍历某个目录下所有文件和目录，不会递归遍历 此方法自动过滤"."和".."两种目录 |
| `cn.hutool.extra.ftp.Ftp` | `List<String> ls(String path)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.Ftp` | `String pwd()` | 远程当前目录 |
| `cn.hutool.extra.ftp.Ftp` | `boolean cd(String directory)` | 改变目录 |
| `cn.hutool.extra.ftp.Ftp` | `boolean delDir(String dirPath)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.Ftp` | `boolean delFile(String path)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.Ftp` | `boolean existFile(String path)` | 判断ftp服务器目录内是否还有子元素（目录或文件） |
| `cn.hutool.extra.ftp.Ftp` | `boolean isBackToPwd()` | 是否执行完操作返回当前目录 |
| `cn.hutool.extra.ftp.Ftp` | `boolean mkdir(String dir)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.Ftp` | `boolean upload(String destPath,File file)` | 上传文件到指定目录，可选： |
| `cn.hutool.extra.ftp.Ftp` | `boolean upload(String destPath,String fileName,File file)` | 上传文件到指定目录，可选： |
| `cn.hutool.extra.ftp.Ftp` | `boolean upload(String destPath,String fileName,InputStream fileStream)` | 上传文件到指定目录，可选： |
| `cn.hutool.extra.ftp.Ftp` | `int stat(String path)` | 获取服务端目录状态。 |
| `cn.hutool.extra.ftp.Ftp` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.Ftp` | `void download(String path,File outFile)` | 下载文件 |
| `cn.hutool.extra.ftp.Ftp` | `void download(String path,String fileName,File outFile)` | 下载文件 |
| `cn.hutool.extra.ftp.Ftp` | `void download(String path,String fileName,OutputStream out)` | 下载文件到输出流 |
| `cn.hutool.extra.ftp.Ftp` | `void download(String path,String fileName,OutputStream out,Charset fileNameCharset)` | 下载文件到输出流 |
| `cn.hutool.extra.ftp.Ftp` | `void recursiveDownloadFolder(String sourcePath,File destDir)` | 递归下载FTP服务器上文件到本地(文件目录和服务器同步) |
| `cn.hutool.extra.ftp.Ftp` | `void rename(String from,String to)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.Ftp` | `void uploadFileOrDirectory(final String remotePath,final File uploadFile)` | 递归上传文件（支持目录） 上传时，如果uploadFile为目录，只复制目录下所有目录和文件到目标路径下，并不会复制目录本身 上传时，自动创建父级目录 |
| `cn.hutool.extra.ftp.FtpConfig` | `Charset getCharset()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `FtpConfig create()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `FtpConfig setCharset(Charset charset)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `FtpConfig setConnectionTimeout(long connectionTimeout)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `FtpConfig setHost(String host)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `FtpConfig setPassword(String password)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `FtpConfig setPort(int port)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `FtpConfig setServerLanguageCode(String serverLanguageCode)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `FtpConfig setSoTimeout(long soTimeout)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `FtpConfig setSystemKey(String systemKey)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `FtpConfig setUser(String user)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `String getHost()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `String getPassword()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `String getServerLanguageCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `String getSystemKey()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `String getUser()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `int getPort()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `long getConnectionTimeout()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.FtpConfig` | `long getSoTimeout()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `FtpServerFactory getServerFactory()` | 获取 FtpServerFactory，用于设置FTP服务器相关信息 |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `ListenerFactory getListenerFactory()` | 获取ListenerFactory，用于设置端口、用户、SSL等信息 |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `SimpleFtpServer addAnonymous(String homePath)` | 添加匿名用户 |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `SimpleFtpServer addFtplet(String name,Ftplet ftplet)` | 增加FTP动作行为监听处理器，通过实现Ftplet，可以对用户的行为监听并执行相应动作 |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `SimpleFtpServer addUser(User user)` | 增加FTP用户 |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `SimpleFtpServer create()` | 创建FTP服务器，调用SimpleFtpServer#start()启动即可 |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `SimpleFtpServer delUser(String userName)` | 删除用户 |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `SimpleFtpServer setConnectionConfig(ConnectionConfig connectionConfig)` | 设置连接相关配置，使用ConnectionConfigFactory创建ConnectionConfig对象 |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `SimpleFtpServer setPort(int port)` | 自定义默认端口，如果不设置，使用默认端口：21 |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `SimpleFtpServer setSsl(File keystoreFile,String password)` | 使用SSL安全连接 |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `SimpleFtpServer setSsl(SslConfiguration ssl)` | 使用SSL安全连接，可以使用SslConfigurationFactory创建SslConfiguration |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `SimpleFtpServer setUserManager(UserManager userManager)` | 自定义用户管理器，一般用于使用配置文件配置用户信息 |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `SimpleFtpServer setUsersConfig(File propertiesFile)` | 自定义用户信息配置文件，此方法会重置用户管理器 |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `UserManager getUserManager()` | 获取用户管理器，用于新增、查找和删除用户信息 |
| `cn.hutool.extra.ftp.SimpleFtpServer` | `void start()` | 启动FTP服务，阻塞当前线程 |
