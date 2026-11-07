# cn.hutool.poi.word

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.poi.word.DocUtil`

```java
public class cn.hutool.poi.word.DocUtil {
  public cn.hutool.poi.word.DocUtil();
  public static org.apache.poi.xwpf.usermodel.XWPFDocument create(java.io.File);
}
```

## `cn.hutool.poi.word.PicType`

```java
public final class cn.hutool.poi.word.PicType extends java.lang.Enum<cn.hutool.poi.word.PicType> {
  public static cn.hutool.poi.word.PicType[] values();
  public static cn.hutool.poi.word.PicType valueOf(java.lang.String);
  public int getValue();
}
```

## `cn.hutool.poi.word.TableUtil`

```java
public class cn.hutool.poi.word.TableUtil {
  public cn.hutool.poi.word.TableUtil();
  public static org.apache.poi.xwpf.usermodel.XWPFTable createTable(org.apache.poi.xwpf.usermodel.XWPFDocument);
  public static org.apache.poi.xwpf.usermodel.XWPFTable createTable(org.apache.poi.xwpf.usermodel.XWPFDocument, java.lang.Iterable<?>);
  public static org.apache.poi.xwpf.usermodel.XWPFTable writeTable(org.apache.poi.xwpf.usermodel.XWPFTable, java.lang.Iterable<?>);
  public static void writeRow(org.apache.poi.xwpf.usermodel.XWPFTableRow, java.lang.Object, boolean);
  public static void writeRow(org.apache.poi.xwpf.usermodel.XWPFTableRow, java.util.Map<?, ?>, boolean);
  public static void writeRow(org.apache.poi.xwpf.usermodel.XWPFTableRow, java.lang.Iterable<?>);
  public static org.apache.poi.xwpf.usermodel.XWPFTableRow getOrCreateRow(org.apache.poi.xwpf.usermodel.XWPFTable, int);
  public static org.apache.poi.xwpf.usermodel.XWPFTableCell getOrCreateCell(org.apache.poi.xwpf.usermodel.XWPFTableRow, int);
}
```

## `cn.hutool.poi.word.Word07Writer`

```java
public class cn.hutool.poi.word.Word07Writer implements java.io.Closeable {
  public cn.hutool.poi.word.Word07Writer();
  public cn.hutool.poi.word.Word07Writer(java.io.File);
  public cn.hutool.poi.word.Word07Writer(org.apache.poi.xwpf.usermodel.XWPFDocument);
  public cn.hutool.poi.word.Word07Writer(org.apache.poi.xwpf.usermodel.XWPFDocument, java.io.File);
  public org.apache.poi.xwpf.usermodel.XWPFDocument getDoc();
  public cn.hutool.poi.word.Word07Writer setDestFile(java.io.File);
  public cn.hutool.poi.word.Word07Writer addText(java.awt.Font, java.lang.String...);
  public cn.hutool.poi.word.Word07Writer addText(java.awt.Font, java.awt.Color, java.lang.String...);
  public cn.hutool.poi.word.Word07Writer addText(org.apache.poi.xwpf.usermodel.ParagraphAlignment, java.awt.Font, java.lang.String...);
  public cn.hutool.poi.word.Word07Writer addText(org.apache.poi.xwpf.usermodel.ParagraphAlignment, java.awt.Font, java.awt.Color, java.lang.String...);
  public cn.hutool.poi.word.Word07Writer addTable(java.lang.Iterable<?>);
  public cn.hutool.poi.word.Word07Writer addPicture(java.io.File, int, int);
  public cn.hutool.poi.word.Word07Writer addPicture(java.io.InputStream, cn.hutool.poi.word.PicType, java.lang.String, int, int);
  public cn.hutool.poi.word.Word07Writer addPicture(java.io.InputStream, cn.hutool.poi.word.PicType, java.lang.String, int, int, org.apache.poi.xwpf.usermodel.ParagraphAlignment);
  public cn.hutool.poi.word.Word07Writer flush() throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.poi.word.Word07Writer flush(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.poi.word.Word07Writer flush(java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.poi.word.Word07Writer flush(java.io.OutputStream, boolean) throws cn.hutool.core.io.IORuntimeException;
  public void close();
}
```

## `cn.hutool.poi.word.WordUtil`

```java
public class cn.hutool.poi.word.WordUtil {
  public cn.hutool.poi.word.WordUtil();
  public static cn.hutool.poi.word.Word07Writer getWriter();
  public static cn.hutool.poi.word.Word07Writer getWriter(java.io.File);
}
```
