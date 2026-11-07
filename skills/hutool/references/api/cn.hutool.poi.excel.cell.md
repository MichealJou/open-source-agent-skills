# cn.hutool.poi.excel.cell

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.poi.excel.cell.CellEditor`

```java
public interface cn.hutool.poi.excel.cell.CellEditor {
  public abstract java.lang.Object edit(org.apache.poi.ss.usermodel.Cell, java.lang.Object);
}
```

## `cn.hutool.poi.excel.cell.CellHandler`

```java
public interface cn.hutool.poi.excel.cell.CellHandler {
  public abstract void handle(org.apache.poi.ss.usermodel.Cell, java.lang.Object);
}
```

## `cn.hutool.poi.excel.cell.CellLocation`

```java
public class cn.hutool.poi.excel.cell.CellLocation implements java.io.Serializable {
  public cn.hutool.poi.excel.cell.CellLocation(int, int);
  public int getX();
  public void setX(int);
  public int getY();
  public void setY(int);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `cn.hutool.poi.excel.cell.CellSetter`

```java
public interface cn.hutool.poi.excel.cell.CellSetter {
  public abstract void setValue(org.apache.poi.ss.usermodel.Cell);
}
```

## `cn.hutool.poi.excel.cell.CellUtil`

```java
public class cn.hutool.poi.excel.cell.CellUtil {
  public cn.hutool.poi.excel.cell.CellUtil();
  public static java.lang.Object getCellValue(org.apache.poi.ss.usermodel.Cell);
  public static java.lang.Object getCellValue(org.apache.poi.ss.usermodel.Cell, boolean);
  public static java.lang.Object getCellValue(org.apache.poi.ss.usermodel.Cell, cn.hutool.poi.excel.cell.CellEditor);
  public static java.lang.Object getCellValue(org.apache.poi.ss.usermodel.Cell, org.apache.poi.ss.usermodel.CellType, boolean);
  public static java.lang.Object getCellValue(org.apache.poi.ss.usermodel.Cell, org.apache.poi.ss.usermodel.CellType, cn.hutool.poi.excel.cell.CellEditor);
  public static void setCellValue(org.apache.poi.ss.usermodel.Cell, java.lang.Object, cn.hutool.poi.excel.StyleSet, boolean);
  public static void setCellValue(org.apache.poi.ss.usermodel.Cell, java.lang.Object, org.apache.poi.ss.usermodel.CellStyle);
  public static void setCellValue(org.apache.poi.ss.usermodel.Cell, java.lang.Object);
  public static org.apache.poi.ss.usermodel.Cell getCell(org.apache.poi.ss.usermodel.Row, int);
  public static org.apache.poi.ss.usermodel.Cell getOrCreateCell(org.apache.poi.ss.usermodel.Row, int);
  public static boolean isMergedRegion(org.apache.poi.ss.usermodel.Sheet, java.lang.String);
  public static boolean isMergedRegion(org.apache.poi.ss.usermodel.Cell);
  public static boolean isMergedRegion(org.apache.poi.ss.usermodel.Sheet, int, int);
  public static org.apache.poi.ss.util.CellRangeAddress getCellRangeAddress(org.apache.poi.ss.usermodel.Sheet, java.lang.String);
  public static org.apache.poi.ss.util.CellRangeAddress getCellRangeAddress(org.apache.poi.ss.usermodel.Cell);
  public static org.apache.poi.ss.util.CellRangeAddress getCellRangeAddress(org.apache.poi.ss.usermodel.Sheet, int, int);
  public static void setMergedRegionStyle(org.apache.poi.ss.usermodel.Cell, org.apache.poi.ss.usermodel.CellStyle);
  public static int mergingCells(org.apache.poi.ss.usermodel.Sheet, int, int, int, int);
  public static int mergingCells(org.apache.poi.ss.usermodel.Sheet, int, int, int, int, org.apache.poi.ss.usermodel.CellStyle);
  public static java.lang.Object getMergedRegionValue(org.apache.poi.ss.usermodel.Sheet, java.lang.String);
  public static java.lang.Object getMergedRegionValue(org.apache.poi.ss.usermodel.Sheet, int, int);
  public static org.apache.poi.ss.usermodel.Cell getMergedRegionCell(org.apache.poi.ss.usermodel.Cell);
  public static org.apache.poi.ss.usermodel.Cell getMergedRegionCell(org.apache.poi.ss.usermodel.Sheet, int, int);
  public static void setComment(org.apache.poi.ss.usermodel.Cell, java.lang.String, java.lang.String, org.apache.poi.ss.usermodel.ClientAnchor);
}
```

## `cn.hutool.poi.excel.cell.CellValue`

```java
public interface cn.hutool.poi.excel.cell.CellValue<T> {
  public abstract T getValue();
}
```

## `cn.hutool.poi.excel.cell.FormulaCellValue`

```java
public class cn.hutool.poi.excel.cell.FormulaCellValue implements cn.hutool.poi.excel.cell.CellValue<java.lang.String>, cn.hutool.poi.excel.cell.CellSetter {
  public cn.hutool.poi.excel.cell.FormulaCellValue(java.lang.String);
  public cn.hutool.poi.excel.cell.FormulaCellValue(java.lang.String, java.lang.Object);
  public java.lang.String getValue();
  public void setValue(org.apache.poi.ss.usermodel.Cell);
  public java.lang.Object getResult();
  public java.lang.String toString();
  public java.lang.Object getValue();
}
```

## `cn.hutool.poi.excel.cell.NullCell`

```java
public class cn.hutool.poi.excel.cell.NullCell implements org.apache.poi.ss.usermodel.Cell {
  public cn.hutool.poi.excel.cell.NullCell(org.apache.poi.ss.usermodel.Row, int);
  public int getColumnIndex();
  public int getRowIndex();
  public org.apache.poi.ss.usermodel.Sheet getSheet();
  public org.apache.poi.ss.usermodel.Row getRow();
  public void setCellType(org.apache.poi.ss.usermodel.CellType);
  public void setBlank();
  public org.apache.poi.ss.usermodel.CellType getCellType();
  public org.apache.poi.ss.usermodel.CellType getCellTypeEnum();
  public org.apache.poi.ss.usermodel.CellType getCachedFormulaResultType();
  public org.apache.poi.ss.usermodel.CellType getCachedFormulaResultTypeEnum();
  public void setCellValue(double);
  public void setCellValue(java.util.Date);
  public void setCellValue(java.time.LocalDateTime);
  public void setCellValue(java.util.Calendar);
  public void setCellValue(org.apache.poi.ss.usermodel.RichTextString);
  public void setCellValue(java.lang.String);
  public void setCellFormula(java.lang.String) throws org.apache.poi.ss.formula.FormulaParseException, java.lang.IllegalStateException;
  public void removeFormula() throws java.lang.IllegalStateException;
  public java.lang.String getCellFormula();
  public double getNumericCellValue();
  public java.util.Date getDateCellValue();
  public java.time.LocalDateTime getLocalDateTimeCellValue();
  public org.apache.poi.ss.usermodel.RichTextString getRichStringCellValue();
  public java.lang.String getStringCellValue();
  public void setCellValue(boolean);
  public void setCellErrorValue(byte);
  public boolean getBooleanCellValue();
  public byte getErrorCellValue();
  public void setCellStyle(org.apache.poi.ss.usermodel.CellStyle);
  public org.apache.poi.ss.usermodel.CellStyle getCellStyle();
  public void setAsActiveCell();
  public org.apache.poi.ss.util.CellAddress getAddress();
  public void setCellComment(org.apache.poi.ss.usermodel.Comment);
  public org.apache.poi.ss.usermodel.Comment getCellComment();
  public void removeCellComment();
  public org.apache.poi.ss.usermodel.Hyperlink getHyperlink();
  public void setHyperlink(org.apache.poi.ss.usermodel.Hyperlink);
  public void removeHyperlink();
  public org.apache.poi.ss.util.CellRangeAddress getArrayFormulaRange();
  public boolean isPartOfArrayFormulaGroup();
}
```
