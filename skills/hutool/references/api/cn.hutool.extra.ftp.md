# cn.hutool.extra.ftp

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.ftp.AbstractFtp`

```java
public abstract class cn.hutool.extra.ftp.AbstractFtp implements java.io.Closeable {
  public abstract cn.hutool.extra.ftp.AbstractFtp reconnectIfTimeout();
  public abstract boolean cd(java.lang.String);
  public boolean toParent();
  public abstract java.lang.String pwd();
  public boolean isDir(java.lang.String);
  public abstract boolean mkdir(java.lang.String);
  public boolean exist(java.lang.String);
  public abstract java.util.List<java.lang.String> ls(java.lang.String);
  public abstract boolean delFile(java.lang.String);
  public abstract boolean delDir(java.lang.String);
  public void mkDirs(java.lang.String);
  public abstract boolean upload(java.lang.String, java.io.File);
  public abstract void download(java.lang.String, java.io.File);
  public void download(java.lang.String, java.io.File, java.lang.String);
  public abstract void recursiveDownloadFolder(java.lang.String, java.io.File);
  public abstract void rename(java.lang.String, java.lang.String);
}
```

## `cn.hutool.extra.ftp.Ftp`

```java
public class cn.hutool.extra.ftp.Ftp extends cn.hutool.extra.ftp.AbstractFtp {
  public cn.hutool.extra.ftp.Ftp(java.lang.String);
  public cn.hutool.extra.ftp.Ftp(java.lang.String, int);
  public cn.hutool.extra.ftp.Ftp(java.lang.String, int, java.lang.String, java.lang.String);
  public cn.hutool.extra.ftp.Ftp(java.lang.String, int, java.lang.String, java.lang.String, java.nio.charset.Charset);
  public cn.hutool.extra.ftp.Ftp(java.lang.String, int, java.lang.String, java.lang.String, java.nio.charset.Charset, java.lang.String, java.lang.String);
  public cn.hutool.extra.ftp.Ftp(java.lang.String, int, java.lang.String, java.lang.String, java.nio.charset.Charset, java.lang.String, java.lang.String, cn.hutool.extra.ftp.FtpMode);
  public cn.hutool.extra.ftp.Ftp(cn.hutool.extra.ftp.FtpConfig, cn.hutool.extra.ftp.FtpMode);
  public cn.hutool.extra.ftp.Ftp(org.apache.commons.net.ftp.FTPClient);
  public cn.hutool.extra.ftp.Ftp init();
  public cn.hutool.extra.ftp.Ftp init(java.lang.String, int, java.lang.String, java.lang.String);
  public cn.hutool.extra.ftp.Ftp init(java.lang.String, int, java.lang.String, java.lang.String, cn.hutool.extra.ftp.FtpMode);
  public cn.hutool.extra.ftp.Ftp init(cn.hutool.extra.ftp.FtpConfig, cn.hutool.extra.ftp.FtpMode);
  public cn.hutool.extra.ftp.Ftp setMode(cn.hutool.extra.ftp.FtpMode);
  public cn.hutool.extra.ftp.Ftp setBackToPwd(boolean);
  public boolean isBackToPwd();
  public cn.hutool.extra.ftp.Ftp reconnectIfTimeout();
  public synchronized boolean cd(java.lang.String);
  public java.lang.String pwd();
  public java.util.List<java.lang.String> ls(java.lang.String);
  public java.util.List<org.apache.commons.net.ftp.FTPFile> lsFiles(java.lang.String, cn.hutool.core.lang.Filter<org.apache.commons.net.ftp.FTPFile>);
  public org.apache.commons.net.ftp.FTPFile[] lsFiles(java.lang.String) throws cn.hutool.extra.ftp.FtpException, cn.hutool.core.io.IORuntimeException;
  public boolean mkdir(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public int stat(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public boolean existFile(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public boolean delFile(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public boolean delDir(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public boolean upload(java.lang.String, java.io.File);
  public boolean upload(java.lang.String, java.lang.String, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public boolean upload(java.lang.String, java.lang.String, java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public void uploadFileOrDirectory(java.lang.String, java.io.File);
  public void download(java.lang.String, java.io.File);
  public void recursiveDownloadFolder(java.lang.String, java.io.File);
  public void download(java.lang.String, java.lang.String, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public void download(java.lang.String, java.lang.String, java.io.OutputStream);
  public void download(java.lang.String, java.lang.String, java.io.OutputStream, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public void rename(java.lang.String, java.lang.String);
  public org.apache.commons.net.ftp.FTPClient getClient();
  public void close() throws java.io.IOException;
  public cn.hutool.extra.ftp.AbstractFtp reconnectIfTimeout();
}
```

## `cn.hutool.extra.ftp.FtpConfig`

```java
public class cn.hutool.extra.ftp.FtpConfig implements java.io.Serializable {
  public static cn.hutool.extra.ftp.FtpConfig create();
  public cn.hutool.extra.ftp.FtpConfig();
  public cn.hutool.extra.ftp.FtpConfig(java.lang.String, int, java.lang.String, java.lang.String, java.nio.charset.Charset);
  public cn.hutool.extra.ftp.FtpConfig(java.lang.String, int, java.lang.String, java.lang.String, java.nio.charset.Charset, java.lang.String, java.lang.String);
  public java.lang.String getHost();
  public cn.hutool.extra.ftp.FtpConfig setHost(java.lang.String);
  public int getPort();
  public cn.hutool.extra.ftp.FtpConfig setPort(int);
  public java.lang.String getUser();
  public cn.hutool.extra.ftp.FtpConfig setUser(java.lang.String);
  public java.lang.String getPassword();
  public cn.hutool.extra.ftp.FtpConfig setPassword(java.lang.String);
  public java.nio.charset.Charset getCharset();
  public cn.hutool.extra.ftp.FtpConfig setCharset(java.nio.charset.Charset);
  public long getConnectionTimeout();
  public cn.hutool.extra.ftp.FtpConfig setConnectionTimeout(long);
  public long getSoTimeout();
  public cn.hutool.extra.ftp.FtpConfig setSoTimeout(long);
  public java.lang.String getServerLanguageCode();
  public cn.hutool.extra.ftp.FtpConfig setServerLanguageCode(java.lang.String);
  public java.lang.String getSystemKey();
  public cn.hutool.extra.ftp.FtpConfig setSystemKey(java.lang.String);
}
```

## `cn.hutool.extra.ftp.FtpException`

```java
public class cn.hutool.extra.ftp.FtpException extends java.lang.RuntimeException {
  public cn.hutool.extra.ftp.FtpException(java.lang.Throwable);
  public cn.hutool.extra.ftp.FtpException(java.lang.String);
  public cn.hutool.extra.ftp.FtpException(java.lang.String, java.lang.Object...);
  public cn.hutool.extra.ftp.FtpException(java.lang.String, java.lang.Throwable);
  public cn.hutool.extra.ftp.FtpException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.extra.ftp.FtpException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.extra.ftp.FtpMode`

```java
public final class cn.hutool.extra.ftp.FtpMode extends java.lang.Enum<cn.hutool.extra.ftp.FtpMode> {
  public static cn.hutool.extra.ftp.FtpMode[] values();
  public static cn.hutool.extra.ftp.FtpMode valueOf(java.lang.String);
}
```

## `cn.hutool.extra.ftp.SimpleFtpServer`

```java
public class cn.hutool.extra.ftp.SimpleFtpServer {
  public static cn.hutool.extra.ftp.SimpleFtpServer create();
  public cn.hutool.extra.ftp.SimpleFtpServer();
  public org.apache.ftpserver.FtpServerFactory getServerFactory();
  public cn.hutool.extra.ftp.SimpleFtpServer setConnectionConfig(org.apache.ftpserver.ConnectionConfig);
  public org.apache.ftpserver.listener.ListenerFactory getListenerFactory();
  public cn.hutool.extra.ftp.SimpleFtpServer setPort(int);
  public org.apache.ftpserver.ftplet.UserManager getUserManager();
  public cn.hutool.extra.ftp.SimpleFtpServer addUser(org.apache.ftpserver.ftplet.User);
  public cn.hutool.extra.ftp.SimpleFtpServer addAnonymous(java.lang.String);
  public cn.hutool.extra.ftp.SimpleFtpServer delUser(java.lang.String);
  public cn.hutool.extra.ftp.SimpleFtpServer setSsl(org.apache.ftpserver.ssl.SslConfiguration);
  public cn.hutool.extra.ftp.SimpleFtpServer setSsl(java.io.File, java.lang.String);
  public cn.hutool.extra.ftp.SimpleFtpServer setUserManager(org.apache.ftpserver.ftplet.UserManager);
  public cn.hutool.extra.ftp.SimpleFtpServer setUsersConfig(java.io.File);
  public cn.hutool.extra.ftp.SimpleFtpServer addFtplet(java.lang.String, org.apache.ftpserver.ftplet.Ftplet);
  public void start();
}
```
