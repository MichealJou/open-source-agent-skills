# com.feilong.io.entity

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.io.entity.FileInfoEntity` | `FileType getFileType()` | Gets the 类型. |
| `com.feilong.io.entity.FileInfoEntity` | `Long getLastModified()` | Gets the 返回此抽象路径名表示的文件最后一次被修改的时间. 表示文件最后一次被修改的时间的 long 值,用与时间点(1970 年 1 月 1 日,00:00:00 GMT)之间的毫秒数表示;如果该文件不存在,或者发生 I/O 错误,则返回 0L. |
| `com.feilong.io.entity.FileInfoEntity` | `Long getSize()` | Gets the 文件大小, 单位 字节,如果是文件夹 不显示size. |
| `com.feilong.io.entity.FileInfoEntity` | `String getFormatLastModified()` | 格式化显示的时间默认 yy-mm hh:ss. |
| `com.feilong.io.entity.FileInfoEntity` | `String getFormatSize()` | 格式化显示的size |
| `com.feilong.io.entity.FileInfoEntity` | `String getName()` | Gets the 名称. |
| `com.feilong.io.entity.FileInfoEntity` | `void setFileType(FileType fileType)` | Sets the 类型. |
| `com.feilong.io.entity.FileInfoEntity` | `void setLastModified(Long lastModified)` | Sets the 返回此抽象路径名表示的文件最后一次被修改的时间. 表示文件最后一次被修改的时间的 long 值,用与时间点(1970 年 1 月 1 日,00:00:00 GMT)之间的毫秒数表示;如果该文件不存在,或者发生 I/O 错误,则返回 0L. |
| `com.feilong.io.entity.FileInfoEntity` | `void setName(String name)` | Sets the 名称. |
| `com.feilong.io.entity.FileInfoEntity` | `void setSize(Long size)` | Sets the 文件大小, 单位 字节,如果是文件夹 不显示size. |
| `com.feilong.io.entity.MimeType` | `String getExtension()` | 获得 扩展名. |
| `com.feilong.io.entity.MimeType` | `String getMime()` | 获得 mime. |
