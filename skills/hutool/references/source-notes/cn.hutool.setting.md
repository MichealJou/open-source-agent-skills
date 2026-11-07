# cn.hutool.setting

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.setting.AbsSetting` | `Boolean getBool(String key,String group)` | 获取布尔型属性值 |
| `cn.hutool.setting.AbsSetting` | `Boolean getBool(String key,String group,Boolean defaultValue)` | 获取布尔型属性值 |
| `cn.hutool.setting.AbsSetting` | `Character getChar(String key,String group)` | 获取char类型属性值 |
| `cn.hutool.setting.AbsSetting` | `Double getDouble(String key,String group)` | 获取double类型属性值 |
| `cn.hutool.setting.AbsSetting` | `Double getDouble(String key,String group,Double defaultValue)` | 获取double类型属性值 |
| `cn.hutool.setting.AbsSetting` | `Integer getInt(String key,String group)` | 获取数字型型属性值 |
| `cn.hutool.setting.AbsSetting` | `Integer getInt(String key,String group,Integer defaultValue)` | 获取数字型型属性值 |
| `cn.hutool.setting.AbsSetting` | `Long getLong(String key,String group)` | 获取long类型属性值 |
| `cn.hutool.setting.AbsSetting` | `Long getLong(String key,String group,Long defaultValue)` | 获取long类型属性值 |
| `cn.hutool.setting.AbsSetting` | `String getByGroup(String key,String group)` | 获得指定分组的键对应值 |
| `cn.hutool.setting.AbsSetting` | `String getByGroupWithLog(String key,String group)` | 带有日志提示的get，如果没有定义指定的KEY，则打印debug日志 |
| `cn.hutool.setting.AbsSetting` | `String getStr(String key,String defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.AbsSetting` | `String getStr(String key,String group,String defaultValue)` | 获得字符串类型值 |
| `cn.hutool.setting.AbsSetting` | `String getStrNotEmpty(String key,String group,String defaultValue)` | 获得字符串类型值，如果字符串为null或者""返回默认值 |
| `cn.hutool.setting.AbsSetting` | `String getWithLog(String key)` | 带有日志提示的get，如果没有定义指定的KEY，则打印debug日志 |
| `cn.hutool.setting.AbsSetting` | `String[] getStrings(String key)` | 获得数组型 |
| `cn.hutool.setting.AbsSetting` | `String[] getStrings(String key,String group)` | 获得数组型 |
| `cn.hutool.setting.AbsSetting` | `String[] getStrings(String key,String group,String delimiter)` | 获得数组型 |
| `cn.hutool.setting.AbsSetting` | `String[] getStringsWithDefault(String key,String[] defaultValue)` | 获得数组型 |
| `cn.hutool.setting.AbsSetting` | `T toBean(Class<T> beanClass)` | 将setting中的键值关系映射到对象中，原理是调用对象对应的set方法 只支持基本类型的转换 |
| `cn.hutool.setting.AbsSetting` | `T toBean(String group,Class<T> beanClass)` | 将setting中的键值关系映射到对象中，原理是调用对象对应的set方法 只支持基本类型的转换 |
| `cn.hutool.setting.AbsSetting` | `T toBean(T bean)` | 将setting中的键值关系映射到对象中，原理是调用对象对应的set方法 只支持基本类型的转换 |
| `cn.hutool.setting.AbsSetting` | `T toBean(final String group,T bean)` | 将setting中的键值关系映射到对象中，原理是调用对象对应的set方法 只支持基本类型的转换 |
| `cn.hutool.setting.GroupedMap` | `Collection<String> values(String group)` | 指定分组下所有值 |
| `cn.hutool.setting.GroupedMap` | `GroupedMap clear(String group)` | 清除指定分组下的所有键值对 |
| `cn.hutool.setting.GroupedMap` | `GroupedMap putAll(String group,Map<? extends String, ? extends String> m)` | 加入多个键值对到某个分组下 |
| `cn.hutool.setting.GroupedMap` | `LinkedHashMap<String, String> get(Object key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.GroupedMap` | `Set<Entry<String, String>> entrySet(String group)` | 指定分组下所有键值对 |
| `cn.hutool.setting.GroupedMap` | `Set<String> keySet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.GroupedMap` | `Set<String> keySet(String group)` | 指定分组所有键的Set |
| `cn.hutool.setting.GroupedMap` | `Set<java.util.Map.Entry<String, LinkedHashMap<String, String>>> entrySet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.GroupedMap` | `String get(String group,String key)` | 获取分组对应的值，如果分组不存在或者值不存在则返回null |
| `cn.hutool.setting.GroupedMap` | `String put(String group,String key,String value)` | 将键值对加入到对应分组中 |
| `cn.hutool.setting.GroupedMap` | `String remove(String group,String key)` | 从指定分组中删除指定值 |
| `cn.hutool.setting.GroupedMap` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.GroupedMap` | `boolean containsKey(String group,String key)` | 指定分组中是否包含指定key |
| `cn.hutool.setting.GroupedMap` | `boolean containsValue(String group,String value)` | 指定分组中是否包含指定值 |
| `cn.hutool.setting.GroupedMap` | `boolean isEmpty()` | 是否为空，如果多个分组同时为空，也按照空处理 |
| `cn.hutool.setting.GroupedMap` | `boolean isEmpty(String group)` | 某个分组对应的键值对是否为空 |
| `cn.hutool.setting.GroupedMap` | `int size()` | 总的键值对数 |
| `cn.hutool.setting.GroupedSet` | `LinkedHashSet<String> getValues(String group)` | 获得对应分组的所有值 |
| `cn.hutool.setting.GroupedSet` | `Set<String> getGroups()` | @return 获得所有分组名 |
| `cn.hutool.setting.GroupedSet` | `String getPath()` | @return 获得设定文件的路径 |
| `cn.hutool.setting.GroupedSet` | `boolean contains(String group,Collection<String> values)` | 是否在给定分组的集合中全部包含指定值集合 如果给定分组对应集合不存在，则返回false |
| `cn.hutool.setting.GroupedSet` | `boolean contains(String group,String value,String... otherValues)` | 是否在给定分组的集合中包含指定值 如果给定分组对应集合不存在，则返回false |
| `cn.hutool.setting.GroupedSet` | `boolean init(URL groupedSetUrl,Charset charset)` | 初始化设定文件 |
| `cn.hutool.setting.GroupedSet` | `boolean load(InputStream settingStream)` | 加载设置文件。 此方法不会关闭流对象 |
| `cn.hutool.setting.GroupedSet` | `boolean load(URL groupedSetUrl)` | 加载设置文件 |
| `cn.hutool.setting.GroupedSet` | `void reload()` | 重新加载配置文件 |
| `cn.hutool.setting.Setting` | `Collection<String> values()` | 获取默认分组（空分组）中的所有值列表 |
| `cn.hutool.setting.Setting` | `Collection<String> values(String group)` | 指定分组下所有值 |
| `cn.hutool.setting.Setting` | `GroupedMap getGroupedMap()` | 获取GroupedMap |
| `cn.hutool.setting.Setting` | `List<String> getGroups()` | 获取所有分组 |
| `cn.hutool.setting.Setting` | `Map<String, String> getMap(String group)` | 获得指定分组的所有键值对，此方法获取的是原始键值对，获取的键值对可以被修改 |
| `cn.hutool.setting.Setting` | `Object getAndRemove(String... keys)` | 获取并删除键值对，当指定键对应值非空时，返回并删除这个值，后边的键对应的值不再查找 |
| `cn.hutool.setting.Setting` | `Properties getProperties(String group)` | 获取group分组下所有配置键值对，组成新的Properties |
| `cn.hutool.setting.Setting` | `Properties toProperties()` | 转换为Properties对象，原分组变为前缀 |
| `cn.hutool.setting.Setting` | `Props getProps(String group)` | 获取group分组下所有配置键值对，组成新的Props |
| `cn.hutool.setting.Setting` | `Set<Entry<String, String>> entrySet()` | 获取默认分组（空分组）中的所有键值对列表 |
| `cn.hutool.setting.Setting` | `Set<Entry<String, String>> entrySet(String group)` | 指定分组下所有键值对 |
| `cn.hutool.setting.Setting` | `Set<String> keySet()` | 获取默认分组（空分组）中的所有键列表 |
| `cn.hutool.setting.Setting` | `Set<String> keySet(String group)` | 指定分组所有键的Set |
| `cn.hutool.setting.Setting` | `Setting addSetting(Setting setting)` | 添加一个Stting到主配置中 |
| `cn.hutool.setting.Setting` | `Setting clear(String group)` | 清除指定分组下的所有键值对 |
| `cn.hutool.setting.Setting` | `Setting create()` | 构建一个空的Setting，用于手动加入参数 |
| `cn.hutool.setting.Setting` | `Setting getSetting(String group)` | 获取group分组下所有配置键值对，组成新的Setting |
| `cn.hutool.setting.Setting` | `Setting putAll(String group,Map<? extends String, ? extends String> m)` | 加入多个键值对到某个分组下 |
| `cn.hutool.setting.Setting` | `Setting set(String key,String value)` | 设置值 |
| `cn.hutool.setting.Setting` | `Setting setByGroup(String key,String group,String value)` | 将键值对加入到对应分组中 此方法用于与getXXX统一参数顺序 |
| `cn.hutool.setting.Setting` | `Setting setCharset(Charset charset)` | 自定义字符编码 |
| `cn.hutool.setting.Setting` | `Setting setVarRegex(String regex)` | 设置变量的正则 正则只能有一个group表示变量本身，剩余为字符 例如 \$\{(name)\}表示${name}变量名为name的一个变量表示 |
| `cn.hutool.setting.Setting` | `String get(Object key)` | 获取默认分组（空分组）中指定key对应的值 |
| `cn.hutool.setting.Setting` | `String get(String group,String key)` | 获取分组对应的值，如果分组不存在或者值不存在则返回null |
| `cn.hutool.setting.Setting` | `String getAndRemoveStr(String... keys)` | 获取并删除键值对，当指定键对应值非空时，返回并删除这个值，后边的键对应的值不再查找 |
| `cn.hutool.setting.Setting` | `String getByGroup(String key,String group)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.Setting` | `String getSettingPath()` | 获得设定文件的路径 |
| `cn.hutool.setting.Setting` | `String put(String key,String value)` | 将指定键值对加入到默认分组（空分组）中 |
| `cn.hutool.setting.Setting` | `String putByGroup(String key,String group,String value)` | 将键值对加入到对应分组中 |
| `cn.hutool.setting.Setting` | `String remove(Object key)` | 移除默认分组（空分组）中指定值 |
| `cn.hutool.setting.Setting` | `String remove(String group,Object key)` | 从指定分组中删除指定值 |
| `cn.hutool.setting.Setting` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.Setting` | `URL getSettingUrl()` | 获得设定文件的URL |
| `cn.hutool.setting.Setting` | `boolean containsKey(Object key)` | 默认分组（空分组）中是否包含指定key对应的值 |
| `cn.hutool.setting.Setting` | `boolean containsKey(String group,String key)` | 指定分组中是否包含指定key |
| `cn.hutool.setting.Setting` | `boolean containsValue(Object value)` | 默认分组（空分组）中是否包含指定值 |
| `cn.hutool.setting.Setting` | `boolean containsValue(String group,String value)` | 指定分组中是否包含指定值 |
| `cn.hutool.setting.Setting` | `boolean equals(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.Setting` | `boolean init(Resource resource,Charset charset,boolean isUseVariable)` | 初始化设定文件 |
| `cn.hutool.setting.Setting` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.Setting` | `boolean isEmpty(String group)` | 某个分组对应的键值对是否为空 |
| `cn.hutool.setting.Setting` | `boolean load()` | 重新加载配置文件 |
| `cn.hutool.setting.Setting` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.Setting` | `int size()` | 键值总数 |
| `cn.hutool.setting.Setting` | `void autoLoad(boolean autoReload)` | 在配置文件变更时自动加载 |
| `cn.hutool.setting.Setting` | `void autoLoad(boolean autoReload,Consumer<Boolean> callback)` | 在配置文件变更时自动加载 |
| `cn.hutool.setting.Setting` | `void clear()` | 清空默认分组（空分组）中的所有键值对 |
| `cn.hutool.setting.Setting` | `void putAll(Map<? extends String, ? extends String> m)` | 将键值对Map加入默认分组（空分组）中 |
| `cn.hutool.setting.Setting` | `void store()` | 持久化当前设置，会覆盖掉之前的设置 持久化不会保留之前的分组，注意如果配置文件在jar内部或者在exe中，此方法会报错。 |
| `cn.hutool.setting.Setting` | `void store(File file)` | 持久化当前设置，会覆盖掉之前的设置 持久化不会保留之前的分组 |
| `cn.hutool.setting.Setting` | `void store(String absolutePath)` | 持久化当前设置，会覆盖掉之前的设置 持久化不会保留之前的分组 |
| `cn.hutool.setting.SettingLoader` | `boolean load(InputStream settingStream)` | 加载设置文件。 此方法不会关闭流对象 |
| `cn.hutool.setting.SettingLoader` | `boolean load(Resource resource)` | 加载设置文件 |
| `cn.hutool.setting.SettingLoader` | `void setAssignFlag(char assignFlag)` | 赋值分隔符（用于分隔键值对） |
| `cn.hutool.setting.SettingLoader` | `void setVarRegex(String regex)` | 设置变量的正则 正则只能有一个group表示变量本身，剩余为字符 例如 \$\{(name)\}表示${name}变量名为name的一个变量表示 |
| `cn.hutool.setting.SettingLoader` | `void store(File file)` | 持久化当前设置，会覆盖掉之前的设置 持久化会不会保留之前的分组 |
| `cn.hutool.setting.SettingLoader` | `void store(String absolutePath)` | 持久化当前设置，会覆盖掉之前的设置 持久化会不会保留之前的分组 |
| `cn.hutool.setting.SettingUtil` | `Setting get(String name)` | 获取当前环境下的配置文件 name可以为不包括扩展名的文件名（默认.setting为结尾），也可以是文件名全称 |
| `cn.hutool.setting.SettingUtil` | `Setting getFirstFound(String... names)` | 获取给定路径找到的第一个配置文件 * name可以为不包括扩展名的文件名（默认.setting为结尾），也可以是文件名全称 |
