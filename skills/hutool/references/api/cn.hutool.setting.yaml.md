# cn.hutool.setting.yaml

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.setting.yaml.YamlUtil`

```java
public class cn.hutool.setting.yaml.YamlUtil {
  public cn.hutool.setting.yaml.YamlUtil();
  public static cn.hutool.core.lang.Dict loadByPath(java.lang.String);
  public static <T> T loadByPath(java.lang.String, java.lang.Class<T>);
  public static <T> T load(java.io.InputStream, java.lang.Class<T>);
  public static cn.hutool.core.lang.Dict load(java.io.Reader);
  public static <T> T load(java.io.Reader, java.lang.Class<T>);
  public static <T> T load(java.io.Reader, java.lang.Class<T>, boolean);
  public static void dump(java.lang.Object, java.io.Writer);
  public static void dump(java.lang.Object, java.io.Writer, org.yaml.snakeyaml.DumperOptions);
}
```
