# cn.hutool.poi.excel.cell

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.poi.excel.cell.CellEditor` | `Object edit(Cell cell,Object value)` | 编辑，根据单元格信息处理结果值，返回处理后的结果 |
| `cn.hutool.poi.excel.cell.CellHandler` | `void handle(Cell cell,Object value)` | 处理 |
| `cn.hutool.poi.excel.cell.CellLocation` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.CellLocation` | `boolean equals(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.CellLocation` | `int getX()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.CellLocation` | `int getY()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.CellLocation` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.CellLocation` | `void setX(int x)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.CellLocation` | `void setY(int y)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.CellSetter` | `void setValue(Cell cell)` | 自定义单元格值设置，同时可以设置单元格样式、格式等信息 |
| `cn.hutool.poi.excel.cell.CellUtil` | `Cell getCell(Row row,int cellIndex)` | 获取单元格，如果单元格不存在，返回NullCell |
| `cn.hutool.poi.excel.cell.CellUtil` | `Cell getMergedRegionCell(Cell cell)` | 获取合并单元格 传入的x,y坐标（列行数）可以是合并单元格范围内的任意一个单元格 |
| `cn.hutool.poi.excel.cell.CellUtil` | `Cell getMergedRegionCell(Sheet sheet,int x,int y)` | 获取合并单元格 传入的x,y坐标（列行数）可以是合并单元格范围内的任意一个单元格 |
| `cn.hutool.poi.excel.cell.CellUtil` | `Cell getOrCreateCell(Row row,int cellIndex)` | 获取已有单元格或创建新单元格 |
| `cn.hutool.poi.excel.cell.CellUtil` | `CellRangeAddress getCellRangeAddress(Cell cell)` | 获取合并单元格CellRangeAddress，如果不是返回null |
| `cn.hutool.poi.excel.cell.CellUtil` | `CellRangeAddress getCellRangeAddress(Sheet sheet,String locationRef)` | 获取合并单元格CellRangeAddress，如果不是返回null |
| `cn.hutool.poi.excel.cell.CellUtil` | `CellRangeAddress getCellRangeAddress(Sheet sheet,int x,int y)` | 获取合并单元格CellRangeAddress，如果不是返回null |
| `cn.hutool.poi.excel.cell.CellUtil` | `Object getCellValue(Cell cell)` | 获取单元格值 |
| `cn.hutool.poi.excel.cell.CellUtil` | `Object getCellValue(Cell cell,CellEditor cellEditor)` | 获取单元格值 |
| `cn.hutool.poi.excel.cell.CellUtil` | `Object getCellValue(Cell cell,CellType cellType,CellEditor cellEditor)` | 获取单元格值 如果单元格值为数字格式，则判断其格式中是否有小数部分，无则返回Long类型，否则返回Double类型 |
| `cn.hutool.poi.excel.cell.CellUtil` | `Object getCellValue(Cell cell,CellType cellType,final boolean isTrimCellValue)` | 获取单元格值 |
| `cn.hutool.poi.excel.cell.CellUtil` | `Object getCellValue(Cell cell,boolean isTrimCellValue)` | 获取单元格值 |
| `cn.hutool.poi.excel.cell.CellUtil` | `Object getMergedRegionValue(Sheet sheet,String locationRef)` | 获取合并单元格的值 传入的x,y坐标（列行数）可以是合并单元格范围内的任意一个单元格 |
| `cn.hutool.poi.excel.cell.CellUtil` | `Object getMergedRegionValue(Sheet sheet,int x,int y)` | 获取合并单元格的值 传入的x,y坐标（列行数）可以是合并单元格范围内的任意一个单元格 |
| `cn.hutool.poi.excel.cell.CellUtil` | `boolean isMergedRegion(Cell cell)` | 判断指定的单元格是否是合并单元格 |
| `cn.hutool.poi.excel.cell.CellUtil` | `boolean isMergedRegion(Sheet sheet,String locationRef)` | 判断指定的单元格是否是合并单元格 |
| `cn.hutool.poi.excel.cell.CellUtil` | `boolean isMergedRegion(Sheet sheet,int x,int y)` | 判断指定的单元格是否是合并单元格 |
| `cn.hutool.poi.excel.cell.CellUtil` | `int mergingCells(Sheet sheet,int firstRow,int lastRow,int firstColumn,int lastColumn)` | 合并单元格，可以根据设置的值来合并行和列 |
| `cn.hutool.poi.excel.cell.CellUtil` | `int mergingCells(Sheet sheet,int firstRow,int lastRow,int firstColumn,int lastColumn,CellStyle cellStyle)` | 合并单元格，可以根据设置的值来合并行和列 |
| `cn.hutool.poi.excel.cell.CellUtil` | `void setCellValue(Cell cell,Object value)` | 设置单元格值 根据传入的styleSet自动匹配样式 当为头部样式时默认赋值头部样式，但是头部中如果有数字、日期等类型，将按照数字、日期样式设置 |
| `cn.hutool.poi.excel.cell.CellUtil` | `void setCellValue(Cell cell,Object value,CellStyle style)` | 设置单元格值 根据传入的styleSet自动匹配样式 当为头部样式时默认赋值头部样式，但是头部中如果有数字、日期等类型，将按照数字、日期样式设置 |
| `cn.hutool.poi.excel.cell.CellUtil` | `void setCellValue(Cell cell,Object value,StyleSet styleSet,boolean isHeader)` | 设置单元格值 根据传入的styleSet自动匹配样式 当为头部样式时默认赋值头部样式，但是头部中如果有数字、日期等类型，将按照数字、日期样式设置 |
| `cn.hutool.poi.excel.cell.CellUtil` | `void setComment(Cell cell,String commentText,String commentAuthor,ClientAnchor anchor)` | 为特定单元格添加批注 |
| `cn.hutool.poi.excel.cell.CellUtil` | `void setMergedRegionStyle(Cell cell,CellStyle cellStyle)` | 设置合并单元格样式，如果不是则不设置 |
| `cn.hutool.poi.excel.cell.CellValue` | `T getValue()` | 获取单元格值 |
| `cn.hutool.poi.excel.cell.FormulaCellValue` | `Object getResult()` | 获取结果 |
| `cn.hutool.poi.excel.cell.FormulaCellValue` | `String getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.FormulaCellValue` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.FormulaCellValue` | `void setValue(Cell cell)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `CellAddress getAddress()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `CellRangeAddress getArrayFormulaRange()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `CellStyle getCellStyle()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `CellType getCachedFormulaResultType()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `CellType getCachedFormulaResultTypeEnum()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `CellType getCellType()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `CellType getCellTypeEnum()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `Comment getCellComment()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `Date getDateCellValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `Hyperlink getHyperlink()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `LocalDateTime getLocalDateTimeCellValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `RichTextString getRichStringCellValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `Row getRow()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `Sheet getSheet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `String getCellFormula()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `String getStringCellValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `boolean getBooleanCellValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `boolean isPartOfArrayFormulaGroup()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `byte getErrorCellValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `double getNumericCellValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `int getColumnIndex()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `int getRowIndex()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void removeCellComment()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void removeFormula()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void removeHyperlink()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setAsActiveCell()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setBlank()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setCellComment(Comment comment)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setCellErrorValue(byte value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setCellFormula(String formula)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setCellStyle(CellStyle style)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setCellType(CellType cellType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setCellValue(Calendar value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setCellValue(Date value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setCellValue(LocalDateTime value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setCellValue(RichTextString value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setCellValue(String value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setCellValue(boolean value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setCellValue(double value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.cell.NullCell` | `void setHyperlink(Hyperlink link)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
