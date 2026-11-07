# cn.hutool.core.map.multi

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.map.multi.AbsCollValueMap` | `V get(K key,int index)` | 获取值 |
| `cn.hutool.core.map.multi.AbsCollValueMap` | `boolean removeValue(K key,V value)` | 移除value集合中的某个值 |
| `cn.hutool.core.map.multi.AbsCollValueMap` | `boolean removeValues(K key,Collection<V> values)` | 移除value集合中的某些值 |
| `cn.hutool.core.map.multi.AbsCollValueMap` | `void putAllValues(Map<? extends K, ? extends Collection<V>> m)` | 放入所有value |
| `cn.hutool.core.map.multi.AbsCollValueMap` | `void putValue(K key,V value)` | 放入Value 如果键对应值列表有值，加入，否则创建一个新列表后加入 |
| `cn.hutool.core.map.multi.AbsTable` | `Collection<V> values()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.AbsTable` | `Iterator<Cell<R, C, V>> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.AbsTable` | `Set<Cell<R, C, V>> cellSet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.AbsTable` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.AbsTable` | `boolean equals(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.AbsTable` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.RowKeyTable` | `List<C> columnKeys()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.RowKeyTable` | `Map<C, Map<R, V>> columnMap()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.RowKeyTable` | `Map<R, Map<C, V>> rowMap()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.RowKeyTable` | `Map<R, V> getColumn(C columnKey)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.RowKeyTable` | `Set<C> columnKeySet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.RowKeyTable` | `V put(R rowKey,C columnKey,V value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.RowKeyTable` | `V remove(R rowKey,C columnKey)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.RowKeyTable` | `boolean containsColumn(C columnKey)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.RowKeyTable` | `boolean isEmpty()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.RowKeyTable` | `void clear()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.map.multi.Table` | `Collection<V> values()` | 所有行列值的集合 |
| `cn.hutool.core.map.multi.Table` | `List<C> columnKeys()` | 返回所有列的key，列的key如果实现Map是可重复key，则返回对应不去重的List。 |
| `cn.hutool.core.map.multi.Table` | `Map<C, Map<R, V>> columnMap()` | 返回列-行对应的map |
| `cn.hutool.core.map.multi.Table` | `Map<C, V> getRow(R rowKey)` | 获取行 |
| `cn.hutool.core.map.multi.Table` | `Map<R, Map<C, V>> rowMap()` | 返回行列对应的Map |
| `cn.hutool.core.map.multi.Table` | `Map<R, V> getColumn(C columnKey)` | 获取列 |
| `cn.hutool.core.map.multi.Table` | `Set<C> columnKeySet()` | 返回所有列的key，列的key不可重复 |
| `cn.hutool.core.map.multi.Table` | `Set<Cell<R, C, V>> cellSet()` | 所有单元格集合 |
| `cn.hutool.core.map.multi.Table` | `Set<R> rowKeySet()` | 返回所有行的key，行的key不可重复 |
| `cn.hutool.core.map.multi.Table` | `V get(R rowKey,C columnKey)` | 获取指定值 |
| `cn.hutool.core.map.multi.Table` | `V put(R rowKey,C columnKey,V value)` | 为表格指定行列赋值，如果不存在，创建之，存在则替换之，返回原值 |
| `cn.hutool.core.map.multi.Table` | `V remove(R rowKey,C columnKey)` | 移除指定值 |
| `cn.hutool.core.map.multi.Table` | `boolean contains(R rowKey,C columnKey)` | 是否包含指定行列的映射 行和列任意一个不存在都会返回false，如果行和列都存在，值为null，也会返回true |
| `cn.hutool.core.map.multi.Table` | `boolean containsColumn(C columnKey)` | 列是否存在 |
| `cn.hutool.core.map.multi.Table` | `boolean containsRow(R rowKey)` | 行是否存在 |
| `cn.hutool.core.map.multi.Table` | `boolean containsValue(V value)` | 指定值是否存在 |
| `cn.hutool.core.map.multi.Table` | `boolean isEmpty()` | 表格是否为空 |
| `cn.hutool.core.map.multi.Table` | `int size()` | 表格大小，一般为单元格的个数 |
| `cn.hutool.core.map.multi.Table` | `void clear()` | 清空表格 |
| `cn.hutool.core.map.multi.Table` | `void forEach(Consumer3<? super R, ? super C, ? super V> consumer)` | 遍历表格的单元格，处理值 |
| `cn.hutool.core.map.multi.Table` | `void putAll(Table<? extends R, ? extends C, ? extends V> table)` | 批量加入 |
| `cn.hutool.core.map.multi.Table$Cell` | `C getColumnKey()` | 获取列键 |
| `cn.hutool.core.map.multi.Table$Cell` | `R getRowKey()` | 获取行键 |
| `cn.hutool.core.map.multi.Table$Cell` | `V getValue()` | 获取值 |
