# com.feilong.core.util.comparator

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.core.util.comparator.BeanComparatorUtil` | `Comparator<T> chainedComparator(String... propertyNameAndOrders)` | 按照不同指定属性 propertyNameAndOrders 排序的 Comparator. |
| `com.feilong.core.util.comparator.BeanComparatorUtil` | `Comparator<T> propertyComparator(String propertyName,List<V> propertyValues)` | 指定属性 propertyName 按照固定顺序值 propertyValues 排序的 Comparator. 调用 #propertyComparator(String, List, UnknownObjectBehavior),默认 UnknownObjectBehavior#AFTER |
| `com.feilong.core.util.comparator.BeanComparatorUtil` | `Comparator<T> propertyComparator(String propertyName,List<V> propertyValues,UnknownObjectBehavior unknownObjectBehavior)` | 指定属性 propertyName 按照固定顺序值 propertyValues ,并且可以指定 unknownObjectBehavior 排序的 Comparator. |
| `com.feilong.core.util.comparator.BeanComparatorUtil` | `Comparator<T> propertyComparator(String propertyName,V... propertyValues)` | 指定属性 propertyName 按照固定顺序值 propertyValues 排序的 Comparator. |
| `com.feilong.core.util.comparator.BeanComparatorUtil` | `Comparator<T> propertyComparator(String propertyNameAndOrder)` | 指定属性 propertyName ,按照自然顺序 排序的 Comparator. |
| `com.feilong.core.util.comparator.ComparatorUtil` | `FixedOrderComparator<T> buildFixedOrderComparator(List<T> list)` | Builds the. 默认使用的是 UnknownObjectBehavior#AFTER ,不在指定固定顺序的元素将排在后面 |
| `com.feilong.core.util.comparator.ComparatorUtil` | `FixedOrderComparator<T> buildFixedOrderComparator(List<T> list,UnknownObjectBehavior unknownObjectBehavior)` | 【原文待译】Builds the. |
| `com.feilong.core.util.comparator.PropertyComparator` | `int compare(T t1,T t2)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.core.util.comparator.RegexGroupNumberComparator` | `int compare(String s1,String s2)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.core.util.comparator.SortHelper` | `String[] parsePropertyNameAndOrder(String propertyNameAndOrder)` | 将 propertyNameAndOrder 字符串转换成数组. 会先进行trim操作,再使用StringUtils#SPACE 分隔成数组 |
| `com.feilong.core.util.comparator.SortHelper` | `boolean isAsc(String[] propertyNameAndOrderArray)` | 判断属性名称和排序因子数组是不是asc排序. |
