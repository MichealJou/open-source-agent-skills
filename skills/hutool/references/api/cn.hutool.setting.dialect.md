# cn.hutool.setting.dialect

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.setting.dialect.Props`

```java
public final class cn.hutool.setting.dialect.Props extends java.util.Properties implements cn.hutool.core.getter.BasicTypeGetter<java.lang.String>, cn.hutool.core.getter.OptBasicTypeGetter<java.lang.String> {
  public static cn.hutool.setting.dialect.Props create();
  public static cn.hutool.setting.dialect.Props getProp(java.lang.String);
  public static cn.hutool.setting.dialect.Props getProp(java.lang.String, java.lang.String);
  public static cn.hutool.setting.dialect.Props getProp(java.lang.String, java.nio.charset.Charset);
  public cn.hutool.setting.dialect.Props();
  public cn.hutool.setting.dialect.Props(java.lang.String);
  public cn.hutool.setting.dialect.Props(java.lang.String, java.lang.String);
  public cn.hutool.setting.dialect.Props(java.lang.String, java.nio.charset.Charset);
  public cn.hutool.setting.dialect.Props(java.io.File);
  public cn.hutool.setting.dialect.Props(java.io.File, java.lang.String);
  public cn.hutool.setting.dialect.Props(java.io.File, java.nio.charset.Charset);
  public cn.hutool.setting.dialect.Props(java.lang.String, java.lang.Class<?>);
  public cn.hutool.setting.dialect.Props(java.lang.String, java.lang.Class<?>, java.lang.String);
  public cn.hutool.setting.dialect.Props(java.lang.String, java.lang.Class<?>, java.nio.charset.Charset);
  public cn.hutool.setting.dialect.Props(java.net.URL);
  public cn.hutool.setting.dialect.Props(java.net.URL, java.lang.String);
  public cn.hutool.setting.dialect.Props(java.net.URL, java.nio.charset.Charset);
  public cn.hutool.setting.dialect.Props(java.util.Properties);
  public void load(java.net.URL);
  public void load(cn.hutool.core.io.resource.Resource);
  public void load();
  public void autoLoad(boolean);
  public java.lang.Object getObj(java.lang.String, java.lang.Object);
  public java.lang.Object getObj(java.lang.String);
  public java.lang.String getStr(java.lang.String, java.lang.String);
  public java.lang.String getStr(java.lang.String);
  public java.lang.Integer getInt(java.lang.String, java.lang.Integer);
  public java.lang.Integer getInt(java.lang.String);
  public java.lang.Boolean getBool(java.lang.String, java.lang.Boolean);
  public java.lang.Boolean getBool(java.lang.String);
  public java.lang.Long getLong(java.lang.String, java.lang.Long);
  public java.lang.Long getLong(java.lang.String);
  public java.lang.Character getChar(java.lang.String, java.lang.Character);
  public java.lang.Character getChar(java.lang.String);
  public java.lang.Float getFloat(java.lang.String);
  public java.lang.Float getFloat(java.lang.String, java.lang.Float);
  public java.lang.Double getDouble(java.lang.String, java.lang.Double) throws java.lang.NumberFormatException;
  public java.lang.Double getDouble(java.lang.String) throws java.lang.NumberFormatException;
  public java.lang.Short getShort(java.lang.String, java.lang.Short);
  public java.lang.Short getShort(java.lang.String);
  public java.lang.Byte getByte(java.lang.String, java.lang.Byte);
  public java.lang.Byte getByte(java.lang.String);
  public java.math.BigDecimal getBigDecimal(java.lang.String, java.math.BigDecimal);
  public java.math.BigDecimal getBigDecimal(java.lang.String);
  public java.math.BigInteger getBigInteger(java.lang.String, java.math.BigInteger);
  public java.math.BigInteger getBigInteger(java.lang.String);
  public <E extends java.lang.Enum<E>> E getEnum(java.lang.Class<E>, java.lang.String, E);
  public <E extends java.lang.Enum<E>> E getEnum(java.lang.Class<E>, java.lang.String);
  public java.util.Date getDate(java.lang.String, java.util.Date);
  public java.util.Date getDate(java.lang.String);
  public java.lang.String getAndRemoveStr(java.lang.String...);
  public java.util.Properties toProperties();
  public <T> T toBean(java.lang.Class<T>);
  public <T> T toBean(java.lang.Class<T>, java.lang.String);
  public <T> T fillBean(T, java.lang.String);
  public void setProperty(java.lang.String, java.lang.Object);
  public void store(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public void store(java.lang.String, java.lang.Class<?>);
  public java.util.Date getDate(java.lang.Object);
  public java.lang.Enum getEnum(java.lang.Class, java.lang.Object);
  public java.math.BigInteger getBigInteger(java.lang.Object);
  public java.math.BigDecimal getBigDecimal(java.lang.Object);
  public java.lang.Byte getByte(java.lang.Object);
  public java.lang.Double getDouble(java.lang.Object);
  public java.lang.Float getFloat(java.lang.Object);
  public java.lang.Character getChar(java.lang.Object);
  public java.lang.Long getLong(java.lang.Object);
  public java.lang.Boolean getBool(java.lang.Object);
  public java.lang.Short getShort(java.lang.Object);
  public java.lang.Integer getInt(java.lang.Object);
  public java.lang.String getStr(java.lang.Object);
  public java.lang.Object getObj(java.lang.Object);
  public java.util.Date getDate(java.lang.Object, java.util.Date);
  public java.lang.Enum getEnum(java.lang.Class, java.lang.Object, java.lang.Enum);
  public java.math.BigInteger getBigInteger(java.lang.Object, java.math.BigInteger);
  public java.math.BigDecimal getBigDecimal(java.lang.Object, java.math.BigDecimal);
  public java.lang.Byte getByte(java.lang.Object, java.lang.Byte);
  public java.lang.Double getDouble(java.lang.Object, java.lang.Double);
  public java.lang.Float getFloat(java.lang.Object, java.lang.Float);
  public java.lang.Character getChar(java.lang.Object, java.lang.Character);
  public java.lang.Long getLong(java.lang.Object, java.lang.Long);
  public java.lang.Boolean getBool(java.lang.Object, java.lang.Boolean);
  public java.lang.Short getShort(java.lang.Object, java.lang.Short);
  public java.lang.Integer getInt(java.lang.Object, java.lang.Integer);
  public java.lang.String getStr(java.lang.Object, java.lang.String);
  public java.lang.Object getObj(java.lang.Object, java.lang.Object);
}
```

## `cn.hutool.setting.dialect.PropsUtil`

```java
public class cn.hutool.setting.dialect.PropsUtil {
  public cn.hutool.setting.dialect.PropsUtil();
  public static cn.hutool.setting.dialect.Props get(java.lang.String);
  public static cn.hutool.setting.dialect.Props getFirstFound(java.lang.String...);
  public static cn.hutool.setting.dialect.Props getSystemProps();
}
```
