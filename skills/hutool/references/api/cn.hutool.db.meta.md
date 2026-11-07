# cn.hutool.db.meta

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.db.meta.Column`

```java
public class cn.hutool.db.meta.Column implements java.io.Serializable,java.lang.Cloneable {
  public static cn.hutool.db.meta.Column create(cn.hutool.db.meta.Table, java.sql.ResultSet);
  public cn.hutool.db.meta.Column();
  public cn.hutool.db.meta.Column(cn.hutool.db.meta.Table, java.sql.ResultSet);
  public void init(cn.hutool.db.meta.Table, java.sql.ResultSet) throws java.sql.SQLException;
  public java.lang.String getTableName();
  public cn.hutool.db.meta.Column setTableName(java.lang.String);
  public java.lang.String getName();
  public cn.hutool.db.meta.Column setName(java.lang.String);
  public cn.hutool.db.meta.JdbcType getTypeEnum();
  public int getType();
  public cn.hutool.db.meta.Column setType(int);
  public java.lang.String getTypeName();
  public cn.hutool.db.meta.Column setTypeName(java.lang.String);
  public long getSize();
  public cn.hutool.db.meta.Column setSize(int);
  public java.lang.Integer getDigit();
  public cn.hutool.db.meta.Column setDigit(int);
  public boolean isNullable();
  public cn.hutool.db.meta.Column setNullable(boolean);
  public java.lang.String getComment();
  public cn.hutool.db.meta.Column setComment(java.lang.String);
  public boolean isAutoIncrement();
  public cn.hutool.db.meta.Column setAutoIncrement(boolean);
  public boolean isPk();
  public cn.hutool.db.meta.Column setPk(boolean);
  public java.lang.String getColumnDef();
  public cn.hutool.db.meta.Column setColumnDef(java.lang.String);
  public java.lang.String toString();
  public cn.hutool.db.meta.Column clone() throws java.lang.CloneNotSupportedException;
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `cn.hutool.db.meta.ColumnIndexInfo`

```java
public class cn.hutool.db.meta.ColumnIndexInfo implements java.io.Serializable,java.lang.Cloneable {
  public static cn.hutool.db.meta.ColumnIndexInfo create(java.sql.ResultSet);
  public cn.hutool.db.meta.ColumnIndexInfo(java.lang.String, java.lang.String);
  public java.lang.String getColumnName();
  public void setColumnName(java.lang.String);
  public java.lang.String getAscOrDesc();
  public void setAscOrDesc(java.lang.String);
  public cn.hutool.db.meta.ColumnIndexInfo clone() throws java.lang.CloneNotSupportedException;
  public java.lang.String toString();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `cn.hutool.db.meta.IndexInfo`

```java
public class cn.hutool.db.meta.IndexInfo implements java.io.Serializable,java.lang.Cloneable {
  public cn.hutool.db.meta.IndexInfo(boolean, java.lang.String, java.lang.String, java.lang.String, java.lang.String);
  public boolean isNonUnique();
  public void setNonUnique(boolean);
  public java.lang.String getIndexName();
  public void setIndexName(java.lang.String);
  public java.lang.String getTableName();
  public void setTableName(java.lang.String);
  public java.lang.String getSchema();
  public void setSchema(java.lang.String);
  public java.lang.String getCatalog();
  public void setCatalog(java.lang.String);
  public java.util.List<cn.hutool.db.meta.ColumnIndexInfo> getColumnIndexInfoList();
  public void setColumnIndexInfoList(java.util.List<cn.hutool.db.meta.ColumnIndexInfo>);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public cn.hutool.db.meta.IndexInfo clone() throws java.lang.CloneNotSupportedException;
  public java.lang.String toString();
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `cn.hutool.db.meta.JdbcType`

```java
public final class cn.hutool.db.meta.JdbcType extends java.lang.Enum<cn.hutool.db.meta.JdbcType> {
  public static cn.hutool.db.meta.JdbcType[] values();
  public static cn.hutool.db.meta.JdbcType valueOf(java.lang.String);
  public static cn.hutool.db.meta.JdbcType valueOf(int);
}
```

## `cn.hutool.db.meta.MetaUtil`

```java
public class cn.hutool.db.meta.MetaUtil {
  public cn.hutool.db.meta.MetaUtil();
  public static java.util.List<java.lang.String> getTables(javax.sql.DataSource);
  public static java.util.List<java.lang.String> getTables(javax.sql.DataSource, cn.hutool.db.meta.TableType...);
  public static java.util.List<java.lang.String> getTables(javax.sql.DataSource, java.lang.String, cn.hutool.db.meta.TableType...);
  public static java.util.List<java.lang.String> getTables(javax.sql.DataSource, java.lang.String, java.lang.String, cn.hutool.db.meta.TableType...);
  public static java.lang.String[] getColumnNames(java.sql.ResultSet) throws cn.hutool.db.DbRuntimeException;
  public static java.lang.String[] getColumnNames(javax.sql.DataSource, java.lang.String);
  public static cn.hutool.db.Entity createLimitedEntity(javax.sql.DataSource, java.lang.String);
  public static cn.hutool.db.meta.Table getTableMeta(javax.sql.DataSource, java.lang.String);
  public static cn.hutool.db.meta.Table getTableMeta(javax.sql.DataSource, java.lang.String, java.lang.String, java.lang.String);
  public static cn.hutool.db.meta.Table getTableMeta(java.sql.Connection, java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String getCataLog(java.sql.Connection);
  public static java.lang.String getCatalog(java.sql.Connection);
  public static java.lang.String getSchema(java.sql.Connection);
  public static java.sql.DatabaseMetaData getMetaData(java.sql.Connection);
  public static java.lang.String getRemarks(java.sql.DatabaseMetaData, java.lang.String, java.lang.String, java.lang.String);
  public static java.util.Set<java.lang.String> getPrimaryKeys(java.sql.DatabaseMetaData, java.lang.String, java.lang.String, java.lang.String);
  public static java.util.Map<java.lang.String, cn.hutool.db.meta.IndexInfo> getIndexInfo(java.sql.DatabaseMetaData, java.lang.String, java.lang.String, java.lang.String);
  public static boolean isOracle(java.sql.DatabaseMetaData) throws cn.hutool.db.DbRuntimeException;
}
```

## `cn.hutool.db.meta.Table`

```java
public class cn.hutool.db.meta.Table implements java.io.Serializable,java.lang.Cloneable {
  public static cn.hutool.db.meta.Table create(java.lang.String);
  public cn.hutool.db.meta.Table(java.lang.String);
  public java.lang.String getSchema();
  public cn.hutool.db.meta.Table setSchema(java.lang.String);
  public java.lang.String getCatalog();
  public cn.hutool.db.meta.Table setCatalog(java.lang.String);
  public java.lang.String getTableName();
  public void setTableName(java.lang.String);
  public java.lang.String getComment();
  public cn.hutool.db.meta.Table setComment(java.lang.String);
  public java.util.Set<java.lang.String> getPkNames();
  public boolean isPk(java.lang.String);
  public void setPkNames(java.util.Set<java.lang.String>);
  public cn.hutool.db.meta.Table setColumn(cn.hutool.db.meta.Column);
  public cn.hutool.db.meta.Column getColumn(java.lang.String);
  public java.util.Collection<cn.hutool.db.meta.Column> getColumns();
  public cn.hutool.db.meta.Table addPk(java.lang.String);
  public java.util.List<cn.hutool.db.meta.IndexInfo> getIndexInfoList();
  public void setIndexInfoList(java.util.List<cn.hutool.db.meta.IndexInfo>);
  public cn.hutool.db.meta.Table clone() throws java.lang.CloneNotSupportedException;
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
}
```

## `cn.hutool.db.meta.TableType`

```java
public final class cn.hutool.db.meta.TableType extends java.lang.Enum<cn.hutool.db.meta.TableType> {
  public static cn.hutool.db.meta.TableType[] values();
  public static cn.hutool.db.meta.TableType valueOf(java.lang.String);
  public java.lang.String value();
  public java.lang.String toString();
}
```
