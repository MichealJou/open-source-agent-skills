# com.feilong.net.filetransfer

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.net.filetransfer.AbstractFileTransfer`

```java
public abstract class com.feilong.net.filetransfer.AbstractFileTransfer implements com.feilong.net.filetransfer.FileTransfer {
  public com.feilong.net.filetransfer.AbstractFileTransfer();
  public void download(java.lang.String, java.lang.String...);
  public boolean upload(java.lang.String, java.lang.String...);
  public java.util.Map<java.lang.String, com.feilong.io.entity.FileInfoEntity> getFileEntityMap(java.lang.String, java.lang.String...);
  public boolean delete(java.lang.String...);
  public java.lang.String getLogTraceContext();
  public void setLogTraceContext(java.lang.String);
}
```

## `com.feilong.net.filetransfer.AbstractFileTransferConfig`

```java
public abstract class com.feilong.net.filetransfer.AbstractFileTransferConfig {
  public com.feilong.net.filetransfer.AbstractFileTransferConfig();
  public java.lang.String getHostName();
  public void setHostName(java.lang.String);
  public java.lang.String getUserName();
  public void setUserName(java.lang.String);
  public java.lang.String getPassword();
  public void setPassword(java.lang.String);
  public java.lang.Integer getPort();
  public void setPort(java.lang.Integer);
}
```

## `com.feilong.net.filetransfer.FileTransfer`

```java
public interface com.feilong.net.filetransfer.FileTransfer {
  public abstract void download(java.lang.String, java.lang.String...);
  public abstract boolean upload(java.lang.String, java.lang.String...);
  public abstract boolean delete(java.lang.String...);
  public abstract java.util.Map<java.lang.String, com.feilong.io.entity.FileInfoEntity> getFileEntityMap(java.lang.String, java.lang.String...);
}
```

## `com.feilong.net.filetransfer.FileTransferException`

```java
public final class com.feilong.net.filetransfer.FileTransferException extends com.feilong.core.DefaultRuntimeException {
  public com.feilong.net.filetransfer.FileTransferException(java.lang.String, java.lang.Object...);
  public com.feilong.net.filetransfer.FileTransferException(java.lang.String, java.lang.Throwable);
}
```
