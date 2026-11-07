# cn.hutool.setting.dialect

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.setting.dialect.Props` | `BigDecimal getBigDecimal(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `BigDecimal getBigDecimal(String key,BigDecimal defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `BigInteger getBigInteger(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `BigInteger getBigInteger(String key,BigInteger defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Boolean getBool(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Boolean getBool(String key,Boolean defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Byte getByte(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Byte getByte(String key,Byte defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Character getChar(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Character getChar(String key,Character defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Date getDate(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Date getDate(String key,Date defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Double getDouble(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Double getDouble(String key,Double defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `E getEnum(Class<E> clazz,String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `E getEnum(Class<E> clazz,String key,E defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Float getFloat(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Float getFloat(String key,Float defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Integer getInt(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Integer getInt(String key,Integer defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Long getLong(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Long getLong(String key,Long defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Object getObj(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Object getObj(String key,Object defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Properties toProperties()` | 转换为标准的Properties对象 |
| `cn.hutool.setting.dialect.Props` | `Props create()` | 构建一个空的Props，用于手动加入参数 |
| `cn.hutool.setting.dialect.Props` | `Props getProp(String resource)` | 获得Classpath下的Properties文件 |
| `cn.hutool.setting.dialect.Props` | `Props getProp(String resource,Charset charset)` | 获得Classpath下的Properties文件 |
| `cn.hutool.setting.dialect.Props` | `Props getProp(String resource,String charsetName)` | 获得Classpath下的Properties文件 |
| `cn.hutool.setting.dialect.Props` | `Short getShort(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `Short getShort(String key,Short defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `String getAndRemoveStr(String... keys)` | 获取并删除键值对，当指定键对应值非空时，返回并删除这个值，后边的键对应的值不再查找 |
| `cn.hutool.setting.dialect.Props` | `String getStr(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `String getStr(String key,String defaultValue)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.setting.dialect.Props` | `T fillBean(T bean,String prefix)` | 将配置文件转换为Bean，支持嵌套Bean 支持的表达式： |
| `cn.hutool.setting.dialect.Props` | `T toBean(Class<T> beanClass)` | 将配置文件转换为Bean，支持嵌套Bean 支持的表达式： |
| `cn.hutool.setting.dialect.Props` | `T toBean(Class<T> beanClass,String prefix)` | 将配置文件转换为Bean，支持嵌套Bean 支持的表达式： |
| `cn.hutool.setting.dialect.Props` | `void autoLoad(boolean autoReload)` | 在配置文件变更时自动加载 |
| `cn.hutool.setting.dialect.Props` | `void load()` | 重新加载配置文件 |
| `cn.hutool.setting.dialect.Props` | `void load(Resource resource)` | 初始化配置文件 |
| `cn.hutool.setting.dialect.Props` | `void load(URL url)` | 初始化配置文件 |
| `cn.hutool.setting.dialect.Props` | `void setProperty(String key,Object value)` | 设置值，无给定键创建之。设置后未持久化 |
| `cn.hutool.setting.dialect.Props` | `void store(String absolutePath)` | 持久化当前设置，会覆盖掉之前的设置 |
| `cn.hutool.setting.dialect.Props` | `void store(String path,Class<?> clazz)` | 存储当前设置，会覆盖掉以前的设置 |
| `cn.hutool.setting.dialect.PropsUtil` | `Props get(String name)` | 获取当前环境下的配置文件 name可以为不包括扩展名的文件名（默认.properties），也可以是文件名全称 |
| `cn.hutool.setting.dialect.PropsUtil` | `Props getFirstFound(String... names)` | 获取给定路径找到的第一个配置文件 * name可以为不包括扩展名的文件名（默认.properties为结尾），也可以是文件名全称 |
| `cn.hutool.setting.dialect.PropsUtil` | `Props getSystemProps()` | 获取系统参数，例如用户在执行java命令时定义的 -Duse=hutool |
