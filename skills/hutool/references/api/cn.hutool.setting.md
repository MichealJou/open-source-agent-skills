# cn.hutool.setting

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.setting.AbsSetting`

```java
public abstract class cn.hutool.setting.AbsSetting implements cn.hutool.core.getter.OptNullBasicTypeFromStringGetter<java.lang.String>, java.io.Serializable {
  public cn.hutool.setting.AbsSetting();
  public java.lang.String getStr(java.lang.String, java.lang.String);
  public java.lang.String getStr(java.lang.String, java.lang.String, java.lang.String);
  public java.lang.String getStrNotEmpty(java.lang.String, java.lang.String, java.lang.String);
  public abstract java.lang.String getByGroup(java.lang.String, java.lang.String);
  public java.lang.String getWithLog(java.lang.String);
  public java.lang.String getByGroupWithLog(java.lang.String, java.lang.String);
  public java.lang.String[] getStrings(java.lang.String);
  public java.lang.String[] getStringsWithDefault(java.lang.String, java.lang.String[]);
  public java.lang.String[] getStrings(java.lang.String, java.lang.String);
  public java.lang.String[] getStrings(java.lang.String, java.lang.String, java.lang.String);
  public java.lang.Integer getInt(java.lang.String, java.lang.String);
  public java.lang.Integer getInt(java.lang.String, java.lang.String, java.lang.Integer);
  public java.lang.Boolean getBool(java.lang.String, java.lang.String);
  public java.lang.Boolean getBool(java.lang.String, java.lang.String, java.lang.Boolean);
  public java.lang.Long getLong(java.lang.String, java.lang.String);
  public java.lang.Long getLong(java.lang.String, java.lang.String, java.lang.Long);
  public java.lang.Character getChar(java.lang.String, java.lang.String);
  public java.lang.Double getDouble(java.lang.String, java.lang.String);
  public java.lang.Double getDouble(java.lang.String, java.lang.String, java.lang.Double);
  public <T> T toBean(java.lang.String, T);
  public <T> T toBean(java.lang.String, java.lang.Class<T>);
  public <T> T toBean(T);
  public <T> T toBean(java.lang.Class<T>);
  public java.lang.String getStr(java.lang.Object, java.lang.String);
}
```

## `cn.hutool.setting.GroupedMap`

```java
public class cn.hutool.setting.GroupedMap extends java.util.LinkedHashMap<java.lang.String, java.util.LinkedHashMap<java.lang.String, java.lang.String>> {
  public cn.hutool.setting.GroupedMap();
  public java.lang.String get(java.lang.String, java.lang.String);
  public java.util.LinkedHashMap<java.lang.String, java.lang.String> get(java.lang.Object);
  public int size();
  public java.lang.String put(java.lang.String, java.lang.String, java.lang.String);
  public cn.hutool.setting.GroupedMap putAll(java.lang.String, java.util.Map<? extends java.lang.String, ? extends java.lang.String>);
  public java.lang.String remove(java.lang.String, java.lang.String);
  public boolean isEmpty(java.lang.String);
  public boolean isEmpty();
  public boolean containsKey(java.lang.String, java.lang.String);
  public boolean containsValue(java.lang.String, java.lang.String);
  public cn.hutool.setting.GroupedMap clear(java.lang.String);
  public java.util.Set<java.lang.String> keySet();
  public java.util.Set<java.lang.String> keySet(java.lang.String);
  public java.util.Collection<java.lang.String> values(java.lang.String);
  public java.util.Set<java.util.Map$Entry<java.lang.String, java.util.LinkedHashMap<java.lang.String, java.lang.String>>> entrySet();
  public java.util.Set<java.util.Map$Entry<java.lang.String, java.lang.String>> entrySet(java.lang.String);
  public java.lang.String toString();
  public java.lang.Object get(java.lang.Object);
}
```

## `cn.hutool.setting.GroupedSet`

```java
public class cn.hutool.setting.GroupedSet extends java.util.HashMap<java.lang.String, java.util.LinkedHashSet<java.lang.String>> {
  public cn.hutool.setting.GroupedSet(java.nio.charset.Charset);
  public cn.hutool.setting.GroupedSet(java.lang.String, java.nio.charset.Charset);
  public cn.hutool.setting.GroupedSet(java.io.File, java.nio.charset.Charset);
  public cn.hutool.setting.GroupedSet(java.lang.String, java.lang.Class<?>, java.nio.charset.Charset);
  public cn.hutool.setting.GroupedSet(java.net.URL, java.nio.charset.Charset);
  public cn.hutool.setting.GroupedSet(java.lang.String);
  public boolean init(java.net.URL, java.nio.charset.Charset);
  public synchronized boolean load(java.net.URL);
  public void reload();
  public boolean load(java.io.InputStream) throws java.io.IOException;
  public java.lang.String getPath();
  public java.util.Set<java.lang.String> getGroups();
  public java.util.LinkedHashSet<java.lang.String> getValues(java.lang.String);
  public boolean contains(java.lang.String, java.lang.String, java.lang.String...);
  public boolean contains(java.lang.String, java.util.Collection<java.lang.String>);
}
```

## `cn.hutool.setting.Setting`

```java
public class cn.hutool.setting.Setting extends cn.hutool.setting.AbsSetting implements java.util.Map<java.lang.String, java.lang.String> {
  public static cn.hutool.setting.Setting create();
  public cn.hutool.setting.Setting();
  public cn.hutool.setting.Setting(java.lang.String);
  public cn.hutool.setting.Setting(java.lang.String, boolean);
  public cn.hutool.setting.Setting(java.lang.String, java.nio.charset.Charset, boolean);
  public cn.hutool.setting.Setting(java.io.File, java.nio.charset.Charset, boolean);
  public cn.hutool.setting.Setting(java.lang.String, java.lang.Class<?>, java.nio.charset.Charset, boolean);
  public cn.hutool.setting.Setting(java.net.URL, java.nio.charset.Charset, boolean);
  public cn.hutool.setting.Setting(cn.hutool.core.io.resource.Resource, java.nio.charset.Charset, boolean);
  public boolean init(cn.hutool.core.io.resource.Resource, java.nio.charset.Charset, boolean);
  public synchronized boolean load();
  public void autoLoad(boolean);
  public void autoLoad(boolean, java.util.function.Consumer<java.lang.Boolean>);
  public java.net.URL getSettingUrl();
  public java.lang.String getSettingPath();
  public int size();
  public java.lang.String getByGroup(java.lang.String, java.lang.String);
  public java.lang.Object getAndRemove(java.lang.String...);
  public java.lang.String getAndRemoveStr(java.lang.String...);
  public java.util.Map<java.lang.String, java.lang.String> getMap(java.lang.String);
  public cn.hutool.setting.Setting getSetting(java.lang.String);
  public java.util.Properties getProperties(java.lang.String);
  public cn.hutool.setting.dialect.Props getProps(java.lang.String);
  public void store();
  public void store(java.lang.String);
  public void store(java.io.File);
  public java.util.Properties toProperties();
  public cn.hutool.setting.GroupedMap getGroupedMap();
  public java.util.List<java.lang.String> getGroups();
  public cn.hutool.setting.Setting setVarRegex(java.lang.String);
  public cn.hutool.setting.Setting setCharset(java.nio.charset.Charset);
  public boolean isEmpty(java.lang.String);
  public boolean containsKey(java.lang.String, java.lang.String);
  public boolean containsValue(java.lang.String, java.lang.String);
  public java.lang.String get(java.lang.String, java.lang.String);
  public java.lang.String putByGroup(java.lang.String, java.lang.String, java.lang.String);
  public java.lang.String remove(java.lang.String, java.lang.Object);
  public cn.hutool.setting.Setting putAll(java.lang.String, java.util.Map<? extends java.lang.String, ? extends java.lang.String>);
  public cn.hutool.setting.Setting addSetting(cn.hutool.setting.Setting);
  public cn.hutool.setting.Setting clear(java.lang.String);
  public java.util.Set<java.lang.String> keySet(java.lang.String);
  public java.util.Collection<java.lang.String> values(java.lang.String);
  public java.util.Set<java.util.Map$Entry<java.lang.String, java.lang.String>> entrySet(java.lang.String);
  public cn.hutool.setting.Setting set(java.lang.String, java.lang.String);
  public cn.hutool.setting.Setting setByGroup(java.lang.String, java.lang.String, java.lang.String);
  public boolean isEmpty();
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public java.lang.String get(java.lang.Object);
  public java.lang.String put(java.lang.String, java.lang.String);
  public java.lang.String remove(java.lang.Object);
  public void putAll(java.util.Map<? extends java.lang.String, ? extends java.lang.String>);
  public void clear();
  public java.util.Set<java.lang.String> keySet();
  public java.util.Collection<java.lang.String> values();
  public java.util.Set<java.util.Map$Entry<java.lang.String, java.lang.String>> entrySet();
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String toString();
  public java.lang.Object remove(java.lang.Object);
  public java.lang.Object put(java.lang.Object, java.lang.Object);
  public java.lang.Object get(java.lang.Object);
}
```

## `cn.hutool.setting.SettingLoader`

```java
public class cn.hutool.setting.SettingLoader {
  public cn.hutool.setting.SettingLoader(cn.hutool.setting.GroupedMap);
  public cn.hutool.setting.SettingLoader(cn.hutool.setting.GroupedMap, java.nio.charset.Charset, boolean);
  public boolean load(cn.hutool.core.io.resource.Resource) throws cn.hutool.core.io.resource.NoResourceException;
  public synchronized boolean load(java.io.InputStream) throws java.io.IOException;
  public void setVarRegex(java.lang.String);
  public void setAssignFlag(char);
  public void store(java.lang.String);
  public void store(java.io.File);
}
```

## `cn.hutool.setting.SettingRuntimeException`

```java
public class cn.hutool.setting.SettingRuntimeException extends java.lang.RuntimeException {
  public cn.hutool.setting.SettingRuntimeException(java.lang.Throwable);
  public cn.hutool.setting.SettingRuntimeException(java.lang.String);
  public cn.hutool.setting.SettingRuntimeException(java.lang.String, java.lang.Object...);
  public cn.hutool.setting.SettingRuntimeException(java.lang.String, java.lang.Throwable);
  public cn.hutool.setting.SettingRuntimeException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.setting.SettingRuntimeException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.setting.SettingUtil`

```java
public class cn.hutool.setting.SettingUtil {
  public cn.hutool.setting.SettingUtil();
  public static cn.hutool.setting.Setting get(java.lang.String);
  public static cn.hutool.setting.Setting getFirstFound(java.lang.String...);
}
```
