# com.feilong.component.upload

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.component.upload.AbstractSimpleListDataHandler` | `void handle(Map<String, Object> data)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.component.upload.DefaultMultipartFileResolver` | `List<String> upload(MultipartFile[] multipartFiles,String directoryName,String[] fileNames)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.component.upload.DefaultMultipartFileResolver` | `String upload(MultipartFile multipartFile,String directoryName,String fileName)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.component.upload.DefaultRequestFileParserDetector` | `FileParser detect(HttpServletRequest request)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.component.upload.DefaultRequestFileParserDetector` | `void setIdentifyParamName(String fileIdentifyParamName)` | 设置 文件标识 参数名字. |
| `com.feilong.component.upload.ExcelFileParser` | `void parse(String fileLocation)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.component.upload.ExcelFileParser` | `void setDataHandler(DataHandler dataHandler)` | 【原文待译】@param dataHandler the dataHandler to set |
| `com.feilong.component.upload.ExcelFileParser` | `void setDataName(String dataName)` | 【原文待译】@param dataName the dataName to set |
| `com.feilong.component.upload.ExcelFileParser` | `void setSheetDefinitionLocation(String sheetDefinitionLocation)` | 【原文待译】@param sheetDefinitionLocation the sheetDefinitionLocation to set |
| `com.feilong.component.upload.ExcelFileParser` | `void setSheetName(String sheetName)` | 【原文待译】@param sheetName the sheetName to set |
| `com.feilong.component.upload.MultipartFileResolver` | `List<String> upload(MultipartFile[] multipartFiles,String directoryName,String[] fileNames)` | 将一组 multipartFiles 上传到指定目录 directoryName 下面,依次重命名指定的文件名称 fileNames . 如果MultipartFile#isEmpty(),那么log warn并跳过 |
| `com.feilong.component.upload.MultipartFileResolver` | `String upload(MultipartFile multipartFile,String directoryName,String fileName)` | 将 MultipartFile 上传到指定目录 directoryName 下面重命名指定的文件名称 fileName . 如果MultipartFile#isEmpty(),那么log warn并跳过 |
| `com.feilong.component.upload.UploadController` | `void upload(HttpServletRequest request,@SuppressWarnings("unused")
HttpServletResponse response,@RequestParam("importFile")
MultipartFile[] multipartFiles)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
