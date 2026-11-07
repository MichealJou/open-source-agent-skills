# cn.hutool.db.handler

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.db.handler.BeanHandler`

```java
public class cn.hutool.db.handler.BeanHandler<E> implements cn.hutool.db.handler.RsHandler<E> {
  public static <E> cn.hutool.db.handler.BeanHandler<E> create(java.lang.Class<E>);
  public cn.hutool.db.handler.BeanHandler(java.lang.Class<E>);
  public E handle(java.sql.ResultSet) throws java.sql.SQLException;
}
```

## `cn.hutool.db.handler.BeanListHandler`

```java
public class cn.hutool.db.handler.BeanListHandler<E> implements cn.hutool.db.handler.RsHandler<java.util.List<E>> {
  public static <E> cn.hutool.db.handler.BeanListHandler<E> create(java.lang.Class<E>);
  public cn.hutool.db.handler.BeanListHandler(java.lang.Class<E>);
  public java.util.List<E> handle(java.sql.ResultSet) throws java.sql.SQLException;
  public java.lang.Object handle(java.sql.ResultSet) throws java.sql.SQLException;
}
```

## `cn.hutool.db.handler.EntityHandler`

```java
public class cn.hutool.db.handler.EntityHandler implements cn.hutool.db.handler.RsHandler<cn.hutool.db.Entity> {
  public static cn.hutool.db.handler.EntityHandler create();
  public cn.hutool.db.handler.EntityHandler();
  public cn.hutool.db.handler.EntityHandler(boolean);
  public cn.hutool.db.Entity handle(java.sql.ResultSet) throws java.sql.SQLException;
  public java.lang.Object handle(java.sql.ResultSet) throws java.sql.SQLException;
}
```

## `cn.hutool.db.handler.EntityListHandler`

```java
public class cn.hutool.db.handler.EntityListHandler implements cn.hutool.db.handler.RsHandler<java.util.List<cn.hutool.db.Entity>> {
  public static cn.hutool.db.handler.EntityListHandler create();
  public cn.hutool.db.handler.EntityListHandler();
  public cn.hutool.db.handler.EntityListHandler(boolean);
  public java.util.List<cn.hutool.db.Entity> handle(java.sql.ResultSet) throws java.sql.SQLException;
  public java.lang.Object handle(java.sql.ResultSet) throws java.sql.SQLException;
}
```

## `cn.hutool.db.handler.EntitySetHandler`

```java
public class cn.hutool.db.handler.EntitySetHandler implements cn.hutool.db.handler.RsHandler<java.util.LinkedHashSet<cn.hutool.db.Entity>> {
  public static cn.hutool.db.handler.EntitySetHandler create();
  public cn.hutool.db.handler.EntitySetHandler();
  public cn.hutool.db.handler.EntitySetHandler(boolean);
  public java.util.LinkedHashSet<cn.hutool.db.Entity> handle(java.sql.ResultSet) throws java.sql.SQLException;
  public java.lang.Object handle(java.sql.ResultSet) throws java.sql.SQLException;
}
```

## `cn.hutool.db.handler.HandleHelper`

```java
public class cn.hutool.db.handler.HandleHelper {
  public cn.hutool.db.handler.HandleHelper();
  public static <T> T handleRow(int, java.sql.ResultSetMetaData, java.sql.ResultSet, T) throws java.sql.SQLException;
  public static <T> T handleRow(int, java.sql.ResultSetMetaData, java.sql.ResultSet, java.lang.Class<T>) throws java.sql.SQLException;
  public static cn.hutool.db.Entity handleRow(int, java.sql.ResultSetMetaData, java.sql.ResultSet) throws java.sql.SQLException;
  public static cn.hutool.db.Entity handleRow(int, java.sql.ResultSetMetaData, java.sql.ResultSet, boolean) throws java.sql.SQLException;
  public static <T extends cn.hutool.db.Entity> T handleRow(T, int, java.sql.ResultSetMetaData, java.sql.ResultSet, boolean) throws java.sql.SQLException;
  public static cn.hutool.db.Entity handleRow(java.sql.ResultSet) throws java.sql.SQLException;
  public static java.util.List<java.lang.Object> handleRowToList(java.sql.ResultSet) throws java.sql.SQLException;
  public static <T extends java.util.Collection<cn.hutool.db.Entity>> T handleRs(java.sql.ResultSet, T) throws java.sql.SQLException;
  public static <T extends java.util.Collection<cn.hutool.db.Entity>> T handleRs(java.sql.ResultSet, T, boolean) throws java.sql.SQLException;
  public static <E, T extends java.util.Collection<E>> T handleRsToBeanList(java.sql.ResultSet, T, java.lang.Class<E>) throws java.sql.SQLException;
}
```

## `cn.hutool.db.handler.NumberHandler`

```java
public class cn.hutool.db.handler.NumberHandler implements cn.hutool.db.handler.RsHandler<java.lang.Number> {
  public cn.hutool.db.handler.NumberHandler();
  public static cn.hutool.db.handler.NumberHandler create();
  public java.lang.Number handle(java.sql.ResultSet) throws java.sql.SQLException;
  public java.lang.Object handle(java.sql.ResultSet) throws java.sql.SQLException;
}
```

## `cn.hutool.db.handler.PageResultHandler`

```java
public class cn.hutool.db.handler.PageResultHandler implements cn.hutool.db.handler.RsHandler<cn.hutool.db.PageResult<cn.hutool.db.Entity>> {
  public static cn.hutool.db.handler.PageResultHandler create(cn.hutool.db.PageResult<cn.hutool.db.Entity>);
  public cn.hutool.db.handler.PageResultHandler(cn.hutool.db.PageResult<cn.hutool.db.Entity>);
  public cn.hutool.db.handler.PageResultHandler(cn.hutool.db.PageResult<cn.hutool.db.Entity>, boolean);
  public cn.hutool.db.PageResult<cn.hutool.db.Entity> handle(java.sql.ResultSet) throws java.sql.SQLException;
  public java.lang.Object handle(java.sql.ResultSet) throws java.sql.SQLException;
}
```

## `cn.hutool.db.handler.RsHandler`

```java
public interface cn.hutool.db.handler.RsHandler<T> extends java.io.Serializable {
  public abstract T handle(java.sql.ResultSet) throws java.sql.SQLException;
}
```

## `cn.hutool.db.handler.StringHandler`

```java
public class cn.hutool.db.handler.StringHandler implements cn.hutool.db.handler.RsHandler<java.lang.String> {
  public cn.hutool.db.handler.StringHandler();
  public static cn.hutool.db.handler.StringHandler create();
  public java.lang.String handle(java.sql.ResultSet) throws java.sql.SQLException;
  public java.lang.Object handle(java.sql.ResultSet) throws java.sql.SQLException;
}
```

## `cn.hutool.db.handler.ValueListHandler`

```java
public class cn.hutool.db.handler.ValueListHandler implements cn.hutool.db.handler.RsHandler<java.util.List<java.util.List<java.lang.Object>>> {
  public cn.hutool.db.handler.ValueListHandler();
  public static cn.hutool.db.handler.ValueListHandler create();
  public java.util.List<java.util.List<java.lang.Object>> handle(java.sql.ResultSet) throws java.sql.SQLException;
  public java.lang.Object handle(java.sql.ResultSet) throws java.sql.SQLException;
}
```
