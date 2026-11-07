# com.feilong.excel.util

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.excel.util.CellReferenceUtil`

```java
public class com.feilong.excel.util.CellReferenceUtil {
  public static java.lang.String getCellRef(int, int);
  public static java.lang.String getCellRef(java.lang.String, int, int);
  public static int[] getCellPosition(java.lang.String);
}
```

## `com.feilong.excel.util.CloneUtil`

```java
public class com.feilong.excel.util.CloneUtil {
  public static java.util.Map<java.lang.String, java.lang.Object> cloneMap(java.util.Map<java.lang.String, java.lang.Object>) throws java.lang.InstantiationException, java.lang.IllegalAccessException;
}
```

## `com.feilong.excel.util.Config`

```java
public class com.feilong.excel.util.Config {
  public static java.lang.String get(java.lang.String);
}
```

## `com.feilong.excel.util.SheetNamesUtil`

```java
public class com.feilong.excel.util.SheetNamesUtil {
  public static boolean isEmptyOrNullElement(java.lang.String...);
}
```

## `com.feilong.excel.util.WorkbookUtil`

```java
public class com.feilong.excel.util.WorkbookUtil {
  public static org.apache.poi.ss.usermodel.Workbook create(java.io.InputStream);
  public static void write(org.apache.poi.ss.usermodel.Workbook, java.io.OutputStream);
}
```
