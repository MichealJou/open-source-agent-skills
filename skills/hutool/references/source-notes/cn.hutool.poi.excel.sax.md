# cn.hutool.poi.excel.sax

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.poi.excel.sax.AttributeName` | `String getValue(Attributes attributes)` | 从属性里列表中获取对应属性值 |
| `cn.hutool.poi.excel.sax.AttributeName` | `boolean match(String attributeName)` | 是否匹配给定属性 |
| `cn.hutool.poi.excel.sax.CellDataType` | `CellDataType of(String name)` | 类型字符串转为枚举 |
| `cn.hutool.poi.excel.sax.CellDataType` | `String getName()` | 获取对应类型的属性值 |
| `cn.hutool.poi.excel.sax.ElementName` | `ElementName of(String elementName)` | 解析支持的节点名枚举 |
| `cn.hutool.poi.excel.sax.ElementName` | `boolean match(String elementName)` | 给定标签名是否匹配当前标签 |
| `cn.hutool.poi.excel.sax.Excel03SaxReader` | `Excel03SaxReader read(File file,String idOrRidOrSheetName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.sax.Excel03SaxReader` | `Excel03SaxReader read(InputStream excelStream,String idOrRidOrSheetName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.sax.Excel03SaxReader` | `Excel03SaxReader read(POIFSFileSystem fs,String idOrRidOrSheetName)` | 读取 |
| `cn.hutool.poi.excel.sax.Excel03SaxReader` | `String getSheetName()` | 获得Sheet名，如果处理所有sheet，获得后一个Sheet名，从0开始 |
| `cn.hutool.poi.excel.sax.Excel03SaxReader` | `int getSheetIndex()` | 获得Sheet序号，如果处理所有sheet，获得最大的Sheet序号，从0开始 |
| `cn.hutool.poi.excel.sax.Excel03SaxReader` | `void processRecord(Record record)` | HSSFListener 监听方法，处理 Record |
| `cn.hutool.poi.excel.sax.Excel07SaxReader` | `Excel07SaxReader read(File file,String idOrRidOrSheetName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.sax.Excel07SaxReader` | `Excel07SaxReader read(File file,int rid)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.sax.Excel07SaxReader` | `Excel07SaxReader read(InputStream in,String idOrRidOrSheetName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.sax.Excel07SaxReader` | `Excel07SaxReader read(InputStream in,int rid)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.sax.Excel07SaxReader` | `Excel07SaxReader read(OPCPackage opcPackage,String idOrRidOrSheetName)` | 开始读取Excel，Sheet编号从0开始计数 |
| `cn.hutool.poi.excel.sax.Excel07SaxReader` | `Excel07SaxReader read(OPCPackage opcPackage,int rid)` | 开始读取Excel，Sheet编号从0开始计数 |
| `cn.hutool.poi.excel.sax.Excel07SaxReader` | `Excel07SaxReader read(XSSFReader xssfReader,String idOrRidOrSheetName)` | 开始读取Excel，Sheet编号从0开始计数 |
| `cn.hutool.poi.excel.sax.Excel07SaxReader` | `Excel07SaxReader setRowHandler(RowHandler rowHandler)` | 设置行处理器 |
| `cn.hutool.poi.excel.sax.ExcelSaxReader` | `T read(File file)` | 开始读取Excel，读取所有sheet |
| `cn.hutool.poi.excel.sax.ExcelSaxReader` | `T read(File file,String idOrRidOrSheetName)` | 开始读取Excel |
| `cn.hutool.poi.excel.sax.ExcelSaxReader` | `T read(File file,int rid)` | 开始读取Excel |
| `cn.hutool.poi.excel.sax.ExcelSaxReader` | `T read(InputStream in)` | 开始读取Excel，读取所有sheet，读取结束后并不关闭流 |
| `cn.hutool.poi.excel.sax.ExcelSaxReader` | `T read(InputStream in,String idOrRidOrSheetName)` | 开始读取Excel，读取结束后并不关闭流 |
| `cn.hutool.poi.excel.sax.ExcelSaxReader` | `T read(InputStream in,int rid)` | 开始读取Excel，读取结束后并不关闭流 |
| `cn.hutool.poi.excel.sax.ExcelSaxReader` | `T read(String path)` | 开始读取Excel，读取所有sheet |
| `cn.hutool.poi.excel.sax.ExcelSaxReader` | `T read(String path,String idOrRidOrSheetName)` | 开始读取Excel |
| `cn.hutool.poi.excel.sax.ExcelSaxReader` | `T read(String path,int idOrRidOrSheetName)` | 开始读取Excel |
| `cn.hutool.poi.excel.sax.ExcelSaxUtil` | `DateTime getDateValue(String value)` | 获取日期 |
| `cn.hutool.poi.excel.sax.ExcelSaxUtil` | `DateTime getDateValue(double value)` | 获取日期 |
| `cn.hutool.poi.excel.sax.ExcelSaxUtil` | `ExcelSaxReader<?> createSaxReader(boolean isXlsx,RowHandler rowHandler)` | 创建 ExcelSaxReader |
| `cn.hutool.poi.excel.sax.ExcelSaxUtil` | `Object getDataValue(CellDataType cellDataType,String value,SharedStrings sharedStrings,String numFmtString)` | 根据数据类型获取数据 |
| `cn.hutool.poi.excel.sax.ExcelSaxUtil` | `Object getNumberOrDateValue(CellValueRecordInterface cell,double value,FormatTrackingHSSFListener formatListener)` | 在Excel03 sax读取中获取日期或数字类型的结果值 |
| `cn.hutool.poi.excel.sax.ExcelSaxUtil` | `String formatCellContent(String value,int numFmtIndex,String numFmtString)` | 格式化数字或日期值 |
| `cn.hutool.poi.excel.sax.ExcelSaxUtil` | `boolean isDateFormat(CellValueRecordInterface cell,FormatTrackingHSSFListener formatListener)` | 判断数字Record中是否为日期格式 |
| `cn.hutool.poi.excel.sax.ExcelSaxUtil` | `boolean isDateFormat(int formatIndex,String formatString)` | 判断日期格式 |
| `cn.hutool.poi.excel.sax.ExcelSaxUtil` | `int countNullCell(String preRef,String ref)` | 计算两个单元格之间的单元格数目(同一行) |
| `cn.hutool.poi.excel.sax.ExcelSaxUtil` | `void readFrom(InputStream xmlDocStream,ContentHandler handler)` | 从Excel的XML文档中读取内容，并使用ContentHandler处理 |
| `cn.hutool.poi.excel.sax.SheetDataSaxHandler` | `void characters(char[] ch,int start,int length)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.sax.SheetDataSaxHandler` | `void endElement(String uri,String localName,String qName)` | 标签结束的回调处理方法 |
| `cn.hutool.poi.excel.sax.SheetDataSaxHandler` | `void setRowHandler(RowHandler rowHandler)` | 设置行处理器 |
| `cn.hutool.poi.excel.sax.SheetDataSaxHandler` | `void startElement(String uri,String localName,String qName,Attributes attributes)` | 读到一个xml开始标签时的回调处理方法 |
| `cn.hutool.poi.excel.sax.SheetRidReader` | `Integer getRidByIndex(int index)` | 通过sheet的序号获取rid |
| `cn.hutool.poi.excel.sax.SheetRidReader` | `Integer getRidByIndexBase0(int index)` | 通过sheet的序号获取rid |
| `cn.hutool.poi.excel.sax.SheetRidReader` | `Integer getRidByName(String sheetName)` | 根据sheet name获取rid，从1开始 |
| `cn.hutool.poi.excel.sax.SheetRidReader` | `Integer getRidByNameBase0(String sheetName)` | 根据sheet name获取rid，从0开始 |
| `cn.hutool.poi.excel.sax.SheetRidReader` | `Integer getRidBySheetId(int sheetId)` | 根据sheetId获取rid，从1开始 |
| `cn.hutool.poi.excel.sax.SheetRidReader` | `Integer getRidBySheetIdBase0(int sheetId)` | 根据sheetId获取rid，从0开始 |
| `cn.hutool.poi.excel.sax.SheetRidReader` | `List<String> getSheetNames()` | 获取所有sheet名称 |
| `cn.hutool.poi.excel.sax.SheetRidReader` | `SheetRidReader parse(XSSFReader reader)` | 从XSSFReader中解析sheet名、sheet id等相关信息 |
| `cn.hutool.poi.excel.sax.SheetRidReader` | `SheetRidReader read(XSSFReader xssfReader)` | 读取Wordkbook的XML中sheet标签中sheetId和rid的对应关系 |
| `cn.hutool.poi.excel.sax.SheetRidReader` | `void startElement(String uri,String localName,String qName,Attributes attributes)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
