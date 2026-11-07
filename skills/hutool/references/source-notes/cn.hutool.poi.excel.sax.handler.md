# cn.hutool.poi.excel.sax.handler

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.poi.excel.sax.handler.AbstractRowHandler` | `void handle(int sheetIndex,long rowIndex,List<Object> rowCells)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.sax.handler.AbstractRowHandler` | `void handleData(int sheetIndex,long rowIndex,T data)` | 处理转换后的数据 |
| `cn.hutool.poi.excel.sax.handler.BeanRowHandler` | `void handle(int sheetIndex,long rowIndex,List<Object> rowCells)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.sax.handler.MapRowHandler` | `void handle(int sheetIndex,long rowIndex,List<Object> rowCells)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.poi.excel.sax.handler.RowHandler` | `void doAfterAllAnalysed()` | 处理一个sheet页完成的操作 |
| `cn.hutool.poi.excel.sax.handler.RowHandler` | `void handle(int sheetIndex,long rowIndex,List<Object> rowCells)` | 处理一行数据 |
| `cn.hutool.poi.excel.sax.handler.RowHandler` | `void handleCell(int sheetIndex,long rowIndex,int cellIndex,Object value,CellStyle xssfCellStyle)` | 处理一个单元格的数据 |
