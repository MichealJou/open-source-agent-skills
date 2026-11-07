# com.feilong.excel

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.excel.DataConvertorConfig` | `Class<?> getSupportedClass(String name)` | 【原文待译】Gets the supported class. |
| `com.feilong.excel.DataConvertorConfig` | `DataConvertor<T> getConvertor(Class<T> clazz)` | 【原文待译】Gets the convertor. |
| `com.feilong.excel.DataConvertorConfig` | `DataConvertorConfig getInstance()` | 【原文待译】Gets the single instance of DataConvertorConfigurator. |
| `com.feilong.excel.DataConvertorConfig` | `void registerDataConvertor(DataConvertor<?> dataConvertor)` | 【原文待译】Register data convertor. |
| `com.feilong.excel.DefaultExcelReader` | `ReadStatus readAll(InputStream inputStream,Map<String, Object> beans)` | 【原文待译】Read all. |
| `com.feilong.excel.DefaultExcelReader` | `ReadStatus readAllPerSheet(InputStream inputStream,Map<String, Object> data)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.excel.DefaultExcelReader` | `ReadStatus readSheet(InputStream inputStream,int sheetNo,Map<String, Object> beans)` | 【原文待译】Read sheet. |
| `com.feilong.excel.DefaultExcelReader` | `void setSkipErrors(boolean skipErrors)` | 【原文待译】Sets the skip errors. |
| `com.feilong.excel.DefaultExcelWriter` | `void initBufferedTemplate(InputStream inputStream)` | 【原文待译】Inits the buffered template. |
| `com.feilong.excel.DefaultExcelWriter` | `void write(OutputStream outputStream,Map<String, Object> data)` | 【原文待译】Write. |
| `com.feilong.excel.DefaultExcelWriter` | `void write(String template,OutputStream outputStream,Map<String, Object> data)` | 【原文待译】Write. |
| `com.feilong.excel.DefaultExcelWriter` | `void writePerSheet(InputStream inputStream,OutputStream outputStream,List<Map<String, Object>> beansList)` | 【原文待译】Write per sheet. |
| `com.feilong.excel.DefaultExcelWriter` | `void writePerSheet(OutputStream outputStream,List<Map<String, Object>> beansList)` | 【原文待译】Write per sheet. |
| `com.feilong.excel.DefaultExcelWriter` | `void writePerSheet(String template,OutputStream os,List<Map<String, Object>> beansList)` | 【原文待译】Write per sheet. |
| `com.feilong.excel.ExcelDefinition` | `Integer getStyleSheetPosition()` | 【原文待译】Gets the style sheet position. |
| `com.feilong.excel.ExcelDefinition` | `List<ExcelSheet> getExcelSheets()` | 【原文待译】Gets the excel sheets. |
| `com.feilong.excel.ExcelDefinition` | `String toString()` | 【原文待译】To string. |
| `com.feilong.excel.ExcelDefinition` | `void setExcelSheets(List<ExcelSheet> excelSheets)` | 【原文待译】Sets the excel sheets. |
| `com.feilong.excel.ExcelDefinition` | `void setStyleSheetPosition(Integer styleSheetPosition)` | 【原文待译】Sets the style sheet position. |
| `com.feilong.excel.ExcelException` | `ExcelCell getExcelCell()` | 【原文待译】@return the excelCell |
| `com.feilong.excel.ExcelException` | `Object getValue()` | 【原文待译】@return the value |
| `com.feilong.excel.ExcelException` | `String getCellIndex()` | 【原文待译】@return the cellIndex |
| `com.feilong.excel.ExcelException` | `String toString()` | 【原文待译】To string. |
| `com.feilong.excel.ExcelException` | `int getErrorCode()` | 【原文待译】@return the errorCode |
| `com.feilong.excel.ExcelException` | `int getSheetNo()` | 【原文待译】@return the sheetNo |
| `com.feilong.excel.ExcelManipulatorFactory` | `ExcelReader createExcelReader(String... sheetNames)` | 【原文待译】Creates a new ExcelManipulator object. |
| `com.feilong.excel.ExcelManipulatorFactory` | `ExcelWriter createExcelWriter(Integer styleSheetPosition,String writeTemplateName,String... sheetNames)` | 【原文待译】Creates a new ExcelManipulator object. |
| `com.feilong.excel.ExcelManipulatorFactory` | `void setConfig(String... sheetDefinitionLocations)` | 【原文待译】Sets the config. |
| `com.feilong.excel.ExcelManipulatorFactory` | `void setSheetDefinitions(Map<String, ExcelSheet> sheetDefinitions)` | 【原文待译】@param sheetDefinitions the sheetDefinitions to set |
| `com.feilong.excel.ExcelReader` | `ReadStatus readAll(InputStream inputStream,Map<String, Object> beans)` | 【原文待译】Read All sheets infos into one beans scope with multiple sheet definitions. |
| `com.feilong.excel.ExcelReader` | `ReadStatus readAllPerSheet(InputStream inputStream,Map<String, Object> beans)` | 【原文待译】Read All sheets using one sheet definition to get colletion infos. |
| `com.feilong.excel.ExcelReader` | `ReadStatus readSheet(InputStream inputStream,int sheetNo,Map<String, Object> beans)` | 【原文待译】Read specific sheet using one sheet definition. |
| `com.feilong.excel.ExcelReaderUtil` | `List<T> read(String excelLocation,String sheetDefinitionLocation,String sheetName,String dataName,int sheetNo)` | 获得 list. |
| `com.feilong.excel.ExcelReaderUtil` | `Map<String, Object> readData(String excelLocation,String sheetDefinitionLocation,String sheetName,int sheetNo)` | 读取数据. |
| `com.feilong.excel.ExcelSheetListBuilder` | `Digester create(String location)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.excel.ExcelWriteUtil` | `String write(String templateLocation,String sheetDefinitionLocation,String sheetName,Map<String, Object> beans,String outputFileName)` | 【原文待译】Write. |
| `com.feilong.excel.ExcelWriteUtil` | `String write(String templateLocation,String sheetDefinitionLocation,String[] sheetNames,Map<String, Object> beans,String outputFileName)` | 【原文待译】Write. |
| `com.feilong.excel.ExcelWriter` | `void write(OutputStream outputStream,Map<String, Object> data)` | 【原文待译】Write. |
| `com.feilong.excel.ExcelWriter` | `void write(String template,OutputStream outputStream,Map<String, Object> data)` | 【原文待译】Write. |
| `com.feilong.excel.ExcelWriter` | `void writePerSheet(InputStream inputStream,OutputStream outputStream,List<Map<String, Object>> dataList)` | 【原文待译】Write per sheet. |
| `com.feilong.excel.ExcelWriter` | `void writePerSheet(OutputStream outputStream,List<Map<String, Object>> dataList)` | 【原文待译】Write per sheet. |
| `com.feilong.excel.ExcelWriter` | `void writePerSheet(String template,OutputStream outputStream,List<Map<String, Object>> dataList)` | 【原文待译】Write per sheet. |
