# com.feilong.csv

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.csv.CsvWrite` | `void write(String fileName,Iterable<T> iterable)` | 将迭代对象写到文件中. 如果 fileName 是null,抛出 NullPointerException 如果 fileName 是blank,抛出 IllegalArgumentException 如果 iterable 是null或者empty,抛出 IllegalArgumentException |
| `com.feilong.csv.CsvWrite` | `void write(String fileName,Iterable<T> iterable,BeanCsvConfig<T> beanCsvConfig)` | 将迭代对象写到文件中. |
| `com.feilong.csv.CsvWrite` | `void write(String fileName,String[] columnTitles,List<Object[]> dataList)` | 写cvs文件. 如果 fileName 是null,抛出 NullPointerException 如果 fileName 是blank,抛出 IllegalArgumentException 如果 columnTitles和dataList 都是null或者empty,抛出 NullPointerException |
| `com.feilong.csv.CsvWrite` | `void write(String fileName,String[] columnTitles,List<Object[]> dataList,CsvConfig csvConfig)` | 写cvs文件. |
| `com.feilong.csv.DefaultCsvWrite` | `void write(String fileName,Iterable<T> iterable)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.csv.DefaultCsvWrite` | `void write(String fileName,Iterable<T> iterable,BeanCsvConfig<T> beanCsvConfig)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.csv.DefaultCsvWrite` | `void write(String fileName,String[] columnTitles,List<Object[]> dataList)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.csv.DefaultCsvWrite` | `void write(String fileName,String[] columnTitles,List<Object[]> dataList,CsvConfig csvConfig)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
