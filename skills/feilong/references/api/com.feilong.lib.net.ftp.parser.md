# com.feilong.lib.net.ftp.parser

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.net.ftp.parser.CompositeFileEntryParser`

```java
public class com.feilong.lib.net.ftp.parser.CompositeFileEntryParser extends com.feilong.lib.net.ftp.FTPFileEntryParserImpl {
  public com.feilong.lib.net.ftp.parser.CompositeFileEntryParser(com.feilong.lib.net.ftp.FTPFileEntryParser[]);
  public com.feilong.lib.net.ftp.FTPFile parseFTPEntry(java.lang.String);
}
```

## `com.feilong.lib.net.ftp.parser.ConfigurableFTPFileEntryParserImpl`

```java
public abstract class com.feilong.lib.net.ftp.parser.ConfigurableFTPFileEntryParserImpl extends com.feilong.lib.net.ftp.parser.RegexFTPFileEntryParserImpl implements com.feilong.lib.net.ftp.Configurable {
  public com.feilong.lib.net.ftp.parser.ConfigurableFTPFileEntryParserImpl(java.lang.String);
  public com.feilong.lib.net.ftp.parser.ConfigurableFTPFileEntryParserImpl(java.lang.String, int);
  public java.util.Calendar parseTimestamp(java.lang.String) throws java.text.ParseException;
  public void configure(com.feilong.lib.net.ftp.FTPClientConfig);
}
```

## `com.feilong.lib.net.ftp.parser.DefaultFTPFileEntryParserFactory`

```java
public class com.feilong.lib.net.ftp.parser.DefaultFTPFileEntryParserFactory implements com.feilong.lib.net.ftp.parser.FTPFileEntryParserFactory {
  public com.feilong.lib.net.ftp.parser.DefaultFTPFileEntryParserFactory();
  public com.feilong.lib.net.ftp.FTPFileEntryParser createFileEntryParser(java.lang.String);
  public com.feilong.lib.net.ftp.FTPFileEntryParser createFileEntryParser(com.feilong.lib.net.ftp.FTPClientConfig) throws com.feilong.lib.net.ftp.parser.ParserInitializationException;
  public com.feilong.lib.net.ftp.FTPFileEntryParser createUnixFTPEntryParser();
  public com.feilong.lib.net.ftp.FTPFileEntryParser createVMSVersioningFTPEntryParser();
  public com.feilong.lib.net.ftp.FTPFileEntryParser createNetwareFTPEntryParser();
  public com.feilong.lib.net.ftp.FTPFileEntryParser createNTFTPEntryParser();
  public com.feilong.lib.net.ftp.FTPFileEntryParser createOS2FTPEntryParser();
  public com.feilong.lib.net.ftp.FTPFileEntryParser createOS400FTPEntryParser();
  public com.feilong.lib.net.ftp.FTPFileEntryParser createMVSEntryParser();
}
```

## `com.feilong.lib.net.ftp.parser.EnterpriseUnixFTPEntryParser`

```java
public class com.feilong.lib.net.ftp.parser.EnterpriseUnixFTPEntryParser extends com.feilong.lib.net.ftp.parser.RegexFTPFileEntryParserImpl {
  public com.feilong.lib.net.ftp.parser.EnterpriseUnixFTPEntryParser();
  public com.feilong.lib.net.ftp.FTPFile parseFTPEntry(java.lang.String);
}
```

## `com.feilong.lib.net.ftp.parser.FTPFileEntryParserFactory`

```java
public interface com.feilong.lib.net.ftp.parser.FTPFileEntryParserFactory {
  public abstract com.feilong.lib.net.ftp.FTPFileEntryParser createFileEntryParser(java.lang.String) throws com.feilong.lib.net.ftp.parser.ParserInitializationException;
  public abstract com.feilong.lib.net.ftp.FTPFileEntryParser createFileEntryParser(com.feilong.lib.net.ftp.FTPClientConfig) throws com.feilong.lib.net.ftp.parser.ParserInitializationException;
}
```

## `com.feilong.lib.net.ftp.parser.FTPTimestampParser`

```java
public interface com.feilong.lib.net.ftp.parser.FTPTimestampParser {
  public abstract java.util.Calendar parseTimestamp(java.lang.String) throws java.text.ParseException;
}
```

## `com.feilong.lib.net.ftp.parser.FTPTimestampParserImpl`

```java
public class com.feilong.lib.net.ftp.parser.FTPTimestampParserImpl implements com.feilong.lib.net.ftp.parser.FTPTimestampParser,com.feilong.lib.net.ftp.Configurable {
  public com.feilong.lib.net.ftp.parser.FTPTimestampParserImpl();
  public java.util.Calendar parseTimestamp(java.lang.String) throws java.text.ParseException;
  public java.util.Calendar parseTimestamp(java.lang.String, java.util.Calendar) throws java.text.ParseException;
  public java.text.SimpleDateFormat getDefaultDateFormat();
  public java.lang.String getDefaultDateFormatString();
  public java.text.SimpleDateFormat getRecentDateFormat();
  public java.lang.String getRecentDateFormatString();
  public java.lang.String[] getShortMonths();
  public java.util.TimeZone getServerTimeZone();
  public void configure(com.feilong.lib.net.ftp.FTPClientConfig);
}
```

## `com.feilong.lib.net.ftp.parser.MLSxEntryParser`

```java
public class com.feilong.lib.net.ftp.parser.MLSxEntryParser extends com.feilong.lib.net.ftp.FTPFileEntryParserImpl {
  public com.feilong.lib.net.ftp.parser.MLSxEntryParser();
  public com.feilong.lib.net.ftp.FTPFile parseFTPEntry(java.lang.String);
  public static java.util.Calendar parseGMTdateTime(java.lang.String);
  public static com.feilong.lib.net.ftp.FTPFile parseEntry(java.lang.String);
  public static com.feilong.lib.net.ftp.parser.MLSxEntryParser getInstance();
}
```

## `com.feilong.lib.net.ftp.parser.MVSFTPEntryParser`

```java
public class com.feilong.lib.net.ftp.parser.MVSFTPEntryParser extends com.feilong.lib.net.ftp.parser.ConfigurableFTPFileEntryParserImpl {
  public com.feilong.lib.net.ftp.parser.MVSFTPEntryParser();
  public com.feilong.lib.net.ftp.FTPFile parseFTPEntry(java.lang.String);
  public java.util.List<java.lang.String> preParse(java.util.List<java.lang.String>);
}
```

## `com.feilong.lib.net.ftp.parser.MacOsPeterFTPEntryParser`

```java
public class com.feilong.lib.net.ftp.parser.MacOsPeterFTPEntryParser extends com.feilong.lib.net.ftp.parser.ConfigurableFTPFileEntryParserImpl {
  public com.feilong.lib.net.ftp.parser.MacOsPeterFTPEntryParser();
  public com.feilong.lib.net.ftp.parser.MacOsPeterFTPEntryParser(com.feilong.lib.net.ftp.FTPClientConfig);
  public com.feilong.lib.net.ftp.FTPFile parseFTPEntry(java.lang.String);
}
```

## `com.feilong.lib.net.ftp.parser.NTFTPEntryParser`

```java
public class com.feilong.lib.net.ftp.parser.NTFTPEntryParser extends com.feilong.lib.net.ftp.parser.ConfigurableFTPFileEntryParserImpl {
  public com.feilong.lib.net.ftp.parser.NTFTPEntryParser();
  public com.feilong.lib.net.ftp.parser.NTFTPEntryParser(com.feilong.lib.net.ftp.FTPClientConfig);
  public com.feilong.lib.net.ftp.FTPFile parseFTPEntry(java.lang.String);
  public com.feilong.lib.net.ftp.FTPClientConfig getDefaultConfiguration();
}
```

## `com.feilong.lib.net.ftp.parser.NetwareFTPEntryParser`

```java
public class com.feilong.lib.net.ftp.parser.NetwareFTPEntryParser extends com.feilong.lib.net.ftp.parser.ConfigurableFTPFileEntryParserImpl {
  public com.feilong.lib.net.ftp.parser.NetwareFTPEntryParser();
  public com.feilong.lib.net.ftp.parser.NetwareFTPEntryParser(com.feilong.lib.net.ftp.FTPClientConfig);
  public com.feilong.lib.net.ftp.FTPFile parseFTPEntry(java.lang.String);
}
```

## `com.feilong.lib.net.ftp.parser.OS2FTPEntryParser`

```java
public class com.feilong.lib.net.ftp.parser.OS2FTPEntryParser extends com.feilong.lib.net.ftp.parser.ConfigurableFTPFileEntryParserImpl {
  public com.feilong.lib.net.ftp.parser.OS2FTPEntryParser();
  public com.feilong.lib.net.ftp.parser.OS2FTPEntryParser(com.feilong.lib.net.ftp.FTPClientConfig);
  public com.feilong.lib.net.ftp.FTPFile parseFTPEntry(java.lang.String);
}
```

## `com.feilong.lib.net.ftp.parser.OS400FTPEntryParser`

```java
public class com.feilong.lib.net.ftp.parser.OS400FTPEntryParser extends com.feilong.lib.net.ftp.parser.ConfigurableFTPFileEntryParserImpl {
  public com.feilong.lib.net.ftp.parser.OS400FTPEntryParser();
  public com.feilong.lib.net.ftp.parser.OS400FTPEntryParser(com.feilong.lib.net.ftp.FTPClientConfig);
  public com.feilong.lib.net.ftp.FTPFile parseFTPEntry(java.lang.String);
}
```

## `com.feilong.lib.net.ftp.parser.ParserInitializationException`

```java
public class com.feilong.lib.net.ftp.parser.ParserInitializationException extends java.lang.RuntimeException {
  public com.feilong.lib.net.ftp.parser.ParserInitializationException(java.lang.String);
  public com.feilong.lib.net.ftp.parser.ParserInitializationException(java.lang.String, java.lang.Throwable);
  public java.lang.Throwable getRootCause();
}
```

## `com.feilong.lib.net.ftp.parser.RegexFTPFileEntryParserImpl`

```java
public abstract class com.feilong.lib.net.ftp.parser.RegexFTPFileEntryParserImpl extends com.feilong.lib.net.ftp.FTPFileEntryParserImpl {
  public com.feilong.lib.net.ftp.parser.RegexFTPFileEntryParserImpl(java.lang.String);
  public com.feilong.lib.net.ftp.parser.RegexFTPFileEntryParserImpl(java.lang.String, int);
  public boolean matches(java.lang.String);
  public int getGroupCnt();
  public java.lang.String group(int);
  public java.lang.String getGroupsAsString();
  public boolean setRegex(java.lang.String);
  public boolean setRegex(java.lang.String, int);
}
```

## `com.feilong.lib.net.ftp.parser.UnixFTPEntryParser`

```java
public class com.feilong.lib.net.ftp.parser.UnixFTPEntryParser extends com.feilong.lib.net.ftp.parser.ConfigurableFTPFileEntryParserImpl {
  public com.feilong.lib.net.ftp.parser.UnixFTPEntryParser();
  public com.feilong.lib.net.ftp.parser.UnixFTPEntryParser(com.feilong.lib.net.ftp.FTPClientConfig);
  public com.feilong.lib.net.ftp.parser.UnixFTPEntryParser(com.feilong.lib.net.ftp.FTPClientConfig, boolean);
  public java.util.List<java.lang.String> preParse(java.util.List<java.lang.String>);
  public com.feilong.lib.net.ftp.FTPFile parseFTPEntry(java.lang.String);
}
```

## `com.feilong.lib.net.ftp.parser.VMSFTPEntryParser`

```java
public class com.feilong.lib.net.ftp.parser.VMSFTPEntryParser extends com.feilong.lib.net.ftp.parser.ConfigurableFTPFileEntryParserImpl {
  public com.feilong.lib.net.ftp.parser.VMSFTPEntryParser();
  public com.feilong.lib.net.ftp.parser.VMSFTPEntryParser(com.feilong.lib.net.ftp.FTPClientConfig);
  public com.feilong.lib.net.ftp.FTPFile parseFTPEntry(java.lang.String);
  public java.lang.String readNextEntry(java.io.BufferedReader) throws java.io.IOException;
  public com.feilong.lib.net.ftp.FTPFile[] parseFileList(java.io.InputStream) throws java.io.IOException;
}
```

## `com.feilong.lib.net.ftp.parser.VMSVersioningFTPEntryParser`

```java
public class com.feilong.lib.net.ftp.parser.VMSVersioningFTPEntryParser extends com.feilong.lib.net.ftp.parser.VMSFTPEntryParser {
  public com.feilong.lib.net.ftp.parser.VMSVersioningFTPEntryParser();
  public com.feilong.lib.net.ftp.parser.VMSVersioningFTPEntryParser(com.feilong.lib.net.ftp.FTPClientConfig);
  public java.util.List<java.lang.String> preParse(java.util.List<java.lang.String>);
}
```
