# com.feilong.excel.definition

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.excel.definition.ExcelBlock`

```java
public class com.feilong.excel.definition.ExcelBlock implements java.lang.Comparable<com.feilong.excel.definition.ExcelBlock> {
  public com.feilong.excel.definition.ExcelBlock();
  public void setStartCellIndex(java.lang.String);
  public java.lang.String getEndCellIndex();
  public void setEndCellIndex(java.lang.String);
  public int getStartRow();
  public void setStartRow(int);
  public int getStartCol();
  public void setStartCol(int);
  public int getEndRow();
  public void setEndRow(int);
  public int getEndCol();
  public void setEndCol(int);
  public java.lang.String getDataName();
  public void setDataName(java.lang.String);
  public boolean isLoop();
  public void setLoop(boolean);
  public java.lang.String getDirection();
  public void setDirection(java.lang.String);
  public java.lang.Class<?> getLoopClass();
  public void setLoopClass(java.lang.Class<?>);
  public java.util.List<com.feilong.excel.definition.ExcelCell> getCells();
  public void setCells(java.util.List<com.feilong.excel.definition.ExcelCell>);
  public void addCell(com.feilong.excel.definition.ExcelCell);
  public com.feilong.excel.definition.ExcelBlock getChildBlock();
  public void setChildBlock(com.feilong.excel.definition.ExcelBlock);
  public com.feilong.excel.definition.LoopBreakCondition getBreakCondition();
  public void setBreakCondition(com.feilong.excel.definition.LoopBreakCondition);
  public boolean isChild();
  public void setChild(boolean);
  public void setLoopClassByClassName(java.lang.String);
  public java.lang.String toString();
  public int compareTo(com.feilong.excel.definition.ExcelBlock);
  public java.util.List<com.feilong.excel.definition.ExcelCellConditionStyle> getStyles();
  public void setStyles(java.util.List<com.feilong.excel.definition.ExcelCellConditionStyle>);
  public int compareTo(java.lang.Object);
}
```

## `com.feilong.excel.definition.ExcelCell`

```java
public class com.feilong.excel.definition.ExcelCell {
  public com.feilong.excel.definition.ExcelCell();
  public int getRow();
  public void setRow(int);
  public int getCol();
  public void setCol(int);
  public java.lang.String getDataName();
  public void setDataName(java.lang.String);
  public boolean isMandatory();
  public void setMandatory(boolean);
  public java.lang.String[] getAvailableChoices();
  public void setAvailableChoices(java.lang.String[]);
  public java.lang.String getPattern();
  public void setPattern(java.lang.String);
  public void setChoiceString(java.lang.String);
  public java.lang.String getCellIndex();
  public void setCellIndex(java.lang.String);
  public java.util.List<com.feilong.excel.definition.ExcelCellConditionStyle> getStyles();
  public void setStyles(java.util.List<com.feilong.excel.definition.ExcelCellConditionStyle>);
  public void addStyle(com.feilong.excel.definition.ExcelCellConditionStyle);
  public java.lang.String getType();
  public void setType(java.lang.String);
  public java.lang.String getDataExpr();
  public void setDataExpr(java.lang.String);
}
```

## `com.feilong.excel.definition.ExcelCellConditionStyle`

```java
public class com.feilong.excel.definition.ExcelCellConditionStyle {
  public com.feilong.excel.definition.ExcelCellConditionStyle();
  public java.lang.String getCondition();
  public void setCondition(java.lang.String);
  public java.lang.String getCellIndex();
  public void setCellIndex(java.lang.String);
  public int getStartRow();
  public void setStartRow(int);
  public int getStartCol();
  public void setStartCol(int);
  public int getEndRow();
  public void setEndRow(int);
  public int getEndCol();
  public void setEndCol(int);
  public java.lang.String getStartCellIndex();
  public void setStartCellIndex(java.lang.String);
  public java.lang.String getEndCellIndex();
  public void setEndCellIndex(java.lang.String);
}
```

## `com.feilong.excel.definition.ExcelSheet`

```java
public class com.feilong.excel.definition.ExcelSheet {
  public com.feilong.excel.definition.ExcelSheet();
  public java.lang.String getName();
  public void setName(java.lang.String);
  public java.lang.String getDisplayName();
  public void setDisplayName(java.lang.String);
  public java.util.List<com.feilong.excel.definition.ExcelBlock> getExcelBlocks();
  public void setExcelBlocks(java.util.List<com.feilong.excel.definition.ExcelBlock>);
  public com.feilong.excel.definition.ExcelBlock getExcelBlock();
  public void setExcelBlock(com.feilong.excel.definition.ExcelBlock);
  public void addExcelBlock(com.feilong.excel.definition.ExcelBlock);
  public java.util.List<com.feilong.excel.definition.ExcelBlock> getSortedExcelBlocks();
  public java.lang.String toString();
}
```

## `com.feilong.excel.definition.LoopBreakCondition`

```java
public class com.feilong.excel.definition.LoopBreakCondition {
  public com.feilong.excel.definition.LoopBreakCondition();
  public int getRowOffset();
  public void setRowOffset(int);
  public int getColOffset();
  public void setColOffset(int);
  public java.lang.String getFlagString();
  public void setFlagString(java.lang.String);
}
```
