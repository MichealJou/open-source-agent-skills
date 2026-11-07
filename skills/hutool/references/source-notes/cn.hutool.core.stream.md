# cn.hutool.core.stream

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.stream.CollectorUtil` | `BinaryOperator<M> mapMerger(BinaryOperator<V> mergeFunction)` | 用户合并map的BinaryOperator，传入合并前需要对value进行的操作 |
| `cn.hutool.core.stream.CollectorUtil` | `Collector<Map<K, V>, ?, Map<K, List<V>>> reduceListMap()` | 聚合这种数据类型:Collection > => Map > 其中key相同的value，会累加到List中 |
| `cn.hutool.core.stream.CollectorUtil` | `Collector<Map<K, V>, ?, R> reduceListMap(final Supplier<R> mapSupplier)` | 聚合这种数据类型:Collection > => Map > 其中key相同的value，会累加到List中 |
| `cn.hutool.core.stream.CollectorUtil` | `Collector<T, ?, M> groupingBy(Function<? super T, ? extends K> classifier,Supplier<M> mapFactory,Collector<? super T, A, D> downstream)` | 提供对null值友好的groupingBy操作的Collector实现，可指定map类型 |
| `cn.hutool.core.stream.CollectorUtil` | `Collector<T, ?, M> groupingBy(final Function<? super T, ? extends K> classifier,final Function<? super T, ? extends R> valueMapper,final Supplier<C> valueCollFactory,final Supplier<M> mapFactory)` | 提供对null值友好的groupingBy操作的Collector实现， 对集合分组，然后对分组后的值集合进行映射 |
| `cn.hutool.core.stream.CollectorUtil` | `Collector<T, ?, M> toMap(Function<? super T, ? extends K> keyMapper,Function<? super T, ? extends U> valueMapper,BinaryOperator<U> mergeFunction,Supplier<M> mapSupplier)` | 对null友好的 toMap 操作的 Collector实现 |
| `cn.hutool.core.stream.CollectorUtil` | `Collector<T, ?, Map<K, C>> groupingBy(final Function<? super T, ? extends K> classifier,final Function<? super T, ? extends R> valueMapper,final Supplier<C> valueCollFactory)` | 提供对null值友好的groupingBy操作的Collector实现， 对集合分组，然后对分组后的值集合进行映射 |
| `cn.hutool.core.stream.CollectorUtil` | `Collector<T, ?, Map<K, D>> groupingBy(Function<? super T, ? extends K> classifier,Collector<? super T, A, D> downstream)` | 提供对null值友好的groupingBy操作的Collector实现 |
| `cn.hutool.core.stream.CollectorUtil` | `Collector<T, ?, Map<K, List<R>>> groupingBy(final Function<? super T, ? extends K> classifier,final Function<? super T, ? extends R> valueMapper)` | 提供对null值友好的groupingBy操作的Collector实现， 对集合分组，然后对分组后的值集合进行映射 |
| `cn.hutool.core.stream.CollectorUtil` | `Collector<T, ?, Map<K, List<T>>> groupingBy(Function<? super T, ? extends K> classifier)` | 提供对null值友好的groupingBy操作的Collector实现 |
| `cn.hutool.core.stream.CollectorUtil` | `Collector<T, ?, Map<K, U>> toMap(Function<? super T, ? extends K> keyMapper,Function<? super T, ? extends U> valueMapper,BinaryOperator<U> mergeFunction)` | 对null友好的 toMap 操作的 Collector实现，默认使用HashMap |
| `cn.hutool.core.stream.CollectorUtil` | `Collector<T, ?, String> joining(CharSequence delimiter)` | 提供任意对象的Join操作的Collector实现，对象默认调用toString方法 |
| `cn.hutool.core.stream.CollectorUtil` | `Collector<T, ?, String> joining(CharSequence delimiter,CharSequence prefix,CharSequence suffix,Function<T, ? extends CharSequence> toStringFunc)` | 提供任意对象的Join操作的Collector实现 |
| `cn.hutool.core.stream.CollectorUtil` | `Collector<T, ?, String> joining(CharSequence delimiter,Function<T, ? extends CharSequence> toStringFunc)` | 提供任意对象的Join操作的Collector实现 |
| `cn.hutool.core.stream.SimpleCollector` | `BiConsumer<A, T> accumulator()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.stream.SimpleCollector` | `BinaryOperator<A> combiner()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.stream.SimpleCollector` | `Function<A, R> finisher()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.stream.SimpleCollector` | `Set<Characteristics> characteristics()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.stream.SimpleCollector` | `Supplier<A> supplier()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.stream.StreamUtil` | `Stream<String> of(File file)` | 按行读取文件为Stream |
| `cn.hutool.core.stream.StreamUtil` | `Stream<String> of(File file,Charset charset)` | 按行读取文件为Stream |
| `cn.hutool.core.stream.StreamUtil` | `Stream<String> of(Path path)` | 按行读取文件为Stream |
| `cn.hutool.core.stream.StreamUtil` | `Stream<String> of(Path path,Charset charset)` | 按行读取文件为Stream |
| `cn.hutool.core.stream.StreamUtil` | `Stream<T> of(Iterable<T> iterable)` | Iterable转换为Stream，默认非并行 |
| `cn.hutool.core.stream.StreamUtil` | `Stream<T> of(Iterable<T> iterable,boolean parallel)` | Iterable转换为Stream |
| `cn.hutool.core.stream.StreamUtil` | `Stream<T> of(Iterator<T> iterator)` | Iterator 转换为 Stream |
| `cn.hutool.core.stream.StreamUtil` | `Stream<T> of(Iterator<T> iterator,boolean parallel)` | Iterator 转换为 Stream |
| `cn.hutool.core.stream.StreamUtil` | `Stream<T> of(T seed,UnaryOperator<T> elementCreator,int limit)` | 通过函数创建Stream |
| `cn.hutool.core.stream.StreamUtil` | `Stream<T> of(T... array)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.stream.StreamUtil` | `String join(Stream<T> stream,CharSequence delimiter)` | 将Stream中所有元素以指定分隔符，合并为一个字符串，对象默认调用toString方法 |
| `cn.hutool.core.stream.StreamUtil` | `String join(Stream<T> stream,CharSequence delimiter,Function<T, ? extends CharSequence> toStringFunc)` | 将Stream中所有元素以指定分隔符，合并为一个字符串 |
