# cn.hutool.poi.excel.style

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.poi.excel.style.Align`

```java
public final class cn.hutool.poi.excel.style.Align extends java.lang.Enum<cn.hutool.poi.excel.style.Align> {
  public static cn.hutool.poi.excel.style.Align[] values();
  public static cn.hutool.poi.excel.style.Align valueOf(java.lang.String);
}
```

## `cn.hutool.poi.excel.style.StyleUtil`

```java
public class cn.hutool.poi.excel.style.StyleUtil {
  public cn.hutool.poi.excel.style.StyleUtil();
  public static org.apache.poi.ss.usermodel.CellStyle cloneCellStyle(org.apache.poi.ss.usermodel.Cell, org.apache.poi.ss.usermodel.CellStyle);
  public static org.apache.poi.ss.usermodel.CellStyle cloneCellStyle(org.apache.poi.ss.usermodel.Workbook, org.apache.poi.ss.usermodel.CellStyle);
  public static org.apache.poi.ss.usermodel.CellStyle setAlign(org.apache.poi.ss.usermodel.CellStyle, org.apache.poi.ss.usermodel.HorizontalAlignment, org.apache.poi.ss.usermodel.VerticalAlignment);
  public static org.apache.poi.ss.usermodel.CellStyle setBorder(org.apache.poi.ss.usermodel.CellStyle, org.apache.poi.ss.usermodel.BorderStyle, org.apache.poi.ss.usermodel.IndexedColors);
  public static org.apache.poi.ss.usermodel.CellStyle setColor(org.apache.poi.ss.usermodel.CellStyle, org.apache.poi.ss.usermodel.IndexedColors, org.apache.poi.ss.usermodel.FillPatternType);
  public static org.apache.poi.ss.usermodel.CellStyle setColor(org.apache.poi.ss.usermodel.CellStyle, short, org.apache.poi.ss.usermodel.FillPatternType);
  public static org.apache.poi.ss.usermodel.Font createFont(org.apache.poi.ss.usermodel.Workbook, short, short, java.lang.String);
  public static org.apache.poi.ss.usermodel.Font setFontStyle(org.apache.poi.ss.usermodel.Font, short, short, java.lang.String);
  public static org.apache.poi.ss.usermodel.CellStyle createCellStyle(org.apache.poi.ss.usermodel.Workbook);
  public static org.apache.poi.ss.usermodel.CellStyle createDefaultCellStyle(org.apache.poi.ss.usermodel.Workbook);
  public static org.apache.poi.ss.usermodel.CellStyle createHeadCellStyle(org.apache.poi.ss.usermodel.Workbook);
  public static boolean isNullOrDefaultStyle(org.apache.poi.ss.usermodel.Workbook, org.apache.poi.ss.usermodel.CellStyle);
  public static java.lang.Short getFormat(org.apache.poi.ss.usermodel.Workbook, java.lang.String);
}
```
