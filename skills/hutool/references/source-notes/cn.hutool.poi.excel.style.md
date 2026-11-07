# cn.hutool.poi.excel.style

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.poi.excel.style.StyleUtil` | `CellStyle cloneCellStyle(Cell cell,CellStyle cellStyle)` | 克隆新的CellStyle |
| `cn.hutool.poi.excel.style.StyleUtil` | `CellStyle cloneCellStyle(Workbook workbook,CellStyle cellStyle)` | 克隆新的CellStyle |
| `cn.hutool.poi.excel.style.StyleUtil` | `CellStyle createCellStyle(Workbook workbook)` | 创建单元格样式 |
| `cn.hutool.poi.excel.style.StyleUtil` | `CellStyle createDefaultCellStyle(Workbook workbook)` | 创建默认普通单元格样式 |
| `cn.hutool.poi.excel.style.StyleUtil` | `CellStyle createHeadCellStyle(Workbook workbook)` | 创建默认头部样式 |
| `cn.hutool.poi.excel.style.StyleUtil` | `CellStyle setAlign(CellStyle cellStyle,HorizontalAlignment halign,VerticalAlignment valign)` | 设置cell文本对齐样式 |
| `cn.hutool.poi.excel.style.StyleUtil` | `CellStyle setBorder(CellStyle cellStyle,BorderStyle borderSize,IndexedColors colorIndex)` | 设置cell的四个边框粗细和颜色 |
| `cn.hutool.poi.excel.style.StyleUtil` | `CellStyle setColor(CellStyle cellStyle,IndexedColors color,FillPatternType fillPattern)` | 给cell设置颜色 |
| `cn.hutool.poi.excel.style.StyleUtil` | `CellStyle setColor(CellStyle cellStyle,short color,FillPatternType fillPattern)` | 给cell设置颜色 |
| `cn.hutool.poi.excel.style.StyleUtil` | `Font createFont(Workbook workbook,short color,short fontSize,String fontName)` | 创建字体 |
| `cn.hutool.poi.excel.style.StyleUtil` | `Font setFontStyle(Font font,short color,short fontSize,String fontName)` | 设置字体样式 |
| `cn.hutool.poi.excel.style.StyleUtil` | `Short getFormat(Workbook workbook,String format)` | 创建数据格式并获取格式 |
| `cn.hutool.poi.excel.style.StyleUtil` | `boolean isNullOrDefaultStyle(Workbook workbook,CellStyle style)` | 给定样式是否为null（无样式）或默认样式，默认样式为workbook.getCellStyleAt(0) |
