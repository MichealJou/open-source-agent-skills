# cn.hutool.poi.excel.sax

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.poi.excel.sax.AttributeName`

```java
public final class cn.hutool.poi.excel.sax.AttributeName extends java.lang.Enum<cn.hutool.poi.excel.sax.AttributeName> {
  public static cn.hutool.poi.excel.sax.AttributeName[] values();
  public static cn.hutool.poi.excel.sax.AttributeName valueOf(java.lang.String);
  public boolean match(java.lang.String);
  public java.lang.String getValue(org.xml.sax.Attributes);
}
```

## `cn.hutool.poi.excel.sax.CellDataType`

```java
public final class cn.hutool.poi.excel.sax.CellDataType extends java.lang.Enum<cn.hutool.poi.excel.sax.CellDataType> {
  public static cn.hutool.poi.excel.sax.CellDataType[] values();
  public static cn.hutool.poi.excel.sax.CellDataType valueOf(java.lang.String);
  public java.lang.String getName();
  public static cn.hutool.poi.excel.sax.CellDataType of(java.lang.String);
}
```

## `cn.hutool.poi.excel.sax.ElementName`

```java
public final class cn.hutool.poi.excel.sax.ElementName extends java.lang.Enum<cn.hutool.poi.excel.sax.ElementName> {
  public static cn.hutool.poi.excel.sax.ElementName[] values();
  public static cn.hutool.poi.excel.sax.ElementName valueOf(java.lang.String);
  public boolean match(java.lang.String);
  public static cn.hutool.poi.excel.sax.ElementName of(java.lang.String);
}
```

## `cn.hutool.poi.excel.sax.Excel03SaxReader`

```java
public class cn.hutool.poi.excel.sax.Excel03SaxReader implements org.apache.poi.hssf.eventusermodel.HSSFListener, cn.hutool.poi.excel.sax.ExcelSaxReader<cn.hutool.poi.excel.sax.Excel03SaxReader> {
  public cn.hutool.poi.excel.sax.Excel03SaxReader(cn.hutool.poi.excel.sax.handler.RowHandler);
  public cn.hutool.poi.excel.sax.Excel03SaxReader read(java.io.File, java.lang.String) throws cn.hutool.poi.exceptions.POIException;
  public cn.hutool.poi.excel.sax.Excel03SaxReader read(java.io.InputStream, java.lang.String) throws cn.hutool.poi.exceptions.POIException;
  public cn.hutool.poi.excel.sax.Excel03SaxReader read(org.apache.poi.poifs.filesystem.POIFSFileSystem, java.lang.String) throws cn.hutool.poi.exceptions.POIException;
  public int getSheetIndex();
  public java.lang.String getSheetName();
  public void processRecord(org.apache.poi.hssf.record.Record);
  public java.lang.Object read(java.io.InputStream, java.lang.String) throws cn.hutool.poi.exceptions.POIException;
  public java.lang.Object read(java.io.File, java.lang.String) throws cn.hutool.poi.exceptions.POIException;
}
```

## `cn.hutool.poi.excel.sax.Excel07SaxReader`

```java
public class cn.hutool.poi.excel.sax.Excel07SaxReader implements cn.hutool.poi.excel.sax.ExcelSaxReader<cn.hutool.poi.excel.sax.Excel07SaxReader> {
  public cn.hutool.poi.excel.sax.Excel07SaxReader(cn.hutool.poi.excel.sax.handler.RowHandler);
  public cn.hutool.poi.excel.sax.Excel07SaxReader setRowHandler(cn.hutool.poi.excel.sax.handler.RowHandler);
  public cn.hutool.poi.excel.sax.Excel07SaxReader read(java.io.File, int) throws cn.hutool.poi.exceptions.POIException;
  public cn.hutool.poi.excel.sax.Excel07SaxReader read(java.io.File, java.lang.String) throws cn.hutool.poi.exceptions.POIException;
  public cn.hutool.poi.excel.sax.Excel07SaxReader read(java.io.InputStream, int) throws cn.hutool.poi.exceptions.POIException;
  public cn.hutool.poi.excel.sax.Excel07SaxReader read(java.io.InputStream, java.lang.String) throws cn.hutool.poi.exceptions.POIException;
  public cn.hutool.poi.excel.sax.Excel07SaxReader read(org.apache.poi.openxml4j.opc.OPCPackage, int) throws cn.hutool.poi.exceptions.POIException;
  public cn.hutool.poi.excel.sax.Excel07SaxReader read(org.apache.poi.openxml4j.opc.OPCPackage, java.lang.String) throws cn.hutool.poi.exceptions.POIException;
  public cn.hutool.poi.excel.sax.Excel07SaxReader read(org.apache.poi.xssf.eventusermodel.XSSFReader, java.lang.String) throws cn.hutool.poi.exceptions.POIException;
  public java.lang.Object read(java.io.InputStream, int) throws cn.hutool.poi.exceptions.POIException;
  public java.lang.Object read(java.io.File, int) throws cn.hutool.poi.exceptions.POIException;
  public java.lang.Object read(java.io.InputStream, java.lang.String) throws cn.hutool.poi.exceptions.POIException;
  public java.lang.Object read(java.io.File, java.lang.String) throws cn.hutool.poi.exceptions.POIException;
}
```

## `cn.hutool.poi.excel.sax.ExcelSaxReader`

```java
public interface cn.hutool.poi.excel.sax.ExcelSaxReader<T> {
  public abstract T read(java.io.File, java.lang.String) throws cn.hutool.poi.exceptions.POIException;
  public abstract T read(java.io.InputStream, java.lang.String) throws cn.hutool.poi.exceptions.POIException;
  public default T read(java.lang.String) throws cn.hutool.poi.exceptions.POIException;
  public default T read(java.io.File) throws cn.hutool.poi.exceptions.POIException;
  public default T read(java.io.InputStream) throws cn.hutool.poi.exceptions.POIException;
  public default T read(java.lang.String, int) throws cn.hutool.poi.exceptions.POIException;
  public default T read(java.lang.String, java.lang.String) throws cn.hutool.poi.exceptions.POIException;
  public default T read(java.io.File, int) throws cn.hutool.poi.exceptions.POIException;
  public default T read(java.io.InputStream, int) throws cn.hutool.poi.exceptions.POIException;
}
```

## `cn.hutool.poi.excel.sax.ExcelSaxUtil`

```java
public class cn.hutool.poi.excel.sax.ExcelSaxUtil {
  public cn.hutool.poi.excel.sax.ExcelSaxUtil();
  public static cn.hutool.poi.excel.sax.ExcelSaxReader<?> createSaxReader(boolean, cn.hutool.poi.excel.sax.handler.RowHandler);
  public static java.lang.Object getDataValue(cn.hutool.poi.excel.sax.CellDataType, java.lang.String, org.apache.poi.xssf.model.SharedStrings, java.lang.String);
  public static java.lang.String formatCellContent(java.lang.String, int, java.lang.String);
  public static int countNullCell(java.lang.String, java.lang.String);
  public static void readFrom(java.io.InputStream, org.xml.sax.ContentHandler) throws cn.hutool.core.exceptions.DependencyException, cn.hutool.poi.exceptions.POIException, cn.hutool.core.io.IORuntimeException;
  public static boolean isDateFormat(org.apache.poi.hssf.record.CellValueRecordInterface, org.apache.poi.hssf.eventusermodel.FormatTrackingHSSFListener);
  public static boolean isDateFormat(int, java.lang.String);
  public static cn.hutool.core.date.DateTime getDateValue(java.lang.String);
  public static cn.hutool.core.date.DateTime getDateValue(double);
  public static java.lang.Object getNumberOrDateValue(org.apache.poi.hssf.record.CellValueRecordInterface, double, org.apache.poi.hssf.eventusermodel.FormatTrackingHSSFListener);
}
```

## `cn.hutool.poi.excel.sax.SheetDataSaxHandler`

```java
public class cn.hutool.poi.excel.sax.SheetDataSaxHandler extends org.xml.sax.helpers.DefaultHandler {
  public cn.hutool.poi.excel.sax.SheetDataSaxHandler(cn.hutool.poi.excel.sax.handler.RowHandler);
  public void setRowHandler(cn.hutool.poi.excel.sax.handler.RowHandler);
  public void startElement(java.lang.String, java.lang.String, java.lang.String, org.xml.sax.Attributes);
  public void endElement(java.lang.String, java.lang.String, java.lang.String);
  public void characters(char[], int, int);
}
```

## `cn.hutool.poi.excel.sax.SheetRidReader`

```java
public class cn.hutool.poi.excel.sax.SheetRidReader extends org.xml.sax.helpers.DefaultHandler {
  public cn.hutool.poi.excel.sax.SheetRidReader();
  public static cn.hutool.poi.excel.sax.SheetRidReader parse(org.apache.poi.xssf.eventusermodel.XSSFReader);
  public cn.hutool.poi.excel.sax.SheetRidReader read(org.apache.poi.xssf.eventusermodel.XSSFReader);
  public java.lang.Integer getRidBySheetId(int);
  public java.lang.Integer getRidBySheetIdBase0(int);
  public java.lang.Integer getRidByName(java.lang.String);
  public java.lang.Integer getRidByNameBase0(java.lang.String);
  public java.lang.Integer getRidByIndex(int);
  public java.lang.Integer getRidByIndexBase0(int);
  public java.util.List<java.lang.String> getSheetNames();
  public void startElement(java.lang.String, java.lang.String, java.lang.String, org.xml.sax.Attributes);
}
```

## `cn.hutool.poi.excel.sax.StopReadException`

```java
public class cn.hutool.poi.excel.sax.StopReadException extends cn.hutool.poi.exceptions.POIException {
  public cn.hutool.poi.excel.sax.StopReadException();
  public cn.hutool.poi.excel.sax.StopReadException(java.lang.String);
}
```
