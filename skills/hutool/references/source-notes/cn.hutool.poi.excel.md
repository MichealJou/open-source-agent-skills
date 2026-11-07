# cn.hutool.poi.excel

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.poi.excel.BigExcelWriter` | `BigExcelWriter autoSizeColumn(int columnIndex)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.BigExcelWriter` | `BigExcelWriter autoSizeColumnAll()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.BigExcelWriter` | `BigExcelWriter autoSizeColumnAll(float widthRatio)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.BigExcelWriter` | `ExcelWriter flush(OutputStream out,boolean isCloseOut)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.BigExcelWriter` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.ExcelBase` | `Cell getCell(String locationRef)` | 获取指定坐标单元格，单元格不存在时返回null |
| `cn.hutool.poi.excel.ExcelBase` | `Cell getCell(String locationRef,boolean isCreateIfNotExist)` | 获取指定坐标单元格，如果isCreateIfNotExist为false，则在单元格不存在时返回null |
| `cn.hutool.poi.excel.ExcelBase` | `Cell getCell(int x,int y)` | 获取指定坐标单元格，单元格不存在时返回null |
| `cn.hutool.poi.excel.ExcelBase` | `Cell getCell(int x,int y,boolean isCreateIfNotExist)` | 获取指定坐标单元格，如果isCreateIfNotExist为false，则在单元格不存在时返回null |
| `cn.hutool.poi.excel.ExcelBase` | `Cell getOrCreateCell(String locationRef)` | 获取或创建指定坐标单元格 |
| `cn.hutool.poi.excel.ExcelBase` | `Cell getOrCreateCell(int x,int y)` | 获取或创建指定坐标单元格 |
| `cn.hutool.poi.excel.ExcelBase` | `CellStyle createCellStyle()` | 创建单元格样式 |
| `cn.hutool.poi.excel.ExcelBase` | `CellStyle createCellStyle(String locationRef)` | 为指定单元格创建样式，返回样式后可以设置样式内容 |
| `cn.hutool.poi.excel.ExcelBase` | `CellStyle createCellStyle(int x,int y)` | 为指定单元格创建样式，返回样式后可以设置样式内容 |
| `cn.hutool.poi.excel.ExcelBase` | `CellStyle createColumnStyle(int x)` | 创建某一列的样式，返回样式后可以设置样式内容 |
| `cn.hutool.poi.excel.ExcelBase` | `CellStyle createRowStyle(int y)` | 创建某一行的样式，返回样式后可以设置样式内容 |
| `cn.hutool.poi.excel.ExcelBase` | `CellStyle getOrCreateCellStyle(String locationRef)` | 为指定单元格获取或者创建样式，返回样式后可以设置样式内容 |
| `cn.hutool.poi.excel.ExcelBase` | `CellStyle getOrCreateCellStyle(int x,int y)` | 为指定单元格获取或者创建样式，返回样式后可以设置样式内容 |
| `cn.hutool.poi.excel.ExcelBase` | `CellStyle getOrCreateColumnStyle(int x)` | 获取或创建某一列的样式，返回样式后可以设置样式内容 需要注意，此方法返回行样式，设置背景色在单元格设置值后会被覆盖，需要单独设置其单元格的样式。 |
| `cn.hutool.poi.excel.ExcelBase` | `CellStyle getOrCreateRowStyle(int y)` | 获取或创建某一行的样式，返回样式后可以设置样式内容 需要注意，此方法返回行样式，设置背景色在单元格设置值后会被覆盖，需要单独设置其单元格的样式。 |
| `cn.hutool.poi.excel.ExcelBase` | `Hyperlink createHyperlink(HyperlinkType type,String address)` | 创建 Hyperlink，默认内容（标签为链接地址本身） |
| `cn.hutool.poi.excel.ExcelBase` | `Hyperlink createHyperlink(HyperlinkType type,String address,String label)` | 创建 Hyperlink，默认内容 |
| `cn.hutool.poi.excel.ExcelBase` | `List<Sheet> getSheets()` | 获取此工作簿所有Sheet表 |
| `cn.hutool.poi.excel.ExcelBase` | `List<String> getSheetNames()` | 获取表名列表 |
| `cn.hutool.poi.excel.ExcelBase` | `Map<String, String> getHeaderAlias()` | 获得标题行的别名Map |
| `cn.hutool.poi.excel.ExcelBase` | `Row getOrCreateRow(int y)` | 获取或者创建行 |
| `cn.hutool.poi.excel.ExcelBase` | `Sheet getSheet()` | 获取当前Sheet |
| `cn.hutool.poi.excel.ExcelBase` | `T addHeaderAlias(String header,String alias)` | 增加标题别名 |
| `cn.hutool.poi.excel.ExcelBase` | `T clearHeaderAlias()` | 清空标题别名，key为Map中的key，value为别名 |
| `cn.hutool.poi.excel.ExcelBase` | `T cloneSheet(int sheetIndex,String newSheetName,boolean setAsCurrentSheet)` | 复制当前sheet为新sheet |
| `cn.hutool.poi.excel.ExcelBase` | `T removeHeaderAlias(String header)` | 去除标题别名 |
| `cn.hutool.poi.excel.ExcelBase` | `T renameSheet(String newName)` | 重命名当前sheet |
| `cn.hutool.poi.excel.ExcelBase` | `T setHeaderAlias(Map<String, String> headerAlias)` | 设置标题行的别名Map |
| `cn.hutool.poi.excel.ExcelBase` | `T setSheet(Sheet sheet)` | 设置自定义Sheet |
| `cn.hutool.poi.excel.ExcelBase` | `T setSheet(String sheetName)` | 自定义需要读取或写出的Sheet，如果给定的sheet不存在，创建之。 在读取中，此方法用于切换读取的sheet，在写出时，此方法用于新建或者切换sheet。 |
| `cn.hutool.poi.excel.ExcelBase` | `T setSheet(int sheetIndex)` | 自定义需要读取或写出的Sheet，如果给定的sheet不存在，创建之（命名为默认） 在读取中，此方法用于切换读取的sheet，在写出时，此方法用于新建或者切换sheet |
| `cn.hutool.poi.excel.ExcelBase` | `Workbook getWorkbook()` | 获取Workbook |
| `cn.hutool.poi.excel.ExcelBase` | `boolean isXlsx()` | 判断是否为xlsx格式的Excel表（Excel07格式） |
| `cn.hutool.poi.excel.ExcelBase` | `int getColumnCount()` | 获取第一行总列数，计算方法为： |
| `cn.hutool.poi.excel.ExcelBase` | `int getColumnCount(int rowNum)` | 获取总列数，计算方法为： |
| `cn.hutool.poi.excel.ExcelBase` | `int getPhysicalRowCount()` | 获取有记录的行数，计算方法为： |
| `cn.hutool.poi.excel.ExcelBase` | `int getRowCount()` | 获取总行数，计算方法为： |
| `cn.hutool.poi.excel.ExcelBase` | `int getSheetCount()` | 返回工作簿表格数 |
| `cn.hutool.poi.excel.ExcelBase` | `void close()` | 关闭工作簿 如果用户设定了目标文件，先写出目标文件后给关闭工作簿 |
| `cn.hutool.poi.excel.ExcelDateUtil` | `boolean isDateFormat(Cell cell)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.ExcelDateUtil` | `boolean isDateFormat(Cell cell,ConditionalFormattingEvaluator cfEvaluator)` | 判断是否日期格式 |
| `cn.hutool.poi.excel.ExcelDateUtil` | `boolean isDateFormat(ExcelNumberFormat numFmt)` | 判断是否日期格式 |
| `cn.hutool.poi.excel.ExcelDateUtil` | `boolean isDateFormat(int formatIndex,String formatString)` | 判断日期格式 |
| `cn.hutool.poi.excel.ExcelExtractorUtil` | `ExcelExtractor getExtractor(Workbook wb)` | 获取 ExcelExtractor 对象 |
| `cn.hutool.poi.excel.ExcelExtractorUtil` | `String readAsText(Workbook wb,boolean withSheetName)` | 读取为文本格式 使用ExcelExtractor 提取Excel内容 |
| `cn.hutool.poi.excel.ExcelFileUtil` | `boolean isXls(InputStream in)` | 是否为XLS格式的Excel文件（HSSF） XLS文件主要用于Excel 97~2003创建 此方法会自动调用InputStream#reset()方法 |
| `cn.hutool.poi.excel.ExcelFileUtil` | `boolean isXlsx(File file)` | 是否为XLSX格式的Excel文件（XSSF） XLSX文件主要用于Excel 2007+创建 |
| `cn.hutool.poi.excel.ExcelFileUtil` | `boolean isXlsx(InputStream in)` | 是否为XLSX格式的Excel文件（XSSF） XLSX文件主要用于Excel 2007+创建 此方法会自动调用InputStream#reset()方法 |
| `cn.hutool.poi.excel.ExcelPicUtil` | `Map<String, PictureData> getPicMap(Workbook workbook,int sheetIndex)` | 获取工作簿指定sheet中图片列表 |
| `cn.hutool.poi.excel.ExcelReader` | `ExcelExtractor getExtractor()` | 获取 ExcelExtractor 对象 |
| `cn.hutool.poi.excel.ExcelReader` | `ExcelReader setCellEditor(CellEditor cellEditor)` | 设置单元格值处理逻辑 当Excel中的值并不能满足我们的读取要求时，通过传入一个编辑接口，可以对单元格值自定义，例如对数字和日期类型值转换为字符串等 |
| `cn.hutool.poi.excel.ExcelReader` | `ExcelReader setIgnoreEmptyRow(boolean ignoreEmptyRow)` | 设置是否忽略空行 |
| `cn.hutool.poi.excel.ExcelReader` | `ExcelWriter getWriter()` | 获取Excel写出器 在读取Excel并做一定编辑后，获取写出器写出，规则如下： 1. 当从流中读取时，转换为Writer直接使用Sheet对象，此时修改不会影响源文件，Writer中flush需要指定新的路径。 2. 当从文件读取时，直接获取文件及sheet名称，此时可以修改原文件。 |
| `cn.hutool.poi.excel.ExcelReader` | `List<List<Object>> read()` | 读取工作簿中指定的Sheet的所有行列数据 |
| `cn.hutool.poi.excel.ExcelReader` | `List<List<Object>> read(int startRowIndex)` | 读取工作簿中指定的Sheet |
| `cn.hutool.poi.excel.ExcelReader` | `List<List<Object>> read(int startRowIndex,int endRowIndex)` | 读取工作簿中指定的Sheet，此方法会把第一行作为标题行，替换标题别名 |
| `cn.hutool.poi.excel.ExcelReader` | `List<List<Object>> read(int startRowIndex,int endRowIndex,boolean aliasFirstLine)` | 读取工作簿中指定的Sheet |
| `cn.hutool.poi.excel.ExcelReader` | `List<Map<String, Object>> read(int headerRowIndex,int startRowIndex,int endRowIndex)` | 读取Excel为Map的列表 Map表示一行，标题为key，单元格内容为value |
| `cn.hutool.poi.excel.ExcelReader` | `List<Map<String, Object>> readAll()` | 读取Excel为Map的列表，读取所有行，默认第一行做为标题，数据从第二行开始 Map表示一行，标题为key，单元格内容为value |
| `cn.hutool.poi.excel.ExcelReader` | `List<Object> readColumn(int columnIndex,int startRowIndex)` | 读取工作簿中指定的Sheet中指定列 |
| `cn.hutool.poi.excel.ExcelReader` | `List<Object> readColumn(int columnIndex,int startRowIndex,int endRowIndex)` | 读取工作簿中指定的Sheet中指定列 |
| `cn.hutool.poi.excel.ExcelReader` | `List<Object> readRow(int rowIndex)` | 读取某一行数据 |
| `cn.hutool.poi.excel.ExcelReader` | `List<T> read(int headerRowIndex,int startRowIndex,Class<T> beanType)` | 读取Excel为Bean的列表 |
| `cn.hutool.poi.excel.ExcelReader` | `List<T> read(int headerRowIndex,int startRowIndex,int endRowIndex,Class<T> beanType)` | 读取Excel为Bean的列表 |
| `cn.hutool.poi.excel.ExcelReader` | `List<T> readAll(Class<T> beanType)` | 读取Excel为Bean的列表，读取所有行，默认第一行做为标题，数据从第二行开始 |
| `cn.hutool.poi.excel.ExcelReader` | `Object readCellValue(int x,int y)` | 读取某个单元格的值 |
| `cn.hutool.poi.excel.ExcelReader` | `String readAsText(boolean withSheetName)` | 读取为文本格式 使用ExcelExtractor 提取Excel内容 |
| `cn.hutool.poi.excel.ExcelReader` | `T read(SheetReader<T> sheetReader)` | 读取数据为指定类型 |
| `cn.hutool.poi.excel.ExcelReader` | `boolean isIgnoreEmptyRow()` | 是否忽略空行 |
| `cn.hutool.poi.excel.ExcelReader` | `void read(CellHandler cellHandler)` | 读取工作簿中指定的Sheet，此方法为类流处理方式，当读到指定单元格时，会调用CellEditor接口 用户通过实现此接口，可以更加灵活地处理每个单元格的数据。 |
| `cn.hutool.poi.excel.ExcelReader` | `void read(int startRowIndex,int endRowIndex,CellHandler cellHandler)` | 读取工作簿中指定的Sheet，此方法为类流处理方式，当读到指定单元格时，会调用CellEditor接口 用户通过实现此接口，可以更加灵活地处理每个单元格的数据。 |
| `cn.hutool.poi.excel.ExcelUtil` | `BigExcelWriter getBigWriter()` | 获得BigExcelWriter，默认写出到第一个sheet 不传入写出的Excel文件路径，只能调用ExcelWriter#flush(OutputStream)方法写出到流 若写出到文件，还需调用BigExcelWriter#setDestFile(File)方法自定义写出的文件，然后调用BigExcelWriter#flush()方法写出到文件 |
| `cn.hutool.poi.excel.ExcelUtil` | `BigExcelWriter getBigWriter(File destFile)` | 获得BigExcelWriter，默认写出到第一个sheet，名字为sheet1 |
| `cn.hutool.poi.excel.ExcelUtil` | `BigExcelWriter getBigWriter(File destFile,String sheetName)` | 获得BigExcelWriter |
| `cn.hutool.poi.excel.ExcelUtil` | `BigExcelWriter getBigWriter(String destFilePath)` | 获得BigExcelWriter，默认写出到第一个sheet |
| `cn.hutool.poi.excel.ExcelUtil` | `BigExcelWriter getBigWriter(String destFilePath,String sheetName)` | 获得BigExcelWriter |
| `cn.hutool.poi.excel.ExcelUtil` | `BigExcelWriter getBigWriter(int rowAccessWindowSize)` | 获得BigExcelWriter，默认写出到第一个sheet 不传入写出的Excel文件路径，只能调用ExcelWriter#flush(OutputStream)方法写出到流 若写出到文件，还需调用BigExcelWriter#setDestFile(File)方法自定义写出的文件，然后调用BigExcelWriter#flush()方法写出到文件 |
| `cn.hutool.poi.excel.ExcelUtil` | `CellLocation toLocation(String locationRef)` | 将Excel中地址标识符（例如A11，B5）等转换为行列表示 例如：A11 -》 x:0,y:10，B5-》x:1,y:4 |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelReader getReader(File bookFile)` | 获取Excel读取器，通过调用ExcelReader的read或readXXX方法读取Excel内容 默认调用第一个sheet |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelReader getReader(File bookFile,String sheetName)` | 获取Excel读取器，通过调用ExcelReader的read或readXXX方法读取Excel内容 |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelReader getReader(File bookFile,int sheetIndex)` | 获取Excel读取器，通过调用ExcelReader的read或readXXX方法读取Excel内容 |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelReader getReader(InputStream bookStream)` | 获取Excel读取器，通过调用ExcelReader的read或readXXX方法读取Excel内容 默认调用第一个sheet，读取结束自动关闭流 |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelReader getReader(InputStream bookStream,String sheetName)` | 获取Excel读取器，通过调用ExcelReader的read或readXXX方法读取Excel内容 读取结束自动关闭流 |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelReader getReader(InputStream bookStream,int sheetIndex)` | 获取Excel读取器，通过调用ExcelReader的read或readXXX方法读取Excel内容 读取结束自动关闭流 |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelReader getReader(String bookFilePath)` | 获取Excel读取器，通过调用ExcelReader的read或readXXX方法读取Excel内容 默认调用第一个sheet |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelReader getReader(String bookFilePath,String sheetName)` | 获取Excel读取器，通过调用ExcelReader的read或readXXX方法读取Excel内容 |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelReader getReader(String bookFilePath,int sheetIndex)` | 获取Excel读取器，通过调用ExcelReader的read或readXXX方法读取Excel内容 |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelWriter getWriter()` | 获得ExcelWriter，默认写出到第一个sheet 不传入写出的Excel文件路径，只能调用ExcelWriter#flush(OutputStream)方法写出到流 若写出到文件，还需调用ExcelWriter#setDestFile(File)方法自定义写出的文件，然后调用ExcelWriter#flush()方法写出到文件 |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelWriter getWriter(File destFile)` | 获得ExcelWriter，默认写出到第一个sheet，名字为sheet1 |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelWriter getWriter(File destFile,String sheetName)` | 获得ExcelWriter |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelWriter getWriter(String destFilePath)` | 获得ExcelWriter，默认写出到第一个sheet |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelWriter getWriter(String destFilePath,String sheetName)` | 获得ExcelWriter |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelWriter getWriter(boolean isXlsx)` | 获得ExcelWriter，默认写出到第一个sheet 不传入写出的Excel文件路径，只能调用ExcelWriter#flush(OutputStream)方法写出到流 若写出到文件，还需调用ExcelWriter#setDestFile(File)方法自定义写出的文件，然后调用ExcelWriter#flush()方法写出到文件 |
| `cn.hutool.poi.excel.ExcelUtil` | `ExcelWriter getWriterWithSheet(String sheetName)` | 获得ExcelWriter，默认写出到第一个sheet |
| `cn.hutool.poi.excel.ExcelUtil` | `String indexToColName(int index)` | 将Sheet列号变为列名 |
| `cn.hutool.poi.excel.ExcelUtil` | `int colNameToIndex(String colName)` | 根据表元的列名转换为列号 |
| `cn.hutool.poi.excel.ExcelUtil` | `void readBySax(File file,String idOrRidOrSheetName,RowHandler rowHandler)` | 通过Sax方式读取Excel，同时支持03和07格式 |
| `cn.hutool.poi.excel.ExcelUtil` | `void readBySax(File file,int rid,RowHandler rowHandler)` | 通过Sax方式读取Excel，同时支持03和07格式 |
| `cn.hutool.poi.excel.ExcelUtil` | `void readBySax(InputStream in,String idOrRidOrSheetName,RowHandler rowHandler)` | 通过Sax方式读取Excel，同时支持03和07格式 |
| `cn.hutool.poi.excel.ExcelUtil` | `void readBySax(InputStream in,int rid,RowHandler rowHandler)` | 通过Sax方式读取Excel，同时支持03和07格式 |
| `cn.hutool.poi.excel.ExcelUtil` | `void readBySax(String path,String idOrRid,RowHandler rowHandler)` | 通过Sax方式读取Excel，同时支持03和07格式 |
| `cn.hutool.poi.excel.ExcelUtil` | `void readBySax(String path,int rid,RowHandler rowHandler)` | 通过Sax方式读取Excel，同时支持03和07格式 |
| `cn.hutool.poi.excel.ExcelWriter` | `CellStyle getCellStyle()` | 获取单元格样式，获取样式后可自定义样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `CellStyle getHeadCellStyle()` | 获取头部样式，获取样式后可自定义样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter addHeaderAlias(String name,String alias)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter addIgnoredErrors(final CellRangeAddress cellRangeAddress,final IgnoredErrorType... ignoredErrorTypes)` | 设置忽略错误，即Excel中的绿色警告小标，只支持XSSFSheet 见：https://stackoverflow.com/questions/23488221/how-to-remove-warning-in-excel-using-apache-poi-in-java |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter addSelect(CellRangeAddressList regions,String... selectList)` | 增加下拉列表 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter addSelect(int x,int y,String... selectList)` | 增加下拉列表 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter addValidationData(DataValidation dataValidation)` | 增加单元格控制，比如下拉列表、日期验证、数字范围验证等 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter autoSizeColumn(int columnIndex)` | 设置某列为自动宽度，不考虑合并单元格 此方法必须在指定列数据完全写出后调用才有效。 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter autoSizeColumn(int columnIndex,boolean useMergedCells)` | 设置某列为自动宽度 此方法必须在指定列数据完全写出后调用才有效。 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter autoSizeColumn(int columnIndex,boolean useMergedCells,float widthRatio)` | 设置某列为自动宽度。注意有中文的情况下，需要根据需求调整宽度扩大比例。 此方法必须在指定列数据完全写出后调用才有效。 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter autoSizeColumn(int columnIndex,float widthRatio)` | 设置某列为自动宽度。注意有中文的情况下，需要根据需求调整宽度扩大比例。 此方法必须在指定列数据完全写出后调用才有效。 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter autoSizeColumnAll()` | 设置所有列为自动宽度，不考虑合并单元格 此方法必须在指定列数据完全写出后调用才有效。 列数计算是通过第一行计算的 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter autoSizeColumnAll(float widthRatio)` | 设置所有列为自动宽度，不考虑合并单元格 此方法必须在指定列数据完全写出后调用才有效。 列数计算是通过第一行计算的 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter clearHeaderAlias()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter disableDefaultStyle()` | 禁用默认样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter flush()` | 将Excel Workbook刷出到预定义的文件 如果用户未自定义输出的文件，将抛出NullPointerException 预定义文件可以通过#setDestFile(File) 方法预定义，或者通过构造定义 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter flush(File destFile)` | 将Excel Workbook刷出到文件 如果用户未自定义输出的文件，将抛出NullPointerException |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter flush(OutputStream out)` | 将Excel Workbook刷出到输出流 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter flush(OutputStream out,boolean isCloseOut)` | 将Excel Workbook刷出到输出流 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter merge(int firstRow,int lastRow,int firstColumn,int lastColumn,Object content,CellStyle cellStyle)` | 合并单元格，并写入对象到单元格,使用指定的样式 指定样式传入null，则不使用任何样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter merge(int firstRow,int lastRow,int firstColumn,int lastColumn,Object content,boolean isSetHeaderStyle)` | 合并某行的单元格，并写入对象到单元格 样式为默认标题样式，可使用#getHeadCellStyle()方法调用后自定义默认样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter merge(int lastColumn)` | 合并当前行的单元格 样式为默认标题样式，可使用#getHeadCellStyle()方法调用后自定义默认样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter merge(int lastColumn,Object content)` | 合并当前行的单元格，并写入对象到单元格 如果写到单元格中的内容非null，行号自动+1，否则当前行号不变 样式为默认标题样式，可使用#getHeadCellStyle()方法调用后自定义默认样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter merge(int lastColumn,Object content,boolean isSetHeaderStyle)` | 合并某行的单元格，并写入对象到单元格 如果写到单元格中的内容非null，行号自动+1，否则当前行号不变 样式为默认标题样式，可使用#getHeadCellStyle()方法调用后自定义默认样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter passCurrentRow()` | 跳过当前行 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter passRows(int rows)` | 跳过指定行数 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter renameSheet(String sheetName)` | 重命名当前sheet |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter renameSheet(int sheet,String sheetName)` | 重命名sheet |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter reset()` | 重置Writer，包括： |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter resetRow()` | 重置当前行为0 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setColumnStyle(int x,CellStyle style)` | 设置列的默认样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setColumnStyleIfHasData(int x,int y,CellStyle style)` | 设置整个列的样式 仅对数据单元格设置 write后调用 cn.hutool.poi.excel.ExcelWriter#setColumnStyle(int, org.apache.poi.ss.usermodel.CellStyle) 这个方法加的样式会使整列没有数据的单元格也有样式 特别是加背景色时很不美观 且有数据的单元格样式会被StyleSet中的样式覆盖掉 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setColumnWidth(int columnIndex,int width)` | 设置列宽（单位为一个字符的宽度，例如传入width为10，表示10个字符的宽度） |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setCurrentRow(int rowIndex)` | 设置当前所在行 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setCurrentRowToEnd()` | 定位到最后一行的后边，用于追加数据 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setDefaultRowHeight(int height)` | 设置默认行高，值为一个点的高度 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setDestFile(File destFile)` | 设置写出的目标文件 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setFreezePane(int colSplit,int rowSplit)` | 设置窗口冻结，之前冻结的窗口会被覆盖，如果colSplit和rowSplit为0表示取消冻结 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setFreezePane(int rowSplit)` | 设置窗口冻结，之前冻结的窗口会被覆盖，如果rowSplit为0表示取消冻结 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setHeaderAlias(Map<String, String> headerAlias)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setHeaderOrFooter(String text,Align align,boolean isFooter)` | 设置Excel页眉或页脚 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setOnlyAlias(boolean isOnlyAlias)` | 设置是否只保留别名中的字段值，如果为true，则不设置alias的字段将不被输出，false表示原样输出 Bean中设置@Alias时，setOnlyAlias是无效的，这个参数只和addHeaderAlias配合使用，原因是注解是Bean内部的操作，而addHeaderAlias是Writer的操作，不互通。 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setRowHeight(int rownum,int height)` | 设置行高，值为一个点的高度 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setRowStyle(int y,CellStyle style)` | 设置行样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setRowStyleIfHasData(int y,CellStyle style)` | 对数据行整行加自定义样式 仅对数据单元格设置 write后调用 cn.hutool.poi.excel.ExcelWriter#setRowStyle(int, org.apache.poi.ss.usermodel.CellStyle) 这个方法加的样式会使整行没有数据的单元格也有样式 特别是加背景色时很不美观 且有数据的单元格样式会被StyleSet中的样式覆盖掉 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setSheet(String sheetName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setSheet(int sheetIndex)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setStyle(CellStyle style,String locationRef)` | 设置某个单元格的样式 此方法用于多个单元格共享样式的情况 可以调用#getOrCreateCellStyle(int, int) 方法创建或取得一个样式对象。 需要注意的是，共享样式会共享同一个CellStyle，一个单元格样式改变，全部改变。 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setStyle(CellStyle style,int x,int y)` | 设置某个单元格的样式 此方法用于多个单元格共享样式的情况 可以调用#getOrCreateCellStyle(int, int) 方法创建或取得一个样式对象。 需要注意的是，共享样式会共享同一个CellStyle，一个单元格样式改变，全部改变。 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter setStyleSet(StyleSet styleSet)` | 设置样式集，如果不使用样式，传入null |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter write(Iterable<?> data)` | 写出数据，本方法只是将数据写入Workbook中的Sheet，并不写出到文件 写出的起始行为当前行号，可使用#getCurrentRow()方法调用，根据写出的的行数，当前行号自动增加 样式为默认样式，可使用#getCellStyle()方法调用后自定义默认样式 默认的，当当前行号为0时，写出标题（如果为Map或Bean），否则不写标题 data中元素支持的类型有： |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter write(Iterable<?> data,Comparator<String> comparator)` | 写出数据，本方法只是将数据写入Workbook中的Sheet，并不写出到文件 写出的起始行为当前行号，可使用#getCurrentRow()方法调用，根据写出的的行数，当前行号自动增加 样式为默认样式，可使用#getCellStyle()方法调用后自定义默认样式 data中元素支持的类型有： 1. Map，即元素为一个Map，第一个Map的keys作为首行，剩下的行为Map的values，data表示多行 2. Bean，即元素为一个Bean，第一个Bean的字段名列表会作为首行，剩下的行为Bean的字段值列表，data表示多行 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter write(Iterable<?> data,boolean isWriteKeyAsHead)` | 写出数据，本方法只是将数据写入Workbook中的Sheet，并不写出到文件 写出的起始行为当前行号，可使用#getCurrentRow()方法调用，根据写出的的行数，当前行号自动增加 样式为默认样式，可使用#getCellStyle()方法调用后自定义默认样式 data中元素支持的类型有： |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeCellValue(String locationRef,Object value)` | 给指定单元格赋值，使用默认单元格样式，默认不是Header |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeCellValue(String locationRef,Object value,boolean isHeader)` | 给指定单元格赋值，使用默认单元格样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeCellValue(int x,int y,Object value)` | 给指定单元格赋值，使用默认单元格样式，默认不是Header |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeCellValue(int x,int y,Object value,boolean isHeader)` | 给指定单元格赋值，使用默认单元格样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeCol(Map<?, ? extends Iterable<?>> colMap,boolean isWriteKeyAsHead)` | 从第1列开始按列写入数据(index 从0开始) 本方法只是将数据写入Workbook中的Sheet，并不写出到文件 写出的起始行为当前行号，可使用#getCurrentRow()方法调用，根据写出的的行数，当前行号自动+1 样式为默认样式，可使用#getCellStyle()方法调用后自定义默认样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeCol(Map<?, ? extends Iterable<?>> colMap,int startColIndex,boolean isWriteKeyAsHead)` | 从指定列开始按列写入数据(index 从0开始) 本方法只是将数据写入Workbook中的Sheet，并不写出到文件 写出的起始行为当前行号，可使用#getCurrentRow()方法调用，根据写出的的行数，当前行号自动+1 样式为默认样式，可使用#getCellStyle()方法调用后自定义默认样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeCol(Object headerVal,Iterable<?> colData,boolean isResetRowIndex)` | 为第一列写入数据 本方法只是将数据写入Workbook中的Sheet，并不写出到文件 写出的起始行为当前行号，可使用#getCurrentRow()方法调用，根据写出的的行数，当前行号自动+1 样式为默认样式，可使用#getCellStyle()方法调用后自定义默认样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeCol(Object headerVal,int colIndex,Iterable<?> colData,boolean isResetRowIndex)` | 为第指定列写入数据 本方法只是将数据写入Workbook中的Sheet，并不写出到文件 写出的起始行为当前行号，可使用#getCurrentRow()方法调用，根据写出的的行数，当前行号自动+1 样式为默认样式，可使用#getCellStyle()方法调用后自定义默认样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeHeadRow(Iterable<?> rowData)` | 写出一行标题数据 本方法只是将数据写入Workbook中的Sheet，并不写出到文件 写出的起始行为当前行号，可使用#getCurrentRow()方法调用，根据写出的的行数，当前行号自动+1 样式为默认标题样式，可使用#getHeadCellStyle()方法调用后自定义默认样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeImg(File imgFile,int col1,int row1,int col2,int row2)` | 写出数据，本方法只是将数据写入Workbook中的Sheet，并不写出到文件 添加图片到当前sheet中 / 默认图片类型png / 默认的起始坐标和结束坐标都为0 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeImg(File imgFile,int dx1,int dy1,int dx2,int dy2,int col1,int row1,int col2,int row2)` | 写出数据，本方法只是将数据写入Workbook中的Sheet，并不写出到文件 添加图片到当前sheet中 / 默认图片类型png |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeImg(File imgFile,int imgType,int dx1,int dy1,int dx2,int dy2,int col1,int row1,int col2,int row2)` | 写出数据，本方法只是将数据写入Workbook中的Sheet，并不写出到文件 添加图片到当前sheet中 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeImg(byte[] pictureData,int imgType,int dx1,int dy1,int dx2,int dy2,int col1,int row1,int col2,int row2)` | 写出数据，本方法只是将数据写入Workbook中的Sheet，并不写出到文件 添加图片到当前sheet中 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeRow(Iterable<?> rowData)` | 写出一行数据 本方法只是将数据写入Workbook中的Sheet，并不写出到文件 写出的起始行为当前行号，可使用#getCurrentRow()方法调用，根据写出的的行数，当前行号自动+1 样式为默认样式，可使用#getCellStyle()方法调用后自定义默认样式 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeRow(Map<?, ?> rowMap,boolean isWriteKeyAsHead)` | 将一个Map写入到Excel，isWriteKeyAsHead为true写出两行，Map的keys做为一行，values做为第二行，否则只写出一行values 如果rowMap为空（包括null），则写出空行 |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeRow(Object rowBean,boolean isWriteKeyAsHead)` | 写出一行，根据rowBean数据类型不同，写出情况如下： |
| `cn.hutool.poi.excel.ExcelWriter` | `ExcelWriter writeSecHeadRow(Iterable<?> rowData)` | 写出复杂标题的第二行标题数据 本方法只是将数据写入Workbook中的Sheet，并不写出到文件 写出的起始行为当前行号，可使用#getCurrentRow()方法调用，根据写出的的行数，当前行号自动+1 样式为默认标题样式，可使用#getHeadCellStyle()方法调用后自定义默认样式 此方法的逻辑是：将一行数据写出到当前行，遇到已存在的单元格跳过，不存在的创建并赋值。 |
| `cn.hutool.poi.excel.ExcelWriter` | `Font createFont()` | 创建字体 |
| `cn.hutool.poi.excel.ExcelWriter` | `String getContentType()` | 获取Content-Type头对应的值，可以通过调用以下方法快速设置下载Excel的头信息： |
| `cn.hutool.poi.excel.ExcelWriter` | `String getDisposition(String fileName,Charset charset)` | 获取Content-Disposition头对应的值，可以通过调用以下方法快速设置下载Excel的头信息： |
| `cn.hutool.poi.excel.ExcelWriter` | `StyleSet getStyleSet()` | 获取样式集，样式集可以自定义包括： |
| `cn.hutool.poi.excel.ExcelWriter` | `int getCurrentRow()` | 获得当前行 |
| `cn.hutool.poi.excel.ExcelWriter` | `void close()` | 关闭工作簿 如果用户设定了目标文件，先写出目标文件后给关闭工作簿 |
| `cn.hutool.poi.excel.RowUtil` | `List<Object> readRow(Row row,CellEditor cellEditor)` | 读取一行 |
| `cn.hutool.poi.excel.RowUtil` | `List<Object> readRow(Row row,int startCellNumInclude,int endCellNumInclude,CellEditor cellEditor)` | 读取一行 |
| `cn.hutool.poi.excel.RowUtil` | `Row getOrCreateRow(Sheet sheet,int rowIndex)` | 获取已有行或创建新行 |
| `cn.hutool.poi.excel.RowUtil` | `void insertRow(Sheet sheet,int startRow,int insertNumber)` | 插入行 |
| `cn.hutool.poi.excel.RowUtil` | `void removeRow(Row row)` | 从工作表中删除指定的行，此方法修复sheet.shiftRows删除行时会拆分合并的单元格的问题 |
| `cn.hutool.poi.excel.RowUtil` | `void writeRow(Row row,Iterable<?> rowData)` | 写一行数据，无样式，非标题 |
| `cn.hutool.poi.excel.RowUtil` | `void writeRow(Row row,Iterable<?> rowData,StyleSet styleSet,boolean isHeader)` | 写一行数据 |
| `cn.hutool.poi.excel.StyleSet` | `CellStyle getCellStyle()` | 获取常规单元格样式，获取后可以定义整体头部样式 |
| `cn.hutool.poi.excel.StyleSet` | `CellStyle getCellStyleForDate()` | 获取日期单元格样式，获取后可以定义整体日期样式 |
| `cn.hutool.poi.excel.StyleSet` | `CellStyle getCellStyleForHyperlink()` | 获取链接单元格样式，获取后可以定义整体链接样式 |
| `cn.hutool.poi.excel.StyleSet` | `CellStyle getCellStyleForNumber()` | 获取数字（带小数点）单元格样式，获取后可以定义整体数字样式 |
| `cn.hutool.poi.excel.StyleSet` | `CellStyle getHeadCellStyle()` | 获取头部样式，获取后可以定义整体头部样式 |
| `cn.hutool.poi.excel.StyleSet` | `CellStyle getStyleByValueType(Object value,boolean isHeader)` | 获取值对应的公共单元格样式 |
| `cn.hutool.poi.excel.StyleSet` | `StyleSet setAlign(HorizontalAlignment halign,VerticalAlignment valign)` | 设置cell文本对齐样式 |
| `cn.hutool.poi.excel.StyleSet` | `StyleSet setBackgroundColor(IndexedColors backgroundColor,boolean withHeadCell)` | 设置单元格背景样式 |
| `cn.hutool.poi.excel.StyleSet` | `StyleSet setBorder(BorderStyle borderSize,IndexedColors colorIndex)` | 定义所有单元格的边框类型 |
| `cn.hutool.poi.excel.StyleSet` | `StyleSet setFont(Font font,boolean ignoreHead)` | 设置全局字体 |
| `cn.hutool.poi.excel.StyleSet` | `StyleSet setFont(short color,short fontSize,String fontName,boolean ignoreHead)` | 设置全局字体 |
| `cn.hutool.poi.excel.StyleSet` | `StyleSet setWrapText()` | 设置单元格文本自动换行 |
| `cn.hutool.poi.excel.WorkbookUtil` | `SXSSFWorkbook createSXSSFBook()` | 创建空的SXSSFWorkbook，用于大批量数据写出 |
| `cn.hutool.poi.excel.WorkbookUtil` | `SXSSFWorkbook createSXSSFBook(File excelFile)` | 创建或加载SXSSFWorkbook工作簿（读写模式） |
| `cn.hutool.poi.excel.WorkbookUtil` | `SXSSFWorkbook createSXSSFBook(File excelFile,String password)` | 创建或加载SXSSFWorkbook工作簿（读写模式） |
| `cn.hutool.poi.excel.WorkbookUtil` | `SXSSFWorkbook createSXSSFBook(File excelFile,String password,boolean readOnly)` | 创建或加载SXSSFWorkbook工作簿 |
| `cn.hutool.poi.excel.WorkbookUtil` | `SXSSFWorkbook createSXSSFBook(File excelFile,boolean readOnly)` | 创建或加载SXSSFWorkbook工作簿 |
| `cn.hutool.poi.excel.WorkbookUtil` | `SXSSFWorkbook createSXSSFBook(InputStream in)` | 创建或加载SXSSFWorkbook工作簿（只读模式） |
| `cn.hutool.poi.excel.WorkbookUtil` | `SXSSFWorkbook createSXSSFBook(InputStream in,String password)` | 创建或加载SXSSFWorkbook工作簿（只读模式） |
| `cn.hutool.poi.excel.WorkbookUtil` | `SXSSFWorkbook createSXSSFBook(String excelFilePath)` | 创建或加载SXSSFWorkbook工作簿（读写模式） |
| `cn.hutool.poi.excel.WorkbookUtil` | `SXSSFWorkbook createSXSSFBook(String excelFilePath,boolean readOnly)` | 创建或加载SXSSFWorkbook工作簿 |
| `cn.hutool.poi.excel.WorkbookUtil` | `SXSSFWorkbook createSXSSFBook(int rowAccessWindowSize)` | 创建空的SXSSFWorkbook，用于大批量数据写出 |
| `cn.hutool.poi.excel.WorkbookUtil` | `SXSSFWorkbook createSXSSFBook(int rowAccessWindowSize,boolean compressTmpFiles,boolean useSharedStringsTable)` | 创建空的SXSSFWorkbook，用于大批量数据写出 |
| `cn.hutool.poi.excel.WorkbookUtil` | `Sheet getOrCreateSheet(Workbook book,String sheetName)` | 获取或者创建sheet表 如果sheet表在Workbook中已经存在，则获取之，否则创建之 |
| `cn.hutool.poi.excel.WorkbookUtil` | `Sheet getOrCreateSheet(Workbook book,int sheetIndex)` | 获取或者创建sheet表 自定义需要读取或写出的Sheet，如果给定的sheet不存在，创建之（命名为默认） 在读取中，此方法用于切换读取的sheet，在写出时，此方法用于新建或者切换sheet |
| `cn.hutool.poi.excel.WorkbookUtil` | `Workbook createBook(File excelFile)` | 创建或加载工作簿（读写模式） |
| `cn.hutool.poi.excel.WorkbookUtil` | `Workbook createBook(File excelFile,String password)` | 创建或加载工作簿（读写模式） |
| `cn.hutool.poi.excel.WorkbookUtil` | `Workbook createBook(File excelFile,String password,boolean readOnly)` | 创建或加载工作簿 |
| `cn.hutool.poi.excel.WorkbookUtil` | `Workbook createBook(File excelFile,boolean readOnly)` | 创建或加载工作簿 |
| `cn.hutool.poi.excel.WorkbookUtil` | `Workbook createBook(InputStream in)` | 创建或加载工作簿（只读模式） |
| `cn.hutool.poi.excel.WorkbookUtil` | `Workbook createBook(InputStream in,String password)` | 创建或加载工作簿（只读模式） |
| `cn.hutool.poi.excel.WorkbookUtil` | `Workbook createBook(String excelFilePath)` | 创建或加载工作簿（读写模式） |
| `cn.hutool.poi.excel.WorkbookUtil` | `Workbook createBook(String excelFilePath,boolean readOnly)` | 创建或加载工作簿 |
| `cn.hutool.poi.excel.WorkbookUtil` | `Workbook createBook(boolean isXlsx)` | 创建新的空白Excel工作簿 |
| `cn.hutool.poi.excel.WorkbookUtil` | `Workbook createBookForWriter(File excelFile)` | 创建工作簿，用于Excel写出（读写模式） |
| `cn.hutool.poi.excel.WorkbookUtil` | `boolean isEmpty(Sheet sheet)` | sheet是否为空 |
| `cn.hutool.poi.excel.WorkbookUtil` | `void writeBook(Workbook book,OutputStream out)` | 将Excel Workbook刷出到输出流，不关闭流 |
