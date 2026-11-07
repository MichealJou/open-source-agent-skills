# com.baomidou.mybatisplus.extension.plugins.pagination

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.plugins.pagination.DialectFactory`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.DialectFactory {
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectFactory();
  public static com.baomidou.mybatisplus.extension.plugins.pagination.dialects.IDialect getDialect(com.baomidou.mybatisplus.annotation.DbType);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel {
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel(java.lang.String);
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel(java.lang.String, long);
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel(java.lang.String, long, long);
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel setConsumer(boolean, java.util.function.Function<java.util.List<org.apache.ibatis.mapping.ParameterMapping>, java.lang.Integer>);
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel setConsumer(boolean);
  public com.baomidou.mybatisplus.extension.plugins.pagination.DialectModel setConsumerChain();
  public void consumers(java.util.List<org.apache.ibatis.mapping.ParameterMapping>, org.apache.ibatis.session.Configuration, java.util.Map<java.lang.String, java.lang.Object>);
  public java.lang.String getDialectSql();
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.Page`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> implements com.baomidou.mybatisplus.core.metadata.IPage<T> {
  public com.baomidou.mybatisplus.extension.plugins.pagination.Page();
  public com.baomidou.mybatisplus.extension.plugins.pagination.Page(long, long);
  public com.baomidou.mybatisplus.extension.plugins.pagination.Page(long, long, long);
  public com.baomidou.mybatisplus.extension.plugins.pagination.Page(long, long, boolean);
  public com.baomidou.mybatisplus.extension.plugins.pagination.Page(long, long, long, boolean);
  public boolean hasPrevious();
  public boolean hasNext();
  public java.util.List<T> getRecords();
  public com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> setRecords(java.util.List<T>);
  public long getTotal();
  public com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> setTotal(long);
  public long getSize();
  public com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> setSize(long);
  public long getCurrent();
  public com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> setCurrent(long);
  public java.lang.String countId();
  public java.lang.Long maxLimit();
  public com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> addOrder(com.baomidou.mybatisplus.core.metadata.OrderItem...);
  public com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> addOrder(java.util.List<com.baomidou.mybatisplus.core.metadata.OrderItem>);
  public java.util.List<com.baomidou.mybatisplus.core.metadata.OrderItem> orders();
  public boolean optimizeCountSql();
  public static <T> com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> of(long, long, long, boolean);
  public boolean optimizeJoinOfCountSql();
  public com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> setSearchCount(boolean);
  public com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> setOptimizeCountSql(boolean);
  public long getPages();
  public static <T> com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> of(long, long);
  public static <T> com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> of(long, long, long);
  public static <T> com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> of(long, long, boolean);
  public boolean searchCount();
  public java.lang.String toString();
  public void setOrders(java.util.List<com.baomidou.mybatisplus.core.metadata.OrderItem>);
  public void setOptimizeJoinOfCountSql(boolean);
  public void setMaxLimit(java.lang.Long);
  public void setCountId(java.lang.String);
  public com.baomidou.mybatisplus.core.metadata.IPage setCurrent(long);
  public com.baomidou.mybatisplus.core.metadata.IPage setSize(long);
  public com.baomidou.mybatisplus.core.metadata.IPage setTotal(long);
  public com.baomidou.mybatisplus.core.metadata.IPage setRecords(java.util.List);
}
```

## `com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO`

```java
public class com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO<T> extends com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> {
  public com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO();
  public com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO(long, long);
  public com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO(long, long, long);
  public com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO(long, long, boolean);
  public com.baomidou.mybatisplus.extension.plugins.pagination.PageDTO(long, long, long, boolean);
  public static <T> com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> of(long, long);
  public static <T> com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> of(long, long, long);
  public static <T> com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> of(long, long, boolean);
  public static <T> com.baomidou.mybatisplus.extension.plugins.pagination.Page<T> of(long, long, long, boolean);
  public java.lang.String getCountId();
  public java.lang.Long getMaxLimit();
  public java.util.List<com.baomidou.mybatisplus.core.metadata.OrderItem> getOrders();
  public boolean isOptimizeCountSql();
  public boolean isSearchCount();
  public boolean isOptimizeJoinOfCountSql();
  public java.lang.String toString();
}
```
