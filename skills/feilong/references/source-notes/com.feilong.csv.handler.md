# com.feilong.csv.handler

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.csv.handler.CsvColumnEntityListBuilder` | `List<CsvColumnEntity> build(BeanCsvConfig<T> beanCsvConfig)` | 获得 csv column entity list. |
| `com.feilong.csv.handler.CsvContentBuilder` | `String build(List<Object[]> allLines,CsvConfig csvConfig)` | 【原文待译】Writes the entire list to a CSV file. The list is assumed to be a String[] |
| `com.feilong.csv.handler.DataListBuilder` | `List<Object[]> build(Iterable<T> iterable,List<CsvColumnEntity> csvColumnEntityList)` | 【原文待译】Builds the data list. |
