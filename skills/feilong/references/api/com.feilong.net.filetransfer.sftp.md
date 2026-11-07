# com.feilong.net.filetransfer.sftp

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.net.filetransfer.sftp.SFTPFileTransfer`

```java
public class com.feilong.net.filetransfer.sftp.SFTPFileTransfer extends com.feilong.net.filetransfer.AbstractFileTransfer {
  public com.feilong.net.filetransfer.sftp.SFTPFileTransfer();
  public void setSftpFileTransferConfig(com.feilong.net.filetransfer.sftp.SFTPFileTransferConfig);
}
```

## `com.feilong.net.filetransfer.sftp.SFTPFileTransferConfig`

```java
public class com.feilong.net.filetransfer.sftp.SFTPFileTransferConfig extends com.feilong.net.filetransfer.AbstractFileTransferConfig {
  public com.feilong.net.filetransfer.sftp.SFTPFileTransferConfig();
  public java.util.Properties getSshConfig();
  public void setSshConfig(java.util.Properties);
  public int getSessionTimeout();
  public void setSessionTimeout(int);
}
```
