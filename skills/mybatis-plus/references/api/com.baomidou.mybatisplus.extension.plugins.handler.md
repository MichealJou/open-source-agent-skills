# com.baomidou.mybatisplus.extension.plugins.handler

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.plugins.handler.DataPermissionHandler`

```java
public interface com.baomidou.mybatisplus.extension.plugins.handler.DataPermissionHandler {
  public abstract net.sf.jsqlparser.expression.Expression getSqlSegment(net.sf.jsqlparser.expression.Expression, java.lang.String);
}
```

## `com.baomidou.mybatisplus.extension.plugins.handler.MultiDataPermissionHandler`

```java
public interface com.baomidou.mybatisplus.extension.plugins.handler.MultiDataPermissionHandler extends com.baomidou.mybatisplus.extension.plugins.handler.DataPermissionHandler {
  public default net.sf.jsqlparser.expression.Expression getSqlSegment(net.sf.jsqlparser.expression.Expression, java.lang.String);
  public abstract net.sf.jsqlparser.expression.Expression getSqlSegment(net.sf.jsqlparser.schema.Table, net.sf.jsqlparser.expression.Expression, java.lang.String);
}
```

## `com.baomidou.mybatisplus.extension.plugins.handler.TableNameHandler`

```java
public interface com.baomidou.mybatisplus.extension.plugins.handler.TableNameHandler {
  public abstract java.lang.String dynamicTableName(java.lang.String, java.lang.String);
}
```

## `com.baomidou.mybatisplus.extension.plugins.handler.TenantLineHandler`

```java
public interface com.baomidou.mybatisplus.extension.plugins.handler.TenantLineHandler {
  public abstract net.sf.jsqlparser.expression.Expression getTenantId();
  public default java.lang.String getTenantIdColumn();
  public default boolean ignoreTable(java.lang.String);
  public default boolean ignoreInsert(java.util.List<net.sf.jsqlparser.schema.Column>, java.lang.String);
}
```
