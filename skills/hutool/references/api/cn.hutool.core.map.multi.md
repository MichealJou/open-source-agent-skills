# cn.hutool.core.map.multi

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.map.multi.AbsCollValueMap`

```java
public abstract class cn.hutool.core.map.multi.AbsCollValueMap<K, V, C extends java.util.Collection<V>> extends cn.hutool.core.map.MapWrapper<K, C> {
  public cn.hutool.core.map.multi.AbsCollValueMap();
  public cn.hutool.core.map.multi.AbsCollValueMap(int);
  public cn.hutool.core.map.multi.AbsCollValueMap(java.util.Map<? extends K, C>);
  public cn.hutool.core.map.multi.AbsCollValueMap(float, java.util.Map<? extends K, C>);
  public cn.hutool.core.map.multi.AbsCollValueMap(int, float);
  public void putAllValues(java.util.Map<? extends K, ? extends java.util.Collection<V>>);
  public void putValue(K, V);
  public V get(K, int);
  public boolean removeValue(K, V);
  public boolean removeValues(K, java.util.Collection<V>);
}
```

## `cn.hutool.core.map.multi.AbsTable`

```java
public abstract class cn.hutool.core.map.multi.AbsTable<R, C, V> implements cn.hutool.core.map.multi.Table<R, C, V> {
  public cn.hutool.core.map.multi.AbsTable();
  public boolean equals(java.lang.Object);
  public int hashCode();
  public java.lang.String toString();
  public java.util.Collection<V> values();
  public java.util.Set<cn.hutool.core.map.multi.Table$Cell<R, C, V>> cellSet();
  public java.util.Iterator<cn.hutool.core.map.multi.Table$Cell<R, C, V>> iterator();
}
```

## `cn.hutool.core.map.multi.CollectionValueMap`

```java
public class cn.hutool.core.map.multi.CollectionValueMap<K, V> extends cn.hutool.core.map.multi.AbsCollValueMap<K, V, java.util.Collection<V>> {
  public cn.hutool.core.map.multi.CollectionValueMap();
  public cn.hutool.core.map.multi.CollectionValueMap(int);
  public cn.hutool.core.map.multi.CollectionValueMap(java.util.Map<? extends K, ? extends java.util.Collection<V>>);
  public cn.hutool.core.map.multi.CollectionValueMap(float, java.util.Map<? extends K, ? extends java.util.Collection<V>>);
  public cn.hutool.core.map.multi.CollectionValueMap(int, float);
  public cn.hutool.core.map.multi.CollectionValueMap(float, java.util.Map<? extends K, ? extends java.util.Collection<V>>, cn.hutool.core.lang.func.Func0<java.util.Collection<V>>);
  public cn.hutool.core.map.multi.CollectionValueMap(int, float, cn.hutool.core.lang.func.Func0<java.util.Collection<V>>);
}
```

## `cn.hutool.core.map.multi.ListValueMap`

```java
public class cn.hutool.core.map.multi.ListValueMap<K, V> extends cn.hutool.core.map.multi.AbsCollValueMap<K, V, java.util.List<V>> {
  public cn.hutool.core.map.multi.ListValueMap();
  public cn.hutool.core.map.multi.ListValueMap(int);
  public cn.hutool.core.map.multi.ListValueMap(java.util.Map<? extends K, ? extends java.util.Collection<V>>);
  public cn.hutool.core.map.multi.ListValueMap(float, java.util.Map<? extends K, ? extends java.util.Collection<V>>);
  public cn.hutool.core.map.multi.ListValueMap(int, float);
}
```

## `cn.hutool.core.map.multi.RowKeyTable`

```java
public class cn.hutool.core.map.multi.RowKeyTable<R, C, V> extends cn.hutool.core.map.multi.AbsTable<R, C, V> {
  public cn.hutool.core.map.multi.RowKeyTable();
  public cn.hutool.core.map.multi.RowKeyTable(boolean);
  public cn.hutool.core.map.multi.RowKeyTable(java.util.Map<R, java.util.Map<C, V>>);
  public cn.hutool.core.map.multi.RowKeyTable(java.util.Map<R, java.util.Map<C, V>>, cn.hutool.core.builder.Builder<? extends java.util.Map<C, V>>);
  public java.util.Map<R, java.util.Map<C, V>> rowMap();
  public V put(R, C, V);
  public V remove(R, C);
  public boolean isEmpty();
  public void clear();
  public boolean containsColumn(C);
  public java.util.Map<C, java.util.Map<R, V>> columnMap();
  public java.util.Set<C> columnKeySet();
  public java.util.List<C> columnKeys();
  public java.util.Map<R, V> getColumn(C);
}
```

## `cn.hutool.core.map.multi.SetValueMap`

```java
public class cn.hutool.core.map.multi.SetValueMap<K, V> extends cn.hutool.core.map.multi.AbsCollValueMap<K, V, java.util.Set<V>> {
  public cn.hutool.core.map.multi.SetValueMap();
  public cn.hutool.core.map.multi.SetValueMap(int);
  public cn.hutool.core.map.multi.SetValueMap(java.util.Map<? extends K, ? extends java.util.Collection<V>>);
  public cn.hutool.core.map.multi.SetValueMap(float, java.util.Map<? extends K, ? extends java.util.Collection<V>>);
  public cn.hutool.core.map.multi.SetValueMap(int, float);
}
```

## `cn.hutool.core.map.multi.Table`

```java
public interface cn.hutool.core.map.multi.Table<R, C, V> extends java.lang.Iterable<cn.hutool.core.map.multi.Table$Cell<R, C, V>> {
  public default boolean contains(R, C);
  public default boolean containsRow(R);
  public default java.util.Map<C, V> getRow(R);
  public default java.util.Set<R> rowKeySet();
  public abstract java.util.Map<R, java.util.Map<C, V>> rowMap();
  public default boolean containsColumn(C);
  public default java.util.Map<R, V> getColumn(C);
  public default java.util.Set<C> columnKeySet();
  public default java.util.List<C> columnKeys();
  public abstract java.util.Map<C, java.util.Map<R, V>> columnMap();
  public default boolean containsValue(V);
  public default V get(R, C);
  public abstract java.util.Collection<V> values();
  public abstract java.util.Set<cn.hutool.core.map.multi.Table$Cell<R, C, V>> cellSet();
  public abstract V put(R, C, V);
  public default void putAll(cn.hutool.core.map.multi.Table<? extends R, ? extends C, ? extends V>);
  public abstract V remove(R, C);
  public abstract boolean isEmpty();
  public default int size();
  public abstract void clear();
  public default void forEach(cn.hutool.core.lang.func.Consumer3<? super R, ? super C, ? super V>);
}
```

## `cn.hutool.core.map.multi.Table$Cell`

```java
public interface cn.hutool.core.map.multi.Table$Cell<R, C, V> {
  public abstract R getRowKey();
  public abstract C getColumnKey();
  public abstract V getValue();
}
```
