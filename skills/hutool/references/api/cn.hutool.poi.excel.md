# cn.hutool.poi.excel

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.poi.excel.BigExcelWriter`

```java
public class cn.hutool.poi.excel.BigExcelWriter extends cn.hutool.poi.excel.ExcelWriter {
  public cn.hutool.poi.excel.BigExcelWriter();
  public cn.hutool.poi.excel.BigExcelWriter(int);
  public cn.hutool.poi.excel.BigExcelWriter(int, boolean, boolean, java.lang.String);
  public cn.hutool.poi.excel.BigExcelWriter(java.lang.String);
  public cn.hutool.poi.excel.BigExcelWriter(int, java.lang.String);
  public cn.hutool.poi.excel.BigExcelWriter(java.lang.String, java.lang.String);
  public cn.hutool.poi.excel.BigExcelWriter(java.io.File);
  public cn.hutool.poi.excel.BigExcelWriter(java.io.File, java.lang.String);
  public cn.hutool.poi.excel.BigExcelWriter(org.apache.poi.xssf.streaming.SXSSFWorkbook, java.lang.String);
  public cn.hutool.poi.excel.BigExcelWriter(org.apache.poi.ss.usermodel.Sheet);
  public cn.hutool.poi.excel.BigExcelWriter autoSizeColumn(int);
  public cn.hutool.poi.excel.BigExcelWriter autoSizeColumnAll();
  public cn.hutool.poi.excel.BigExcelWriter autoSizeColumnAll(float);
  public cn.hutool.poi.excel.ExcelWriter flush(java.io.OutputStream, boolean) throws cn.hutool.core.io.IORuntimeException;
  public void close();
  public cn.hutool.poi.excel.ExcelWriter autoSizeColumn(int);
  public cn.hutool.poi.excel.ExcelWriter autoSizeColumnAll(float);
  public cn.hutool.poi.excel.ExcelWriter autoSizeColumnAll();
}
```

## `cn.hutool.poi.excel.ExcelBase`

```java
public class cn.hutool.poi.excel.ExcelBase<T extends cn.hutool.poi.excel.ExcelBase<T>> implements java.io.Closeable {
  public cn.hutool.poi.excel.ExcelBase(org.apache.poi.ss.usermodel.Sheet);
  public org.apache.poi.ss.usermodel.Workbook getWorkbook();
  public int getSheetCount();
  public java.util.List<org.apache.poi.ss.usermodel.Sheet> getSheets();
  public java.util.List<java.lang.String> getSheetNames();
  public org.apache.poi.ss.usermodel.Sheet getSheet();
  public T renameSheet(java.lang.String);
  public T setSheet(java.lang.String);
  public T setSheet(int);
  public T setSheet(org.apache.poi.ss.usermodel.Sheet);
  public T cloneSheet(int, java.lang.String, boolean);
  public org.apache.poi.ss.usermodel.Cell getCell(java.lang.String);
  public org.apache.poi.ss.usermodel.Cell getCell(int, int);
  public org.apache.poi.ss.usermodel.Cell getOrCreateCell(java.lang.String);
  public org.apache.poi.ss.usermodel.Cell getOrCreateCell(int, int);
  public org.apache.poi.ss.usermodel.Cell getCell(java.lang.String, boolean);
  public org.apache.poi.ss.usermodel.Cell getCell(int, int, boolean);
  public org.apache.poi.ss.usermodel.Row getOrCreateRow(int);
  public org.apache.poi.ss.usermodel.CellStyle getOrCreateCellStyle(java.lang.String);
  public org.apache.poi.ss.usermodel.CellStyle getOrCreateCellStyle(int, int);
  public org.apache.poi.ss.usermodel.CellStyle createCellStyle(java.lang.String);
  public org.apache.poi.ss.usermodel.CellStyle createCellStyle(int, int);
  public org.apache.poi.ss.usermodel.CellStyle createCellStyle();
  public org.apache.poi.ss.usermodel.CellStyle getOrCreateRowStyle(int);
  public org.apache.poi.ss.usermodel.CellStyle createRowStyle(int);
  public org.apache.poi.ss.usermodel.CellStyle getOrCreateColumnStyle(int);
  public org.apache.poi.ss.usermodel.CellStyle createColumnStyle(int);
  public org.apache.poi.ss.usermodel.Hyperlink createHyperlink(org.apache.poi.common.usermodel.HyperlinkType, java.lang.String);
  public org.apache.poi.ss.usermodel.Hyperlink createHyperlink(org.apache.poi.common.usermodel.HyperlinkType, java.lang.String, java.lang.String);
  public int getRowCount();
  public int getPhysicalRowCount();
  public int getColumnCount();
  public int getColumnCount(int);
  public boolean isXlsx();
  public void close();
  public java.util.Map<java.lang.String, java.lang.String> getHeaderAlias();
  public T setHeaderAlias(java.util.Map<java.lang.String, java.lang.String>);
  public T addHeaderAlias(java.lang.String, java.lang.String);
  public T removeHeaderAlias(java.lang.String);
  public T clearHeaderAlias();
}
```

## `cn.hutool.poi.excel.ExcelDateUtil`

```java
public class cn.hutool.poi.excel.ExcelDateUtil {
  public cn.hutool.poi.excel.ExcelDateUtil();
  public static boolean isDateFormat(org.apache.poi.ss.usermodel.Cell);
  public static boolean isDateFormat(org.apache.poi.ss.usermodel.Cell, org.apache.poi.ss.formula.ConditionalFormattingEvaluator);
  public static boolean isDateFormat(org.apache.poi.ss.usermodel.ExcelNumberFormat);
  public static boolean isDateFormat(int, java.lang.String);
}
```

## `cn.hutool.poi.excel.ExcelExtractorUtil`

```java
public class cn.hutool.poi.excel.ExcelExtractorUtil {
  public cn.hutool.poi.excel.ExcelExtractorUtil();
  public static org.apache.poi.ss.extractor.ExcelExtractor getExtractor(org.apache.poi.ss.usermodel.Workbook);
  public static java.lang.String readAsText(org.apache.poi.ss.usermodel.Workbook, boolean);
}
```

## `cn.hutool.poi.excel.ExcelFileUtil`

```java
public class cn.hutool.poi.excel.ExcelFileUtil {
  public cn.hutool.poi.excel.ExcelFileUtil();
  public static boolean isXls(java.io.InputStream);
  public static boolean isXlsx(java.io.InputStream);
  public static boolean isXlsx(java.io.File);
}
```

## `cn.hutool.poi.excel.ExcelPicUtil`

```java
public class cn.hutool.poi.excel.ExcelPicUtil {
  public cn.hutool.poi.excel.ExcelPicUtil();
  public static java.util.Map<java.lang.String, org.apache.poi.ss.usermodel.PictureData> getPicMap(org.apache.poi.ss.usermodel.Workbook, int);
}
```

## `cn.hutool.poi.excel.ExcelReader`

```java
public class cn.hutool.poi.excel.ExcelReader extends cn.hutool.poi.excel.ExcelBase<cn.hutool.poi.excel.ExcelReader> {
  public cn.hutool.poi.excel.ExcelReader(java.lang.String, int);
  public cn.hutool.poi.excel.ExcelReader(java.lang.String, java.lang.String);
  public cn.hutool.poi.excel.ExcelReader(java.io.File, int);
  public cn.hutool.poi.excel.ExcelReader(java.io.File, java.lang.String);
  public cn.hutool.poi.excel.ExcelReader(java.io.InputStream, int);
  public cn.hutool.poi.excel.ExcelReader(java.io.InputStream, java.lang.String);
  public cn.hutool.poi.excel.ExcelReader(org.apache.poi.ss.usermodel.Workbook, int);
  public cn.hutool.poi.excel.ExcelReader(org.apache.poi.ss.usermodel.Workbook, java.lang.String);
  public cn.hutool.poi.excel.ExcelReader(org.apache.poi.ss.usermodel.Sheet);
  public boolean isIgnoreEmptyRow();
  public cn.hutool.poi.excel.ExcelReader setIgnoreEmptyRow(boolean);
  public cn.hutool.poi.excel.ExcelReader setCellEditor(cn.hutool.poi.excel.cell.CellEditor);
  public java.util.List<java.util.List<java.lang.Object>> read();
  public java.util.List<java.util.List<java.lang.Object>> read(int);
  public java.util.List<java.util.List<java.lang.Object>> read(int, int);
  public java.util.List<java.util.List<java.lang.Object>> read(int, int, boolean);
  public java.util.List<java.lang.Object> readColumn(int, int);
  public java.util.List<java.lang.Object> readColumn(int, int, int);
  public void read(cn.hutool.poi.excel.cell.CellHandler);
  public void read(int, int, cn.hutool.poi.excel.cell.CellHandler);
  public java.util.List<java.util.Map<java.lang.String, java.lang.Object>> readAll();
  public java.util.List<java.util.Map<java.lang.String, java.lang.Object>> read(int, int, int);
  public <T> java.util.List<T> readAll(java.lang.Class<T>);
  public <T> java.util.List<T> read(int, int, java.lang.Class<T>);
  public <T> java.util.List<T> read(int, int, int, java.lang.Class<T>);
  public <T> T read(cn.hutool.poi.excel.reader.SheetReader<T>);
  public java.lang.String readAsText(boolean);
  public org.apache.poi.ss.extractor.ExcelExtractor getExtractor();
  public java.util.List<java.lang.Object> readRow(int);
  public java.lang.Object readCellValue(int, int);
  public cn.hutool.poi.excel.ExcelWriter getWriter();
}
```

## `cn.hutool.poi.excel.ExcelUtil`

```java
public class cn.hutool.poi.excel.ExcelUtil {
  public cn.hutool.poi.excel.ExcelUtil();
  public static void readBySax(java.lang.String, int, cn.hutool.poi.excel.sax.handler.RowHandler);
  public static void readBySax(java.lang.String, java.lang.String, cn.hutool.poi.excel.sax.handler.RowHandler);
  public static void readBySax(java.io.File, int, cn.hutool.poi.excel.sax.handler.RowHandler);
  public static void readBySax(java.io.File, java.lang.String, cn.hutool.poi.excel.sax.handler.RowHandler);
  public static void readBySax(java.io.InputStream, int, cn.hutool.poi.excel.sax.handler.RowHandler);
  public static void readBySax(java.io.InputStream, java.lang.String, cn.hutool.poi.excel.sax.handler.RowHandler);
  public static cn.hutool.poi.excel.ExcelReader getReader(java.lang.String);
  public static cn.hutool.poi.excel.ExcelReader getReader(java.io.File);
  public static cn.hutool.poi.excel.ExcelReader getReader(java.lang.String, int);
  public static cn.hutool.poi.excel.ExcelReader getReader(java.lang.String, java.lang.String);
  public static cn.hutool.poi.excel.ExcelReader getReader(java.io.File, int);
  public static cn.hutool.poi.excel.ExcelReader getReader(java.io.File, java.lang.String);
  public static cn.hutool.poi.excel.ExcelReader getReader(java.io.InputStream);
  public static cn.hutool.poi.excel.ExcelReader getReader(java.io.InputStream, int);
  public static cn.hutool.poi.excel.ExcelReader getReader(java.io.InputStream, java.lang.String);
  public static cn.hutool.poi.excel.ExcelWriter getWriter();
  public static cn.hutool.poi.excel.ExcelWriter getWriter(boolean);
  public static cn.hutool.poi.excel.ExcelWriter getWriter(java.lang.String);
  public static cn.hutool.poi.excel.ExcelWriter getWriterWithSheet(java.lang.String);
  public static cn.hutool.poi.excel.ExcelWriter getWriter(java.io.File);
  public static cn.hutool.poi.excel.ExcelWriter getWriter(java.lang.String, java.lang.String);
  public static cn.hutool.poi.excel.ExcelWriter getWriter(java.io.File, java.lang.String);
  public static cn.hutool.poi.excel.BigExcelWriter getBigWriter();
  public static cn.hutool.poi.excel.BigExcelWriter getBigWriter(int);
  public static cn.hutool.poi.excel.BigExcelWriter getBigWriter(java.lang.String);
  public static cn.hutool.poi.excel.BigExcelWriter getBigWriter(java.io.File);
  public static cn.hutool.poi.excel.BigExcelWriter getBigWriter(java.lang.String, java.lang.String);
  public static cn.hutool.poi.excel.BigExcelWriter getBigWriter(java.io.File, java.lang.String);
  public static java.lang.String indexToColName(int);
  public static int colNameToIndex(java.lang.String);
  public static cn.hutool.poi.excel.cell.CellLocation toLocation(java.lang.String);
}
```

## `cn.hutool.poi.excel.ExcelWriter`

```java
public class cn.hutool.poi.excel.ExcelWriter extends cn.hutool.poi.excel.ExcelBase<cn.hutool.poi.excel.ExcelWriter> {
  public cn.hutool.poi.excel.ExcelWriter();
  public cn.hutool.poi.excel.ExcelWriter(boolean);
  public cn.hutool.poi.excel.ExcelWriter(java.lang.String);
  public cn.hutool.poi.excel.ExcelWriter(boolean, java.lang.String);
  public cn.hutool.poi.excel.ExcelWriter(java.lang.String, java.lang.String);
  public cn.hutool.poi.excel.ExcelWriter(java.io.File);
  public cn.hutool.poi.excel.ExcelWriter(java.io.File, java.lang.String);
  public cn.hutool.poi.excel.ExcelWriter(org.apache.poi.ss.usermodel.Workbook, java.lang.String);
  public cn.hutool.poi.excel.ExcelWriter(org.apache.poi.ss.usermodel.Sheet);
  public cn.hutool.poi.excel.ExcelWriter setSheet(int);
  public cn.hutool.poi.excel.ExcelWriter setSheet(java.lang.String);
  public cn.hutool.poi.excel.ExcelWriter reset();
  public cn.hutool.poi.excel.ExcelWriter renameSheet(java.lang.String);
  public cn.hutool.poi.excel.ExcelWriter renameSheet(int, java.lang.String);
  public cn.hutool.poi.excel.ExcelWriter autoSizeColumnAll();
  public cn.hutool.poi.excel.ExcelWriter autoSizeColumnAll(float);
  public cn.hutool.poi.excel.ExcelWriter autoSizeColumn(int);
  public cn.hutool.poi.excel.ExcelWriter autoSizeColumn(int, boolean);
  public cn.hutool.poi.excel.ExcelWriter autoSizeColumn(int, float);
  public cn.hutool.poi.excel.ExcelWriter autoSizeColumn(int, boolean, float);
  public cn.hutool.poi.excel.ExcelWriter disableDefaultStyle();
  public cn.hutool.poi.excel.ExcelWriter setStyleSet(cn.hutool.poi.excel.StyleSet);
  public cn.hutool.poi.excel.StyleSet getStyleSet();
  public org.apache.poi.ss.usermodel.CellStyle getHeadCellStyle();
  public org.apache.poi.ss.usermodel.CellStyle getCellStyle();
  public int getCurrentRow();
  public java.lang.String getDisposition(java.lang.String, java.nio.charset.Charset);
  public java.lang.String getContentType();
  public cn.hutool.poi.excel.ExcelWriter setCurrentRow(int);
  public cn.hutool.poi.excel.ExcelWriter setCurrentRowToEnd();
  public cn.hutool.poi.excel.ExcelWriter passCurrentRow();
  public cn.hutool.poi.excel.ExcelWriter passRows(int);
  public cn.hutool.poi.excel.ExcelWriter resetRow();
  public cn.hutool.poi.excel.ExcelWriter setDestFile(java.io.File);
  public cn.hutool.poi.excel.ExcelWriter setHeaderAlias(java.util.Map<java.lang.String, java.lang.String>);
  public cn.hutool.poi.excel.ExcelWriter clearHeaderAlias();
  public cn.hutool.poi.excel.ExcelWriter addHeaderAlias(java.lang.String, java.lang.String);
  public cn.hutool.poi.excel.ExcelWriter setOnlyAlias(boolean);
  public cn.hutool.poi.excel.ExcelWriter setFreezePane(int);
  public cn.hutool.poi.excel.ExcelWriter setFreezePane(int, int);
  public cn.hutool.poi.excel.ExcelWriter setColumnWidth(int, int);
  public cn.hutool.poi.excel.ExcelWriter setDefaultRowHeight(int);
  public cn.hutool.poi.excel.ExcelWriter setRowHeight(int, int);
  public cn.hutool.poi.excel.ExcelWriter setHeaderOrFooter(java.lang.String, cn.hutool.poi.excel.style.Align, boolean);
  public cn.hutool.poi.excel.ExcelWriter addIgnoredErrors(org.apache.poi.ss.util.CellRangeAddress, org.apache.poi.ss.usermodel.IgnoredErrorType...) throws java.lang.UnsupportedOperationException;
  public cn.hutool.poi.excel.ExcelWriter addSelect(int, int, java.lang.String...);
  public cn.hutool.poi.excel.ExcelWriter addSelect(org.apache.poi.ss.util.CellRangeAddressList, java.lang.String...);
  public cn.hutool.poi.excel.ExcelWriter addValidationData(org.apache.poi.ss.usermodel.DataValidation);
  public cn.hutool.poi.excel.ExcelWriter merge(int);
  public cn.hutool.poi.excel.ExcelWriter merge(int, java.lang.Object);
  public cn.hutool.poi.excel.ExcelWriter merge(int, java.lang.Object, boolean);
  public cn.hutool.poi.excel.ExcelWriter merge(int, int, int, int, java.lang.Object, boolean);
  public cn.hutool.poi.excel.ExcelWriter merge(int, int, int, int, java.lang.Object, org.apache.poi.ss.usermodel.CellStyle);
  public cn.hutool.poi.excel.ExcelWriter write(java.lang.Iterable<?>);
  public cn.hutool.poi.excel.ExcelWriter write(java.lang.Iterable<?>, boolean);
  public cn.hutool.poi.excel.ExcelWriter write(java.lang.Iterable<?>, java.util.Comparator<java.lang.String>);
  public cn.hutool.poi.excel.ExcelWriter writeImg(java.io.File, int, int, int, int);
  public cn.hutool.poi.excel.ExcelWriter writeImg(java.io.File, int, int, int, int, int, int, int, int);
  public cn.hutool.poi.excel.ExcelWriter writeImg(java.io.File, int, int, int, int, int, int, int, int, int);
  public cn.hutool.poi.excel.ExcelWriter writeImg(byte[], int, int, int, int, int, int, int, int, int);
  public cn.hutool.poi.excel.ExcelWriter writeHeadRow(java.lang.Iterable<?>);
  public cn.hutool.poi.excel.ExcelWriter writeSecHeadRow(java.lang.Iterable<?>);
  public cn.hutool.poi.excel.ExcelWriter writeRow(java.lang.Object, boolean);
  public cn.hutool.poi.excel.ExcelWriter writeRow(java.util.Map<?, ?>, boolean);
  public cn.hutool.poi.excel.ExcelWriter writeRow(java.lang.Iterable<?>);
  public cn.hutool.poi.excel.ExcelWriter writeCol(java.util.Map<?, ? extends java.lang.Iterable<?>>, boolean);
  public cn.hutool.poi.excel.ExcelWriter writeCol(java.util.Map<?, ? extends java.lang.Iterable<?>>, int, boolean);
  public cn.hutool.poi.excel.ExcelWriter writeCol(java.lang.Object, java.lang.Iterable<?>, boolean);
  public cn.hutool.poi.excel.ExcelWriter writeCol(java.lang.Object, int, java.lang.Iterable<?>, boolean);
  public cn.hutool.poi.excel.ExcelWriter writeCellValue(java.lang.String, java.lang.Object);
  public cn.hutool.poi.excel.ExcelWriter writeCellValue(java.lang.String, java.lang.Object, boolean);
  public cn.hutool.poi.excel.ExcelWriter writeCellValue(int, int, java.lang.Object);
  public cn.hutool.poi.excel.ExcelWriter writeCellValue(int, int, java.lang.Object, boolean);
  public cn.hutool.poi.excel.ExcelWriter setStyle(org.apache.poi.ss.usermodel.CellStyle, java.lang.String);
  public cn.hutool.poi.excel.ExcelWriter setStyle(org.apache.poi.ss.usermodel.CellStyle, int, int);
  public cn.hutool.poi.excel.ExcelWriter setRowStyle(int, org.apache.poi.ss.usermodel.CellStyle);
  public cn.hutool.poi.excel.ExcelWriter setRowStyleIfHasData(int, org.apache.poi.ss.usermodel.CellStyle);
  public cn.hutool.poi.excel.ExcelWriter setColumnStyle(int, org.apache.poi.ss.usermodel.CellStyle);
  public cn.hutool.poi.excel.ExcelWriter setColumnStyleIfHasData(int, int, org.apache.poi.ss.usermodel.CellStyle);
  public org.apache.poi.ss.usermodel.Font createFont();
  public cn.hutool.poi.excel.ExcelWriter flush() throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.poi.excel.ExcelWriter flush(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.poi.excel.ExcelWriter flush(java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.poi.excel.ExcelWriter flush(java.io.OutputStream, boolean) throws cn.hutool.core.io.IORuntimeException;
  public void close();
  public cn.hutool.poi.excel.ExcelBase clearHeaderAlias();
  public cn.hutool.poi.excel.ExcelBase addHeaderAlias(java.lang.String, java.lang.String);
  public cn.hutool.poi.excel.ExcelBase setHeaderAlias(java.util.Map);
  public cn.hutool.poi.excel.ExcelBase setSheet(int);
  public cn.hutool.poi.excel.ExcelBase setSheet(java.lang.String);
  public cn.hutool.poi.excel.ExcelBase renameSheet(java.lang.String);
}
```

## `cn.hutool.poi.excel.RowUtil`

```java
public class cn.hutool.poi.excel.RowUtil {
  public cn.hutool.poi.excel.RowUtil();
  public static org.apache.poi.ss.usermodel.Row getOrCreateRow(org.apache.poi.ss.usermodel.Sheet, int);
  public static java.util.List<java.lang.Object> readRow(org.apache.poi.ss.usermodel.Row, cn.hutool.poi.excel.cell.CellEditor);
  public static java.util.List<java.lang.Object> readRow(org.apache.poi.ss.usermodel.Row, int, int, cn.hutool.poi.excel.cell.CellEditor);
  public static void writeRow(org.apache.poi.ss.usermodel.Row, java.lang.Iterable<?>);
  public static void writeRow(org.apache.poi.ss.usermodel.Row, java.lang.Iterable<?>, cn.hutool.poi.excel.StyleSet, boolean);
  public static void insertRow(org.apache.poi.ss.usermodel.Sheet, int, int);
  public static void removeRow(org.apache.poi.ss.usermodel.Row);
}
```

## `cn.hutool.poi.excel.StyleSet`

```java
public class cn.hutool.poi.excel.StyleSet implements java.io.Serializable {
  public cn.hutool.poi.excel.StyleSet(org.apache.poi.ss.usermodel.Workbook);
  public org.apache.poi.ss.usermodel.CellStyle getHeadCellStyle();
  public org.apache.poi.ss.usermodel.CellStyle getCellStyle();
  public org.apache.poi.ss.usermodel.CellStyle getCellStyleForNumber();
  public org.apache.poi.ss.usermodel.CellStyle getCellStyleForDate();
  public org.apache.poi.ss.usermodel.CellStyle getCellStyleForHyperlink();
  public cn.hutool.poi.excel.StyleSet setBorder(org.apache.poi.ss.usermodel.BorderStyle, org.apache.poi.ss.usermodel.IndexedColors);
  public cn.hutool.poi.excel.StyleSet setAlign(org.apache.poi.ss.usermodel.HorizontalAlignment, org.apache.poi.ss.usermodel.VerticalAlignment);
  public cn.hutool.poi.excel.StyleSet setBackgroundColor(org.apache.poi.ss.usermodel.IndexedColors, boolean);
  public cn.hutool.poi.excel.StyleSet setFont(short, short, java.lang.String, boolean);
  public cn.hutool.poi.excel.StyleSet setFont(org.apache.poi.ss.usermodel.Font, boolean);
  public cn.hutool.poi.excel.StyleSet setWrapText();
  public org.apache.poi.ss.usermodel.CellStyle getStyleByValueType(java.lang.Object, boolean);
}
```

## `cn.hutool.poi.excel.WorkbookUtil`

```java
public class cn.hutool.poi.excel.WorkbookUtil {
  public cn.hutool.poi.excel.WorkbookUtil();
  public static org.apache.poi.ss.usermodel.Workbook createBook(java.lang.String);
  public static org.apache.poi.ss.usermodel.Workbook createBook(java.lang.String, boolean);
  public static org.apache.poi.ss.usermodel.Workbook createBook(java.io.File);
  public static org.apache.poi.ss.usermodel.Workbook createBook(java.io.File, boolean);
  public static org.apache.poi.ss.usermodel.Workbook createBookForWriter(java.io.File);
  public static org.apache.poi.ss.usermodel.Workbook createBook(java.io.File, java.lang.String);
  public static org.apache.poi.ss.usermodel.Workbook createBook(java.io.File, java.lang.String, boolean);
  public static org.apache.poi.ss.usermodel.Workbook createBook(java.io.InputStream);
  public static org.apache.poi.ss.usermodel.Workbook createBook(java.io.InputStream, java.lang.String);
  public static org.apache.poi.ss.usermodel.Workbook createBook(boolean);
  public static org.apache.poi.xssf.streaming.SXSSFWorkbook createSXSSFBook(java.lang.String);
  public static org.apache.poi.xssf.streaming.SXSSFWorkbook createSXSSFBook(java.lang.String, boolean);
  public static org.apache.poi.xssf.streaming.SXSSFWorkbook createSXSSFBook(java.io.File);
  public static org.apache.poi.xssf.streaming.SXSSFWorkbook createSXSSFBook(java.io.File, boolean);
  public static org.apache.poi.xssf.streaming.SXSSFWorkbook createSXSSFBook(java.io.File, java.lang.String);
  public static org.apache.poi.xssf.streaming.SXSSFWorkbook createSXSSFBook(java.io.File, java.lang.String, boolean);
  public static org.apache.poi.xssf.streaming.SXSSFWorkbook createSXSSFBook(java.io.InputStream);
  public static org.apache.poi.xssf.streaming.SXSSFWorkbook createSXSSFBook(java.io.InputStream, java.lang.String);
  public static org.apache.poi.xssf.streaming.SXSSFWorkbook createSXSSFBook();
  public static org.apache.poi.xssf.streaming.SXSSFWorkbook createSXSSFBook(int);
  public static org.apache.poi.xssf.streaming.SXSSFWorkbook createSXSSFBook(int, boolean, boolean);
  public static void writeBook(org.apache.poi.ss.usermodel.Workbook, java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static org.apache.poi.ss.usermodel.Sheet getOrCreateSheet(org.apache.poi.ss.usermodel.Workbook, java.lang.String);
  public static org.apache.poi.ss.usermodel.Sheet getOrCreateSheet(org.apache.poi.ss.usermodel.Workbook, int);
  public static boolean isEmpty(org.apache.poi.ss.usermodel.Sheet);
}
```
