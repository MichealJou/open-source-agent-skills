# cn.hutool.core.comparator

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.comparator.ComparableComparator` | `boolean equals(final Object object)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.ComparableComparator` | `int compare(final E obj1,final E obj2)` | 比较两个Comparable对象 |
| `cn.hutool.core.comparator.ComparableComparator` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.ComparatorChain` | `ComparatorChain<E> addChain(Comparator<E> element)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.ComparatorChain` | `ComparatorChain<E> addComparator(final Comparator<E> comparator)` | 在链的尾部添加比较器，使用正向排序 |
| `cn.hutool.core.comparator.ComparatorChain` | `ComparatorChain<E> addComparator(final Comparator<E> comparator,final boolean reverse)` | 在链的尾部添加比较器，使用给定排序方式 |
| `cn.hutool.core.comparator.ComparatorChain` | `ComparatorChain<E> of(Comparator<E> comparator)` | 构建 ComparatorChain |
| `cn.hutool.core.comparator.ComparatorChain` | `ComparatorChain<E> of(Comparator<E> comparator,boolean reverse)` | 构建 ComparatorChain |
| `cn.hutool.core.comparator.ComparatorChain` | `ComparatorChain<E> of(Comparator<E>... comparators)` | 构建 ComparatorChain |
| `cn.hutool.core.comparator.ComparatorChain` | `ComparatorChain<E> of(List<Comparator<E>> comparators)` | 构建 ComparatorChain |
| `cn.hutool.core.comparator.ComparatorChain` | `ComparatorChain<E> of(List<Comparator<E>> comparators,BitSet bits)` | 构建 ComparatorChain |
| `cn.hutool.core.comparator.ComparatorChain` | `ComparatorChain<E> setComparator(final int index,final Comparator<E> comparator)` | 替换指定位置的比较器，保持原排序方式 |
| `cn.hutool.core.comparator.ComparatorChain` | `ComparatorChain<E> setComparator(final int index,final Comparator<E> comparator,final boolean reverse)` | 替换指定位置的比较器，替换指定排序方式 |
| `cn.hutool.core.comparator.ComparatorChain` | `ComparatorChain<E> setForwardSort(final int index)` | 更改指定位置的排序方式为正序 |
| `cn.hutool.core.comparator.ComparatorChain` | `ComparatorChain<E> setReverseSort(final int index)` | 更改指定位置的排序方式为反序 |
| `cn.hutool.core.comparator.ComparatorChain` | `Iterator<Comparator<E>> iterator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.ComparatorChain` | `boolean equals(final Object object)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.ComparatorChain` | `boolean isLocked()` | 是否已经被锁定。当开始比较时（调用compare方法）此值为true |
| `cn.hutool.core.comparator.ComparatorChain` | `int compare(final E o1,final E o2)` | 执行比较 按照比较器链的顺序分别比较，如果比较出相等则转向下一个比较器，否则直接返回 |
| `cn.hutool.core.comparator.ComparatorChain` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.ComparatorChain` | `int size()` | 比较器链中比较器个数 |
| `cn.hutool.core.comparator.CompareUtil` | `Comparator<E> naturalComparator()` | 获取自然排序器，即默认排序器 |
| `cn.hutool.core.comparator.CompareUtil` | `Comparator<T> comparingIndexed(Function<? super T, ? extends U> keyExtractor,U... objs)` | 索引比较器 通过keyExtractor函数，提取对象的某个属性或规则，根据提供的排序数组，完成比较 |
| `cn.hutool.core.comparator.CompareUtil` | `Comparator<T> comparingIndexed(Function<? super T, ? extends U> keyExtractor,boolean atEndIfMiss,U... objs)` | 索引比较器 通过keyExtractor函数，提取对象的某个属性或规则，根据提供的排序数组，完成比较 |
| `cn.hutool.core.comparator.CompareUtil` | `Comparator<T> comparingPinyin(Function<T, String> keyExtractor)` | 中文比较器 |
| `cn.hutool.core.comparator.CompareUtil` | `Comparator<T> comparingPinyin(Function<T, String> keyExtractor,boolean reverse)` | 中文（拼音）比较器 |
| `cn.hutool.core.comparator.CompareUtil` | `int compare(T c1,T c2)` | null安全的对象比较，null对象小于任何对象 |
| `cn.hutool.core.comparator.CompareUtil` | `int compare(T c1,T c2,Comparator<T> comparator)` | 对象比较，比较结果取决于comparator，如果被比较对象为null，传入的comparator对象应处理此情况 如果传入comparator为null，则使用默认规则比较（此时被比较对象必须实现Comparable接口） 一般而言，如果c1 < c2，返回数小于0，c1==c2返回0，c1 > c2 大于0 |
| `cn.hutool.core.comparator.CompareUtil` | `int compare(T c1,T c2,boolean isNullGreater)` | null安全的对象比较 |
| `cn.hutool.core.comparator.CompareUtil` | `int compare(T o1,T o2,boolean isNullGreater)` | 自然比较两个对象的大小，比较规则如下： |
| `cn.hutool.core.comparator.IndexedComparator` | `int compare(T o1,T o2)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.InstanceComparator` | `int compare(T o1,T o2)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.LengthComparator` | `int compare(CharSequence o1,CharSequence o2)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.NullComparator` | `Comparator<T> thenComparing(Comparator<? super T> other)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.NullComparator` | `int compare(T a,T b)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.PinyinComparator` | `int compare(String o1,String o2)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.ReverseComparator` | `boolean equals(final Object object)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.ReverseComparator` | `int compare(E o1,E o2)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.ReverseComparator` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.comparator.VersionComparator` | `int compare(String version1,String version2)` | 比较两个版本 null版本排在最小：即： |
| `cn.hutool.core.comparator.WindowsExplorerStringComparator` | `int compare(CharSequence str1,CharSequence str2)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
