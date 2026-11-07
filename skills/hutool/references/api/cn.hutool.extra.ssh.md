# cn.hutool.extra.ssh

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.ssh.ChannelType`

```java
public final class cn.hutool.extra.ssh.ChannelType extends java.lang.Enum<cn.hutool.extra.ssh.ChannelType> {
  public static cn.hutool.extra.ssh.ChannelType[] values();
  public static cn.hutool.extra.ssh.ChannelType valueOf(java.lang.String);
  public java.lang.String getValue();
}
```

## `cn.hutool.extra.ssh.Connector`

```java
public class cn.hutool.extra.ssh.Connector {
  public cn.hutool.extra.ssh.Connector();
  public cn.hutool.extra.ssh.Connector(java.lang.String, java.lang.String, java.lang.String);
  public cn.hutool.extra.ssh.Connector(java.lang.String, int, java.lang.String, java.lang.String);
  public java.lang.String getHost();
  public void setHost(java.lang.String);
  public int getPort();
  public void setPort(int);
  public java.lang.String getUser();
  public void setUser(java.lang.String);
  public java.lang.String getPassword();
  public void setPassword(java.lang.String);
  public java.lang.String getGroup();
  public void setGroup(java.lang.String);
  public java.lang.String toString();
}
```

## `cn.hutool.extra.ssh.GanymedUtil`

```java
public class cn.hutool.extra.ssh.GanymedUtil {
  public cn.hutool.extra.ssh.GanymedUtil();
  public static ch.ethz.ssh2.Connection connect(java.lang.String, int);
  public static ch.ethz.ssh2.Session openSession(java.lang.String, int, java.lang.String, java.lang.String);
  public static java.lang.String exec(ch.ethz.ssh2.Session, java.lang.String, java.nio.charset.Charset, java.io.OutputStream);
  public static java.lang.String execByShell(ch.ethz.ssh2.Session, java.lang.String, java.nio.charset.Charset, java.io.OutputStream);
  public static void close(ch.ethz.ssh2.Session);
}
```

## `cn.hutool.extra.ssh.JschRuntimeException`

```java
public class cn.hutool.extra.ssh.JschRuntimeException extends java.lang.RuntimeException {
  public cn.hutool.extra.ssh.JschRuntimeException(java.lang.Throwable);
  public cn.hutool.extra.ssh.JschRuntimeException(java.lang.String);
  public cn.hutool.extra.ssh.JschRuntimeException(java.lang.String, java.lang.Object...);
  public cn.hutool.extra.ssh.JschRuntimeException(java.lang.String, java.lang.Throwable);
  public cn.hutool.extra.ssh.JschRuntimeException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.extra.ssh.JschRuntimeException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.extra.ssh.JschSessionPool`

```java
public final class cn.hutool.extra.ssh.JschSessionPool extends java.lang.Enum<cn.hutool.extra.ssh.JschSessionPool> {
  public static cn.hutool.extra.ssh.JschSessionPool[] values();
  public static cn.hutool.extra.ssh.JschSessionPool valueOf(java.lang.String);
  public com.jcraft.jsch.Session get(java.lang.String);
  public com.jcraft.jsch.Session getSession(java.lang.String, int, java.lang.String, java.lang.String);
  public com.jcraft.jsch.Session getSession(java.lang.String, int, java.lang.String, java.lang.String, byte[]);
  public com.jcraft.jsch.Session getSession(java.lang.String, int, java.lang.String, byte[], byte[]);
  public void put(java.lang.String, com.jcraft.jsch.Session);
  public void close(java.lang.String);
  public void remove(com.jcraft.jsch.Session);
  public void closeAll();
}
```

## `cn.hutool.extra.ssh.JschUtil`

```java
public class cn.hutool.extra.ssh.JschUtil {
  public cn.hutool.extra.ssh.JschUtil();
  public static int generateLocalPort();
  public static com.jcraft.jsch.Session getSession(java.lang.String, int, java.lang.String, java.lang.String);
  public static com.jcraft.jsch.Session getSession(java.lang.String, int, java.lang.String, java.lang.String, byte[]);
  public static com.jcraft.jsch.Session getSession(java.lang.String, int, java.lang.String, byte[], byte[]);
  public static com.jcraft.jsch.Session openSession(java.lang.String, int, java.lang.String, java.lang.String);
  public static com.jcraft.jsch.Session openSession(java.lang.String, int, java.lang.String, java.lang.String, int);
  public static com.jcraft.jsch.Session openSession(java.lang.String, int, java.lang.String, java.lang.String, byte[]);
  public static com.jcraft.jsch.Session openSession(java.lang.String, int, java.lang.String, byte[], byte[]);
  public static com.jcraft.jsch.Session openSession(java.lang.String, int, java.lang.String, byte[], byte[], int);
  public static com.jcraft.jsch.Session openSession(java.lang.String, int, java.lang.String, java.lang.String, byte[], int);
  public static com.jcraft.jsch.Session createSession(java.lang.String, int, java.lang.String, java.lang.String);
  public static com.jcraft.jsch.Session createSession(java.lang.String, int, java.lang.String, java.lang.String, byte[]);
  public static com.jcraft.jsch.Session createSession(java.lang.String, int, java.lang.String, byte[], byte[]);
  public static com.jcraft.jsch.Session createSession(com.jcraft.jsch.JSch, java.lang.String, int, java.lang.String);
  public static boolean bindPort(com.jcraft.jsch.Session, java.lang.String, int, int) throws cn.hutool.extra.ssh.JschRuntimeException;
  public static boolean bindPort(com.jcraft.jsch.Session, java.lang.String, int, java.lang.String, int) throws cn.hutool.extra.ssh.JschRuntimeException;
  public static boolean bindRemotePort(com.jcraft.jsch.Session, int, java.lang.String, int) throws cn.hutool.extra.ssh.JschRuntimeException;
  public static boolean unBindPort(com.jcraft.jsch.Session, int);
  public static int openAndBindPortToLocal(cn.hutool.extra.ssh.Connector, java.lang.String, int) throws cn.hutool.extra.ssh.JschRuntimeException;
  public static com.jcraft.jsch.ChannelSftp openSftp(com.jcraft.jsch.Session);
  public static com.jcraft.jsch.ChannelSftp openSftp(com.jcraft.jsch.Session, int);
  public static cn.hutool.extra.ssh.Sftp createSftp(java.lang.String, int, java.lang.String, java.lang.String);
  public static cn.hutool.extra.ssh.Sftp createSftp(com.jcraft.jsch.Session);
  public static com.jcraft.jsch.ChannelShell openShell(com.jcraft.jsch.Session);
  public static com.jcraft.jsch.Channel openChannel(com.jcraft.jsch.Session, cn.hutool.extra.ssh.ChannelType);
  public static com.jcraft.jsch.Channel openChannel(com.jcraft.jsch.Session, cn.hutool.extra.ssh.ChannelType, int);
  public static com.jcraft.jsch.Channel createChannel(com.jcraft.jsch.Session, cn.hutool.extra.ssh.ChannelType);
  public static java.lang.String exec(com.jcraft.jsch.Session, java.lang.String, java.nio.charset.Charset);
  public static java.lang.String exec(com.jcraft.jsch.Session, java.lang.String, java.nio.charset.Charset, java.io.OutputStream);
  public static java.lang.String execByShell(com.jcraft.jsch.Session, java.lang.String, java.nio.charset.Charset);
  public static void close(com.jcraft.jsch.Session);
  public static void close(com.jcraft.jsch.Channel);
  public static void close(java.lang.String);
  public static void closeAll();
}
```

## `cn.hutool.extra.ssh.Sftp`

```java
public class cn.hutool.extra.ssh.Sftp extends cn.hutool.extra.ftp.AbstractFtp {
  public cn.hutool.extra.ssh.Sftp(java.lang.String, int, java.lang.String, java.lang.String);
  public cn.hutool.extra.ssh.Sftp(java.lang.String, int, java.lang.String, java.lang.String, java.nio.charset.Charset);
  public cn.hutool.extra.ssh.Sftp(cn.hutool.extra.ftp.FtpConfig);
  public cn.hutool.extra.ssh.Sftp(cn.hutool.extra.ftp.FtpConfig, boolean);
  public cn.hutool.extra.ssh.Sftp(com.jcraft.jsch.Session);
  public cn.hutool.extra.ssh.Sftp(com.jcraft.jsch.Session, java.nio.charset.Charset);
  public cn.hutool.extra.ssh.Sftp(com.jcraft.jsch.Session, java.nio.charset.Charset, long);
  public cn.hutool.extra.ssh.Sftp(com.jcraft.jsch.ChannelSftp, java.nio.charset.Charset, long);
  public cn.hutool.extra.ssh.Sftp(com.jcraft.jsch.ChannelSftp, java.nio.charset.Charset);
  public void init(java.lang.String, int, java.lang.String, java.lang.String, java.nio.charset.Charset);
  public void init();
  public void init(cn.hutool.extra.ftp.FtpConfig);
  public void init(com.jcraft.jsch.Session, java.nio.charset.Charset);
  public void init(com.jcraft.jsch.ChannelSftp, java.nio.charset.Charset);
  public cn.hutool.extra.ssh.Sftp reconnectIfTimeout();
  public com.jcraft.jsch.ChannelSftp getClient();
  public java.lang.String pwd();
  public java.lang.String home();
  public java.util.List<java.lang.String> ls(java.lang.String);
  public java.util.List<java.lang.String> lsDirs(java.lang.String);
  public java.util.List<java.lang.String> lsFiles(java.lang.String);
  public java.util.List<java.lang.String> ls(java.lang.String, cn.hutool.core.lang.Filter<com.jcraft.jsch.ChannelSftp$LsEntry>);
  public java.util.List<com.jcraft.jsch.ChannelSftp$LsEntry> lsEntries(java.lang.String);
  public java.util.List<com.jcraft.jsch.ChannelSftp$LsEntry> lsEntries(java.lang.String, cn.hutool.core.lang.Filter<com.jcraft.jsch.ChannelSftp$LsEntry>);
  public boolean mkdir(java.lang.String);
  public boolean isDir(java.lang.String);
  public synchronized boolean cd(java.lang.String) throws cn.hutool.extra.ftp.FtpException;
  public boolean delFile(java.lang.String);
  public boolean delDir(java.lang.String);
  public void syncUpload(java.io.File, java.lang.String);
  public boolean upload(java.lang.String, java.io.File);
  public boolean upload(java.lang.String, java.lang.String, java.io.InputStream);
  public cn.hutool.extra.ssh.Sftp put(java.lang.String, java.lang.String);
  public cn.hutool.extra.ssh.Sftp put(java.lang.String, java.lang.String, cn.hutool.extra.ssh.Sftp$Mode);
  public cn.hutool.extra.ssh.Sftp put(java.lang.String, java.lang.String, com.jcraft.jsch.SftpProgressMonitor, cn.hutool.extra.ssh.Sftp$Mode);
  public cn.hutool.extra.ssh.Sftp put(java.io.InputStream, java.lang.String, com.jcraft.jsch.SftpProgressMonitor, cn.hutool.extra.ssh.Sftp$Mode);
  public void download(java.lang.String, java.io.File);
  public void download(java.lang.String, java.io.OutputStream);
  public void recursiveDownloadFolder(java.lang.String, java.io.File) throws cn.hutool.extra.ssh.JschRuntimeException;
  public void rename(java.lang.String, java.lang.String);
  public cn.hutool.extra.ssh.Sftp get(java.lang.String, java.lang.String);
  public cn.hutool.extra.ssh.Sftp get(java.lang.String, java.io.OutputStream);
  public void close();
  public java.lang.String toString();
  public cn.hutool.extra.ftp.AbstractFtp reconnectIfTimeout();
}
```

## `cn.hutool.extra.ssh.Sftp$Mode`

```java
public final class cn.hutool.extra.ssh.Sftp$Mode extends java.lang.Enum<cn.hutool.extra.ssh.Sftp$Mode> {
  public static cn.hutool.extra.ssh.Sftp$Mode[] values();
  public static cn.hutool.extra.ssh.Sftp$Mode valueOf(java.lang.String);
}
```

## `cn.hutool.extra.ssh.SshjSftp`

```java
public class cn.hutool.extra.ssh.SshjSftp extends cn.hutool.extra.ftp.AbstractFtp {
  public cn.hutool.extra.ssh.SshjSftp(java.lang.String);
  public cn.hutool.extra.ssh.SshjSftp(java.lang.String, java.lang.String, java.lang.String);
  public cn.hutool.extra.ssh.SshjSftp(java.lang.String, int, java.lang.String, java.lang.String);
  public cn.hutool.extra.ssh.SshjSftp(java.lang.String, int, java.lang.String, java.lang.String, java.nio.charset.Charset);
  public cn.hutool.extra.ssh.SshjSftp(cn.hutool.extra.ftp.FtpConfig);
  public void init();
  public cn.hutool.extra.ftp.AbstractFtp reconnectIfTimeout();
  public boolean cd(java.lang.String);
  public java.lang.String pwd();
  public boolean mkdir(java.lang.String);
  public java.util.List<java.lang.String> ls(java.lang.String);
  public boolean delFile(java.lang.String);
  public boolean delDir(java.lang.String);
  public boolean upload(java.lang.String, java.io.File);
  public void download(java.lang.String, java.io.File);
  public void recursiveDownloadFolder(java.lang.String, java.io.File);
  public void rename(java.lang.String, java.lang.String);
  public void close();
  public boolean containsFile(java.lang.String);
  public java.lang.String command(java.lang.String);
}
```
