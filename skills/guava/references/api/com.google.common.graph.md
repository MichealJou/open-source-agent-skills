# com.google.common.graph

版本：33.4.8-jre。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.google.common.graph.AbstractGraph`

```java
public abstract class com.google.common.graph.AbstractGraph<N> extends com.google.common.graph.AbstractBaseGraph<N> implements com.google.common.graph.Graph<N> {
  public com.google.common.graph.AbstractGraph();
  public final boolean equals(java.lang.Object);
  public final int hashCode();
  public java.lang.String toString();
  public boolean hasEdgeConnecting(com.google.common.graph.EndpointPair);
  public boolean hasEdgeConnecting(java.lang.Object, java.lang.Object);
  public int outDegree(java.lang.Object);
  public int inDegree(java.lang.Object);
  public int degree(java.lang.Object);
  public java.util.Set incidentEdges(java.lang.Object);
  public com.google.common.graph.ElementOrder incidentEdgeOrder();
  public java.util.Set edges();
}
```

## `com.google.common.graph.AbstractNetwork`

```java
public abstract class com.google.common.graph.AbstractNetwork<N, E> implements com.google.common.graph.Network<N, E> {
  public com.google.common.graph.AbstractNetwork();
  public com.google.common.graph.Graph<N> asGraph();
  public int degree(N);
  public int inDegree(N);
  public int outDegree(N);
  public java.util.Set<E> adjacentEdges(E);
  public java.util.Set<E> edgesConnecting(N, N);
  public java.util.Set<E> edgesConnecting(com.google.common.graph.EndpointPair<N>);
  public java.util.Optional<E> edgeConnecting(N, N);
  public java.util.Optional<E> edgeConnecting(com.google.common.graph.EndpointPair<N>);
  public E edgeConnectingOrNull(N, N);
  public E edgeConnectingOrNull(com.google.common.graph.EndpointPair<N>);
  public boolean hasEdgeConnecting(N, N);
  public boolean hasEdgeConnecting(com.google.common.graph.EndpointPair<N>);
  public final boolean equals(java.lang.Object);
  public final int hashCode();
  public java.lang.String toString();
}
```

## `com.google.common.graph.AbstractValueGraph`

```java
public abstract class com.google.common.graph.AbstractValueGraph<N, V> extends com.google.common.graph.AbstractBaseGraph<N> implements com.google.common.graph.ValueGraph<N, V> {
  public com.google.common.graph.AbstractValueGraph();
  public com.google.common.graph.Graph<N> asGraph();
  public java.util.Optional<V> edgeValue(N, N);
  public java.util.Optional<V> edgeValue(com.google.common.graph.EndpointPair<N>);
  public final boolean equals(java.lang.Object);
  public final int hashCode();
  public java.lang.String toString();
  public boolean hasEdgeConnecting(com.google.common.graph.EndpointPair);
  public boolean hasEdgeConnecting(java.lang.Object, java.lang.Object);
  public int outDegree(java.lang.Object);
  public int inDegree(java.lang.Object);
  public int degree(java.lang.Object);
  public java.util.Set incidentEdges(java.lang.Object);
  public com.google.common.graph.ElementOrder incidentEdgeOrder();
  public java.util.Set edges();
}
```

## `com.google.common.graph.ElementOrder`

```java
public final class com.google.common.graph.ElementOrder<T> {
  public static <S> com.google.common.graph.ElementOrder<S> unordered();
  public static <S> com.google.common.graph.ElementOrder<S> stable();
  public static <S> com.google.common.graph.ElementOrder<S> insertion();
  public static <S extends java.lang.Comparable<? super S>> com.google.common.graph.ElementOrder<S> natural();
  public static <S> com.google.common.graph.ElementOrder<S> sorted(java.util.Comparator<S>);
  public com.google.common.graph.ElementOrder$Type type();
  public java.util.Comparator<T> comparator();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
}
```

## `com.google.common.graph.ElementOrder$Type`

```java
public final class com.google.common.graph.ElementOrder$Type extends java.lang.Enum<com.google.common.graph.ElementOrder$Type> {
  public static com.google.common.graph.ElementOrder$Type[] values();
  public static com.google.common.graph.ElementOrder$Type valueOf(java.lang.String);
}
```

## `com.google.common.graph.EndpointPair`

```java
public abstract class com.google.common.graph.EndpointPair<N> implements java.lang.Iterable<N> {
  public static <N> com.google.common.graph.EndpointPair<N> ordered(N, N);
  public static <N> com.google.common.graph.EndpointPair<N> unordered(N, N);
  public abstract N source();
  public abstract N target();
  public final N nodeU();
  public final N nodeV();
  public final N adjacentNode(N);
  public abstract boolean isOrdered();
  public final com.google.common.collect.UnmodifiableIterator<N> iterator();
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
  public java.util.Iterator iterator();
}
```

## `com.google.common.graph.Graph`

```java
public interface com.google.common.graph.Graph<N> extends com.google.common.graph.BaseGraph<N> {
  public abstract java.util.Set<N> nodes();
  public abstract java.util.Set<com.google.common.graph.EndpointPair<N>> edges();
  public abstract boolean isDirected();
  public abstract boolean allowsSelfLoops();
  public abstract com.google.common.graph.ElementOrder<N> nodeOrder();
  public abstract com.google.common.graph.ElementOrder<N> incidentEdgeOrder();
  public abstract java.util.Set<N> adjacentNodes(N);
  public abstract java.util.Set<N> predecessors(N);
  public abstract java.util.Set<N> successors(N);
  public abstract java.util.Set<com.google.common.graph.EndpointPair<N>> incidentEdges(N);
  public abstract int degree(N);
  public abstract int inDegree(N);
  public abstract int outDegree(N);
  public abstract boolean hasEdgeConnecting(N, N);
  public abstract boolean hasEdgeConnecting(com.google.common.graph.EndpointPair<N>);
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
  public default java.lang.Iterable successors(java.lang.Object);
  public default java.lang.Iterable predecessors(java.lang.Object);
}
```

## `com.google.common.graph.GraphBuilder`

```java
public final class com.google.common.graph.GraphBuilder<N> extends com.google.common.graph.AbstractGraphBuilder<N> {
  public static com.google.common.graph.GraphBuilder<java.lang.Object> directed();
  public static com.google.common.graph.GraphBuilder<java.lang.Object> undirected();
  public static <N> com.google.common.graph.GraphBuilder<N> from(com.google.common.graph.Graph<N>);
  public <N1 extends N> com.google.common.graph.ImmutableGraph$Builder<N1> immutable();
  public com.google.common.graph.GraphBuilder<N> allowsSelfLoops(boolean);
  public com.google.common.graph.GraphBuilder<N> expectedNodeCount(int);
  public <N1 extends N> com.google.common.graph.GraphBuilder<N1> nodeOrder(com.google.common.graph.ElementOrder<N1>);
  public <N1 extends N> com.google.common.graph.GraphBuilder<N1> incidentEdgeOrder(com.google.common.graph.ElementOrder<N1>);
  public <N1 extends N> com.google.common.graph.MutableGraph<N1> build();
}
```

## `com.google.common.graph.Graphs`

```java
public final class com.google.common.graph.Graphs extends com.google.common.graph.GraphsBridgeMethods {
  public static <N> boolean hasCycle(com.google.common.graph.Graph<N>);
  public static boolean hasCycle(com.google.common.graph.Network<?, ?>);
  public static <N> com.google.common.graph.ImmutableGraph<N> transitiveClosure(com.google.common.graph.Graph<N>);
  public static <N> com.google.common.collect.ImmutableSet<N> reachableNodes(com.google.common.graph.Graph<N>, N);
  public static <N> com.google.common.graph.Graph<N> transpose(com.google.common.graph.Graph<N>);
  public static <N, V> com.google.common.graph.ValueGraph<N, V> transpose(com.google.common.graph.ValueGraph<N, V>);
  public static <N, E> com.google.common.graph.Network<N, E> transpose(com.google.common.graph.Network<N, E>);
  public static <N> com.google.common.graph.MutableGraph<N> inducedSubgraph(com.google.common.graph.Graph<N>, java.lang.Iterable<? extends N>);
  public static <N, V> com.google.common.graph.MutableValueGraph<N, V> inducedSubgraph(com.google.common.graph.ValueGraph<N, V>, java.lang.Iterable<? extends N>);
  public static <N, E> com.google.common.graph.MutableNetwork<N, E> inducedSubgraph(com.google.common.graph.Network<N, E>, java.lang.Iterable<? extends N>);
  public static <N> com.google.common.graph.MutableGraph<N> copyOf(com.google.common.graph.Graph<N>);
  public static <N, V> com.google.common.graph.MutableValueGraph<N, V> copyOf(com.google.common.graph.ValueGraph<N, V>);
  public static <N, E> com.google.common.graph.MutableNetwork<N, E> copyOf(com.google.common.graph.Network<N, E>);
}
```

## `com.google.common.graph.ImmutableGraph`

```java
public class com.google.common.graph.ImmutableGraph<N> extends com.google.common.graph.ForwardingGraph<N> {
  public static <N> com.google.common.graph.ImmutableGraph<N> copyOf(com.google.common.graph.Graph<N>);
  public static <N> com.google.common.graph.ImmutableGraph<N> copyOf(com.google.common.graph.ImmutableGraph<N>);
  public com.google.common.graph.ElementOrder<N> incidentEdgeOrder();
  public boolean hasEdgeConnecting(com.google.common.graph.EndpointPair);
  public boolean hasEdgeConnecting(java.lang.Object, java.lang.Object);
  public int outDegree(java.lang.Object);
  public int inDegree(java.lang.Object);
  public int degree(java.lang.Object);
  public java.util.Set incidentEdges(java.lang.Object);
  public java.util.Set successors(java.lang.Object);
  public java.util.Set predecessors(java.lang.Object);
  public java.util.Set adjacentNodes(java.lang.Object);
  public com.google.common.graph.ElementOrder nodeOrder();
  public boolean allowsSelfLoops();
  public boolean isDirected();
  public java.util.Set nodes();
}
```

## `com.google.common.graph.ImmutableGraph$Builder`

```java
public class com.google.common.graph.ImmutableGraph$Builder<N> {
  public com.google.common.graph.ImmutableGraph$Builder<N> addNode(N);
  public com.google.common.graph.ImmutableGraph$Builder<N> putEdge(N, N);
  public com.google.common.graph.ImmutableGraph$Builder<N> putEdge(com.google.common.graph.EndpointPair<N>);
  public com.google.common.graph.ImmutableGraph<N> build();
}
```

## `com.google.common.graph.ImmutableNetwork`

```java
public final class com.google.common.graph.ImmutableNetwork<N, E> extends com.google.common.graph.StandardNetwork<N, E> {
  public static <N, E> com.google.common.graph.ImmutableNetwork<N, E> copyOf(com.google.common.graph.Network<N, E>);
  public static <N, E> com.google.common.graph.ImmutableNetwork<N, E> copyOf(com.google.common.graph.ImmutableNetwork<N, E>);
  public com.google.common.graph.ImmutableGraph<N> asGraph();
  public java.util.Set successors(java.lang.Object);
  public java.util.Set predecessors(java.lang.Object);
  public java.util.Set outEdges(java.lang.Object);
  public java.util.Set inEdges(java.lang.Object);
  public java.util.Set edgesConnecting(java.lang.Object, java.lang.Object);
  public java.util.Set adjacentNodes(java.lang.Object);
  public com.google.common.graph.EndpointPair incidentNodes(java.lang.Object);
  public java.util.Set incidentEdges(java.lang.Object);
  public com.google.common.graph.ElementOrder edgeOrder();
  public com.google.common.graph.ElementOrder nodeOrder();
  public boolean allowsSelfLoops();
  public boolean allowsParallelEdges();
  public boolean isDirected();
  public java.util.Set edges();
  public java.util.Set nodes();
  public com.google.common.graph.Graph asGraph();
}
```

## `com.google.common.graph.ImmutableNetwork$Builder`

```java
public class com.google.common.graph.ImmutableNetwork$Builder<N, E> {
  public com.google.common.graph.ImmutableNetwork$Builder<N, E> addNode(N);
  public com.google.common.graph.ImmutableNetwork$Builder<N, E> addEdge(N, N, E);
  public com.google.common.graph.ImmutableNetwork$Builder<N, E> addEdge(com.google.common.graph.EndpointPair<N>, E);
  public com.google.common.graph.ImmutableNetwork<N, E> build();
}
```

## `com.google.common.graph.ImmutableValueGraph`

```java
public final class com.google.common.graph.ImmutableValueGraph<N, V> extends com.google.common.graph.StandardValueGraph<N, V> {
  public static <N, V> com.google.common.graph.ImmutableValueGraph<N, V> copyOf(com.google.common.graph.ValueGraph<N, V>);
  public static <N, V> com.google.common.graph.ImmutableValueGraph<N, V> copyOf(com.google.common.graph.ImmutableValueGraph<N, V>);
  public com.google.common.graph.ElementOrder<N> incidentEdgeOrder();
  public com.google.common.graph.ImmutableGraph<N> asGraph();
  public java.lang.Object edgeValueOrDefault(com.google.common.graph.EndpointPair, java.lang.Object);
  public java.lang.Object edgeValueOrDefault(java.lang.Object, java.lang.Object, java.lang.Object);
  public boolean hasEdgeConnecting(com.google.common.graph.EndpointPair);
  public boolean hasEdgeConnecting(java.lang.Object, java.lang.Object);
  public java.util.Set incidentEdges(java.lang.Object);
  public java.util.Set successors(java.lang.Object);
  public java.util.Set predecessors(java.lang.Object);
  public java.util.Set adjacentNodes(java.lang.Object);
  public com.google.common.graph.ElementOrder nodeOrder();
  public boolean allowsSelfLoops();
  public boolean isDirected();
  public java.util.Set nodes();
  public com.google.common.graph.Graph asGraph();
}
```

## `com.google.common.graph.ImmutableValueGraph$Builder`

```java
public class com.google.common.graph.ImmutableValueGraph$Builder<N, V> {
  public com.google.common.graph.ImmutableValueGraph$Builder<N, V> addNode(N);
  public com.google.common.graph.ImmutableValueGraph$Builder<N, V> putEdgeValue(N, N, V);
  public com.google.common.graph.ImmutableValueGraph$Builder<N, V> putEdgeValue(com.google.common.graph.EndpointPair<N>, V);
  public com.google.common.graph.ImmutableValueGraph<N, V> build();
}
```

## `com.google.common.graph.MutableGraph`

```java
public interface com.google.common.graph.MutableGraph<N> extends com.google.common.graph.Graph<N> {
  public abstract boolean addNode(N);
  public abstract boolean putEdge(N, N);
  public abstract boolean putEdge(com.google.common.graph.EndpointPair<N>);
  public abstract boolean removeNode(N);
  public abstract boolean removeEdge(N, N);
  public abstract boolean removeEdge(com.google.common.graph.EndpointPair<N>);
}
```

## `com.google.common.graph.MutableNetwork`

```java
public interface com.google.common.graph.MutableNetwork<N, E> extends com.google.common.graph.Network<N, E> {
  public abstract boolean addNode(N);
  public abstract boolean addEdge(N, N, E);
  public abstract boolean addEdge(com.google.common.graph.EndpointPair<N>, E);
  public abstract boolean removeNode(N);
  public abstract boolean removeEdge(E);
}
```

## `com.google.common.graph.MutableValueGraph`

```java
public interface com.google.common.graph.MutableValueGraph<N, V> extends com.google.common.graph.ValueGraph<N, V> {
  public abstract boolean addNode(N);
  public abstract V putEdgeValue(N, N, V);
  public abstract V putEdgeValue(com.google.common.graph.EndpointPair<N>, V);
  public abstract boolean removeNode(N);
  public abstract V removeEdge(N, N);
  public abstract V removeEdge(com.google.common.graph.EndpointPair<N>);
}
```

## `com.google.common.graph.Network`

```java
public interface com.google.common.graph.Network<N, E> extends com.google.common.graph.SuccessorsFunction<N>, com.google.common.graph.PredecessorsFunction<N> {
  public abstract java.util.Set<N> nodes();
  public abstract java.util.Set<E> edges();
  public abstract com.google.common.graph.Graph<N> asGraph();
  public abstract boolean isDirected();
  public abstract boolean allowsParallelEdges();
  public abstract boolean allowsSelfLoops();
  public abstract com.google.common.graph.ElementOrder<N> nodeOrder();
  public abstract com.google.common.graph.ElementOrder<E> edgeOrder();
  public abstract java.util.Set<N> adjacentNodes(N);
  public abstract java.util.Set<N> predecessors(N);
  public abstract java.util.Set<N> successors(N);
  public abstract java.util.Set<E> incidentEdges(N);
  public abstract java.util.Set<E> inEdges(N);
  public abstract java.util.Set<E> outEdges(N);
  public abstract int degree(N);
  public abstract int inDegree(N);
  public abstract int outDegree(N);
  public abstract com.google.common.graph.EndpointPair<N> incidentNodes(E);
  public abstract java.util.Set<E> adjacentEdges(E);
  public abstract java.util.Set<E> edgesConnecting(N, N);
  public abstract java.util.Set<E> edgesConnecting(com.google.common.graph.EndpointPair<N>);
  public abstract java.util.Optional<E> edgeConnecting(N, N);
  public abstract java.util.Optional<E> edgeConnecting(com.google.common.graph.EndpointPair<N>);
  public abstract E edgeConnectingOrNull(N, N);
  public abstract E edgeConnectingOrNull(com.google.common.graph.EndpointPair<N>);
  public abstract boolean hasEdgeConnecting(N, N);
  public abstract boolean hasEdgeConnecting(com.google.common.graph.EndpointPair<N>);
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
  public default java.lang.Iterable successors(java.lang.Object);
  public default java.lang.Iterable predecessors(java.lang.Object);
}
```

## `com.google.common.graph.NetworkBuilder`

```java
public final class com.google.common.graph.NetworkBuilder<N, E> extends com.google.common.graph.AbstractGraphBuilder<N> {
  public static com.google.common.graph.NetworkBuilder<java.lang.Object, java.lang.Object> directed();
  public static com.google.common.graph.NetworkBuilder<java.lang.Object, java.lang.Object> undirected();
  public static <N, E> com.google.common.graph.NetworkBuilder<N, E> from(com.google.common.graph.Network<N, E>);
  public <N1 extends N, E1 extends E> com.google.common.graph.ImmutableNetwork$Builder<N1, E1> immutable();
  public com.google.common.graph.NetworkBuilder<N, E> allowsParallelEdges(boolean);
  public com.google.common.graph.NetworkBuilder<N, E> allowsSelfLoops(boolean);
  public com.google.common.graph.NetworkBuilder<N, E> expectedNodeCount(int);
  public com.google.common.graph.NetworkBuilder<N, E> expectedEdgeCount(int);
  public <N1 extends N> com.google.common.graph.NetworkBuilder<N1, E> nodeOrder(com.google.common.graph.ElementOrder<N1>);
  public <E1 extends E> com.google.common.graph.NetworkBuilder<N, E1> edgeOrder(com.google.common.graph.ElementOrder<E1>);
  public <N1 extends N, E1 extends E> com.google.common.graph.MutableNetwork<N1, E1> build();
}
```

## `com.google.common.graph.PredecessorsFunction`

```java
public interface com.google.common.graph.PredecessorsFunction<N> {
  public abstract java.lang.Iterable<? extends N> predecessors(N);
}
```

## `com.google.common.graph.SuccessorsFunction`

```java
public interface com.google.common.graph.SuccessorsFunction<N> {
  public abstract java.lang.Iterable<? extends N> successors(N);
}
```

## `com.google.common.graph.Traverser`

```java
public abstract class com.google.common.graph.Traverser<N> {
  public static <N> com.google.common.graph.Traverser<N> forGraph(com.google.common.graph.SuccessorsFunction<N>);
  public static <N> com.google.common.graph.Traverser<N> forTree(com.google.common.graph.SuccessorsFunction<N>);
  public final java.lang.Iterable<N> breadthFirst(N);
  public final java.lang.Iterable<N> breadthFirst(java.lang.Iterable<? extends N>);
  public final java.lang.Iterable<N> depthFirstPreOrder(N);
  public final java.lang.Iterable<N> depthFirstPreOrder(java.lang.Iterable<? extends N>);
  public final java.lang.Iterable<N> depthFirstPostOrder(N);
  public final java.lang.Iterable<N> depthFirstPostOrder(java.lang.Iterable<? extends N>);
}
```

## `com.google.common.graph.ValueGraph`

```java
public interface com.google.common.graph.ValueGraph<N, V> extends com.google.common.graph.BaseGraph<N> {
  public abstract java.util.Set<N> nodes();
  public abstract java.util.Set<com.google.common.graph.EndpointPair<N>> edges();
  public abstract com.google.common.graph.Graph<N> asGraph();
  public abstract boolean isDirected();
  public abstract boolean allowsSelfLoops();
  public abstract com.google.common.graph.ElementOrder<N> nodeOrder();
  public abstract com.google.common.graph.ElementOrder<N> incidentEdgeOrder();
  public abstract java.util.Set<N> adjacentNodes(N);
  public abstract java.util.Set<N> predecessors(N);
  public abstract java.util.Set<N> successors(N);
  public abstract java.util.Set<com.google.common.graph.EndpointPair<N>> incidentEdges(N);
  public abstract int degree(N);
  public abstract int inDegree(N);
  public abstract int outDegree(N);
  public abstract boolean hasEdgeConnecting(N, N);
  public abstract boolean hasEdgeConnecting(com.google.common.graph.EndpointPair<N>);
  public abstract java.util.Optional<V> edgeValue(N, N);
  public abstract java.util.Optional<V> edgeValue(com.google.common.graph.EndpointPair<N>);
  public abstract V edgeValueOrDefault(N, N, V);
  public abstract V edgeValueOrDefault(com.google.common.graph.EndpointPair<N>, V);
  public abstract boolean equals(java.lang.Object);
  public abstract int hashCode();
  public default java.lang.Iterable successors(java.lang.Object);
  public default java.lang.Iterable predecessors(java.lang.Object);
}
```

## `com.google.common.graph.ValueGraphBuilder`

```java
public final class com.google.common.graph.ValueGraphBuilder<N, V> extends com.google.common.graph.AbstractGraphBuilder<N> {
  public static com.google.common.graph.ValueGraphBuilder<java.lang.Object, java.lang.Object> directed();
  public static com.google.common.graph.ValueGraphBuilder<java.lang.Object, java.lang.Object> undirected();
  public static <N, V> com.google.common.graph.ValueGraphBuilder<N, V> from(com.google.common.graph.ValueGraph<N, V>);
  public <N1 extends N, V1 extends V> com.google.common.graph.ImmutableValueGraph$Builder<N1, V1> immutable();
  public com.google.common.graph.ValueGraphBuilder<N, V> allowsSelfLoops(boolean);
  public com.google.common.graph.ValueGraphBuilder<N, V> expectedNodeCount(int);
  public <N1 extends N> com.google.common.graph.ValueGraphBuilder<N1, V> nodeOrder(com.google.common.graph.ElementOrder<N1>);
  public <N1 extends N> com.google.common.graph.ValueGraphBuilder<N1, V> incidentEdgeOrder(com.google.common.graph.ElementOrder<N1>);
  public <N1 extends N, V1 extends V> com.google.common.graph.MutableValueGraph<N1, V1> build();
}
```
