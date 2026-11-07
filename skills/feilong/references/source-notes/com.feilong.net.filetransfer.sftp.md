# com.feilong.net.filetransfer.sftp

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.net.filetransfer.sftp.SFTPFileTransfer` | `void setSftpFileTransferConfig(SFTPFileTransferConfig sftpFileTransferConfig)` | 设置 sftp file transfer config. |
| `com.feilong.net.filetransfer.sftp.SFTPFileTransferConfig` | `Properties getSshConfig()` | 获得 the ssh config. |
| `com.feilong.net.filetransfer.sftp.SFTPFileTransferConfig` | `int getSessionTimeout()` | 超时时间,用于设置 Socket setSoTimeout ,单位 毫秒, 可以使用 TimeInterval常量. Enable/disable SocketOptions#SO_TIMEOUT SO_TIMEOUT With this option set to a non-zero timeout, a read() call on the InputStream associated with this Socket will block for only this amount of time. If the timeout expires, a java.net.SocketTim… |
| `com.feilong.net.filetransfer.sftp.SFTPFileTransferConfig` | `void setSessionTimeout(int sessionTimeout)` | 超时时间,用于设置 Socket setSoTimeout ,单位 毫秒, 可以使用 TimeInterval常量. Enable/disable SocketOptions#SO_TIMEOUT SO_TIMEOUT With this option set to a non-zero timeout, a read() call on the InputStream associated with this Socket will block for only this amount of time. If the timeout expires, a java.net.SocketTim… |
| `com.feilong.net.filetransfer.sftp.SFTPFileTransferConfig` | `void setSshConfig(Properties sshConfig)` | 设置 the ssh config. |
