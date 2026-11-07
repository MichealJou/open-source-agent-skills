# cn.hutool.poi.excel.reader

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.poi.excel.reader.AbstractSheetReader`

```java
public abstract class cn.hutool.poi.excel.reader.AbstractSheetReader<T> implements cn.hutool.poi.excel.reader.SheetReader<T> {
  public cn.hutool.poi.excel.reader.AbstractSheetReader(int, int);
  public void setCellEditor(cn.hutool.poi.excel.cell.CellEditor);
  public void setIgnoreEmptyRow(boolean);
  public void setHeaderAlias(java.util.Map<java.lang.String, java.lang.String>);
  public void addHeaderAlias(java.lang.String, java.lang.String);
}
```

## `cn.hutool.poi.excel.reader.BeanSheetReader`

```java
public class cn.hutool.poi.excel.reader.BeanSheetReader<T> implements cn.hutool.poi.excel.reader.SheetReader<java.util.List<T>> {
  public cn.hutool.poi.excel.reader.BeanSheetReader(int, int, int, java.lang.Class<T>);
  public java.util.List<T> read(org.apache.poi.ss.usermodel.Sheet);
  public void setCellEditor(cn.hutool.poi.excel.cell.CellEditor);
  public void setIgnoreEmptyRow(boolean);
  public void setHeaderAlias(java.util.Map<java.lang.String, java.lang.String>);
  public void addHeaderAlias(java.lang.String, java.lang.String);
  public java.lang.Object read(org.apache.poi.ss.usermodel.Sheet);
}
```

## `cn.hutool.poi.excel.reader.ColumnSheetReader`

```java
public class cn.hutool.poi.excel.reader.ColumnSheetReader extends cn.hutool.poi.excel.reader.AbstractSheetReader<java.util.List<java.lang.Object>> {
  public cn.hutool.poi.excel.reader.ColumnSheetReader(int, int, int);
  public java.util.List<java.lang.Object> read(org.apache.poi.ss.usermodel.Sheet);
  public java.lang.Object read(org.apache.poi.ss.usermodel.Sheet);
}
```

## `cn.hutool.poi.excel.reader.ListSheetReader`

```java
public class cn.hutool.poi.excel.reader.ListSheetReader extends cn.hutool.poi.excel.reader.AbstractSheetReader<java.util.List<java.util.List<java.lang.Object>>> {
  public cn.hutool.poi.excel.reader.ListSheetReader(int, int, boolean);
  public java.util.List<java.util.List<java.lang.Object>> read(org.apache.poi.ss.usermodel.Sheet);
  public java.lang.Object read(org.apache.poi.ss.usermodel.Sheet);
}
```

## `cn.hutool.poi.excel.reader.MapSheetReader`

```java
public class cn.hutool.poi.excel.reader.MapSheetReader extends cn.hutool.poi.excel.reader.AbstractSheetReader<java.util.List<java.util.Map<java.lang.String, java.lang.Object>>> {
  public cn.hutool.poi.excel.reader.MapSheetReader(int, int, int);
  public java.util.List<java.util.Map<java.lang.String, java.lang.Object>> read(org.apache.poi.ss.usermodel.Sheet);
  public java.lang.Object read(org.apache.poi.ss.usermodel.Sheet);
}
```

## `cn.hutool.poi.excel.reader.SheetReader`

```java
public interface cn.hutool.poi.excel.reader.SheetReader<T> {
  public abstract T read(org.apache.poi.ss.usermodel.Sheet);
}
```
