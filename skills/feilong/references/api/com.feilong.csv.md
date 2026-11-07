# com.feilong.csv

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.csv.CsvWrite`

```java
public interface com.feilong.csv.CsvWrite {
  public abstract <T> void write(java.lang.String, java.lang.Iterable<T>);
  public abstract <T> void write(java.lang.String, java.lang.Iterable<T>, com.feilong.csv.entity.BeanCsvConfig<T>);
  public abstract void write(java.lang.String, java.lang.String[], java.util.List<java.lang.Object[]>);
  public abstract void write(java.lang.String, java.lang.String[], java.util.List<java.lang.Object[]>, com.feilong.csv.entity.CsvConfig);
}
```

## `com.feilong.csv.DefaultCsvWrite`

```java
public class com.feilong.csv.DefaultCsvWrite implements com.feilong.csv.CsvWrite {
  public com.feilong.csv.DefaultCsvWrite();
  public <T> void write(java.lang.String, java.lang.Iterable<T>);
  public <T> void write(java.lang.String, java.lang.Iterable<T>, com.feilong.csv.entity.BeanCsvConfig<T>);
  public void write(java.lang.String, java.lang.String[], java.util.List<java.lang.Object[]>);
  public void write(java.lang.String, java.lang.String[], java.util.List<java.lang.Object[]>, com.feilong.csv.entity.CsvConfig);
}
```
