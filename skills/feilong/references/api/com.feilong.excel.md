# com.feilong.excel

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.excel.DataConvertorConfig`

```java
public class com.feilong.excel.DataConvertorConfig implements java.io.Serializable {
  public void registerDataConvertor(com.feilong.lib.excel.convertor.DataConvertor<?>);
  public <T> com.feilong.lib.excel.convertor.DataConvertor<T> getConvertor(java.lang.Class<T>);
  public java.lang.Class<?> getSupportedClass(java.lang.String);
  public static com.feilong.excel.DataConvertorConfig getInstance();
}
```

## `com.feilong.excel.DefaultExcelReader`

```java
public class com.feilong.excel.DefaultExcelReader extends com.feilong.excel.AbstractExcelConfig implements com.feilong.excel.ExcelReader {
  public com.feilong.excel.DefaultExcelReader();
  public com.feilong.excel.DefaultExcelReader(com.feilong.excel.ExcelDefinition);
  public com.feilong.excel.reader.ReadStatus readAll(java.io.InputStream, java.util.Map<java.lang.String, java.lang.Object>);
  public com.feilong.excel.reader.ReadStatus readAllPerSheet(java.io.InputStream, java.util.Map<java.lang.String, java.lang.Object>);
  public com.feilong.excel.reader.ReadStatus readSheet(java.io.InputStream, int, java.util.Map<java.lang.String, java.lang.Object>);
  public void setSkipErrors(boolean);
  public void setDefinition(com.feilong.excel.ExcelDefinition);
  public com.feilong.excel.ExcelDefinition getDefinition();
}
```

## `com.feilong.excel.DefaultExcelWriter`

```java
public class com.feilong.excel.DefaultExcelWriter extends com.feilong.excel.AbstractExcelConfig implements com.feilong.excel.ExcelWriter {
  public com.feilong.excel.DefaultExcelWriter();
  public com.feilong.excel.DefaultExcelWriter(com.feilong.excel.ExcelDefinition);
  public void write(java.lang.String, java.io.OutputStream, java.util.Map<java.lang.String, java.lang.Object>);
  public void write(java.io.OutputStream, java.util.Map<java.lang.String, java.lang.Object>);
  public void writePerSheet(java.lang.String, java.io.OutputStream, java.util.List<java.util.Map<java.lang.String, java.lang.Object>>);
  public void writePerSheet(java.io.OutputStream, java.util.List<java.util.Map<java.lang.String, java.lang.Object>>);
  public void writePerSheet(java.io.InputStream, java.io.OutputStream, java.util.List<java.util.Map<java.lang.String, java.lang.Object>>);
  public void initBufferedTemplate(java.io.InputStream);
  public void setDefinition(com.feilong.excel.ExcelDefinition);
  public com.feilong.excel.ExcelDefinition getDefinition();
}
```

## `com.feilong.excel.ExcelDefinition`

```java
public class com.feilong.excel.ExcelDefinition {
  public com.feilong.excel.ExcelDefinition();
  public java.util.List<com.feilong.excel.definition.ExcelSheet> getExcelSheets();
  public void setExcelSheets(java.util.List<com.feilong.excel.definition.ExcelSheet>);
  public java.lang.Integer getStyleSheetPosition();
  public void setStyleSheetPosition(java.lang.Integer);
  public java.lang.String toString();
}
```

## `com.feilong.excel.ExcelException`

```java
public class com.feilong.excel.ExcelException extends java.lang.RuntimeException {
  public com.feilong.excel.ExcelException(int, int, java.lang.String, java.lang.Object, com.feilong.excel.definition.ExcelCell);
  public int getErrorCode();
  public int getSheetNo();
  public java.lang.String getCellIndex();
  public java.lang.Object getValue();
  public com.feilong.excel.definition.ExcelCell getExcelCell();
  public java.lang.String toString();
}
```

## `com.feilong.excel.ExcelManipulatorFactory`

```java
public class com.feilong.excel.ExcelManipulatorFactory {
  public com.feilong.excel.ExcelManipulatorFactory();
  public void setConfig(java.lang.String...);
  public com.feilong.excel.ExcelWriter createExcelWriter(java.lang.Integer, java.lang.String, java.lang.String...);
  public com.feilong.excel.ExcelReader createExcelReader(java.lang.String...);
  public void setSheetDefinitions(java.util.Map<java.lang.String, com.feilong.excel.definition.ExcelSheet>);
}
```

## `com.feilong.excel.ExcelReader`

```java
public interface com.feilong.excel.ExcelReader extends com.feilong.excel.ExcelConfig {
  public abstract com.feilong.excel.reader.ReadStatus readAll(java.io.InputStream, java.util.Map<java.lang.String, java.lang.Object>);
  public abstract com.feilong.excel.reader.ReadStatus readAllPerSheet(java.io.InputStream, java.util.Map<java.lang.String, java.lang.Object>);
  public abstract com.feilong.excel.reader.ReadStatus readSheet(java.io.InputStream, int, java.util.Map<java.lang.String, java.lang.Object>);
}
```

## `com.feilong.excel.ExcelReaderUtil`

```java
public class com.feilong.excel.ExcelReaderUtil {
  public static <T> java.util.List<T> read(java.lang.String, java.lang.String, java.lang.String, java.lang.String, int);
  public static java.util.Map<java.lang.String, java.lang.Object> readData(java.lang.String, java.lang.String, java.lang.String, int);
}
```

## `com.feilong.excel.ExcelSheetListBuilder`

```java
public class com.feilong.excel.ExcelSheetListBuilder {
  public static com.feilong.lib.digester3.Digester create(java.lang.String);
}
```

## `com.feilong.excel.ExcelWriteUtil`

```java
public class com.feilong.excel.ExcelWriteUtil {
  public static java.lang.String write(java.lang.String, java.lang.String, java.lang.String, java.util.Map<java.lang.String, java.lang.Object>, java.lang.String);
  public static java.lang.String write(java.lang.String, java.lang.String, java.lang.String[], java.util.Map<java.lang.String, java.lang.Object>, java.lang.String);
}
```

## `com.feilong.excel.ExcelWriter`

```java
public interface com.feilong.excel.ExcelWriter extends com.feilong.excel.ExcelConfig {
  public abstract void write(java.io.OutputStream, java.util.Map<java.lang.String, java.lang.Object>);
  public abstract void write(java.lang.String, java.io.OutputStream, java.util.Map<java.lang.String, java.lang.Object>);
  public abstract void writePerSheet(java.io.OutputStream, java.util.List<java.util.Map<java.lang.String, java.lang.Object>>);
  public abstract void writePerSheet(java.lang.String, java.io.OutputStream, java.util.List<java.util.Map<java.lang.String, java.lang.Object>>);
  public abstract void writePerSheet(java.io.InputStream, java.io.OutputStream, java.util.List<java.util.Map<java.lang.String, java.lang.Object>>);
}
```
