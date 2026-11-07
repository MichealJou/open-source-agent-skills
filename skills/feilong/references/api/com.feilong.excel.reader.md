# com.feilong.excel.reader

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.excel.reader.ReadStatus`

```java
public class com.feilong.excel.reader.ReadStatus {
  public com.feilong.excel.reader.ReadStatus();
  public com.feilong.excel.reader.ReadStatus(int, java.lang.String);
  public com.feilong.excel.reader.ReadStatus(int, java.lang.String, java.util.List<java.lang.Exception>);
  public int getStatus();
  public void setStatus(int);
  public java.lang.String getMessage();
  public void setMessage(java.lang.String);
  public java.util.List<java.lang.Exception> getExceptions();
  public void setExceptions(java.util.List<java.lang.Exception>);
  public void addException(java.lang.Exception);
}
```

## `com.feilong.excel.reader.SheetReader`

```java
public class com.feilong.excel.reader.SheetReader {
  public static void readSheet(org.apache.poi.ss.usermodel.Workbook, int, com.feilong.excel.definition.ExcelSheet, com.feilong.lib.excel.ognl.OgnlStack, com.feilong.excel.reader.ReadStatus, boolean);
}
```
