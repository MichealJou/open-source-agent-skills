# com.feilong.csv.entity

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.csv.entity.BeanCsvConfig`

```java
public class com.feilong.csv.entity.BeanCsvConfig<T> extends com.feilong.csv.entity.CsvConfig {
  public com.feilong.csv.entity.BeanCsvConfig(java.lang.Class<T>);
  public java.lang.String[] getExcludePropertyNames();
  public void setExcludePropertyNames(java.lang.String...);
  public java.lang.String[] getIncludePropertyNames();
  public void setIncludePropertyNames(java.lang.String...);
  public java.lang.Class<T> getBeanClass();
  public void setBeanClass(java.lang.Class<T>);
}
```

## `com.feilong.csv.entity.CsvColumn`

```java
public interface com.feilong.csv.entity.CsvColumn extends java.lang.annotation.Annotation {
  public abstract java.lang.String name();
  public abstract int order();
}
```

## `com.feilong.csv.entity.CsvColumnEntity`

```java
public class com.feilong.csv.entity.CsvColumnEntity {
  public com.feilong.csv.entity.CsvColumnEntity(java.lang.String, java.lang.String, int);
  public java.lang.String getName();
  public void setName(java.lang.String);
  public int getOrder();
  public void setOrder(int);
  public java.lang.String getPropertyName();
  public void setPropertyName(java.lang.String);
  public java.lang.String toString();
}
```

## `com.feilong.csv.entity.CsvConfig`

```java
public class com.feilong.csv.entity.CsvConfig {
  public com.feilong.csv.entity.CsvConfig();
  public com.feilong.csv.entity.CsvConfig(java.lang.String);
  public com.feilong.csv.entity.CsvConfig(java.lang.String, char);
  public java.lang.String getEncode();
  public void setEncode(java.lang.String);
  public char getSeparator();
  public void setSeparator(char);
  public boolean getIsPrintHeaderLine();
  public void setIsPrintHeaderLine(boolean);
}
```
