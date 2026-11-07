# cn.hutool.http.webservice

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.http.webservice.JakartaSoapClient`

```java
public class cn.hutool.http.webservice.JakartaSoapClient extends cn.hutool.http.HttpBase<cn.hutool.http.webservice.JakartaSoapClient> {
  public static cn.hutool.http.webservice.JakartaSoapClient create(java.lang.String);
  public static cn.hutool.http.webservice.JakartaSoapClient create(java.lang.String, cn.hutool.http.webservice.SoapProtocol);
  public static cn.hutool.http.webservice.JakartaSoapClient create(java.lang.String, cn.hutool.http.webservice.SoapProtocol, java.lang.String);
  public cn.hutool.http.webservice.JakartaSoapClient(java.lang.String);
  public cn.hutool.http.webservice.JakartaSoapClient(java.lang.String, cn.hutool.http.webservice.SoapProtocol);
  public cn.hutool.http.webservice.JakartaSoapClient(java.lang.String, cn.hutool.http.webservice.SoapProtocol, java.lang.String);
  public cn.hutool.http.webservice.JakartaSoapClient init(cn.hutool.http.webservice.SoapProtocol);
  public cn.hutool.http.webservice.JakartaSoapClient reset();
  public cn.hutool.http.webservice.JakartaSoapClient setCharset(java.nio.charset.Charset);
  public cn.hutool.http.webservice.JakartaSoapClient charset(java.nio.charset.Charset);
  public cn.hutool.http.webservice.JakartaSoapClient setUrl(java.lang.String);
  public jakarta.xml.soap.SOAPHeaderElement addSOAPHeader(javax.xml.namespace.QName, java.lang.String, java.lang.String, java.lang.Boolean, java.lang.Boolean);
  public jakarta.xml.soap.SOAPHeaderElement addSOAPHeader(java.lang.String);
  public jakarta.xml.soap.SOAPHeaderElement addSOAPHeader(java.lang.String, java.lang.String);
  public jakarta.xml.soap.SOAPHeaderElement addSOAPHeader(javax.xml.namespace.QName);
  public cn.hutool.http.webservice.JakartaSoapClient setMethod(jakarta.xml.soap.Name, java.util.Map<java.lang.String, java.lang.Object>, boolean);
  public cn.hutool.http.webservice.JakartaSoapClient setMethod(javax.xml.namespace.QName, java.util.Map<java.lang.String, java.lang.Object>, boolean);
  public cn.hutool.http.webservice.JakartaSoapClient setMethod(java.lang.String);
  public cn.hutool.http.webservice.JakartaSoapClient setMethod(java.lang.String, java.lang.String);
  public cn.hutool.http.webservice.JakartaSoapClient setMethod(javax.xml.namespace.QName);
  public cn.hutool.http.webservice.JakartaSoapClient setParam(java.lang.String, java.lang.Object);
  public cn.hutool.http.webservice.JakartaSoapClient setParam(java.lang.String, java.lang.Object, boolean);
  public cn.hutool.http.webservice.JakartaSoapClient setParams(java.util.Map<java.lang.String, java.lang.Object>);
  public cn.hutool.http.webservice.JakartaSoapClient setParams(java.util.Map<java.lang.String, java.lang.Object>, boolean);
  public jakarta.xml.soap.SOAPBodyElement getMethodEle();
  public jakarta.xml.soap.SOAPMessage getMessage();
  public java.lang.String getMsgStr(boolean);
  public cn.hutool.http.webservice.JakartaSoapClient write(java.io.OutputStream);
  public cn.hutool.http.webservice.JakartaSoapClient timeout(int);
  public cn.hutool.http.webservice.JakartaSoapClient setConnectionTimeout(int);
  public cn.hutool.http.webservice.JakartaSoapClient setReadTimeout(int);
  public jakarta.xml.soap.SOAPMessage sendForMessage();
  public java.lang.String send();
  public java.lang.String send(boolean);
  public cn.hutool.http.HttpResponse sendForResponse();
  public java.lang.Object charset(java.nio.charset.Charset);
}
```

## `cn.hutool.http.webservice.JakartaSoapProtocol`

```java
public final class cn.hutool.http.webservice.JakartaSoapProtocol extends java.lang.Enum<cn.hutool.http.webservice.JakartaSoapProtocol> {
  public static cn.hutool.http.webservice.JakartaSoapProtocol[] values();
  public static cn.hutool.http.webservice.JakartaSoapProtocol valueOf(java.lang.String);
  public java.lang.String getValue();
}
```

## `cn.hutool.http.webservice.JakartaSoapUtil`

```java
public class cn.hutool.http.webservice.JakartaSoapUtil {
  public cn.hutool.http.webservice.JakartaSoapUtil();
  public static cn.hutool.http.webservice.SoapClient createClient(java.lang.String);
  public static cn.hutool.http.webservice.SoapClient createClient(java.lang.String, cn.hutool.http.webservice.SoapProtocol);
  public static cn.hutool.http.webservice.SoapClient createClient(java.lang.String, cn.hutool.http.webservice.SoapProtocol, java.lang.String);
  public static java.lang.String toString(jakarta.xml.soap.SOAPMessage, boolean);
  public static java.lang.String toString(jakarta.xml.soap.SOAPMessage, boolean, java.nio.charset.Charset);
}
```

## `cn.hutool.http.webservice.SoapClient`

```java
public class cn.hutool.http.webservice.SoapClient extends cn.hutool.http.HttpBase<cn.hutool.http.webservice.SoapClient> {
  public static cn.hutool.http.webservice.SoapClient create(java.lang.String);
  public static cn.hutool.http.webservice.SoapClient create(java.lang.String, cn.hutool.http.webservice.SoapProtocol);
  public static cn.hutool.http.webservice.SoapClient create(java.lang.String, cn.hutool.http.webservice.SoapProtocol, java.lang.String);
  public cn.hutool.http.webservice.SoapClient(java.lang.String);
  public cn.hutool.http.webservice.SoapClient(java.lang.String, cn.hutool.http.webservice.SoapProtocol);
  public cn.hutool.http.webservice.SoapClient(java.lang.String, cn.hutool.http.webservice.SoapProtocol, java.lang.String);
  public cn.hutool.http.webservice.SoapClient init(cn.hutool.http.webservice.SoapProtocol);
  public cn.hutool.http.webservice.SoapClient reset();
  public cn.hutool.http.webservice.SoapClient setCharset(java.nio.charset.Charset);
  public cn.hutool.http.webservice.SoapClient charset(java.nio.charset.Charset);
  public cn.hutool.http.webservice.SoapClient setUrl(java.lang.String);
  public javax.xml.soap.SOAPHeaderElement addSOAPHeader(javax.xml.namespace.QName, java.lang.String, java.lang.String, java.lang.Boolean, java.lang.Boolean);
  public javax.xml.soap.SOAPHeaderElement addSOAPHeader(java.lang.String);
  public javax.xml.soap.SOAPHeaderElement addSOAPHeader(java.lang.String, java.lang.String);
  public javax.xml.soap.SOAPHeaderElement addSOAPHeader(javax.xml.namespace.QName);
  public cn.hutool.http.webservice.SoapClient setMethod(javax.xml.soap.Name, java.util.Map<java.lang.String, java.lang.Object>, boolean);
  public cn.hutool.http.webservice.SoapClient setMethod(javax.xml.namespace.QName, java.util.Map<java.lang.String, java.lang.Object>, boolean);
  public cn.hutool.http.webservice.SoapClient setMethod(java.lang.String);
  public cn.hutool.http.webservice.SoapClient setMethod(java.lang.String, java.lang.String);
  public cn.hutool.http.webservice.SoapClient setMethod(javax.xml.namespace.QName);
  public cn.hutool.http.webservice.SoapClient setParam(java.lang.String, java.lang.Object);
  public cn.hutool.http.webservice.SoapClient setParam(java.lang.String, java.lang.Object, boolean);
  public cn.hutool.http.webservice.SoapClient setParams(java.util.Map<java.lang.String, java.lang.Object>);
  public cn.hutool.http.webservice.SoapClient setParams(java.util.Map<java.lang.String, java.lang.Object>, boolean);
  public javax.xml.soap.SOAPBodyElement getMethodEle();
  public javax.xml.soap.SOAPMessage getMessage();
  public java.lang.String getMsgStr(boolean);
  public cn.hutool.http.webservice.SoapClient write(java.io.OutputStream);
  public cn.hutool.http.webservice.SoapClient timeout(int);
  public cn.hutool.http.webservice.SoapClient setConnectionTimeout(int);
  public cn.hutool.http.webservice.SoapClient setReadTimeout(int);
  public javax.xml.soap.SOAPMessage sendForMessage();
  public java.lang.String send();
  public java.lang.String send(boolean);
  public cn.hutool.http.HttpResponse sendForResponse();
  public java.lang.Object charset(java.nio.charset.Charset);
}
```

## `cn.hutool.http.webservice.SoapProtocol`

```java
public final class cn.hutool.http.webservice.SoapProtocol extends java.lang.Enum<cn.hutool.http.webservice.SoapProtocol> {
  public static cn.hutool.http.webservice.SoapProtocol[] values();
  public static cn.hutool.http.webservice.SoapProtocol valueOf(java.lang.String);
  public java.lang.String getValue();
}
```

## `cn.hutool.http.webservice.SoapRuntimeException`

```java
public class cn.hutool.http.webservice.SoapRuntimeException extends java.lang.RuntimeException {
  public cn.hutool.http.webservice.SoapRuntimeException(java.lang.Throwable);
  public cn.hutool.http.webservice.SoapRuntimeException(java.lang.String);
  public cn.hutool.http.webservice.SoapRuntimeException(java.lang.String, java.lang.Object...);
  public cn.hutool.http.webservice.SoapRuntimeException(java.lang.String, java.lang.Throwable);
  public cn.hutool.http.webservice.SoapRuntimeException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.http.webservice.SoapUtil`

```java
public class cn.hutool.http.webservice.SoapUtil {
  public cn.hutool.http.webservice.SoapUtil();
  public static cn.hutool.http.webservice.SoapClient createClient(java.lang.String);
  public static cn.hutool.http.webservice.SoapClient createClient(java.lang.String, cn.hutool.http.webservice.SoapProtocol);
  public static cn.hutool.http.webservice.SoapClient createClient(java.lang.String, cn.hutool.http.webservice.SoapProtocol, java.lang.String);
  public static java.lang.String toString(javax.xml.soap.SOAPMessage, boolean);
  public static java.lang.String toString(javax.xml.soap.SOAPMessage, boolean, java.nio.charset.Charset);
}
```
