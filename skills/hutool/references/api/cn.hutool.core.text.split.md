# cn.hutool.core.text.split

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.text.split.SplitIter`

```java
public class cn.hutool.core.text.split.SplitIter extends cn.hutool.core.collection.ComputeIter<java.lang.String> implements java.io.Serializable {
  public cn.hutool.core.text.split.SplitIter(java.lang.CharSequence, cn.hutool.core.text.finder.TextFinder, int, boolean);
  public void reset();
  public java.lang.String[] toArray(boolean);
  public java.util.List<java.lang.String> toList(boolean);
  public <T> java.util.List<T> toList(java.util.function.Function<java.lang.String, T>);
}
```
