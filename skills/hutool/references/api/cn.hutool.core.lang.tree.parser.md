# cn.hutool.core.lang.tree.parser

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.lang.tree.parser.DefaultNodeParser`

```java
public class cn.hutool.core.lang.tree.parser.DefaultNodeParser<T> implements cn.hutool.core.lang.tree.parser.NodeParser<cn.hutool.core.lang.tree.TreeNode<T>, T> {
  public cn.hutool.core.lang.tree.parser.DefaultNodeParser();
  public void parse(cn.hutool.core.lang.tree.TreeNode<T>, cn.hutool.core.lang.tree.Tree<T>);
  public void parse(java.lang.Object, cn.hutool.core.lang.tree.Tree);
}
```

## `cn.hutool.core.lang.tree.parser.NodeParser`

```java
public interface cn.hutool.core.lang.tree.parser.NodeParser<T, E> {
  public abstract void parse(T, cn.hutool.core.lang.tree.Tree<E>);
}
```
