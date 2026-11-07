# com.feilong.template.extension

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.template.extension.TemplateFileData` | `Map<String, ?> getData()` | 获得 数据. |
| `com.feilong.template.extension.TemplateFileData` | `String getOutPutFilePath()` | 获得 输出的文件. |
| `com.feilong.template.extension.TemplateFileData` | `String getTemplatePath()` | 获得 velocity 模板地址. |
| `com.feilong.template.extension.TemplateFileData` | `void setData(Map<String, ?> data)` | 设置 数据. |
| `com.feilong.template.extension.TemplateFileData` | `void setOutPutFilePath(String outPutFilePath)` | 设置 输出的文件. |
| `com.feilong.template.extension.TemplateFileData` | `void setTemplatePath(String templatePath)` | 设置 velocity 模板地址. |
| `com.feilong.template.extension.TemplateFileDataUtil` | `void writeAndOpen(TemplateFileData templateFileData)` | writeAndOpen. 如果 outPutFilePath 是null,抛出 NullPointerException 如果 outPutFilePath 是blank,抛出 IllegalArgumentException |
