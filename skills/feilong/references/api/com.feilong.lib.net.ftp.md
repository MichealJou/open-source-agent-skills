# com.feilong.lib.net.ftp

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.net.ftp.Configurable`

```java
public interface com.feilong.lib.net.ftp.Configurable {
  public abstract void configure(com.feilong.lib.net.ftp.FTPClientConfig);
}
```

## `com.feilong.lib.net.ftp.FTP`

```java
public class com.feilong.lib.net.ftp.FTP extends com.feilong.lib.net.SocketClient {
  public com.feilong.lib.net.ftp.FTP();
  public void setControlEncoding(java.lang.String);
  public java.lang.String getControlEncoding();
  public void disconnect() throws java.io.IOException;
  public int sendCommand(java.lang.String, java.lang.String) throws java.io.IOException;
  public int sendCommand(com.feilong.lib.net.ftp.FTPCmd) throws java.io.IOException;
  public int sendCommand(com.feilong.lib.net.ftp.FTPCmd, java.lang.String) throws java.io.IOException;
  public int sendCommand(java.lang.String) throws java.io.IOException;
  public int getReplyCode();
  public int getReply() throws java.io.IOException;
  public java.lang.String[] getReplyStrings();
  public java.lang.String getReplyString();
  public int user(java.lang.String) throws java.io.IOException;
  public int pass(java.lang.String) throws java.io.IOException;
  public int acct(java.lang.String) throws java.io.IOException;
  public int abor() throws java.io.IOException;
  public int cwd(java.lang.String) throws java.io.IOException;
  public int cdup() throws java.io.IOException;
  public int quit() throws java.io.IOException;
  public int rein() throws java.io.IOException;
  public int smnt(java.lang.String) throws java.io.IOException;
  public int port(java.net.InetAddress, int) throws java.io.IOException;
  public int eprt(java.net.InetAddress, int) throws java.io.IOException;
  public int pasv() throws java.io.IOException;
  public int epsv() throws java.io.IOException;
  public int type(int, int) throws java.io.IOException;
  public int type(int) throws java.io.IOException;
  public int stru(int) throws java.io.IOException;
  public int mode(int) throws java.io.IOException;
  public int retr(java.lang.String) throws java.io.IOException;
  public int stor(java.lang.String) throws java.io.IOException;
  public int stou() throws java.io.IOException;
  public int stou(java.lang.String) throws java.io.IOException;
  public int appe(java.lang.String) throws java.io.IOException;
  public int allo(int) throws java.io.IOException;
  public int feat() throws java.io.IOException;
  public int allo(int, int) throws java.io.IOException;
  public int rest(java.lang.String) throws java.io.IOException;
  public int mdtm(java.lang.String) throws java.io.IOException;
  public int mfmt(java.lang.String, java.lang.String) throws java.io.IOException;
  public int rnfr(java.lang.String) throws java.io.IOException;
  public int rnto(java.lang.String) throws java.io.IOException;
  public int dele(java.lang.String) throws java.io.IOException;
  public int rmd(java.lang.String) throws java.io.IOException;
  public int mkd(java.lang.String) throws java.io.IOException;
  public int pwd() throws java.io.IOException;
  public int list() throws java.io.IOException;
  public int list(java.lang.String) throws java.io.IOException;
  public int mlsd() throws java.io.IOException;
  public int mlsd(java.lang.String) throws java.io.IOException;
  public int mlst() throws java.io.IOException;
  public int mlst(java.lang.String) throws java.io.IOException;
  public int nlst() throws java.io.IOException;
  public int nlst(java.lang.String) throws java.io.IOException;
  public int site(java.lang.String) throws java.io.IOException;
  public int syst() throws java.io.IOException;
  public int stat() throws java.io.IOException;
  public int stat(java.lang.String) throws java.io.IOException;
  public int help() throws java.io.IOException;
  public int help(java.lang.String) throws java.io.IOException;
  public int noop() throws java.io.IOException;
  public boolean isStrictMultilineParsing();
  public void setStrictMultilineParsing(boolean);
  public boolean isStrictReplyParsing();
  public void setStrictReplyParsing(boolean);
}
```

## `com.feilong.lib.net.ftp.FTPClient`

```java
public class com.feilong.lib.net.ftp.FTPClient extends com.feilong.lib.net.ftp.FTP implements com.feilong.lib.net.ftp.Configurable {
  public com.feilong.lib.net.ftp.FTPClient();
  public void setDataTimeout(int);
  public void setParserFactory(com.feilong.lib.net.ftp.parser.FTPFileEntryParserFactory);
  public void disconnect() throws java.io.IOException;
  public void setRemoteVerificationEnabled(boolean);
  public boolean isRemoteVerificationEnabled();
  public boolean login(java.lang.String, java.lang.String) throws java.io.IOException;
  public boolean login(java.lang.String, java.lang.String, java.lang.String) throws java.io.IOException;
  public boolean logout() throws java.io.IOException;
  public boolean changeWorkingDirectory(java.lang.String) throws java.io.IOException;
  public boolean changeToParentDirectory() throws java.io.IOException;
  public boolean structureMount(java.lang.String) throws java.io.IOException;
  public boolean reinitialize() throws java.io.IOException;
  public void enterLocalActiveMode();
  public void enterLocalPassiveMode();
  public boolean enterRemoteActiveMode(java.net.InetAddress, int) throws java.io.IOException;
  public boolean enterRemotePassiveMode() throws java.io.IOException;
  public java.lang.String getPassiveHost();
  public int getPassivePort();
  public int getDataConnectionMode();
  public void setActivePortRange(int, int);
  public void setActiveExternalIPAddress(java.lang.String) throws java.net.UnknownHostException;
  public void setPassiveLocalIPAddress(java.lang.String) throws java.net.UnknownHostException;
  public void setPassiveLocalIPAddress(java.net.InetAddress);
  public java.net.InetAddress getPassiveLocalIPAddress();
  public void setReportActiveExternalIPAddress(java.lang.String) throws java.net.UnknownHostException;
  public boolean setFileType(int) throws java.io.IOException;
  public boolean setFileType(int, int) throws java.io.IOException;
  public boolean setFileStructure(int) throws java.io.IOException;
  public boolean setFileTransferMode(int) throws java.io.IOException;
  public boolean remoteRetrieve(java.lang.String) throws java.io.IOException;
  public boolean remoteStore(java.lang.String) throws java.io.IOException;
  public boolean remoteStoreUnique(java.lang.String) throws java.io.IOException;
  public boolean remoteStoreUnique() throws java.io.IOException;
  public boolean remoteAppend(java.lang.String) throws java.io.IOException;
  public boolean completePendingCommand() throws java.io.IOException;
  public boolean retrieveFile(java.lang.String, java.io.OutputStream) throws java.io.IOException;
  public java.io.InputStream retrieveFileStream(java.lang.String) throws java.io.IOException;
  public boolean storeFile(java.lang.String, java.io.InputStream) throws java.io.IOException;
  public java.io.OutputStream storeFileStream(java.lang.String) throws java.io.IOException;
  public boolean appendFile(java.lang.String, java.io.InputStream) throws java.io.IOException;
  public java.io.OutputStream appendFileStream(java.lang.String) throws java.io.IOException;
  public boolean storeUniqueFile(java.lang.String, java.io.InputStream) throws java.io.IOException;
  public java.io.OutputStream storeUniqueFileStream(java.lang.String) throws java.io.IOException;
  public boolean storeUniqueFile(java.io.InputStream) throws java.io.IOException;
  public java.io.OutputStream storeUniqueFileStream() throws java.io.IOException;
  public boolean allocate(int) throws java.io.IOException;
  public boolean features() throws java.io.IOException;
  public java.lang.String[] featureValues(java.lang.String) throws java.io.IOException;
  public java.lang.String featureValue(java.lang.String) throws java.io.IOException;
  public boolean hasFeature(java.lang.String) throws java.io.IOException;
  public boolean hasFeature(java.lang.String, java.lang.String) throws java.io.IOException;
  public boolean allocate(int, int) throws java.io.IOException;
  public boolean doCommand(java.lang.String, java.lang.String) throws java.io.IOException;
  public java.lang.String[] doCommandAsStrings(java.lang.String, java.lang.String) throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPFile mlistFile(java.lang.String) throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPFile[] mlistDir() throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPFile[] mlistDir(java.lang.String) throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPFile[] mlistDir(java.lang.String, com.feilong.lib.net.ftp.FTPFileFilter) throws java.io.IOException;
  public void setRestartOffset(long);
  public long getRestartOffset();
  public boolean rename(java.lang.String, java.lang.String) throws java.io.IOException;
  public boolean abort() throws java.io.IOException;
  public boolean deleteFile(java.lang.String) throws java.io.IOException;
  public boolean removeDirectory(java.lang.String) throws java.io.IOException;
  public boolean makeDirectory(java.lang.String) throws java.io.IOException;
  public java.lang.String printWorkingDirectory() throws java.io.IOException;
  public boolean sendSiteCommand(java.lang.String) throws java.io.IOException;
  public java.lang.String getSystemType() throws java.io.IOException;
  public java.lang.String listHelp() throws java.io.IOException;
  public java.lang.String listHelp(java.lang.String) throws java.io.IOException;
  public boolean sendNoOp() throws java.io.IOException;
  public java.lang.String[] listNames(java.lang.String) throws java.io.IOException;
  public java.lang.String[] listNames() throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPFile[] listFiles(java.lang.String) throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPFile[] listFiles() throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPFile[] listFiles(java.lang.String, com.feilong.lib.net.ftp.FTPFileFilter) throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPFile[] listDirectories() throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPFile[] listDirectories(java.lang.String) throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPListParseEngine initiateListParsing() throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPListParseEngine initiateListParsing(java.lang.String) throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPListParseEngine initiateListParsing(java.lang.String, java.lang.String) throws java.io.IOException;
  public java.lang.String getStatus() throws java.io.IOException;
  public java.lang.String getStatus(java.lang.String) throws java.io.IOException;
  public java.lang.String getModificationTime(java.lang.String) throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPFile mdtmFile(java.lang.String) throws java.io.IOException;
  public boolean setModificationTime(java.lang.String, java.lang.String) throws java.io.IOException;
  public void setBufferSize(int);
  public int getBufferSize();
  public void setSendDataSocketBufferSize(int);
  public int getSendDataSocketBufferSize();
  public void setReceieveDataSocketBufferSize(int);
  public int getReceiveDataSocketBufferSize();
  public void configure(com.feilong.lib.net.ftp.FTPClientConfig);
  public void setListHiddenFiles(boolean);
  public boolean getListHiddenFiles();
  public boolean isUseEPSVwithIPv4();
  public void setUseEPSVwithIPv4(boolean);
  public void setCopyStreamListener(com.feilong.lib.net.io.CopyStreamListener);
  public com.feilong.lib.net.io.CopyStreamListener getCopyStreamListener();
  public void setControlKeepAliveTimeout(long);
  public long getControlKeepAliveTimeout();
  public void setControlKeepAliveReplyTimeout(int);
  public int getControlKeepAliveReplyTimeout();
  public void setPassiveNatWorkaround(boolean);
  public void setPassiveNatWorkaroundStrategy(com.feilong.lib.net.ftp.FTPClient$HostnameResolver);
  public void setAutodetectUTF8(boolean);
  public boolean getAutodetectUTF8();
  public java.lang.String getSystemName() throws java.io.IOException;
}
```

## `com.feilong.lib.net.ftp.FTPClient$HostnameResolver`

```java
public interface com.feilong.lib.net.ftp.FTPClient$HostnameResolver {
  public abstract java.lang.String resolve(java.lang.String) throws java.net.UnknownHostException;
}
```

## `com.feilong.lib.net.ftp.FTPClient$NatServerResolverImpl`

```java
public class com.feilong.lib.net.ftp.FTPClient$NatServerResolverImpl implements com.feilong.lib.net.ftp.FTPClient$HostnameResolver {
  public com.feilong.lib.net.ftp.FTPClient$NatServerResolverImpl(com.feilong.lib.net.ftp.FTPClient);
  public java.lang.String resolve(java.lang.String) throws java.net.UnknownHostException;
}
```

## `com.feilong.lib.net.ftp.FTPClientConfig`

```java
public class com.feilong.lib.net.ftp.FTPClientConfig {
  public com.feilong.lib.net.ftp.FTPClientConfig(java.lang.String);
  public com.feilong.lib.net.ftp.FTPClientConfig();
  public com.feilong.lib.net.ftp.FTPClientConfig(java.lang.String, java.lang.String, java.lang.String);
  public com.feilong.lib.net.ftp.FTPClientConfig(java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String);
  public com.feilong.lib.net.ftp.FTPClientConfig(java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String, boolean, boolean);
  public com.feilong.lib.net.ftp.FTPClientConfig(com.feilong.lib.net.ftp.FTPClientConfig);
  public java.lang.String getServerSystemKey();
  public java.lang.String getDefaultDateFormatStr();
  public java.lang.String getRecentDateFormatStr();
  public java.lang.String getServerTimeZoneId();
  public java.lang.String getShortMonthNames();
  public java.lang.String getServerLanguageCode();
  public boolean isLenientFutureDates();
  public void setDefaultDateFormatStr(java.lang.String);
  public void setRecentDateFormatStr(java.lang.String);
  public void setLenientFutureDates(boolean);
  public void setServerTimeZoneId(java.lang.String);
  public void setShortMonthNames(java.lang.String);
  public void setServerLanguageCode(java.lang.String);
  public static java.text.DateFormatSymbols lookupDateFormatSymbols(java.lang.String);
  public static java.text.DateFormatSymbols getDateFormatSymbols(java.lang.String);
  public static java.util.Collection<java.lang.String> getSupportedLanguageCodes();
  public void setUnparseableEntries(boolean);
  public boolean getUnparseableEntries();
}
```

## `com.feilong.lib.net.ftp.FTPCmd`

```java
public final class com.feilong.lib.net.ftp.FTPCmd extends java.lang.Enum<com.feilong.lib.net.ftp.FTPCmd> {
  public static com.feilong.lib.net.ftp.FTPCmd[] values();
  public static com.feilong.lib.net.ftp.FTPCmd valueOf(java.lang.String);
  public final java.lang.String getCommand();
}
```

## `com.feilong.lib.net.ftp.FTPConnectionClosedException`

```java
public class com.feilong.lib.net.ftp.FTPConnectionClosedException extends java.io.IOException {
  public com.feilong.lib.net.ftp.FTPConnectionClosedException();
  public com.feilong.lib.net.ftp.FTPConnectionClosedException(java.lang.String);
}
```

## `com.feilong.lib.net.ftp.FTPFile`

```java
public class com.feilong.lib.net.ftp.FTPFile implements java.io.Serializable {
  public com.feilong.lib.net.ftp.FTPFile();
  public void setRawListing(java.lang.String);
  public java.lang.String getRawListing();
  public boolean isDirectory();
  public boolean isFile();
  public boolean isSymbolicLink();
  public boolean isUnknown();
  public boolean isValid();
  public void setType(int);
  public int getType();
  public void setName(java.lang.String);
  public java.lang.String getName();
  public void setSize(long);
  public long getSize();
  public void setHardLinkCount(int);
  public int getHardLinkCount();
  public void setGroup(java.lang.String);
  public java.lang.String getGroup();
  public void setUser(java.lang.String);
  public java.lang.String getUser();
  public void setLink(java.lang.String);
  public java.lang.String getLink();
  public void setTimestamp(java.util.Calendar);
  public java.util.Calendar getTimestamp();
  public void setPermission(int, int, boolean);
  public boolean hasPermission(int, int);
  public java.lang.String toString();
  public java.lang.String toFormattedString();
  public java.lang.String toFormattedString(java.lang.String);
}
```

## `com.feilong.lib.net.ftp.FTPFileEntryParser`

```java
public interface com.feilong.lib.net.ftp.FTPFileEntryParser {
  public abstract com.feilong.lib.net.ftp.FTPFile parseFTPEntry(java.lang.String);
  public abstract java.lang.String readNextEntry(java.io.BufferedReader) throws java.io.IOException;
  public abstract java.util.List<java.lang.String> preParse(java.util.List<java.lang.String>);
}
```

## `com.feilong.lib.net.ftp.FTPFileEntryParserImpl`

```java
public abstract class com.feilong.lib.net.ftp.FTPFileEntryParserImpl implements com.feilong.lib.net.ftp.FTPFileEntryParser {
  public com.feilong.lib.net.ftp.FTPFileEntryParserImpl();
  public java.lang.String readNextEntry(java.io.BufferedReader) throws java.io.IOException;
  public java.util.List<java.lang.String> preParse(java.util.List<java.lang.String>);
}
```

## `com.feilong.lib.net.ftp.FTPFileFilter`

```java
public interface com.feilong.lib.net.ftp.FTPFileFilter {
  public abstract boolean accept(com.feilong.lib.net.ftp.FTPFile);
}
```

## `com.feilong.lib.net.ftp.FTPFileFilters`

```java
public class com.feilong.lib.net.ftp.FTPFileFilters {
  public com.feilong.lib.net.ftp.FTPFileFilters();
}
```

## `com.feilong.lib.net.ftp.FTPHTTPClient`

```java
public class com.feilong.lib.net.ftp.FTPHTTPClient extends com.feilong.lib.net.ftp.FTPClient {
  public com.feilong.lib.net.ftp.FTPHTTPClient(java.lang.String, int, java.lang.String, java.lang.String);
  public com.feilong.lib.net.ftp.FTPHTTPClient(java.lang.String, int);
  public void connect(java.lang.String, int) throws java.net.SocketException, java.io.IOException;
}
```

## `com.feilong.lib.net.ftp.FTPListParseEngine`

```java
public class com.feilong.lib.net.ftp.FTPListParseEngine {
  public com.feilong.lib.net.ftp.FTPListParseEngine(com.feilong.lib.net.ftp.FTPFileEntryParser);
  public void readServerList(java.io.InputStream, java.lang.String) throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPFile[] getNext(int);
  public com.feilong.lib.net.ftp.FTPFile[] getPrevious(int);
  public com.feilong.lib.net.ftp.FTPFile[] getFiles() throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPFile[] getFiles(com.feilong.lib.net.ftp.FTPFileFilter) throws java.io.IOException;
  public boolean hasNext();
  public boolean hasPrevious();
  public void resetIterator();
  public void readServerList(java.io.InputStream) throws java.io.IOException;
}
```

## `com.feilong.lib.net.ftp.FTPReply`

```java
public final class com.feilong.lib.net.ftp.FTPReply {
  public static boolean isPositivePreliminary(int);
  public static boolean isPositiveCompletion(int);
  public static boolean isPositiveIntermediate(int);
  public static boolean isNegativeTransient(int);
  public static boolean isNegativePermanent(int);
  public static boolean isProtectedReplyCode(int);
}
```

## `com.feilong.lib.net.ftp.FTPSClient`

```java
public class com.feilong.lib.net.ftp.FTPSClient extends com.feilong.lib.net.ftp.FTPClient {
  public com.feilong.lib.net.ftp.FTPSClient();
  public com.feilong.lib.net.ftp.FTPSClient(boolean);
  public com.feilong.lib.net.ftp.FTPSClient(java.lang.String);
  public com.feilong.lib.net.ftp.FTPSClient(java.lang.String, boolean);
  public com.feilong.lib.net.ftp.FTPSClient(boolean, javax.net.ssl.SSLContext);
  public com.feilong.lib.net.ftp.FTPSClient(javax.net.ssl.SSLContext);
  public void setAuthValue(java.lang.String);
  public java.lang.String getAuthValue();
  public void setKeyManager(javax.net.ssl.KeyManager);
  public void setEnabledSessionCreation(boolean);
  public boolean getEnableSessionCreation();
  public void setNeedClientAuth(boolean);
  public boolean getNeedClientAuth();
  public void setWantClientAuth(boolean);
  public boolean getWantClientAuth();
  public void setUseClientMode(boolean);
  public boolean getUseClientMode();
  public void setEnabledCipherSuites(java.lang.String[]);
  public java.lang.String[] getEnabledCipherSuites();
  public void setEnabledProtocols(java.lang.String[]);
  public java.lang.String[] getEnabledProtocols();
  public void execPBSZ(long) throws javax.net.ssl.SSLException, java.io.IOException;
  public long parsePBSZ(long) throws javax.net.ssl.SSLException, java.io.IOException;
  public void execPROT(java.lang.String) throws javax.net.ssl.SSLException, java.io.IOException;
  public int sendCommand(java.lang.String, java.lang.String) throws java.io.IOException;
  public javax.net.ssl.TrustManager getTrustManager();
  public void setTrustManager(javax.net.ssl.TrustManager);
  public javax.net.ssl.HostnameVerifier getHostnameVerifier();
  public void setHostnameVerifier(javax.net.ssl.HostnameVerifier);
  public boolean isEndpointCheckingEnabled();
  public void setEndpointCheckingEnabled(boolean);
  public void disconnect() throws java.io.IOException;
  public int execAUTH(java.lang.String) throws java.io.IOException;
  public int execADAT(byte[]) throws java.io.IOException;
  public int execCCC() throws java.io.IOException;
  public int execMIC(byte[]) throws java.io.IOException;
  public int execCONF(byte[]) throws java.io.IOException;
  public int execENC(byte[]) throws java.io.IOException;
  public byte[] parseADATReply(java.lang.String);
}
```

## `com.feilong.lib.net.ftp.FTPSServerSocketFactory`

```java
public class com.feilong.lib.net.ftp.FTPSServerSocketFactory extends javax.net.ServerSocketFactory {
  public com.feilong.lib.net.ftp.FTPSServerSocketFactory(javax.net.ssl.SSLContext);
  public java.net.ServerSocket createServerSocket() throws java.io.IOException;
  public java.net.ServerSocket createServerSocket(int) throws java.io.IOException;
  public java.net.ServerSocket createServerSocket(int, int) throws java.io.IOException;
  public java.net.ServerSocket createServerSocket(int, int, java.net.InetAddress) throws java.io.IOException;
  public java.net.ServerSocket init(java.net.ServerSocket);
}
```

## `com.feilong.lib.net.ftp.FTPSSocketFactory`

```java
public class com.feilong.lib.net.ftp.FTPSSocketFactory extends javax.net.SocketFactory {
  public com.feilong.lib.net.ftp.FTPSSocketFactory(javax.net.ssl.SSLContext);
  public java.net.Socket createSocket() throws java.io.IOException;
  public java.net.Socket createSocket(java.lang.String, int) throws java.net.UnknownHostException, java.io.IOException;
  public java.net.Socket createSocket(java.net.InetAddress, int) throws java.io.IOException;
  public java.net.Socket createSocket(java.lang.String, int, java.net.InetAddress, int) throws java.net.UnknownHostException, java.io.IOException;
  public java.net.Socket createSocket(java.net.InetAddress, int, java.net.InetAddress, int) throws java.io.IOException;
  public java.net.ServerSocket createServerSocket(int) throws java.io.IOException;
  public java.net.ServerSocket createServerSocket(int, int) throws java.io.IOException;
  public java.net.ServerSocket createServerSocket(int, int, java.net.InetAddress) throws java.io.IOException;
  public java.net.ServerSocket init(java.net.ServerSocket) throws java.io.IOException;
}
```
