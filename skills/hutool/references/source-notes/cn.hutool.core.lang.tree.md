# cn.hutool.core.lang.tree

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.lang.tree.Node` | `CharSequence getName()` | 获取节点标签名称 |
| `cn.hutool.core.lang.tree.Node` | `Comparable<?> getWeight()` | 获取权重 |
| `cn.hutool.core.lang.tree.Node` | `Node<T> setId(T id)` | 设置ID |
| `cn.hutool.core.lang.tree.Node` | `Node<T> setName(CharSequence name)` | 设置节点标签名称 |
| `cn.hutool.core.lang.tree.Node` | `Node<T> setParentId(T parentId)` | 设置父节点ID |
| `cn.hutool.core.lang.tree.Node` | `Node<T> setWeight(Comparable<?> weight)` | 设置权重 |
| `cn.hutool.core.lang.tree.Node` | `T getId()` | 获取ID |
| `cn.hutool.core.lang.tree.Node` | `T getParentId()` | 获取父节点ID |
| `cn.hutool.core.lang.tree.Node` | `int compareTo(Node node)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.Tree` | `CharSequence getName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.Tree` | `Comparable<?> getWeight()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.Tree` | `List<CharSequence> getParentsName(T id,boolean includeCurrentNode)` | 获取所有父节点名称列表 比如有个人在研发1部，他上面有研发部，接着上面有技术中心 返回结果就是：[研发一部, 研发中心, 技术中心] |
| `cn.hutool.core.lang.tree.Tree` | `List<CharSequence> getParentsName(boolean includeCurrentNode)` | 获取所有父节点名称列表 比如有个人在研发1部，他上面有研发部，接着上面有技术中心 返回结果就是：[研发一部, 研发中心, 技术中心] |
| `cn.hutool.core.lang.tree.Tree` | `List<Tree<T>> getChildren()` | 获取所有子节点 |
| `cn.hutool.core.lang.tree.Tree` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.Tree` | `T getId()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.Tree` | `T getParentId()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.Tree` | `Tree<T> addChildren(Tree<T>... children)` | 增加子节点，同时关联子节点的父节点为当前节点 |
| `cn.hutool.core.lang.tree.Tree` | `Tree<T> cloneTree()` | 递归克隆当前节点（即克隆整个树，保留字段值） 注意，此方法只会克隆节点，节点属性如果是引用类型，不会克隆 |
| `cn.hutool.core.lang.tree.Tree` | `Tree<T> filter(Filter<Tree<T>> filter)` | 递归过滤当前树，注意此方法会修改当前树 通过Filter指定的过滤规则，本节点或子节点满足过滤条件，则保留当前节点及其所有子节点，否则抛弃节点及其子节点 |
| `cn.hutool.core.lang.tree.Tree` | `Tree<T> filterNew(Filter<Tree<T>> filter)` | 递归过滤并生成新的树 通过Filter指定的过滤规则，本节点或子节点满足过滤条件，则保留当前节点，否则抛弃节点及其子节点 |
| `cn.hutool.core.lang.tree.Tree` | `Tree<T> getNode(T id)` | 获取ID对应的节点，如果有多个ID相同的节点，只返回第一个。 此方法只查找此节点及子节点，采用广度优先遍历。 |
| `cn.hutool.core.lang.tree.Tree` | `Tree<T> getParent()` | 获取父节点 |
| `cn.hutool.core.lang.tree.Tree` | `Tree<T> setChildren(List<Tree<T>> children)` | 设置子节点，设置后会覆盖所有原有子节点 |
| `cn.hutool.core.lang.tree.Tree` | `Tree<T> setId(T id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.Tree` | `Tree<T> setName(CharSequence name)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.Tree` | `Tree<T> setParent(Tree<T> parent)` | 设置父节点 |
| `cn.hutool.core.lang.tree.Tree` | `Tree<T> setParentId(T parentId)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.Tree` | `Tree<T> setWeight(Comparable<?> weight)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.Tree` | `TreeNodeConfig getConfig()` | 获取节点配置 |
| `cn.hutool.core.lang.tree.Tree` | `boolean hasChild()` | 是否有子节点，无子节点则此为叶子节点 |
| `cn.hutool.core.lang.tree.Tree` | `void putExtra(String key,Object value)` | 扩展属性 |
| `cn.hutool.core.lang.tree.Tree` | `void walk(Consumer<Tree<T>> consumer)` | 递归树并处理子树下的节点： |
| `cn.hutool.core.lang.tree.TreeBuilder` | `List<Tree<E>> buildList()` | 构建树列表，没有顶层节点，例如： |
| `cn.hutool.core.lang.tree.TreeBuilder` | `Tree<E> build()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.TreeBuilder` | `TreeBuilder<E> append(Iterable<Tree<E>> trees)` | 增加节点列表，增加的节点是不带子节点的 |
| `cn.hutool.core.lang.tree.TreeBuilder` | `TreeBuilder<E> append(List<T> list,E rootId,NodeParser<T, E> nodeParser)` | 增加节点列表，增加的节点是不带子节点的 |
| `cn.hutool.core.lang.tree.TreeBuilder` | `TreeBuilder<E> append(List<T> list,NodeParser<T, E> nodeParser)` | 增加节点列表，增加的节点是不带子节点的 |
| `cn.hutool.core.lang.tree.TreeBuilder` | `TreeBuilder<E> append(Map<E, Tree<E>> map)` | 增加节点列表，增加的节点是不带子节点的 |
| `cn.hutool.core.lang.tree.TreeBuilder` | `TreeBuilder<E> putExtra(String key,Object value)` | 扩展属性 |
| `cn.hutool.core.lang.tree.TreeBuilder` | `TreeBuilder<E> reset()` | 重置Builder，实现复用 |
| `cn.hutool.core.lang.tree.TreeBuilder` | `TreeBuilder<E> setId(E id)` | 设置ID |
| `cn.hutool.core.lang.tree.TreeBuilder` | `TreeBuilder<E> setName(CharSequence name)` | 设置节点标签名称 |
| `cn.hutool.core.lang.tree.TreeBuilder` | `TreeBuilder<E> setParentId(E parentId)` | 设置父节点ID |
| `cn.hutool.core.lang.tree.TreeBuilder` | `TreeBuilder<E> setWeight(Comparable<?> weight)` | 设置权重 |
| `cn.hutool.core.lang.tree.TreeBuilder` | `TreeBuilder<T> of(T rootId)` | 创建Tree构建器 |
| `cn.hutool.core.lang.tree.TreeBuilder` | `TreeBuilder<T> of(T rootId,TreeNodeConfig config)` | 创建Tree构建器 |
| `cn.hutool.core.lang.tree.TreeNode` | `CharSequence getName()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.TreeNode` | `Comparable<?> getWeight()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.TreeNode` | `Map<String, Object> getExtra()` | 获取扩展字段 |
| `cn.hutool.core.lang.tree.TreeNode` | `T getId()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.TreeNode` | `T getParentId()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.TreeNode` | `TreeNode<T> setExtra(Map<String, Object> extra)` | 设置扩展字段 |
| `cn.hutool.core.lang.tree.TreeNode` | `TreeNode<T> setId(T id)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.TreeNode` | `TreeNode<T> setName(CharSequence name)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.TreeNode` | `TreeNode<T> setParentId(T parentId)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.TreeNode` | `TreeNode<T> setWeight(Comparable<?> weight)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.TreeNode` | `boolean equals(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.TreeNode` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.tree.TreeNodeConfig` | `Integer getDeep()` | 获取递归深度 |
| `cn.hutool.core.lang.tree.TreeNodeConfig` | `String getChildrenKey()` | 获取子点对应的名称 |
| `cn.hutool.core.lang.tree.TreeNodeConfig` | `String getIdKey()` | 获取ID对应的名称 |
| `cn.hutool.core.lang.tree.TreeNodeConfig` | `String getNameKey()` | 获取节点名对应的名称 |
| `cn.hutool.core.lang.tree.TreeNodeConfig` | `String getParentIdKey()` | 获取父节点ID对应的名称 |
| `cn.hutool.core.lang.tree.TreeNodeConfig` | `String getWeightKey()` | 获取权重对应的名称 |
| `cn.hutool.core.lang.tree.TreeNodeConfig` | `TreeNodeConfig setChildrenKey(String childrenKey)` | 设置子点对应的名称 |
| `cn.hutool.core.lang.tree.TreeNodeConfig` | `TreeNodeConfig setDeep(Integer deep)` | 设置递归深度 |
| `cn.hutool.core.lang.tree.TreeNodeConfig` | `TreeNodeConfig setIdKey(String idKey)` | 设置ID对应的名称 |
| `cn.hutool.core.lang.tree.TreeNodeConfig` | `TreeNodeConfig setNameKey(String nameKey)` | 设置节点名对应的名称 |
| `cn.hutool.core.lang.tree.TreeNodeConfig` | `TreeNodeConfig setParentIdKey(String parentIdKey)` | 设置父点对应的名称 |
| `cn.hutool.core.lang.tree.TreeNodeConfig` | `TreeNodeConfig setWeightKey(String weightKey)` | 设置权重对应的名称 |
| `cn.hutool.core.lang.tree.TreeUtil` | `List<CharSequence> getParentsName(Tree<T> node,boolean includeCurrentNode)` | 获取所有父节点名称列表 比如有个人在研发1部，他上面有研发部，接着上面有技术中心 返回结果就是：[研发一部, 研发中心, 技术中心] |
| `cn.hutool.core.lang.tree.TreeUtil` | `List<E> build(List<E> nodes,T rootId,Function<E, T> idFunc,Function<E, T> parentIdFunc,BiConsumer<E, List<E>> setChildFunc)` | 函数式构建树状结构(无需继承Tree类) |
| `cn.hutool.core.lang.tree.TreeUtil` | `List<T> getParentsId(Tree<T> node,boolean includeCurrentNode)` | 获取所有父节点ID列表 比如有个人在研发1部，他上面有研发部，接着上面有技术中心 返回结果就是：[研发部, 技术中心] |
| `cn.hutool.core.lang.tree.TreeUtil` | `List<Tree<E>> build(List<T> list,E parentId,NodeParser<T, E> nodeParser)` | 树构建 |
| `cn.hutool.core.lang.tree.TreeUtil` | `List<Tree<E>> build(List<T> list,E rootId,TreeNodeConfig treeNodeConfig,NodeParser<T, E> nodeParser)` | 树构建 |
| `cn.hutool.core.lang.tree.TreeUtil` | `List<Tree<E>> build(List<TreeNode<E>> list,E parentId)` | 树构建 |
| `cn.hutool.core.lang.tree.TreeUtil` | `List<Tree<E>> build(Map<E, Tree<E>> map,E rootId)` | 树构建，按照权重排序 |
| `cn.hutool.core.lang.tree.TreeUtil` | `List<Tree<Integer>> build(List<TreeNode<Integer>> list)` | 树构建 |
| `cn.hutool.core.lang.tree.TreeUtil` | `Tree<E> buildSingle(List<T> list,E parentId,NodeParser<T, E> nodeParser)` | 构建单root节点树 它会生成一个以指定ID为ID的空的节点，然后逐级增加子节点。 |
| `cn.hutool.core.lang.tree.TreeUtil` | `Tree<E> buildSingle(List<T> list,E rootId,TreeNodeConfig treeNodeConfig,NodeParser<T, E> nodeParser)` | 构建单root节点树 它会生成一个以指定ID为ID的空的节点，然后逐级增加子节点。 |
| `cn.hutool.core.lang.tree.TreeUtil` | `Tree<E> buildSingle(List<TreeNode<E>> list,E parentId)` | 构建单root节点树 它会生成一个以指定ID为ID的空的节点，然后逐级增加子节点。 |
| `cn.hutool.core.lang.tree.TreeUtil` | `Tree<E> buildSingle(Map<E, Tree<E>> map,E rootId)` | 单点树构建，按照权重排序 它会生成一个以指定ID为ID的空的节点，然后逐级增加子节点。 |
| `cn.hutool.core.lang.tree.TreeUtil` | `Tree<E> createEmptyNode(E id)` | 创建空Tree的节点 |
| `cn.hutool.core.lang.tree.TreeUtil` | `Tree<Integer> buildSingle(List<TreeNode<Integer>> list)` | 构建单root节点树 |
| `cn.hutool.core.lang.tree.TreeUtil` | `Tree<T> getNode(Tree<T> node,T id)` | 获取ID对应的节点，如果有多个ID相同的节点，只返回第一个。 此方法只查找此节点及子节点，采用递归深度优先遍历。 |
