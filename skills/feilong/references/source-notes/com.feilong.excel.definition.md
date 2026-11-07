# com.feilong.excel.definition

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.excel.definition.ExcelBlock` | `Class<?> getLoopClass()` | 获得 loop class. 写数据的时候, 可以不配置 |
| `com.feilong.excel.definition.ExcelBlock` | `ExcelBlock getChildBlock()` | 【原文待译】Gets the child block. |
| `com.feilong.excel.definition.ExcelBlock` | `List<ExcelCell> getCells()` | 【原文待译】Gets the cells. |
| `com.feilong.excel.definition.ExcelBlock` | `List<ExcelCellConditionStyle> getStyles()` | 【原文待译】Gets the styles. |
| `com.feilong.excel.definition.ExcelBlock` | `LoopBreakCondition getBreakCondition()` | 【原文待译】Gets the break condition. |
| `com.feilong.excel.definition.ExcelBlock` | `String getDataName()` | 【原文待译】Gets the data name. |
| `com.feilong.excel.definition.ExcelBlock` | `String getDirection()` | 【原文待译】Gets the direction. |
| `com.feilong.excel.definition.ExcelBlock` | `String getEndCellIndex()` | 【原文待译】Gets the end cell index. |
| `com.feilong.excel.definition.ExcelBlock` | `String toString()` | 【原文待译】To string. |
| `com.feilong.excel.definition.ExcelBlock` | `boolean isChild()` | 【原文待译】Checks if is child. |
| `com.feilong.excel.definition.ExcelBlock` | `boolean isLoop()` | 【原文待译】Checks if is loop. |
| `com.feilong.excel.definition.ExcelBlock` | `int compareTo(ExcelBlock excelBlock)` | 【原文待译】Compare to. |
| `com.feilong.excel.definition.ExcelBlock` | `int getEndCol()` | 【原文待译】Gets the end col. |
| `com.feilong.excel.definition.ExcelBlock` | `int getEndRow()` | 【原文待译】Gets the end row. |
| `com.feilong.excel.definition.ExcelBlock` | `int getStartCol()` | 【原文待译】Gets the start col. |
| `com.feilong.excel.definition.ExcelBlock` | `int getStartRow()` | 【原文待译】Gets the start row. |
| `com.feilong.excel.definition.ExcelBlock` | `void addCell(ExcelCell cell)` | 添加 cell. |
| `com.feilong.excel.definition.ExcelBlock` | `void setBreakCondition(LoopBreakCondition breakCondition)` | 【原文待译】Sets the break condition. |
| `com.feilong.excel.definition.ExcelBlock` | `void setCells(List<ExcelCell> cells)` | 【原文待译】Sets the cells. |
| `com.feilong.excel.definition.ExcelBlock` | `void setChild(boolean isChildBlock)` | 【原文待译】Sets the child. |
| `com.feilong.excel.definition.ExcelBlock` | `void setChildBlock(ExcelBlock childBlock)` | 【原文待译】Sets the child block. |
| `com.feilong.excel.definition.ExcelBlock` | `void setDataName(String dataName)` | 【原文待译】Sets the data name. |
| `com.feilong.excel.definition.ExcelBlock` | `void setDirection(String direction)` | 【原文待译】Sets the direction. |
| `com.feilong.excel.definition.ExcelBlock` | `void setEndCellIndex(String endCellIndex)` | 【原文待译】Sets the end cell index. |
| `com.feilong.excel.definition.ExcelBlock` | `void setEndCol(int endCol)` | 【原文待译】Sets the end col. |
| `com.feilong.excel.definition.ExcelBlock` | `void setEndRow(int endRow)` | 【原文待译】Sets the end row. |
| `com.feilong.excel.definition.ExcelBlock` | `void setLoop(boolean isLoop)` | 【原文待译】Sets the loop. |
| `com.feilong.excel.definition.ExcelBlock` | `void setLoopClass(Class<?> loopClass)` | Sets the loop class. 写数据的时候, 可以不配置 |
| `com.feilong.excel.definition.ExcelBlock` | `void setLoopClassByClassName(String className)` | 【原文待译】Sets the loop class by class name. |
| `com.feilong.excel.definition.ExcelBlock` | `void setStartCellIndex(String startCellIndex)` | 【原文待译】Sets the start cell index. |
| `com.feilong.excel.definition.ExcelBlock` | `void setStartCol(int startCol)` | 【原文待译】Sets the start col. |
| `com.feilong.excel.definition.ExcelBlock` | `void setStartRow(int startRow)` | 【原文待译】Sets the start row. |
| `com.feilong.excel.definition.ExcelBlock` | `void setStyles(List<ExcelCellConditionStyle> styles)` | 【原文待译】Sets the styles. |
| `com.feilong.excel.definition.ExcelCell` | `List<ExcelCellConditionStyle> getStyles()` | 【原文待译】Gets the styles. |
| `com.feilong.excel.definition.ExcelCell` | `String getCellIndex()` | 【原文待译】Gets the cell index. |
| `com.feilong.excel.definition.ExcelCell` | `String getDataExpr()` | 【原文待译】Gets the data expr. |
| `com.feilong.excel.definition.ExcelCell` | `String getDataName()` | 【原文待译】Gets the data name. |
| `com.feilong.excel.definition.ExcelCell` | `String getPattern()` | 【原文待译】Gets the pattern. |
| `com.feilong.excel.definition.ExcelCell` | `String getType()` | 【原文待译】Gets the type. |
| `com.feilong.excel.definition.ExcelCell` | `String[] getAvailableChoices()` | 【原文待译】Gets the available choices. |
| `com.feilong.excel.definition.ExcelCell` | `boolean isMandatory()` | 【原文待译】Checks if is mandatory. |
| `com.feilong.excel.definition.ExcelCell` | `int getCol()` | 【原文待译】Gets the col. |
| `com.feilong.excel.definition.ExcelCell` | `int getRow()` | 【原文待译】Gets the row. |
| `com.feilong.excel.definition.ExcelCell` | `void addStyle(ExcelCellConditionStyle style)` | 添加 style. |
| `com.feilong.excel.definition.ExcelCell` | `void setAvailableChoices(String[] availableChoices)` | 【原文待译】Sets the available choices. |
| `com.feilong.excel.definition.ExcelCell` | `void setCellIndex(String cellIndex)` | 【原文待译】Sets the cell index. |
| `com.feilong.excel.definition.ExcelCell` | `void setChoiceString(String choiceString)` | 【原文待译】Sets the choice string. |
| `com.feilong.excel.definition.ExcelCell` | `void setCol(int col)` | 【原文待译】Sets the col. |
| `com.feilong.excel.definition.ExcelCell` | `void setDataExpr(String dataExpr)` | 【原文待译】Sets the data expr. |
| `com.feilong.excel.definition.ExcelCell` | `void setDataName(String dataName)` | 【原文待译】Sets the data name. |
| `com.feilong.excel.definition.ExcelCell` | `void setMandatory(boolean isMandatory)` | 【原文待译】Sets the mandatory. |
| `com.feilong.excel.definition.ExcelCell` | `void setPattern(String pattern)` | 【原文待译】Sets the pattern. |
| `com.feilong.excel.definition.ExcelCell` | `void setRow(int row)` | 【原文待译】Sets the row. |
| `com.feilong.excel.definition.ExcelCell` | `void setStyles(List<ExcelCellConditionStyle> styles)` | 【原文待译】Sets the styles. |
| `com.feilong.excel.definition.ExcelCell` | `void setType(String type)` | 【原文待译】Sets the type. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `String getCellIndex()` | 【原文待译】Gets the cell index. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `String getCondition()` | 【原文待译】Gets the condition. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `String getEndCellIndex()` | 【原文待译】Gets the end cell index. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `String getStartCellIndex()` | 【原文待译】Gets the start cell index. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `int getEndCol()` | 【原文待译】Gets the end col. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `int getEndRow()` | 【原文待译】Gets the end row. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `int getStartCol()` | 【原文待译】Gets the start col. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `int getStartRow()` | 【原文待译】Gets the start row. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `void setCellIndex(String cellIndex)` | 【原文待译】Sets the cell index. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `void setCondition(String condition)` | 【原文待译】Sets the condition. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `void setEndCellIndex(String endCellIndex)` | 【原文待译】Sets the end cell index. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `void setEndCol(int endCol)` | 【原文待译】Sets the end col. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `void setEndRow(int endRow)` | 【原文待译】Sets the end row. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `void setStartCellIndex(String startCellIndex)` | 【原文待译】Sets the start cell index. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `void setStartCol(int startCol)` | 【原文待译】Sets the start col. |
| `com.feilong.excel.definition.ExcelCellConditionStyle` | `void setStartRow(int startRow)` | 【原文待译】Sets the start row. |
| `com.feilong.excel.definition.ExcelSheet` | `ExcelBlock getExcelBlock()` | 【原文待译】Gets the excel block. |
| `com.feilong.excel.definition.ExcelSheet` | `List<ExcelBlock> getExcelBlocks()` | 【原文待译】Gets the excel blocks. |
| `com.feilong.excel.definition.ExcelSheet` | `List<ExcelBlock> getSortedExcelBlocks()` | 【原文待译】Gets the sorted excel blocks. |
| `com.feilong.excel.definition.ExcelSheet` | `String getDisplayName()` | 【原文待译】Gets the display name. |
| `com.feilong.excel.definition.ExcelSheet` | `String getName()` | 【原文待译】Gets the name. |
| `com.feilong.excel.definition.ExcelSheet` | `String toString()` | 【原文待译】To string. |
| `com.feilong.excel.definition.ExcelSheet` | `void addExcelBlock(ExcelBlock excelBlock)` | 添加 excel block. |
| `com.feilong.excel.definition.ExcelSheet` | `void setDisplayName(String displayName)` | 【原文待译】Sets the display name. |
| `com.feilong.excel.definition.ExcelSheet` | `void setExcelBlock(ExcelBlock excelBlock)` | 【原文待译】Sets the excel block. |
| `com.feilong.excel.definition.ExcelSheet` | `void setExcelBlocks(List<ExcelBlock> excelBlocks)` | 【原文待译】Sets the excel blocks. |
| `com.feilong.excel.definition.ExcelSheet` | `void setName(String name)` | 【原文待译】Sets the name. |
| `com.feilong.excel.definition.LoopBreakCondition` | `String getFlagString()` | 【原文待译】Gets the flag string. |
| `com.feilong.excel.definition.LoopBreakCondition` | `int getColOffset()` | 【原文待译】Gets the col offset. |
| `com.feilong.excel.definition.LoopBreakCondition` | `int getRowOffset()` | 【原文待译】Gets the row offset. |
| `com.feilong.excel.definition.LoopBreakCondition` | `void setColOffset(int colOffset)` | 【原文待译】Sets the col offset. |
| `com.feilong.excel.definition.LoopBreakCondition` | `void setFlagString(String flagString)` | 【原文待译】Sets the flag string. |
| `com.feilong.excel.definition.LoopBreakCondition` | `void setRowOffset(int rowOffset)` | 【原文待译】Sets the row offset. |
