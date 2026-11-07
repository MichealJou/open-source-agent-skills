# cn.hutool.extra.ssh

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.ssh.ChannelType` | `String getValue()` | 获取值 |
| `cn.hutool.extra.ssh.Connector` | `String getGroup()` | 获得用户组名 |
| `cn.hutool.extra.ssh.Connector` | `String getHost()` | 获得主机名 |
| `cn.hutool.extra.ssh.Connector` | `String getPassword()` | 获得密码 |
| `cn.hutool.extra.ssh.Connector` | `String getUser()` | 获得用户名 |
| `cn.hutool.extra.ssh.Connector` | `String toString()` | toString方法仅用于测试显示 |
| `cn.hutool.extra.ssh.Connector` | `int getPort()` | 获得端口号 |
| `cn.hutool.extra.ssh.Connector` | `void setGroup(String group)` | 设定用户组名 |
| `cn.hutool.extra.ssh.Connector` | `void setHost(String host)` | 设定主机名 |
| `cn.hutool.extra.ssh.Connector` | `void setPassword(String password)` | 设定密码 |
| `cn.hutool.extra.ssh.Connector` | `void setPort(int port)` | 设定端口号 |
| `cn.hutool.extra.ssh.Connector` | `void setUser(String name)` | 设定用户名 |
| `cn.hutool.extra.ssh.GanymedUtil` | `Connection connect(String sshHost,int sshPort)` | 连接到服务器 |
| `cn.hutool.extra.ssh.GanymedUtil` | `Session openSession(String sshHost,int sshPort,String sshUser,String sshPass)` | 打开远程会话 |
| `cn.hutool.extra.ssh.GanymedUtil` | `String exec(Session session,String cmd,Charset charset,OutputStream errStream)` | 执行Shell命令（使用EXEC方式） 此方法单次发送一个命令到服务端，不读取环境变量，执行结束后自动关闭Session，不会产生阻塞。 |
| `cn.hutool.extra.ssh.GanymedUtil` | `String execByShell(Session session,String cmd,Charset charset,OutputStream errStream)` | 执行Shell命令 此方法单次发送一个命令到服务端，自动读取环境变量，执行结束后自动关闭Session，可能产生阻塞。 |
| `cn.hutool.extra.ssh.GanymedUtil` | `void close(Session session)` | 关闭会话 |
| `cn.hutool.extra.ssh.JschSessionPool` | `Session get(String key)` | 获取Session，不存在返回null |
| `cn.hutool.extra.ssh.JschSessionPool` | `Session getSession(String sshHost,int sshPort,String sshUser,String prvkey,byte[] passphrase)` | 获得一个SSH跳板机会话，重用已经使用的会话 |
| `cn.hutool.extra.ssh.JschSessionPool` | `Session getSession(String sshHost,int sshPort,String sshUser,String sshPass)` | 获得一个SSH跳板机会话，重用已经使用的会话 |
| `cn.hutool.extra.ssh.JschSessionPool` | `Session getSession(String sshHost,int sshPort,String sshUser,byte[] prvkey,byte[] passphrase)` | 获得一个SSH跳板机会话，重用已经使用的会话 |
| `cn.hutool.extra.ssh.JschSessionPool` | `void close(String key)` | 关闭SSH连接会话 |
| `cn.hutool.extra.ssh.JschSessionPool` | `void closeAll()` | 关闭所有SSH连接会话 |
| `cn.hutool.extra.ssh.JschSessionPool` | `void put(String key,Session session)` | 加入Session |
| `cn.hutool.extra.ssh.JschSessionPool` | `void remove(Session session)` | 移除指定Session |
| `cn.hutool.extra.ssh.JschUtil` | `Channel createChannel(Session session,ChannelType channelType)` | 创建Channel连接 |
| `cn.hutool.extra.ssh.JschUtil` | `Channel openChannel(Session session,ChannelType channelType)` | 打开Channel连接 |
| `cn.hutool.extra.ssh.JschUtil` | `Channel openChannel(Session session,ChannelType channelType,int timeout)` | 打开Channel连接 |
| `cn.hutool.extra.ssh.JschUtil` | `ChannelSftp openSftp(Session session)` | 打开SFTP连接 |
| `cn.hutool.extra.ssh.JschUtil` | `ChannelSftp openSftp(Session session,int timeout)` | 打开SFTP连接 |
| `cn.hutool.extra.ssh.JschUtil` | `ChannelShell openShell(Session session)` | 打开Shell连接 |
| `cn.hutool.extra.ssh.JschUtil` | `Session createSession(JSch jsch,String sshHost,int sshPort,String sshUser)` | 创建一个SSH会话，重用已经使用的会话 |
| `cn.hutool.extra.ssh.JschUtil` | `Session createSession(String sshHost,int sshPort,String sshUser,String privateKeyPath,byte[] passphrase)` | 新建一个新的SSH会话，此方法并不打开会话（既不调用connect方法） |
| `cn.hutool.extra.ssh.JschUtil` | `Session createSession(String sshHost,int sshPort,String sshUser,String sshPass)` | 新建一个新的SSH会话，此方法并不打开会话（既不调用connect方法） |
| `cn.hutool.extra.ssh.JschUtil` | `Session createSession(String sshHost,int sshPort,String sshUser,byte[] privateKey,byte[] passphrase)` | 新建一个新的SSH会话，此方法并不打开会话（既不调用connect方法） |
| `cn.hutool.extra.ssh.JschUtil` | `Session getSession(String sshHost,int sshPort,String sshUser,String privateKeyPath,byte[] passphrase)` | 获得一个SSH会话，重用已经使用的会话 |
| `cn.hutool.extra.ssh.JschUtil` | `Session getSession(String sshHost,int sshPort,String sshUser,String sshPass)` | 获得一个SSH会话，重用已经使用的会话 |
| `cn.hutool.extra.ssh.JschUtil` | `Session getSession(String sshHost,int sshPort,String sshUser,byte[] privateKey,byte[] passphrase)` | 获得一个SSH会话，重用已经使用的会话 |
| `cn.hutool.extra.ssh.JschUtil` | `Session openSession(String sshHost,int sshPort,String sshUser,String privateKeyPath,byte[] passphrase)` | 打开一个新的SSH会话 |
| `cn.hutool.extra.ssh.JschUtil` | `Session openSession(String sshHost,int sshPort,String sshUser,String privateKeyPath,byte[] passphrase,int timeOut)` | 打开一个新的SSH会话 |
| `cn.hutool.extra.ssh.JschUtil` | `Session openSession(String sshHost,int sshPort,String sshUser,String sshPass)` | 打开一个新的SSH会话 |
| `cn.hutool.extra.ssh.JschUtil` | `Session openSession(String sshHost,int sshPort,String sshUser,String sshPass,int timeout)` | 打开一个新的SSH会话 |
| `cn.hutool.extra.ssh.JschUtil` | `Session openSession(String sshHost,int sshPort,String sshUser,byte[] privateKey,byte[] passphrase)` | 打开一个新的SSH会话 |
| `cn.hutool.extra.ssh.JschUtil` | `Session openSession(String sshHost,int sshPort,String sshUser,byte[] privateKey,byte[] passphrase,int timeOut)` | 打开一个新的SSH会话 |
| `cn.hutool.extra.ssh.JschUtil` | `Sftp createSftp(Session session)` | 创建Sftp |
| `cn.hutool.extra.ssh.JschUtil` | `Sftp createSftp(String sshHost,int sshPort,String sshUser,String sshPass)` | 创建Sftp |
| `cn.hutool.extra.ssh.JschUtil` | `String exec(Session session,String cmd,Charset charset)` | 执行Shell命令 |
| `cn.hutool.extra.ssh.JschUtil` | `String exec(Session session,String cmd,Charset charset,OutputStream errStream)` | 执行Shell命令（使用EXEC方式） 此方法单次发送一个命令到服务端，不读取环境变量，执行结束后自动关闭channel，不会产生阻塞。 |
| `cn.hutool.extra.ssh.JschUtil` | `String execByShell(Session session,String cmd,Charset charset)` | 执行Shell命令 此方法单次发送一个命令到服务端，自动读取环境变量，执行结束后自动关闭channel，不会产生阻塞。 |
| `cn.hutool.extra.ssh.JschUtil` | `boolean bindPort(Session session,String remoteHost,int remotePort,String localHost,int localPort)` | 绑定端口到本地。 一个会话可绑定多个端口 |
| `cn.hutool.extra.ssh.JschUtil` | `boolean bindPort(Session session,String remoteHost,int remotePort,int localPort)` | 绑定端口到本地。 一个会话可绑定多个端口 |
| `cn.hutool.extra.ssh.JschUtil` | `boolean bindRemotePort(Session session,int bindPort,String host,int port)` | 绑定ssh服务端的serverPort端口, 到host主机的port端口上. 即数据从ssh服务端的serverPort端口, 流经ssh客户端, 达到host:port上. |
| `cn.hutool.extra.ssh.JschUtil` | `boolean unBindPort(Session session,int localPort)` | 解除端口映射 |
| `cn.hutool.extra.ssh.JschUtil` | `int generateLocalPort()` | 生成一个本地端口，用于远程端口映射 |
| `cn.hutool.extra.ssh.JschUtil` | `int openAndBindPortToLocal(Connector sshConn,String remoteHost,int remotePort)` | 打开SSH会话，并绑定远程端口到本地的一个随机端口 |
| `cn.hutool.extra.ssh.JschUtil` | `void close(Channel channel)` | 关闭会话通道 |
| `cn.hutool.extra.ssh.JschUtil` | `void close(Session session)` | 关闭SSH连接会话 |
| `cn.hutool.extra.ssh.JschUtil` | `void close(String key)` | 关闭SSH连接会话 |
| `cn.hutool.extra.ssh.JschUtil` | `void closeAll()` | 关闭所有SSH连接会话 |
| `cn.hutool.extra.ssh.Sftp` | `ChannelSftp getClient()` | 获取SFTP通道客户端 |
| `cn.hutool.extra.ssh.Sftp` | `List<LsEntry> lsEntries(String path)` | 遍历某个目录下所有文件或目录，生成LsEntry列表，不会递归遍历 此方法自动过滤"."和".."两种目录 |
| `cn.hutool.extra.ssh.Sftp` | `List<LsEntry> lsEntries(String path,Filter<LsEntry> filter)` | 遍历某个目录下所有文件或目录，生成LsEntry列表，不会递归遍历 此方法自动过滤"."和".."两种目录 |
| `cn.hutool.extra.ssh.Sftp` | `List<String> ls(String path)` | 遍历某个目录下所有文件或目录，不会递归遍历 |
| `cn.hutool.extra.ssh.Sftp` | `List<String> ls(String path,final Filter<LsEntry> filter)` | 遍历某个目录下所有文件或目录，不会递归遍历 此方法自动过滤"."和".."两种目录 |
| `cn.hutool.extra.ssh.Sftp` | `List<String> lsDirs(String path)` | 遍历某个目录下所有目录，不会递归遍历 |
| `cn.hutool.extra.ssh.Sftp` | `List<String> lsFiles(String path)` | 遍历某个目录下所有文件，不会递归遍历 |
| `cn.hutool.extra.ssh.Sftp` | `Sftp get(String src,OutputStream out)` | 获取远程文件 |
| `cn.hutool.extra.ssh.Sftp` | `Sftp get(String src,String dest)` | 获取远程文件 |
| `cn.hutool.extra.ssh.Sftp` | `Sftp put(InputStream srcStream,String destPath,SftpProgressMonitor monitor,Mode mode)` | 将本地数据流上传到目标服务器，目标文件名为destPath，目标必须为文件 |
| `cn.hutool.extra.ssh.Sftp` | `Sftp put(String srcFilePath,String destPath)` | 将本地文件上传到目标服务器，目标文件名为destPath，若destPath为目录，则目标文件名将与srcFilePath文件名相同。覆盖模式 |
| `cn.hutool.extra.ssh.Sftp` | `Sftp put(String srcFilePath,String destPath,Mode mode)` | 将本地文件上传到目标服务器，目标文件名为destPath，若destPath为目录，则目标文件名将与srcFilePath文件名相同。 |
| `cn.hutool.extra.ssh.Sftp` | `Sftp put(String srcFilePath,String destPath,SftpProgressMonitor monitor,Mode mode)` | 将本地文件上传到目标服务器，目标文件名为destPath，若destPath为目录，则目标文件名将与srcFilePath文件名相同。 |
| `cn.hutool.extra.ssh.Sftp` | `Sftp reconnectIfTimeout()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.Sftp` | `String home()` | 获取HOME路径 |
| `cn.hutool.extra.ssh.Sftp` | `String pwd()` | 远程当前目录 |
| `cn.hutool.extra.ssh.Sftp` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.Sftp` | `boolean cd(String directory)` | 打开指定目录，如果指定路径非目录或不存在抛出异常 |
| `cn.hutool.extra.ssh.Sftp` | `boolean delDir(String dirPath)` | 删除文件夹及其文件夹下的所有文件 |
| `cn.hutool.extra.ssh.Sftp` | `boolean delFile(String filePath)` | 删除文件 |
| `cn.hutool.extra.ssh.Sftp` | `boolean isDir(String dir)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.Sftp` | `boolean mkdir(String dir)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.Sftp` | `boolean upload(String destPath,File file)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.Sftp` | `boolean upload(String destPath,String fileName,InputStream fileStream)` | 上传文件到指定目录，可选： |
| `cn.hutool.extra.ssh.Sftp` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.Sftp` | `void download(String src,File destFile)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.Sftp` | `void download(String src,OutputStream out)` | 下载文件到OutputStream中 |
| `cn.hutool.extra.ssh.Sftp` | `void init()` | 初始化 |
| `cn.hutool.extra.ssh.Sftp` | `void init(ChannelSftp channel,Charset charset)` | 初始化 |
| `cn.hutool.extra.ssh.Sftp` | `void init(FtpConfig config)` | 初始化 |
| `cn.hutool.extra.ssh.Sftp` | `void init(Session session,Charset charset)` | 初始化 |
| `cn.hutool.extra.ssh.Sftp` | `void init(String sshHost,int sshPort,String sshUser,String sshPass,Charset charset)` | 构造 |
| `cn.hutool.extra.ssh.Sftp` | `void recursiveDownloadFolder(String sourcePath,File destDir)` | 递归下载FTP服务器上文件到本地(文件目录和服务器同步) |
| `cn.hutool.extra.ssh.Sftp` | `void rename(String from,String to)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.Sftp` | `void syncUpload(File file,String remotePath)` | 将本地文件或者文件夹同步（覆盖）上传到远程路径 |
| `cn.hutool.extra.ssh.SshjSftp` | `AbstractFtp reconnectIfTimeout()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.SshjSftp` | `List<String> ls(String path)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.SshjSftp` | `String command(String exec)` | 执行Linux 命令 |
| `cn.hutool.extra.ssh.SshjSftp` | `String pwd()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.SshjSftp` | `boolean cd(String directory)` | 改变目录，注意目前不支持.. |
| `cn.hutool.extra.ssh.SshjSftp` | `boolean containsFile(String fileDir)` | 是否包含该文件 |
| `cn.hutool.extra.ssh.SshjSftp` | `boolean delDir(String dirPath)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.SshjSftp` | `boolean delFile(String path)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.SshjSftp` | `boolean mkdir(String dir)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.SshjSftp` | `boolean upload(String destPath,File file)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.SshjSftp` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.SshjSftp` | `void download(String path,File outFile)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.SshjSftp` | `void init()` | SSH 初始化并创建一个sftp客户端. |
| `cn.hutool.extra.ssh.SshjSftp` | `void recursiveDownloadFolder(String sourcePath,File destDir)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.ssh.SshjSftp` | `void rename(String from,String to)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
