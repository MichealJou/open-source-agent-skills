# cn.hutool.poi.excel.sax.handler

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.poi.excel.sax.handler.AbstractRowHandler`

```java
public abstract class cn.hutool.poi.excel.sax.handler.AbstractRowHandler<T> implements cn.hutool.poi.excel.sax.handler.RowHandler {
  public cn.hutool.poi.excel.sax.handler.AbstractRowHandler(int, int);
  public void handle(int, long, java.util.List<java.lang.Object>);
  public abstract void handleData(int, long, T);
}
```

## `cn.hutool.poi.excel.sax.handler.BeanRowHandler`

```java
public abstract class cn.hutool.poi.excel.sax.handler.BeanRowHandler<T> extends cn.hutool.poi.excel.sax.handler.AbstractRowHandler<T> {
  public cn.hutool.poi.excel.sax.handler.BeanRowHandler(int, int, int, java.lang.Class<T>);
  public void handle(int, long, java.util.List<java.lang.Object>);
}
```

## `cn.hutool.poi.excel.sax.handler.MapRowHandler`

```java
public abstract class cn.hutool.poi.excel.sax.handler.MapRowHandler extends cn.hutool.poi.excel.sax.handler.AbstractRowHandler<java.util.Map<java.lang.String, java.lang.Object>> {
  public cn.hutool.poi.excel.sax.handler.MapRowHandler(int, int, int);
  public void handle(int, long, java.util.List<java.lang.Object>);
}
```

## `cn.hutool.poi.excel.sax.handler.RowHandler`

```java
public interface cn.hutool.poi.excel.sax.handler.RowHandler {
  public abstract void handle(int, long, java.util.List<java.lang.Object>);
  public default void handleCell(int, long, int, java.lang.Object, org.apache.poi.ss.usermodel.CellStyle);
  public default void doAfterAllAnalysed();
}
```
