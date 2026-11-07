# cn.hutool.core.text.csv

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.text.csv.CsvBaseReader` | `CsvData read(File file)` | 读取CSV文件，默认UTF-8编码 |
| `cn.hutool.core.text.csv.CsvBaseReader` | `CsvData read(File file,Charset charset)` | 读取CSV文件 |
| `cn.hutool.core.text.csv.CsvBaseReader` | `CsvData read(Path path)` | 读取CSV文件，默认UTF-8编码 |
| `cn.hutool.core.text.csv.CsvBaseReader` | `CsvData read(Path path,Charset charset)` | 读取CSV文件 |
| `cn.hutool.core.text.csv.CsvBaseReader` | `CsvData read(Reader reader)` | 从Reader中读取CSV数据，读取后关闭Reader |
| `cn.hutool.core.text.csv.CsvBaseReader` | `CsvData read(Reader reader,boolean close)` | 从Reader中读取CSV数据 |
| `cn.hutool.core.text.csv.CsvBaseReader` | `CsvData readFromStr(String csvStr)` | 从字符串中读取CSV数据 |
| `cn.hutool.core.text.csv.CsvBaseReader` | `List<Map<String, String>> readMapList(Reader reader)` | 从Reader中读取CSV数据，结果为Map，读取后关闭Reader。 此方法默认识别首行为标题行。 |
| `cn.hutool.core.text.csv.CsvBaseReader` | `List<T> read(Reader reader,Class<T> clazz)` | 从Reader中读取CSV数据并转换为Bean列表，读取后关闭Reader。 此方法默认识别首行为标题行。 |
| `cn.hutool.core.text.csv.CsvBaseReader` | `List<T> read(String csvStr,Class<T> clazz)` | 从字符串中读取CSV数据并转换为Bean列表，读取后关闭Reader。 此方法默认识别首行为标题行。 |
| `cn.hutool.core.text.csv.CsvBaseReader` | `void read(Reader reader,CsvRowHandler rowHandler)` | 从Reader中读取CSV数据，读取后关闭Reader |
| `cn.hutool.core.text.csv.CsvBaseReader` | `void read(Reader reader,boolean close,CsvRowHandler rowHandler)` | 从Reader中读取CSV数据，读取后关闭Reader |
| `cn.hutool.core.text.csv.CsvBaseReader` | `void readFromStr(String csvStr,CsvRowHandler rowHandler)` | 从字符串中读取CSV数据 |
| `cn.hutool.core.text.csv.CsvBaseReader` | `void setContainsHeader(boolean containsHeader)` | 设置是否首行做为标题行，默认false |
| `cn.hutool.core.text.csv.CsvBaseReader` | `void setErrorOnDifferentFieldCount(boolean errorOnDifferentFieldCount)` | 设置每行字段个数不同时是否抛出异常，默认false |
| `cn.hutool.core.text.csv.CsvBaseReader` | `void setFieldSeparator(char fieldSeparator)` | 设置字段分隔符，默认逗号',' |
| `cn.hutool.core.text.csv.CsvBaseReader` | `void setSkipEmptyRows(boolean skipEmptyRows)` | 设置是否跳过空白行，默认true |
| `cn.hutool.core.text.csv.CsvBaseReader` | `void setTextDelimiter(char textDelimiter)` | 设置 文本分隔符，文本包装符，默认双引号'"' |
| `cn.hutool.core.text.csv.CsvConfig` | `T addHeaderAlias(String header,String alias)` | 增加标题别名 |
| `cn.hutool.core.text.csv.CsvConfig` | `T disableComment()` | 设置注释无效 当写出CSV时，CsvWriter#writeComment(String)将抛出异常 当读取CSV时，注释行按照正常行读取 |
| `cn.hutool.core.text.csv.CsvConfig` | `T removeHeaderAlias(String header)` | 去除标题别名 |
| `cn.hutool.core.text.csv.CsvConfig` | `T setCommentCharacter(Character commentCharacter)` | 设置 注释符号，用于区分注释行，null表示忽略注释 |
| `cn.hutool.core.text.csv.CsvConfig` | `T setFieldSeparator(final char fieldSeparator)` | 设置字段分隔符，默认逗号',' |
| `cn.hutool.core.text.csv.CsvConfig` | `T setHeaderAlias(Map<String, String> headerAlias)` | 设置标题行的别名Map |
| `cn.hutool.core.text.csv.CsvConfig` | `T setTextDelimiter(char textDelimiter)` | 设置 文本分隔符，文本包装符，默认双引号'"' |
| `cn.hutool.core.text.csv.CsvData` | `CsvRow getRow(final int index)` | 获取指定行，从0开始 |
| `cn.hutool.core.text.csv.CsvData` | `Iterator<CsvRow> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvData` | `List<CsvRow> getRows()` | 获取所有行 |
| `cn.hutool.core.text.csv.CsvData` | `List<String> getHeader()` | 获取头信息列表，如果无头信息为Null，返回列表为只读列表 |
| `cn.hutool.core.text.csv.CsvData` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvData` | `int getRowCount()` | 总行数 |
| `cn.hutool.core.text.csv.CsvParser` | `CsvRow nextRow()` | 读取下一行数据 |
| `cn.hutool.core.text.csv.CsvParser` | `List<String> getHeader()` | 获取头部字段列表，如果headerLineNo < 0，抛出异常 |
| `cn.hutool.core.text.csv.CsvParser` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvReadConfig` | `CsvReadConfig defaultConfig()` | 默认配置 |
| `cn.hutool.core.text.csv.CsvReadConfig` | `CsvReadConfig setBeginLineNo(long beginLineNo)` | 设置开始的行（包括），默认0，此处为原始文件行号 |
| `cn.hutool.core.text.csv.CsvReadConfig` | `CsvReadConfig setContainsHeader(boolean containsHeader)` | 设置是否首行做为标题行，默认false 当设置为true时，默认标题行号是#beginLineNo，false为-1，表示无行号 |
| `cn.hutool.core.text.csv.CsvReadConfig` | `CsvReadConfig setEndLineNo(long endLineNo)` | 设置结束的行（包括），默认不限制，此处为原始文件行号 |
| `cn.hutool.core.text.csv.CsvReadConfig` | `CsvReadConfig setErrorOnDifferentFieldCount(boolean errorOnDifferentFieldCount)` | 设置每行字段个数不同时是否抛出异常，默认false |
| `cn.hutool.core.text.csv.CsvReadConfig` | `CsvReadConfig setHeaderLineNo(long headerLineNo)` | 设置标题行行号，默认-1，表示无标题行 |
| `cn.hutool.core.text.csv.CsvReadConfig` | `CsvReadConfig setSkipEmptyRows(boolean skipEmptyRows)` | 设置是否跳过空白行，默认true |
| `cn.hutool.core.text.csv.CsvReadConfig` | `CsvReadConfig setTrimField(boolean trimField)` | 设置每个字段是否去除两边空白符 如果字段以#textDelimiter包围，则保留两边空格 |
| `cn.hutool.core.text.csv.CsvReader` | `CsvData read()` | 读取CSV文件，此方法只能调用一次 调用此方法的前提是构造中传入文件路径或Reader |
| `cn.hutool.core.text.csv.CsvReader` | `Iterator<CsvRow> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvReader` | `Stream<CsvRow> stream()` | 根据Reader创建Stream，以便使用stream方式读取csv行 |
| `cn.hutool.core.text.csv.CsvReader` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvReader` | `void read(CsvRowHandler rowHandler)` | 读取CSV数据，此方法只能调用一次 调用此方法的前提是构造中传入文件路径或Reader |
| `cn.hutool.core.text.csv.CsvRow` | `Iterator<String> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `List<String> getRawList()` | 获取本行所有字段值列表 |
| `cn.hutool.core.text.csv.CsvRow` | `List<String> subList(int fromIndex,int toIndex)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `ListIterator<String> listIterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `ListIterator<String> listIterator(int index)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `Map<String, String> getFieldMap()` | 获取标题与字段值对应的Map |
| `cn.hutool.core.text.csv.CsvRow` | `Object[] toArray()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `String get(int index)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `String getByName(String name)` | 获取标题对应的字段内容 |
| `cn.hutool.core.text.csv.CsvRow` | `String remove(int index)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `String set(int index,String element)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `T toBean(Class<T> clazz)` | 一行数据转换为Bean对象 |
| `cn.hutool.core.text.csv.CsvRow` | `T[] toArray(T[] a)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `boolean add(String e)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `boolean addAll(Collection<? extends String> c)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `boolean addAll(int index,Collection<? extends String> c)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `boolean contains(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `boolean containsAll(Collection<?> c)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `boolean remove(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `boolean removeAll(Collection<?> c)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `boolean retainAll(Collection<?> c)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `int getFieldCount()` | 获取字段格式 |
| `cn.hutool.core.text.csv.CsvRow` | `int indexOf(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `int lastIndexOf(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `int size()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `long getOriginalLineNumber()` | 获取原始行号，多行情况下为首行行号。忽略注释行 |
| `cn.hutool.core.text.csv.CsvRow` | `void add(int index,String element)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRow` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvRowHandler` | `void handle(CsvRow row)` | 处理行数据 |
| `cn.hutool.core.text.csv.CsvTokener` | `int next()` | 读取下一个字符，并记录位置 |
| `cn.hutool.core.text.csv.CsvTokener` | `long getIndex()` | 获取当前位置 |
| `cn.hutool.core.text.csv.CsvTokener` | `void back()` | 将标记回退到第一个字符 |
| `cn.hutool.core.text.csv.CsvTokener` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvUtil` | `CsvReader getReader()` | 获取CSV读取器，调用此方法创建的Reader须自行指定读取的资源 |
| `cn.hutool.core.text.csv.CsvUtil` | `CsvReader getReader(CsvReadConfig config)` | 获取CSV读取器，调用此方法创建的Reader须自行指定读取的资源 |
| `cn.hutool.core.text.csv.CsvUtil` | `CsvReader getReader(Reader reader)` | 获取CSV读取器 |
| `cn.hutool.core.text.csv.CsvUtil` | `CsvReader getReader(Reader reader,CsvReadConfig config)` | 获取CSV读取器 |
| `cn.hutool.core.text.csv.CsvUtil` | `CsvWriter getWriter(File file,Charset charset)` | 获取CSV生成器（写出器），使用默认配置，覆盖已有文件（如果存在） |
| `cn.hutool.core.text.csv.CsvUtil` | `CsvWriter getWriter(File file,Charset charset,boolean isAppend)` | 获取CSV生成器（写出器），使用默认配置 |
| `cn.hutool.core.text.csv.CsvUtil` | `CsvWriter getWriter(File file,Charset charset,boolean isAppend,CsvWriteConfig config)` | 获取CSV生成器（写出器） |
| `cn.hutool.core.text.csv.CsvUtil` | `CsvWriter getWriter(String filePath,Charset charset)` | 获取CSV生成器（写出器），使用默认配置，覆盖已有文件（如果存在） |
| `cn.hutool.core.text.csv.CsvUtil` | `CsvWriter getWriter(String filePath,Charset charset,boolean isAppend)` | 获取CSV生成器（写出器），使用默认配置 |
| `cn.hutool.core.text.csv.CsvUtil` | `CsvWriter getWriter(Writer writer)` | 获取CSV生成器（写出器） |
| `cn.hutool.core.text.csv.CsvUtil` | `CsvWriter getWriter(Writer writer,CsvWriteConfig config)` | 获取CSV生成器（写出器） |
| `cn.hutool.core.text.csv.CsvWriteConfig` | `CsvWriteConfig defaultConfig()` | 默认配置 |
| `cn.hutool.core.text.csv.CsvWriteConfig` | `CsvWriteConfig setAlwaysDelimitText(boolean alwaysDelimitText)` | 设置是否始终使用文本分隔符，文本包装符，默认false，按需添加 |
| `cn.hutool.core.text.csv.CsvWriteConfig` | `CsvWriteConfig setEndingLineBreak(boolean endingLineBreak)` | 文件末尾是否添加换行符 按照https://datatracker.ietf.org/doc/html/rfc4180#section-2 规范，末尾换行符可有可无。 |
| `cn.hutool.core.text.csv.CsvWriteConfig` | `CsvWriteConfig setLineDelimiter(char[] lineDelimiter)` | 设置换行符 |
| `cn.hutool.core.text.csv.CsvWriter` | `CsvWriter setAlwaysDelimitText(boolean alwaysDelimitText)` | 设置是否始终使用文本分隔符，文本包装符，默认false，按需添加 |
| `cn.hutool.core.text.csv.CsvWriter` | `CsvWriter setLineDelimiter(char[] lineDelimiter)` | 设置换行符 |
| `cn.hutool.core.text.csv.CsvWriter` | `CsvWriter write(CsvData csvData)` | 将一个 CsvData 集合写出到Writer |
| `cn.hutool.core.text.csv.CsvWriter` | `CsvWriter write(Iterable<?> lines)` | 将多行写出到Writer |
| `cn.hutool.core.text.csv.CsvWriter` | `CsvWriter write(String[]... lines)` | 将多行写出到Writer |
| `cn.hutool.core.text.csv.CsvWriter` | `CsvWriter writeBeans(Iterable<?> beans)` | 将一个Bean集合写出到Writer，并自动生成表头 |
| `cn.hutool.core.text.csv.CsvWriter` | `CsvWriter writeBeans(Iterable<?> beans,String... properties)` | 将一个Bean集合写出到Writer，并自动生成表头 |
| `cn.hutool.core.text.csv.CsvWriter` | `CsvWriter writeBeans(Iterable<?> beans,boolean writeHeaderLine,String... properties)` | 将一个Bean集合写出到Writer，并自动生成表头 |
| `cn.hutool.core.text.csv.CsvWriter` | `CsvWriter writeComment(String comment)` | 写出一行注释，注释符号可自定义 如果注释符不存在，则抛出异常 |
| `cn.hutool.core.text.csv.CsvWriter` | `CsvWriter writeHeaderLine(String... fields)` | 写出一行头部行，支持标题别名 |
| `cn.hutool.core.text.csv.CsvWriter` | `CsvWriter writeLine()` | 追加新行（换行） |
| `cn.hutool.core.text.csv.CsvWriter` | `CsvWriter writeLine(String... fields)` | 写出一行 |
| `cn.hutool.core.text.csv.CsvWriter` | `void close()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.text.csv.CsvWriter` | `void flush()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
