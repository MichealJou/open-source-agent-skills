# cn.hutool.setting.yaml

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.setting.yaml.YamlUtil` | `Dict load(Reader reader)` | 加载YAML，加载完毕后关闭Reader |
| `cn.hutool.setting.yaml.YamlUtil` | `Dict loadByPath(String path)` | 从classpath或绝对路径加载YAML文件 |
| `cn.hutool.setting.yaml.YamlUtil` | `T load(InputStream in,Class<T> type)` | 从流中加载YAML |
| `cn.hutool.setting.yaml.YamlUtil` | `T load(Reader reader,Class<T> type)` | 加载YAML，加载完毕后关闭Reader |
| `cn.hutool.setting.yaml.YamlUtil` | `T load(Reader reader,Class<T> type,boolean isCloseReader)` | 加载YAML |
| `cn.hutool.setting.yaml.YamlUtil` | `T loadByPath(String path,Class<T> type)` | 从classpath或绝对路径加载YAML文件 |
| `cn.hutool.setting.yaml.YamlUtil` | `void dump(Object object,Writer writer)` | 将Bean对象或者Map写出到Writer |
| `cn.hutool.setting.yaml.YamlUtil` | `void dump(Object object,Writer writer,DumperOptions dumperOptions)` | 将Bean对象或者Map写出到Writer |
