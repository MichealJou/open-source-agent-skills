# cn.hutool.poi.ofd

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.poi.ofd.OfdWriter`

```java
public class cn.hutool.poi.ofd.OfdWriter implements java.io.Serializable,java.io.Closeable {
  public cn.hutool.poi.ofd.OfdWriter(java.io.File);
  public cn.hutool.poi.ofd.OfdWriter(java.nio.file.Path);
  public cn.hutool.poi.ofd.OfdWriter(java.io.OutputStream);
  public cn.hutool.poi.ofd.OfdWriter addText(org.ofdrw.font.Font, java.lang.String...);
  public cn.hutool.poi.ofd.OfdWriter addPicture(java.io.File, int, int);
  public cn.hutool.poi.ofd.OfdWriter addPicture(java.nio.file.Path, int, int);
  public cn.hutool.poi.ofd.OfdWriter add(org.ofdrw.layout.element.Div);
  public cn.hutool.poi.ofd.OfdWriter add(int, org.ofdrw.layout.edit.Annotation);
  public void close();
}
```
