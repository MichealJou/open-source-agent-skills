# com.feilong.core.util.predicate

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.core.util.predicate.BeanPredicate` | `boolean evaluate(T object)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.core.util.predicate.BeanPredicateUtil` | `Predicate<T> comparatorPredicate(String propertyName,V valueToCompare,Comparator<V> comparator,Criterion criterion)` | 判断指定的值 valueToCompare criterion 提取的bean对象属性 propertyName 的值 . |
| `com.feilong.core.util.predicate.BeanPredicateUtil` | `Predicate<T> comparatorPredicate(String propertyName,V valueToCompare,Criterion criterion)` | 判断指定的值 valueToCompare criterion 提取的bean对象属性 propertyName 的值 . 注意: 是参数 valueToCompare 和 属性值进行比较 criterion , BeanPredicateUtil.comparatorPredicate("age", 20, Criterion.LESS) 表示提取所有比20 大的结果 |
| `com.feilong.core.util.predicate.BeanPredicateUtil` | `Predicate<T> containsPredicate(final String propertyName,final Collection<V> propertyValueList)` | 调用 PropertyUtil#getProperty(Object, String) 获得 propertyName 的值,使用java.util.Collection#contains(Object) Collection.contains 判断是否在 values 集合中. |
| `com.feilong.core.util.predicate.BeanPredicateUtil` | `Predicate<T> containsPredicate(final String propertyName,final V... propertyValues)` | 调用 PropertyUtil#getProperty(Object, String) 获得 propertyName 的值,使用 com.feilong.lib.lang3.ArrayUtils#contains(Object[], Object) ArrayUtils.contains 判断是否在 values 数组中. |
| `com.feilong.core.util.predicate.BeanPredicateUtil` | `Predicate<T> equalIgnoreCasePredicate(String propertyName,String propertyValue)` | 用来指定 T 对象的特定属性 propertyName equalsIgnoreCase 指定的 propertyValue . |
| `com.feilong.core.util.predicate.BeanPredicateUtil` | `Predicate<T> equalPredicate(Map<String, ?> propertyNameAndPropertyValueMap)` | 用来判断一个对象指定的属性以及属性值是否相等. |
| `com.feilong.core.util.predicate.BeanPredicateUtil` | `Predicate<T> equalPredicate(String propertyName,V propertyValue)` | 用来指定 T 对象的特定属性 propertyName equals 指定的 propertyValue . |
| `com.feilong.core.util.predicate.BeanPredicateUtil` | `Predicate<T> equalPredicate(T bean,String... propertyNames)` | 构造属性与一个指定对象 bean 的一组属性的值 propertyNames 都相等的判断器. |
| `com.feilong.core.util.predicate.ContainsStringPredicate` | `CharSequence getSearchCharSequence()` | 【原文待译】Gets the search char sequence. |
| `com.feilong.core.util.predicate.ContainsStringPredicate` | `boolean evaluate(String value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.core.util.predicate.ContainsStringPredicate` | `void setSearchCharSequence(CharSequence searchCharSequence)` | 【原文待译】Sets the search char sequence. |
| `com.feilong.core.util.predicate.NotNullOrEmptyStringPredicate` | `boolean evaluate(String value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.core.util.predicate.RegexStringPredicate` | `boolean evaluate(String value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
