# cn.hutool.core.lang.tree

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.lang.tree.Node`

```java
public interface cn.hutool.core.lang.tree.Node<T> extends java.lang.Comparable<cn.hutool.core.lang.tree.Node<T>>, java.io.Serializable {
  public abstract T getId();
  public abstract cn.hutool.core.lang.tree.Node<T> setId(T);
  public abstract T getParentId();
  public abstract cn.hutool.core.lang.tree.Node<T> setParentId(T);
  public abstract java.lang.CharSequence getName();
  public abstract cn.hutool.core.lang.tree.Node<T> setName(java.lang.CharSequence);
  public abstract java.lang.Comparable<?> getWeight();
  public abstract cn.hutool.core.lang.tree.Node<T> setWeight(java.lang.Comparable<?>);
  public default int compareTo(cn.hutool.core.lang.tree.Node);
  public default int compareTo(java.lang.Object);
}
```

## `cn.hutool.core.lang.tree.Tree`

```java
public class cn.hutool.core.lang.tree.Tree<T> extends java.util.LinkedHashMap<java.lang.String, java.lang.Object> implements cn.hutool.core.lang.tree.Node<T> {
  public cn.hutool.core.lang.tree.Tree();
  public cn.hutool.core.lang.tree.Tree(cn.hutool.core.lang.tree.TreeNodeConfig);
  public cn.hutool.core.lang.tree.TreeNodeConfig getConfig();
  public cn.hutool.core.lang.tree.Tree<T> getParent();
  public cn.hutool.core.lang.tree.Tree<T> getNode(T);
  public java.util.List<java.lang.CharSequence> getParentsName(T, boolean);
  public java.util.List<java.lang.CharSequence> getParentsName(boolean);
  public cn.hutool.core.lang.tree.Tree<T> setParent(cn.hutool.core.lang.tree.Tree<T>);
  public T getId();
  public cn.hutool.core.lang.tree.Tree<T> setId(T);
  public T getParentId();
  public cn.hutool.core.lang.tree.Tree<T> setParentId(T);
  public java.lang.CharSequence getName();
  public cn.hutool.core.lang.tree.Tree<T> setName(java.lang.CharSequence);
  public java.lang.Comparable<?> getWeight();
  public cn.hutool.core.lang.tree.Tree<T> setWeight(java.lang.Comparable<?>);
  public java.util.List<cn.hutool.core.lang.tree.Tree<T>> getChildren();
  public boolean hasChild();
  public void walk(java.util.function.Consumer<cn.hutool.core.lang.tree.Tree<T>>);
  public cn.hutool.core.lang.tree.Tree<T> filterNew(cn.hutool.core.lang.Filter<cn.hutool.core.lang.tree.Tree<T>>);
  public cn.hutool.core.lang.tree.Tree<T> filter(cn.hutool.core.lang.Filter<cn.hutool.core.lang.tree.Tree<T>>);
  public cn.hutool.core.lang.tree.Tree<T> setChildren(java.util.List<cn.hutool.core.lang.tree.Tree<T>>);
  public final cn.hutool.core.lang.tree.Tree<T> addChildren(cn.hutool.core.lang.tree.Tree<T>...);
  public void putExtra(java.lang.String, java.lang.Object);
  public java.lang.String toString();
  public cn.hutool.core.lang.tree.Tree<T> cloneTree();
  public cn.hutool.core.lang.tree.Node setWeight(java.lang.Comparable);
  public cn.hutool.core.lang.tree.Node setName(java.lang.CharSequence);
  public cn.hutool.core.lang.tree.Node setParentId(java.lang.Object);
  public cn.hutool.core.lang.tree.Node setId(java.lang.Object);
}
```

## `cn.hutool.core.lang.tree.TreeBuilder`

```java
public class cn.hutool.core.lang.tree.TreeBuilder<E> implements cn.hutool.core.builder.Builder<cn.hutool.core.lang.tree.Tree<E>> {
  public static <T> cn.hutool.core.lang.tree.TreeBuilder<T> of(T);
  public static <T> cn.hutool.core.lang.tree.TreeBuilder<T> of(T, cn.hutool.core.lang.tree.TreeNodeConfig);
  public cn.hutool.core.lang.tree.TreeBuilder(E, cn.hutool.core.lang.tree.TreeNodeConfig);
  public cn.hutool.core.lang.tree.TreeBuilder(cn.hutool.core.lang.tree.Tree<E>);
  public cn.hutool.core.lang.tree.TreeBuilder<E> setId(E);
  public cn.hutool.core.lang.tree.TreeBuilder<E> setParentId(E);
  public cn.hutool.core.lang.tree.TreeBuilder<E> setName(java.lang.CharSequence);
  public cn.hutool.core.lang.tree.TreeBuilder<E> setWeight(java.lang.Comparable<?>);
  public cn.hutool.core.lang.tree.TreeBuilder<E> putExtra(java.lang.String, java.lang.Object);
  public cn.hutool.core.lang.tree.TreeBuilder<E> append(java.util.Map<E, cn.hutool.core.lang.tree.Tree<E>>);
  public cn.hutool.core.lang.tree.TreeBuilder<E> append(java.lang.Iterable<cn.hutool.core.lang.tree.Tree<E>>);
  public <T> cn.hutool.core.lang.tree.TreeBuilder<E> append(java.util.List<T>, cn.hutool.core.lang.tree.parser.NodeParser<T, E>);
  public <T> cn.hutool.core.lang.tree.TreeBuilder<E> append(java.util.List<T>, E, cn.hutool.core.lang.tree.parser.NodeParser<T, E>);
  public cn.hutool.core.lang.tree.TreeBuilder<E> reset();
  public cn.hutool.core.lang.tree.Tree<E> build();
  public java.util.List<cn.hutool.core.lang.tree.Tree<E>> buildList();
  public java.lang.Object build();
}
```

## `cn.hutool.core.lang.tree.TreeNode`

```java
public class cn.hutool.core.lang.tree.TreeNode<T> implements cn.hutool.core.lang.tree.Node<T> {
  public cn.hutool.core.lang.tree.TreeNode();
  public cn.hutool.core.lang.tree.TreeNode(T, T, java.lang.String, java.lang.Comparable<?>);
  public T getId();
  public cn.hutool.core.lang.tree.TreeNode<T> setId(T);
  public T getParentId();
  public cn.hutool.core.lang.tree.TreeNode<T> setParentId(T);
  public java.lang.CharSequence getName();
  public cn.hutool.core.lang.tree.TreeNode<T> setName(java.lang.CharSequence);
  public java.lang.Comparable<?> getWeight();
  public cn.hutool.core.lang.tree.TreeNode<T> setWeight(java.lang.Comparable<?>);
  public java.util.Map<java.lang.String, java.lang.Object> getExtra();
  public cn.hutool.core.lang.tree.TreeNode<T> setExtra(java.util.Map<java.lang.String, java.lang.Object>);
  public boolean equals(java.lang.Object);
  public int hashCode();
  public cn.hutool.core.lang.tree.Node setWeight(java.lang.Comparable);
  public cn.hutool.core.lang.tree.Node setName(java.lang.CharSequence);
  public cn.hutool.core.lang.tree.Node setParentId(java.lang.Object);
  public cn.hutool.core.lang.tree.Node setId(java.lang.Object);
}
```

## `cn.hutool.core.lang.tree.TreeNodeConfig`

```java
public class cn.hutool.core.lang.tree.TreeNodeConfig implements java.io.Serializable {
  public cn.hutool.core.lang.tree.TreeNodeConfig();
  public java.lang.String getIdKey();
  public cn.hutool.core.lang.tree.TreeNodeConfig setIdKey(java.lang.String);
  public java.lang.String getWeightKey();
  public cn.hutool.core.lang.tree.TreeNodeConfig setWeightKey(java.lang.String);
  public java.lang.String getNameKey();
  public cn.hutool.core.lang.tree.TreeNodeConfig setNameKey(java.lang.String);
  public java.lang.String getChildrenKey();
  public cn.hutool.core.lang.tree.TreeNodeConfig setChildrenKey(java.lang.String);
  public java.lang.String getParentIdKey();
  public cn.hutool.core.lang.tree.TreeNodeConfig setParentIdKey(java.lang.String);
  public java.lang.Integer getDeep();
  public cn.hutool.core.lang.tree.TreeNodeConfig setDeep(java.lang.Integer);
}
```

## `cn.hutool.core.lang.tree.TreeUtil`

```java
public class cn.hutool.core.lang.tree.TreeUtil {
  public cn.hutool.core.lang.tree.TreeUtil();
  public static cn.hutool.core.lang.tree.Tree<java.lang.Integer> buildSingle(java.util.List<cn.hutool.core.lang.tree.TreeNode<java.lang.Integer>>);
  public static java.util.List<cn.hutool.core.lang.tree.Tree<java.lang.Integer>> build(java.util.List<cn.hutool.core.lang.tree.TreeNode<java.lang.Integer>>);
  public static <E> cn.hutool.core.lang.tree.Tree<E> buildSingle(java.util.List<cn.hutool.core.lang.tree.TreeNode<E>>, E);
  public static <E> java.util.List<cn.hutool.core.lang.tree.Tree<E>> build(java.util.List<cn.hutool.core.lang.tree.TreeNode<E>>, E);
  public static <T, E> cn.hutool.core.lang.tree.Tree<E> buildSingle(java.util.List<T>, E, cn.hutool.core.lang.tree.parser.NodeParser<T, E>);
  public static <T, E> java.util.List<cn.hutool.core.lang.tree.Tree<E>> build(java.util.List<T>, E, cn.hutool.core.lang.tree.parser.NodeParser<T, E>);
  public static <T, E> java.util.List<cn.hutool.core.lang.tree.Tree<E>> build(java.util.List<T>, E, cn.hutool.core.lang.tree.TreeNodeConfig, cn.hutool.core.lang.tree.parser.NodeParser<T, E>);
  public static <T, E> cn.hutool.core.lang.tree.Tree<E> buildSingle(java.util.List<T>, E, cn.hutool.core.lang.tree.TreeNodeConfig, cn.hutool.core.lang.tree.parser.NodeParser<T, E>);
  public static <E> java.util.List<cn.hutool.core.lang.tree.Tree<E>> build(java.util.Map<E, cn.hutool.core.lang.tree.Tree<E>>, E);
  public static <E> cn.hutool.core.lang.tree.Tree<E> buildSingle(java.util.Map<E, cn.hutool.core.lang.tree.Tree<E>>, E);
  public static <T> cn.hutool.core.lang.tree.Tree<T> getNode(cn.hutool.core.lang.tree.Tree<T>, T);
  public static <T> java.util.List<java.lang.CharSequence> getParentsName(cn.hutool.core.lang.tree.Tree<T>, boolean);
  public static <T> java.util.List<T> getParentsId(cn.hutool.core.lang.tree.Tree<T>, boolean);
  public static <E> cn.hutool.core.lang.tree.Tree<E> createEmptyNode(E);
  public static <T, E> java.util.List<E> build(java.util.List<E>, T, java.util.function.Function<E, T>, java.util.function.Function<E, T>, java.util.function.BiConsumer<E, java.util.List<E>>);
}
```
