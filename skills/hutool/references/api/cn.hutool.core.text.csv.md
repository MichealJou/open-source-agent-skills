# cn.hutool.core.text.csv

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.text.csv.CsvBaseReader`

```java
public class cn.hutool.core.text.csv.CsvBaseReader implements java.io.Serializable {
  public cn.hutool.core.text.csv.CsvBaseReader();
  public cn.hutool.core.text.csv.CsvBaseReader(cn.hutool.core.text.csv.CsvReadConfig);
  public void setFieldSeparator(char);
  public void setTextDelimiter(char);
  public void setContainsHeader(boolean);
  public void setSkipEmptyRows(boolean);
  public void setErrorOnDifferentFieldCount(boolean);
  public cn.hutool.core.text.csv.CsvData read(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.text.csv.CsvData readFromStr(java.lang.String);
  public void readFromStr(java.lang.String, cn.hutool.core.text.csv.CsvRowHandler);
  public cn.hutool.core.text.csv.CsvData read(java.io.File, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.text.csv.CsvData read(java.nio.file.Path) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.text.csv.CsvData read(java.nio.file.Path, java.nio.charset.Charset) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.text.csv.CsvData read(java.io.Reader) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.text.csv.CsvData read(java.io.Reader, boolean) throws cn.hutool.core.io.IORuntimeException;
  public java.util.List<java.util.Map<java.lang.String, java.lang.String>> readMapList(java.io.Reader) throws cn.hutool.core.io.IORuntimeException;
  public <T> java.util.List<T> read(java.io.Reader, java.lang.Class<T>);
  public <T> java.util.List<T> read(java.lang.String, java.lang.Class<T>);
  public void read(java.io.Reader, cn.hutool.core.text.csv.CsvRowHandler) throws cn.hutool.core.io.IORuntimeException;
  public void read(java.io.Reader, boolean, cn.hutool.core.text.csv.CsvRowHandler) throws cn.hutool.core.io.IORuntimeException;
}
```

## `cn.hutool.core.text.csv.CsvConfig`

```java
public class cn.hutool.core.text.csv.CsvConfig<T extends cn.hutool.core.text.csv.CsvConfig<T>> implements java.io.Serializable {
  public cn.hutool.core.text.csv.CsvConfig();
  public T setFieldSeparator(char);
  public T setTextDelimiter(char);
  public T disableComment();
  public T setCommentCharacter(java.lang.Character);
  public T setHeaderAlias(java.util.Map<java.lang.String, java.lang.String>);
  public T addHeaderAlias(java.lang.String, java.lang.String);
  public T removeHeaderAlias(java.lang.String);
}
```

## `cn.hutool.core.text.csv.CsvData`

```java
public class cn.hutool.core.text.csv.CsvData implements java.lang.Iterable<cn.hutool.core.text.csv.CsvRow>, java.io.Serializable {
  public cn.hutool.core.text.csv.CsvData(java.util.List<java.lang.String>, java.util.List<cn.hutool.core.text.csv.CsvRow>);
  public int getRowCount();
  public java.util.List<java.lang.String> getHeader();
  public cn.hutool.core.text.csv.CsvRow getRow(int);
  public java.util.List<cn.hutool.core.text.csv.CsvRow> getRows();
  public java.util.Iterator<cn.hutool.core.text.csv.CsvRow> iterator();
  public java.lang.String toString();
}
```

## `cn.hutool.core.text.csv.CsvParser`

```java
public final class cn.hutool.core.text.csv.CsvParser extends cn.hutool.core.collection.ComputeIter<cn.hutool.core.text.csv.CsvRow> implements java.io.Closeable, java.io.Serializable {
  public cn.hutool.core.text.csv.CsvParser(java.io.Reader, cn.hutool.core.text.csv.CsvReadConfig);
  public java.util.List<java.lang.String> getHeader();
  public cn.hutool.core.text.csv.CsvRow nextRow() throws cn.hutool.core.io.IORuntimeException;
  public void close() throws java.io.IOException;
}
```

## `cn.hutool.core.text.csv.CsvReadConfig`

```java
public class cn.hutool.core.text.csv.CsvReadConfig extends cn.hutool.core.text.csv.CsvConfig<cn.hutool.core.text.csv.CsvReadConfig> implements java.io.Serializable {
  public cn.hutool.core.text.csv.CsvReadConfig();
  public static cn.hutool.core.text.csv.CsvReadConfig defaultConfig();
  public cn.hutool.core.text.csv.CsvReadConfig setContainsHeader(boolean);
  public cn.hutool.core.text.csv.CsvReadConfig setHeaderLineNo(long);
  public cn.hutool.core.text.csv.CsvReadConfig setSkipEmptyRows(boolean);
  public cn.hutool.core.text.csv.CsvReadConfig setErrorOnDifferentFieldCount(boolean);
  public cn.hutool.core.text.csv.CsvReadConfig setBeginLineNo(long);
  public cn.hutool.core.text.csv.CsvReadConfig setEndLineNo(long);
  public cn.hutool.core.text.csv.CsvReadConfig setTrimField(boolean);
}
```

## `cn.hutool.core.text.csv.CsvReader`

```java
public class cn.hutool.core.text.csv.CsvReader extends cn.hutool.core.text.csv.CsvBaseReader implements java.lang.Iterable<cn.hutool.core.text.csv.CsvRow>, java.io.Closeable {
  public cn.hutool.core.text.csv.CsvReader();
  public cn.hutool.core.text.csv.CsvReader(cn.hutool.core.text.csv.CsvReadConfig);
  public cn.hutool.core.text.csv.CsvReader(java.io.File, cn.hutool.core.text.csv.CsvReadConfig);
  public cn.hutool.core.text.csv.CsvReader(java.nio.file.Path, cn.hutool.core.text.csv.CsvReadConfig);
  public cn.hutool.core.text.csv.CsvReader(java.io.File, java.nio.charset.Charset, cn.hutool.core.text.csv.CsvReadConfig);
  public cn.hutool.core.text.csv.CsvReader(java.nio.file.Path, java.nio.charset.Charset, cn.hutool.core.text.csv.CsvReadConfig);
  public cn.hutool.core.text.csv.CsvReader(java.io.Reader, cn.hutool.core.text.csv.CsvReadConfig);
  public cn.hutool.core.text.csv.CsvData read() throws cn.hutool.core.io.IORuntimeException;
  public void read(cn.hutool.core.text.csv.CsvRowHandler) throws cn.hutool.core.io.IORuntimeException;
  public java.util.stream.Stream<cn.hutool.core.text.csv.CsvRow> stream();
  public java.util.Iterator<cn.hutool.core.text.csv.CsvRow> iterator();
  public void close() throws java.io.IOException;
}
```

## `cn.hutool.core.text.csv.CsvRow`

```java
public final class cn.hutool.core.text.csv.CsvRow implements java.util.List<java.lang.String> {
  public cn.hutool.core.text.csv.CsvRow(long, java.util.Map<java.lang.String, java.lang.Integer>, java.util.List<java.lang.String>);
  public long getOriginalLineNumber();
  public java.lang.String getByName(java.lang.String);
  public java.util.List<java.lang.String> getRawList();
  public java.util.Map<java.lang.String, java.lang.String> getFieldMap();
  public <T> T toBean(java.lang.Class<T>);
  public int getFieldCount();
  public int size();
  public boolean isEmpty();
  public boolean contains(java.lang.Object);
  public java.util.Iterator<java.lang.String> iterator();
  public java.lang.Object[] toArray();
  public <T> T[] toArray(T[]);
  public boolean add(java.lang.String);
  public boolean remove(java.lang.Object);
  public boolean containsAll(java.util.Collection<?>);
  public boolean addAll(java.util.Collection<? extends java.lang.String>);
  public boolean addAll(int, java.util.Collection<? extends java.lang.String>);
  public boolean removeAll(java.util.Collection<?>);
  public boolean retainAll(java.util.Collection<?>);
  public void clear();
  public java.lang.String get(int);
  public java.lang.String set(int, java.lang.String);
  public void add(int, java.lang.String);
  public java.lang.String remove(int);
  public int indexOf(java.lang.Object);
  public int lastIndexOf(java.lang.Object);
  public java.util.ListIterator<java.lang.String> listIterator();
  public java.util.ListIterator<java.lang.String> listIterator(int);
  public java.util.List<java.lang.String> subList(int, int);
  public java.lang.String toString();
  public java.lang.Object remove(int);
  public void add(int, java.lang.Object);
  public java.lang.Object set(int, java.lang.Object);
  public java.lang.Object get(int);
  public boolean add(java.lang.Object);
}
```

## `cn.hutool.core.text.csv.CsvRowHandler`

```java
public interface cn.hutool.core.text.csv.CsvRowHandler {
  public abstract void handle(cn.hutool.core.text.csv.CsvRow);
}
```

## `cn.hutool.core.text.csv.CsvTokener`

```java
public class cn.hutool.core.text.csv.CsvTokener implements java.io.Closeable {
  public cn.hutool.core.text.csv.CsvTokener(java.io.Reader);
  public int next();
  public void back() throws java.lang.IllegalStateException;
  public long getIndex();
  public void close() throws java.io.IOException;
}
```

## `cn.hutool.core.text.csv.CsvUtil`

```java
public class cn.hutool.core.text.csv.CsvUtil {
  public cn.hutool.core.text.csv.CsvUtil();
  public static cn.hutool.core.text.csv.CsvReader getReader(cn.hutool.core.text.csv.CsvReadConfig);
  public static cn.hutool.core.text.csv.CsvReader getReader();
  public static cn.hutool.core.text.csv.CsvReader getReader(java.io.Reader, cn.hutool.core.text.csv.CsvReadConfig);
  public static cn.hutool.core.text.csv.CsvReader getReader(java.io.Reader);
  public static cn.hutool.core.text.csv.CsvWriter getWriter(java.lang.String, java.nio.charset.Charset);
  public static cn.hutool.core.text.csv.CsvWriter getWriter(java.io.File, java.nio.charset.Charset);
  public static cn.hutool.core.text.csv.CsvWriter getWriter(java.lang.String, java.nio.charset.Charset, boolean);
  public static cn.hutool.core.text.csv.CsvWriter getWriter(java.io.File, java.nio.charset.Charset, boolean);
  public static cn.hutool.core.text.csv.CsvWriter getWriter(java.io.File, java.nio.charset.Charset, boolean, cn.hutool.core.text.csv.CsvWriteConfig);
  public static cn.hutool.core.text.csv.CsvWriter getWriter(java.io.Writer);
  public static cn.hutool.core.text.csv.CsvWriter getWriter(java.io.Writer, cn.hutool.core.text.csv.CsvWriteConfig);
}
```

## `cn.hutool.core.text.csv.CsvWriteConfig`

```java
public class cn.hutool.core.text.csv.CsvWriteConfig extends cn.hutool.core.text.csv.CsvConfig<cn.hutool.core.text.csv.CsvWriteConfig> implements java.io.Serializable {
  public cn.hutool.core.text.csv.CsvWriteConfig();
  public static cn.hutool.core.text.csv.CsvWriteConfig defaultConfig();
  public cn.hutool.core.text.csv.CsvWriteConfig setAlwaysDelimitText(boolean);
  public cn.hutool.core.text.csv.CsvWriteConfig setLineDelimiter(char[]);
  public cn.hutool.core.text.csv.CsvWriteConfig setEndingLineBreak(boolean);
}
```

## `cn.hutool.core.text.csv.CsvWriter`

```java
public final class cn.hutool.core.text.csv.CsvWriter implements java.io.Closeable,java.io.Flushable,java.io.Serializable {
  public cn.hutool.core.text.csv.CsvWriter(java.lang.String);
  public cn.hutool.core.text.csv.CsvWriter(java.io.File);
  public cn.hutool.core.text.csv.CsvWriter(java.lang.String, java.nio.charset.Charset);
  public cn.hutool.core.text.csv.CsvWriter(java.io.File, java.nio.charset.Charset);
  public cn.hutool.core.text.csv.CsvWriter(java.lang.String, java.nio.charset.Charset, boolean);
  public cn.hutool.core.text.csv.CsvWriter(java.io.File, java.nio.charset.Charset, boolean);
  public cn.hutool.core.text.csv.CsvWriter(java.lang.String, java.nio.charset.Charset, boolean, cn.hutool.core.text.csv.CsvWriteConfig);
  public cn.hutool.core.text.csv.CsvWriter(java.io.File, java.nio.charset.Charset, boolean, cn.hutool.core.text.csv.CsvWriteConfig);
  public cn.hutool.core.text.csv.CsvWriter(java.io.Writer);
  public cn.hutool.core.text.csv.CsvWriter(java.io.Writer, cn.hutool.core.text.csv.CsvWriteConfig);
  public cn.hutool.core.text.csv.CsvWriter setAlwaysDelimitText(boolean);
  public cn.hutool.core.text.csv.CsvWriter setLineDelimiter(char[]);
  public cn.hutool.core.text.csv.CsvWriter write(java.lang.String[]...) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.text.csv.CsvWriter write(java.lang.Iterable<?>) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.text.csv.CsvWriter write(cn.hutool.core.text.csv.CsvData);
  public cn.hutool.core.text.csv.CsvWriter writeBeans(java.lang.Iterable<?>);
  public cn.hutool.core.text.csv.CsvWriter writeBeans(java.lang.Iterable<?>, java.lang.String...);
  public cn.hutool.core.text.csv.CsvWriter writeBeans(java.lang.Iterable<?>, boolean, java.lang.String...);
  public cn.hutool.core.text.csv.CsvWriter writeHeaderLine(java.lang.String...) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.text.csv.CsvWriter writeLine(java.lang.String...) throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.text.csv.CsvWriter writeLine() throws cn.hutool.core.io.IORuntimeException;
  public cn.hutool.core.text.csv.CsvWriter writeComment(java.lang.String);
  public void close();
  public void flush() throws cn.hutool.core.io.IORuntimeException;
}
```
