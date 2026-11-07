# cn.hutool.poi.excel.reader

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.poi.excel.reader.AbstractSheetReader` | `void addHeaderAlias(String header,String alias)` | 增加标题别名 |
| `cn.hutool.poi.excel.reader.AbstractSheetReader` | `void setCellEditor(CellEditor cellEditor)` | 设置单元格值处理逻辑 当Excel中的值并不能满足我们的读取要求时，通过传入一个编辑接口，可以对单元格值自定义，例如对数字和日期类型值转换为字符串等 |
| `cn.hutool.poi.excel.reader.AbstractSheetReader` | `void setHeaderAlias(Map<String, String> headerAlias)` | 设置标题行的别名Map |
| `cn.hutool.poi.excel.reader.AbstractSheetReader` | `void setIgnoreEmptyRow(boolean ignoreEmptyRow)` | 设置是否忽略空行 |
| `cn.hutool.poi.excel.reader.BeanSheetReader` | `List<T> read(Sheet sheet)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.reader.BeanSheetReader` | `void addHeaderAlias(String header,String alias)` | 增加标题别名 |
| `cn.hutool.poi.excel.reader.BeanSheetReader` | `void setCellEditor(CellEditor cellEditor)` | 设置单元格值处理逻辑 当Excel中的值并不能满足我们的读取要求时，通过传入一个编辑接口，可以对单元格值自定义，例如对数字和日期类型值转换为字符串等 |
| `cn.hutool.poi.excel.reader.BeanSheetReader` | `void setHeaderAlias(Map<String, String> headerAlias)` | 设置标题行的别名Map |
| `cn.hutool.poi.excel.reader.BeanSheetReader` | `void setIgnoreEmptyRow(boolean ignoreEmptyRow)` | 设置是否忽略空行 |
| `cn.hutool.poi.excel.reader.ColumnSheetReader` | `List<Object> read(Sheet sheet)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.reader.ListSheetReader` | `List<List<Object>> read(Sheet sheet)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.reader.MapSheetReader` | `List<Map<String, Object>> read(Sheet sheet)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.reader.SheetReader` | `T read(Sheet sheet)` | 读取数据 |
