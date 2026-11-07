# com.feilong.lib.org.apache.http.message

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.org.apache.http.message.AbstractHttpMessage`

```java
public abstract class com.feilong.lib.org.apache.http.message.AbstractHttpMessage implements com.feilong.lib.org.apache.http.HttpMessage {
  public boolean containsHeader(java.lang.String);
  public com.feilong.lib.org.apache.http.Header[] getHeaders(java.lang.String);
  public com.feilong.lib.org.apache.http.Header getFirstHeader(java.lang.String);
  public com.feilong.lib.org.apache.http.Header getLastHeader(java.lang.String);
  public com.feilong.lib.org.apache.http.Header[] getAllHeaders();
  public void addHeader(com.feilong.lib.org.apache.http.Header);
  public void addHeader(java.lang.String, java.lang.String);
  public void setHeader(com.feilong.lib.org.apache.http.Header);
  public void setHeader(java.lang.String, java.lang.String);
  public void setHeaders(com.feilong.lib.org.apache.http.Header[]);
  public void removeHeader(com.feilong.lib.org.apache.http.Header);
  public void removeHeaders(java.lang.String);
  public com.feilong.lib.org.apache.http.HeaderIterator headerIterator();
  public com.feilong.lib.org.apache.http.HeaderIterator headerIterator(java.lang.String);
}
```

## `com.feilong.lib.org.apache.http.message.BasicHeader`

```java
public class com.feilong.lib.org.apache.http.message.BasicHeader implements com.feilong.lib.org.apache.http.Header,java.lang.Cloneable,java.io.Serializable {
  public com.feilong.lib.org.apache.http.message.BasicHeader(java.lang.String, java.lang.String);
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
  public com.feilong.lib.org.apache.http.HeaderElement[] getElements() throws com.feilong.lib.org.apache.http.ParseException;
  public java.lang.String getName();
  public java.lang.String getValue();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.message.BasicHeaderElement`

```java
public class com.feilong.lib.org.apache.http.message.BasicHeaderElement implements com.feilong.lib.org.apache.http.HeaderElement,java.lang.Cloneable {
  public com.feilong.lib.org.apache.http.message.BasicHeaderElement(java.lang.String, java.lang.String, com.feilong.lib.org.apache.http.NameValuePair[]);
  public com.feilong.lib.org.apache.http.message.BasicHeaderElement(java.lang.String, java.lang.String);
  public java.lang.String getName();
  public java.lang.String getValue();
  public com.feilong.lib.org.apache.http.NameValuePair[] getParameters();
  public int getParameterCount();
  public com.feilong.lib.org.apache.http.NameValuePair getParameter(int);
  public com.feilong.lib.org.apache.http.NameValuePair getParameterByName(java.lang.String);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.message.BasicHeaderElementIterator`

```java
public class com.feilong.lib.org.apache.http.message.BasicHeaderElementIterator implements com.feilong.lib.org.apache.http.HeaderElementIterator {
  public com.feilong.lib.org.apache.http.message.BasicHeaderElementIterator(com.feilong.lib.org.apache.http.HeaderIterator, com.feilong.lib.org.apache.http.message.HeaderValueParser);
  public com.feilong.lib.org.apache.http.message.BasicHeaderElementIterator(com.feilong.lib.org.apache.http.HeaderIterator);
  public boolean hasNext();
  public com.feilong.lib.org.apache.http.HeaderElement nextElement() throws java.util.NoSuchElementException;
  public final java.lang.Object next() throws java.util.NoSuchElementException;
  public void remove() throws java.lang.UnsupportedOperationException;
}
```

## `com.feilong.lib.org.apache.http.message.BasicHeaderIterator`

```java
public class com.feilong.lib.org.apache.http.message.BasicHeaderIterator implements com.feilong.lib.org.apache.http.HeaderIterator {
  public com.feilong.lib.org.apache.http.message.BasicHeaderIterator(com.feilong.lib.org.apache.http.Header[], java.lang.String);
  public boolean hasNext();
  public com.feilong.lib.org.apache.http.Header nextHeader() throws java.util.NoSuchElementException;
  public final java.lang.Object next() throws java.util.NoSuchElementException;
  public void remove() throws java.lang.UnsupportedOperationException;
}
```

## `com.feilong.lib.org.apache.http.message.BasicHeaderValueFormatter`

```java
public class com.feilong.lib.org.apache.http.message.BasicHeaderValueFormatter implements com.feilong.lib.org.apache.http.message.HeaderValueFormatter {
  public com.feilong.lib.org.apache.http.message.BasicHeaderValueFormatter();
  public static java.lang.String formatElements(com.feilong.lib.org.apache.http.HeaderElement[], boolean, com.feilong.lib.org.apache.http.message.HeaderValueFormatter);
  public com.feilong.lib.org.apache.http.util.CharArrayBuffer formatElements(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.HeaderElement[], boolean);
  public static java.lang.String formatHeaderElement(com.feilong.lib.org.apache.http.HeaderElement, boolean, com.feilong.lib.org.apache.http.message.HeaderValueFormatter);
  public com.feilong.lib.org.apache.http.util.CharArrayBuffer formatHeaderElement(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.HeaderElement, boolean);
  public static java.lang.String formatParameters(com.feilong.lib.org.apache.http.NameValuePair[], boolean, com.feilong.lib.org.apache.http.message.HeaderValueFormatter);
  public com.feilong.lib.org.apache.http.util.CharArrayBuffer formatParameters(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.NameValuePair[], boolean);
  public static java.lang.String formatNameValuePair(com.feilong.lib.org.apache.http.NameValuePair, boolean, com.feilong.lib.org.apache.http.message.HeaderValueFormatter);
  public com.feilong.lib.org.apache.http.util.CharArrayBuffer formatNameValuePair(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.NameValuePair, boolean);
}
```

## `com.feilong.lib.org.apache.http.message.BasicHeaderValueParser`

```java
public class com.feilong.lib.org.apache.http.message.BasicHeaderValueParser implements com.feilong.lib.org.apache.http.message.HeaderValueParser {
  public com.feilong.lib.org.apache.http.message.BasicHeaderValueParser();
  public static com.feilong.lib.org.apache.http.HeaderElement[] parseElements(java.lang.String, com.feilong.lib.org.apache.http.message.HeaderValueParser) throws com.feilong.lib.org.apache.http.ParseException;
  public com.feilong.lib.org.apache.http.HeaderElement[] parseElements(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor);
  public static com.feilong.lib.org.apache.http.HeaderElement parseHeaderElement(java.lang.String, com.feilong.lib.org.apache.http.message.HeaderValueParser) throws com.feilong.lib.org.apache.http.ParseException;
  public com.feilong.lib.org.apache.http.HeaderElement parseHeaderElement(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor);
  public static com.feilong.lib.org.apache.http.NameValuePair[] parseParameters(java.lang.String, com.feilong.lib.org.apache.http.message.HeaderValueParser) throws com.feilong.lib.org.apache.http.ParseException;
  public com.feilong.lib.org.apache.http.NameValuePair[] parseParameters(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor);
  public static com.feilong.lib.org.apache.http.NameValuePair parseNameValuePair(java.lang.String, com.feilong.lib.org.apache.http.message.HeaderValueParser) throws com.feilong.lib.org.apache.http.ParseException;
  public com.feilong.lib.org.apache.http.NameValuePair parseNameValuePair(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor);
  public com.feilong.lib.org.apache.http.NameValuePair parseNameValuePair(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor, char[]);
}
```

## `com.feilong.lib.org.apache.http.message.BasicHttpEntityEnclosingRequest`

```java
public class com.feilong.lib.org.apache.http.message.BasicHttpEntityEnclosingRequest extends com.feilong.lib.org.apache.http.message.BasicHttpRequest implements com.feilong.lib.org.apache.http.HttpEntityEnclosingRequest {
  public com.feilong.lib.org.apache.http.message.BasicHttpEntityEnclosingRequest(java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.message.BasicHttpEntityEnclosingRequest(java.lang.String, java.lang.String, com.feilong.lib.org.apache.http.ProtocolVersion);
  public com.feilong.lib.org.apache.http.message.BasicHttpEntityEnclosingRequest(com.feilong.lib.org.apache.http.RequestLine);
  public com.feilong.lib.org.apache.http.HttpEntity getEntity();
  public void setEntity(com.feilong.lib.org.apache.http.HttpEntity);
  public boolean expectContinue();
}
```

## `com.feilong.lib.org.apache.http.message.BasicHttpRequest`

```java
public class com.feilong.lib.org.apache.http.message.BasicHttpRequest extends com.feilong.lib.org.apache.http.message.AbstractHttpMessage implements com.feilong.lib.org.apache.http.HttpRequest {
  public com.feilong.lib.org.apache.http.message.BasicHttpRequest(java.lang.String, java.lang.String);
  public com.feilong.lib.org.apache.http.message.BasicHttpRequest(java.lang.String, java.lang.String, com.feilong.lib.org.apache.http.ProtocolVersion);
  public com.feilong.lib.org.apache.http.message.BasicHttpRequest(com.feilong.lib.org.apache.http.RequestLine);
  public com.feilong.lib.org.apache.http.ProtocolVersion getProtocolVersion();
  public com.feilong.lib.org.apache.http.RequestLine getRequestLine();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.message.BasicHttpResponse`

```java
public class com.feilong.lib.org.apache.http.message.BasicHttpResponse extends com.feilong.lib.org.apache.http.message.AbstractHttpMessage implements com.feilong.lib.org.apache.http.HttpResponse {
  public com.feilong.lib.org.apache.http.message.BasicHttpResponse(com.feilong.lib.org.apache.http.StatusLine, com.feilong.lib.org.apache.http.ReasonPhraseCatalog, java.util.Locale);
  public com.feilong.lib.org.apache.http.message.BasicHttpResponse(com.feilong.lib.org.apache.http.StatusLine);
  public com.feilong.lib.org.apache.http.message.BasicHttpResponse(com.feilong.lib.org.apache.http.ProtocolVersion, int, java.lang.String);
  public com.feilong.lib.org.apache.http.ProtocolVersion getProtocolVersion();
  public com.feilong.lib.org.apache.http.StatusLine getStatusLine();
  public com.feilong.lib.org.apache.http.HttpEntity getEntity();
  public java.util.Locale getLocale();
  public void setStatusLine(com.feilong.lib.org.apache.http.StatusLine);
  public void setStatusLine(com.feilong.lib.org.apache.http.ProtocolVersion, int);
  public void setStatusLine(com.feilong.lib.org.apache.http.ProtocolVersion, int, java.lang.String);
  public void setStatusCode(int);
  public void setReasonPhrase(java.lang.String);
  public void setEntity(com.feilong.lib.org.apache.http.HttpEntity);
  public void setLocale(java.util.Locale);
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.message.BasicLineFormatter`

```java
public class com.feilong.lib.org.apache.http.message.BasicLineFormatter implements com.feilong.lib.org.apache.http.message.LineFormatter {
  public com.feilong.lib.org.apache.http.message.BasicLineFormatter();
  public static java.lang.String formatProtocolVersion(com.feilong.lib.org.apache.http.ProtocolVersion, com.feilong.lib.org.apache.http.message.LineFormatter);
  public com.feilong.lib.org.apache.http.util.CharArrayBuffer appendProtocolVersion(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.ProtocolVersion);
  public static java.lang.String formatRequestLine(com.feilong.lib.org.apache.http.RequestLine, com.feilong.lib.org.apache.http.message.LineFormatter);
  public com.feilong.lib.org.apache.http.util.CharArrayBuffer formatRequestLine(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.RequestLine);
  public static java.lang.String formatStatusLine(com.feilong.lib.org.apache.http.StatusLine, com.feilong.lib.org.apache.http.message.LineFormatter);
  public com.feilong.lib.org.apache.http.util.CharArrayBuffer formatStatusLine(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.StatusLine);
  public static java.lang.String formatHeader(com.feilong.lib.org.apache.http.Header, com.feilong.lib.org.apache.http.message.LineFormatter);
  public com.feilong.lib.org.apache.http.util.CharArrayBuffer formatHeader(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.Header);
}
```

## `com.feilong.lib.org.apache.http.message.BasicLineParser`

```java
public class com.feilong.lib.org.apache.http.message.BasicLineParser implements com.feilong.lib.org.apache.http.message.LineParser {
  public com.feilong.lib.org.apache.http.message.BasicLineParser(com.feilong.lib.org.apache.http.ProtocolVersion);
  public com.feilong.lib.org.apache.http.message.BasicLineParser();
  public static com.feilong.lib.org.apache.http.ProtocolVersion parseProtocolVersion(java.lang.String, com.feilong.lib.org.apache.http.message.LineParser) throws com.feilong.lib.org.apache.http.ParseException;
  public com.feilong.lib.org.apache.http.ProtocolVersion parseProtocolVersion(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor) throws com.feilong.lib.org.apache.http.ParseException;
  public boolean hasProtocolVersion(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor);
  public static com.feilong.lib.org.apache.http.RequestLine parseRequestLine(java.lang.String, com.feilong.lib.org.apache.http.message.LineParser) throws com.feilong.lib.org.apache.http.ParseException;
  public com.feilong.lib.org.apache.http.RequestLine parseRequestLine(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor) throws com.feilong.lib.org.apache.http.ParseException;
  public static com.feilong.lib.org.apache.http.StatusLine parseStatusLine(java.lang.String, com.feilong.lib.org.apache.http.message.LineParser) throws com.feilong.lib.org.apache.http.ParseException;
  public com.feilong.lib.org.apache.http.StatusLine parseStatusLine(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor) throws com.feilong.lib.org.apache.http.ParseException;
  public static com.feilong.lib.org.apache.http.Header parseHeader(java.lang.String, com.feilong.lib.org.apache.http.message.LineParser) throws com.feilong.lib.org.apache.http.ParseException;
  public com.feilong.lib.org.apache.http.Header parseHeader(com.feilong.lib.org.apache.http.util.CharArrayBuffer) throws com.feilong.lib.org.apache.http.ParseException;
}
```

## `com.feilong.lib.org.apache.http.message.BasicListHeaderIterator`

```java
public class com.feilong.lib.org.apache.http.message.BasicListHeaderIterator implements com.feilong.lib.org.apache.http.HeaderIterator {
  public com.feilong.lib.org.apache.http.message.BasicListHeaderIterator(java.util.List<com.feilong.lib.org.apache.http.Header>, java.lang.String);
  public boolean hasNext();
  public com.feilong.lib.org.apache.http.Header nextHeader() throws java.util.NoSuchElementException;
  public final java.lang.Object next() throws java.util.NoSuchElementException;
  public void remove() throws java.lang.UnsupportedOperationException;
}
```

## `com.feilong.lib.org.apache.http.message.BasicNameValuePair`

```java
public class com.feilong.lib.org.apache.http.message.BasicNameValuePair implements com.feilong.lib.org.apache.http.NameValuePair,java.lang.Cloneable,java.io.Serializable {
  public com.feilong.lib.org.apache.http.message.BasicNameValuePair(java.lang.String, java.lang.String);
  public java.lang.String getName();
  public java.lang.String getValue();
  public java.lang.String toString();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.message.BasicRequestLine`

```java
public class com.feilong.lib.org.apache.http.message.BasicRequestLine implements com.feilong.lib.org.apache.http.RequestLine,java.lang.Cloneable,java.io.Serializable {
  public com.feilong.lib.org.apache.http.message.BasicRequestLine(java.lang.String, java.lang.String, com.feilong.lib.org.apache.http.ProtocolVersion);
  public java.lang.String getMethod();
  public com.feilong.lib.org.apache.http.ProtocolVersion getProtocolVersion();
  public java.lang.String getUri();
  public java.lang.String toString();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.message.BasicStatusLine`

```java
public class com.feilong.lib.org.apache.http.message.BasicStatusLine implements com.feilong.lib.org.apache.http.StatusLine,java.lang.Cloneable,java.io.Serializable {
  public com.feilong.lib.org.apache.http.message.BasicStatusLine(com.feilong.lib.org.apache.http.ProtocolVersion, int, java.lang.String);
  public int getStatusCode();
  public com.feilong.lib.org.apache.http.ProtocolVersion getProtocolVersion();
  public java.lang.String getReasonPhrase();
  public java.lang.String toString();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.message.BasicTokenIterator`

```java
public class com.feilong.lib.org.apache.http.message.BasicTokenIterator implements com.feilong.lib.org.apache.http.TokenIterator {
  public com.feilong.lib.org.apache.http.message.BasicTokenIterator(com.feilong.lib.org.apache.http.HeaderIterator);
  public boolean hasNext();
  public java.lang.String nextToken() throws java.util.NoSuchElementException, com.feilong.lib.org.apache.http.ParseException;
  public final java.lang.Object next() throws java.util.NoSuchElementException, com.feilong.lib.org.apache.http.ParseException;
  public final void remove() throws java.lang.UnsupportedOperationException;
}
```

## `com.feilong.lib.org.apache.http.message.BufferedHeader`

```java
public class com.feilong.lib.org.apache.http.message.BufferedHeader implements com.feilong.lib.org.apache.http.FormattedHeader,java.lang.Cloneable,java.io.Serializable {
  public com.feilong.lib.org.apache.http.message.BufferedHeader(com.feilong.lib.org.apache.http.util.CharArrayBuffer) throws com.feilong.lib.org.apache.http.ParseException;
  public java.lang.String getName();
  public java.lang.String getValue();
  public com.feilong.lib.org.apache.http.HeaderElement[] getElements() throws com.feilong.lib.org.apache.http.ParseException;
  public int getValuePos();
  public com.feilong.lib.org.apache.http.util.CharArrayBuffer getBuffer();
  public java.lang.String toString();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `com.feilong.lib.org.apache.http.message.HeaderGroup`

```java
public class com.feilong.lib.org.apache.http.message.HeaderGroup implements java.lang.Cloneable,java.io.Serializable {
  public com.feilong.lib.org.apache.http.message.HeaderGroup();
  public void clear();
  public void addHeader(com.feilong.lib.org.apache.http.Header);
  public void removeHeader(com.feilong.lib.org.apache.http.Header);
  public void updateHeader(com.feilong.lib.org.apache.http.Header);
  public void setHeaders(com.feilong.lib.org.apache.http.Header[]);
  public com.feilong.lib.org.apache.http.Header getCondensedHeader(java.lang.String);
  public com.feilong.lib.org.apache.http.Header[] getHeaders(java.lang.String);
  public com.feilong.lib.org.apache.http.Header getFirstHeader(java.lang.String);
  public com.feilong.lib.org.apache.http.Header getLastHeader(java.lang.String);
  public com.feilong.lib.org.apache.http.Header[] getAllHeaders();
  public boolean containsHeader(java.lang.String);
  public com.feilong.lib.org.apache.http.HeaderIterator iterator();
  public com.feilong.lib.org.apache.http.HeaderIterator iterator(java.lang.String);
  public com.feilong.lib.org.apache.http.message.HeaderGroup copy();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.message.HeaderValueFormatter`

```java
public interface com.feilong.lib.org.apache.http.message.HeaderValueFormatter {
  public abstract com.feilong.lib.org.apache.http.util.CharArrayBuffer formatElements(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.HeaderElement[], boolean);
  public abstract com.feilong.lib.org.apache.http.util.CharArrayBuffer formatHeaderElement(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.HeaderElement, boolean);
  public abstract com.feilong.lib.org.apache.http.util.CharArrayBuffer formatParameters(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.NameValuePair[], boolean);
  public abstract com.feilong.lib.org.apache.http.util.CharArrayBuffer formatNameValuePair(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.NameValuePair, boolean);
}
```

## `com.feilong.lib.org.apache.http.message.HeaderValueParser`

```java
public interface com.feilong.lib.org.apache.http.message.HeaderValueParser {
  public abstract com.feilong.lib.org.apache.http.HeaderElement[] parseElements(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor) throws com.feilong.lib.org.apache.http.ParseException;
  public abstract com.feilong.lib.org.apache.http.HeaderElement parseHeaderElement(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor) throws com.feilong.lib.org.apache.http.ParseException;
  public abstract com.feilong.lib.org.apache.http.NameValuePair[] parseParameters(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor) throws com.feilong.lib.org.apache.http.ParseException;
  public abstract com.feilong.lib.org.apache.http.NameValuePair parseNameValuePair(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor) throws com.feilong.lib.org.apache.http.ParseException;
}
```

## `com.feilong.lib.org.apache.http.message.LineFormatter`

```java
public interface com.feilong.lib.org.apache.http.message.LineFormatter {
  public abstract com.feilong.lib.org.apache.http.util.CharArrayBuffer appendProtocolVersion(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.ProtocolVersion);
  public abstract com.feilong.lib.org.apache.http.util.CharArrayBuffer formatRequestLine(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.RequestLine);
  public abstract com.feilong.lib.org.apache.http.util.CharArrayBuffer formatStatusLine(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.StatusLine);
  public abstract com.feilong.lib.org.apache.http.util.CharArrayBuffer formatHeader(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.Header);
}
```

## `com.feilong.lib.org.apache.http.message.LineParser`

```java
public interface com.feilong.lib.org.apache.http.message.LineParser {
  public abstract com.feilong.lib.org.apache.http.ProtocolVersion parseProtocolVersion(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor) throws com.feilong.lib.org.apache.http.ParseException;
  public abstract boolean hasProtocolVersion(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor);
  public abstract com.feilong.lib.org.apache.http.RequestLine parseRequestLine(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor) throws com.feilong.lib.org.apache.http.ParseException;
  public abstract com.feilong.lib.org.apache.http.StatusLine parseStatusLine(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor) throws com.feilong.lib.org.apache.http.ParseException;
  public abstract com.feilong.lib.org.apache.http.Header parseHeader(com.feilong.lib.org.apache.http.util.CharArrayBuffer) throws com.feilong.lib.org.apache.http.ParseException;
}
```

## `com.feilong.lib.org.apache.http.message.ParserCursor`

```java
public class com.feilong.lib.org.apache.http.message.ParserCursor {
  public com.feilong.lib.org.apache.http.message.ParserCursor(int, int);
  public int getLowerBound();
  public int getUpperBound();
  public int getPos();
  public void updatePos(int);
  public boolean atEnd();
  public java.lang.String toString();
}
```

## `com.feilong.lib.org.apache.http.message.TokenParser`

```java
public class com.feilong.lib.org.apache.http.message.TokenParser {
  public com.feilong.lib.org.apache.http.message.TokenParser();
  public static java.util.BitSet INIT_BITSET(int...);
  public static boolean isWhitespace(char);
  public java.lang.String parseToken(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor, java.util.BitSet);
  public java.lang.String parseValue(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor, java.util.BitSet);
  public void skipWhiteSpace(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor);
  public void copyContent(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor, java.util.BitSet, java.lang.StringBuilder);
  public void copyUnquotedContent(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor, java.util.BitSet, java.lang.StringBuilder);
  public void copyQuotedContent(com.feilong.lib.org.apache.http.util.CharArrayBuffer, com.feilong.lib.org.apache.http.message.ParserCursor, java.lang.StringBuilder);
}
```
