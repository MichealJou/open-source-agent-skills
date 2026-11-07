# com.feilong.core.util.predicate

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.core.util.predicate.BeanPredicate`

```java
public class com.feilong.core.util.predicate.BeanPredicate<T> implements org.apache.commons.collections4.Predicate<T> {
  public com.feilong.core.util.predicate.BeanPredicate(java.lang.String, org.apache.commons.collections4.Predicate);
  public boolean evaluate(T);
}
```

## `com.feilong.core.util.predicate.BeanPredicateUtil`

```java
public final class com.feilong.core.util.predicate.BeanPredicateUtil {
  public static <T, V> org.apache.commons.collections4.Predicate<T> equalPredicate(java.lang.String, V);
  public static <T> org.apache.commons.collections4.Predicate<T> equalIgnoreCasePredicate(java.lang.String, java.lang.String);
  public static <T> org.apache.commons.collections4.Predicate<T> equalPredicate(java.util.Map<java.lang.String, ?>);
  public static <T> org.apache.commons.collections4.Predicate<T> equalPredicate(T, java.lang.String...);
  public static <T, V> org.apache.commons.collections4.Predicate<T> containsPredicate(java.lang.String, V...);
  public static <T, V> org.apache.commons.collections4.Predicate<T> containsPredicate(java.lang.String, java.util.Collection<V>);
  public static <T, V extends java.lang.Comparable<? super V>> org.apache.commons.collections4.Predicate<T> comparatorPredicate(java.lang.String, V, com.feilong.lib.collection4.functors.ComparatorPredicate$Criterion);
  public static <T, V extends java.lang.Comparable<? super V>> org.apache.commons.collections4.Predicate<T> comparatorPredicate(java.lang.String, V, java.util.Comparator<V>, com.feilong.lib.collection4.functors.ComparatorPredicate$Criterion);
}
```

## `com.feilong.core.util.predicate.ContainsStringPredicate`

```java
public class com.feilong.core.util.predicate.ContainsStringPredicate implements com.feilong.core.util.predicate.StringPredicate {
  public com.feilong.core.util.predicate.ContainsStringPredicate();
  public com.feilong.core.util.predicate.ContainsStringPredicate(java.lang.CharSequence);
  public boolean evaluate(java.lang.String);
  public java.lang.CharSequence getSearchCharSequence();
  public void setSearchCharSequence(java.lang.CharSequence);
  public boolean evaluate(java.lang.Object);
}
```

## `com.feilong.core.util.predicate.NotNullOrEmptyStringPredicate`

```java
public class com.feilong.core.util.predicate.NotNullOrEmptyStringPredicate implements com.feilong.core.util.predicate.StringPredicate {
  public com.feilong.core.util.predicate.NotNullOrEmptyStringPredicate();
  public boolean evaluate(java.lang.String);
  public boolean evaluate(java.lang.Object);
}
```

## `com.feilong.core.util.predicate.RegexStringPredicate`

```java
public class com.feilong.core.util.predicate.RegexStringPredicate implements com.feilong.core.util.predicate.StringPredicate {
  public com.feilong.core.util.predicate.RegexStringPredicate(java.lang.String);
  public boolean evaluate(java.lang.String);
  public boolean evaluate(java.lang.Object);
}
```
