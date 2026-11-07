# cn.hutool.core.map.reference

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.map.reference.ReferenceConcurrentMap`

```java
public abstract class cn.hutool.core.map.reference.ReferenceConcurrentMap<K, V> implements java.util.concurrent.ConcurrentMap<K, V>, java.lang.Iterable<java.util.Map$Entry<K, V>>, java.io.Serializable {
  public cn.hutool.core.map.reference.ReferenceConcurrentMap(java.util.concurrent.ConcurrentMap<cn.hutool.core.lang.ref.Ref<K>, cn.hutool.core.lang.ref.Ref<V>>);
  public void setPurgeListener(java.util.function.BiConsumer<cn.hutool.core.lang.ref.Ref<? extends K>, cn.hutool.core.lang.ref.Ref<? extends V>>);
  public int size();
  public boolean isEmpty();
  public V get(java.lang.Object);
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public V put(K, V);
  public V putIfAbsent(K, V);
  public void putAll(java.util.Map<? extends K, ? extends V>);
  public V replace(K, V);
  public boolean replace(K, V, V);
  public void replaceAll(java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public V computeIfAbsent(K, java.util.function.Function<? super K, ? extends V>);
  public V computeIfPresent(K, java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public V remove(java.lang.Object);
  public boolean remove(java.lang.Object, java.lang.Object);
  public void clear();
  public java.util.Set<K> keySet();
  public java.util.Collection<V> values();
  public java.util.Set<java.util.Map$Entry<K, V>> entrySet();
  public void forEach(java.util.function.BiConsumer<? super K, ? super V>);
  public java.util.Iterator<java.util.Map$Entry<K, V>> iterator();
  public V compute(K, java.util.function.BiFunction<? super K, ? super V, ? extends V>);
  public V merge(K, V, java.util.function.BiFunction<? super V, ? super V, ? extends V>);
}
```

## `cn.hutool.core.map.reference.SoftConcurrentMap`

```java
public class cn.hutool.core.map.reference.SoftConcurrentMap<K, V> extends cn.hutool.core.map.reference.ReferenceConcurrentMap<K, V> {
  public cn.hutool.core.map.reference.SoftConcurrentMap();
  public cn.hutool.core.map.reference.SoftConcurrentMap(java.util.concurrent.ConcurrentMap<cn.hutool.core.lang.ref.Ref<K>, cn.hutool.core.lang.ref.Ref<V>>);
}
```

## `cn.hutool.core.map.reference.WeakKeyConcurrentMap`

```java
public class cn.hutool.core.map.reference.WeakKeyConcurrentMap<K, V> extends cn.hutool.core.map.reference.ReferenceConcurrentMap<K, V> {
  public cn.hutool.core.map.reference.WeakKeyConcurrentMap();
  public cn.hutool.core.map.reference.WeakKeyConcurrentMap(java.util.concurrent.ConcurrentMap<cn.hutool.core.lang.ref.Ref<K>, cn.hutool.core.lang.ref.Ref<V>>);
}
```

## `cn.hutool.core.map.reference.WeakKeyValueConcurrentMap`

```java
public class cn.hutool.core.map.reference.WeakKeyValueConcurrentMap<K, V> extends cn.hutool.core.map.reference.ReferenceConcurrentMap<K, V> {
  public cn.hutool.core.map.reference.WeakKeyValueConcurrentMap();
  public cn.hutool.core.map.reference.WeakKeyValueConcurrentMap(java.util.concurrent.ConcurrentMap<cn.hutool.core.lang.ref.Ref<K>, cn.hutool.core.lang.ref.Ref<V>>);
}
```
