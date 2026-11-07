# cn.hutool.poi.word

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.poi.word.DocUtil` | `XWPFDocument create(File file)` | 创建XWPFDocument，如果文件已存在则读取之，否则创建新的 |
| `cn.hutool.poi.word.PicType` | `int getValue()` | 获取图片类型对应值 |
| `cn.hutool.poi.word.TableUtil` | `XWPFTable createTable(XWPFDocument doc)` | 创建空表，只有一行 |
| `cn.hutool.poi.word.TableUtil` | `XWPFTable createTable(XWPFDocument doc,Iterable<?> data)` | 创建表格并填充数据，默认表格 |
| `cn.hutool.poi.word.TableUtil` | `XWPFTable writeTable(XWPFTable table,Iterable<?> data)` | 为table填充数据 |
| `cn.hutool.poi.word.TableUtil` | `XWPFTableCell getOrCreateCell(XWPFTableRow row,int index)` | 获取或创建新单元格 存在则直接返回，不存在创建新的单元格 |
| `cn.hutool.poi.word.TableUtil` | `XWPFTableRow getOrCreateRow(XWPFTable table,int index)` | 获取或创建新行 存在则直接返回，不存在创建新的行 |
| `cn.hutool.poi.word.TableUtil` | `void writeRow(XWPFTableRow row,Iterable<?> rowData)` | 写行数据 |
| `cn.hutool.poi.word.TableUtil` | `void writeRow(XWPFTableRow row,Map<?, ?> rowMap,boolean isWriteKeyAsHead)` | 写行数据 |
| `cn.hutool.poi.word.TableUtil` | `void writeRow(XWPFTableRow row,Object rowBean,boolean isWriteKeyAsHead)` | 写一行数据 |
| `cn.hutool.poi.word.Word07Writer` | `Word07Writer addPicture(File picFile,int width,int height)` | 增加图片，单独成段落 |
| `cn.hutool.poi.word.Word07Writer` | `Word07Writer addPicture(InputStream in,PicType picType,String fileName,int width,int height)` | 增加图片，单独成段落，增加后图片流关闭，默认居中对齐 |
| `cn.hutool.poi.word.Word07Writer` | `Word07Writer addPicture(InputStream in,PicType picType,String fileName,int width,int height,ParagraphAlignment align)` | 增加图片，单独成段落，增加后图片流关闭 |
| `cn.hutool.poi.word.Word07Writer` | `Word07Writer addTable(Iterable<?> data)` | 增加表格数据 |
| `cn.hutool.poi.word.Word07Writer` | `Word07Writer addText(Font font,Color color,String... texts)` | 增加一个段落 |
| `cn.hutool.poi.word.Word07Writer` | `Word07Writer addText(Font font,String... texts)` | 增加一个段落 |
| `cn.hutool.poi.word.Word07Writer` | `Word07Writer addText(ParagraphAlignment align,Font font,Color color,String... texts)` | 增加一个段落 |
| `cn.hutool.poi.word.Word07Writer` | `Word07Writer addText(ParagraphAlignment align,Font font,String... texts)` | 增加一个段落 |
| `cn.hutool.poi.word.Word07Writer` | `Word07Writer flush()` | 将Excel Workbook刷出到预定义的文件 如果用户未自定义输出的文件，将抛出NullPointerException 预定义文件可以通过#setDestFile(File) 方法预定义，或者通过构造定义 |
| `cn.hutool.poi.word.Word07Writer` | `Word07Writer flush(File destFile)` | 将Excel Workbook刷出到文件 如果用户未自定义输出的文件，将抛出NullPointerException |
| `cn.hutool.poi.word.Word07Writer` | `Word07Writer flush(OutputStream out)` | 将Word Workbook刷出到输出流 |
| `cn.hutool.poi.word.Word07Writer` | `Word07Writer flush(OutputStream out,boolean isCloseOut)` | 将Word Document刷出到输出流 |
| `cn.hutool.poi.word.Word07Writer` | `Word07Writer setDestFile(File destFile)` | 设置写出的目标文件 |
| `cn.hutool.poi.word.Word07Writer` | `XWPFDocument getDoc()` | 获取XWPFDocument |
| `cn.hutool.poi.word.Word07Writer` | `void close()` | 关闭Word文档 如果用户设定了目标文件，先写出目标文件后给关闭工作簿 |
| `cn.hutool.poi.word.WordUtil` | `Word07Writer getWriter()` | 创建Word 07格式的生成器 |
| `cn.hutool.poi.word.WordUtil` | `Word07Writer getWriter(File destFile)` | 创建Word 07格式的生成器 |
