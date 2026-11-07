# com.feilong.lib.collection4.functors

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.collection4.functors.AbstractQuantifierPredicate`

```java
public abstract class com.feilong.lib.collection4.functors.AbstractQuantifierPredicate<T> implements com.feilong.lib.collection4.functors.PredicateDecorator<T>, java.io.Serializable {
  public com.feilong.lib.collection4.functors.AbstractQuantifierPredicate(org.apache.commons.collections4.Predicate<? super T>...);
  public org.apache.commons.collections4.Predicate<? super T>[] getPredicates();
}
```

## `com.feilong.lib.collection4.functors.AllPredicate`

```java
public final class com.feilong.lib.collection4.functors.AllPredicate<T> extends com.feilong.lib.collection4.functors.AbstractQuantifierPredicate<T> {
  public static <T> org.apache.commons.collections4.Predicate<T> allPredicate(org.apache.commons.collections4.Predicate<? super T>...);
  public static <T> org.apache.commons.collections4.Predicate<T> allPredicate(java.util.Collection<? extends org.apache.commons.collections4.Predicate<? super T>>);
  public com.feilong.lib.collection4.functors.AllPredicate(org.apache.commons.collections4.Predicate<? super T>...);
  public boolean evaluate(T);
}
```

## `com.feilong.lib.collection4.functors.AndPredicate`

```java
public final class com.feilong.lib.collection4.functors.AndPredicate<T> implements com.feilong.lib.collection4.functors.PredicateDecorator<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> andPredicate(org.apache.commons.collections4.Predicate<? super T>, org.apache.commons.collections4.Predicate<? super T>);
  public com.feilong.lib.collection4.functors.AndPredicate(org.apache.commons.collections4.Predicate<? super T>, org.apache.commons.collections4.Predicate<? super T>);
  public boolean evaluate(T);
  public org.apache.commons.collections4.Predicate<? super T>[] getPredicates();
}
```

## `com.feilong.lib.collection4.functors.AnyPredicate`

```java
public final class com.feilong.lib.collection4.functors.AnyPredicate<T> extends com.feilong.lib.collection4.functors.AbstractQuantifierPredicate<T> {
  public static <T> org.apache.commons.collections4.Predicate<T> anyPredicate(org.apache.commons.collections4.Predicate<? super T>...);
  public static <T> org.apache.commons.collections4.Predicate<T> anyPredicate(java.util.Collection<? extends org.apache.commons.collections4.Predicate<? super T>>);
  public com.feilong.lib.collection4.functors.AnyPredicate(org.apache.commons.collections4.Predicate<? super T>...);
  public boolean evaluate(T);
}
```

## `com.feilong.lib.collection4.functors.CatchAndRethrowClosure`

```java
public abstract class com.feilong.lib.collection4.functors.CatchAndRethrowClosure<E> implements org.apache.commons.collections4.Closure<E> {
  public com.feilong.lib.collection4.functors.CatchAndRethrowClosure();
  public void execute(E);
}
```

## `com.feilong.lib.collection4.functors.ChainedClosure`

```java
public class com.feilong.lib.collection4.functors.ChainedClosure<E> implements org.apache.commons.collections4.Closure<E>, java.io.Serializable {
  public static <E> org.apache.commons.collections4.Closure<E> chainedClosure(org.apache.commons.collections4.Closure<? super E>...);
  public static <E> org.apache.commons.collections4.Closure<E> chainedClosure(java.util.Collection<? extends org.apache.commons.collections4.Closure<? super E>>);
  public com.feilong.lib.collection4.functors.ChainedClosure(org.apache.commons.collections4.Closure<? super E>...);
  public void execute(E);
  public org.apache.commons.collections4.Closure<? super E>[] getClosures();
}
```

## `com.feilong.lib.collection4.functors.ChainedTransformer`

```java
public class com.feilong.lib.collection4.functors.ChainedTransformer<T> implements org.apache.commons.collections4.Transformer<T, T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Transformer<T, T> chainedTransformer(org.apache.commons.collections4.Transformer<? super T, ? extends T>...);
  public static <T> org.apache.commons.collections4.Transformer<T, T> chainedTransformer(java.util.Collection<? extends org.apache.commons.collections4.Transformer<? super T, ? extends T>>);
  public com.feilong.lib.collection4.functors.ChainedTransformer(org.apache.commons.collections4.Transformer<? super T, ? extends T>...);
  public T transform(T);
  public org.apache.commons.collections4.Transformer<? super T, ? extends T>[] getTransformers();
}
```

## `com.feilong.lib.collection4.functors.ClosureTransformer`

```java
public class com.feilong.lib.collection4.functors.ClosureTransformer<T> implements org.apache.commons.collections4.Transformer<T, T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Transformer<T, T> closureTransformer(org.apache.commons.collections4.Closure<? super T>);
  public com.feilong.lib.collection4.functors.ClosureTransformer(org.apache.commons.collections4.Closure<? super T>);
  public T transform(T);
  public org.apache.commons.collections4.Closure<? super T> getClosure();
}
```

## `com.feilong.lib.collection4.functors.ComparatorPredicate`

```java
public class com.feilong.lib.collection4.functors.ComparatorPredicate<T> implements org.apache.commons.collections4.Predicate<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> comparatorPredicate(T, java.util.Comparator<T>);
  public static <T> org.apache.commons.collections4.Predicate<T> comparatorPredicate(T, java.util.Comparator<T>, com.feilong.lib.collection4.functors.ComparatorPredicate$Criterion);
  public com.feilong.lib.collection4.functors.ComparatorPredicate(T, java.util.Comparator<T>, com.feilong.lib.collection4.functors.ComparatorPredicate$Criterion);
  public boolean evaluate(T);
}
```

## `com.feilong.lib.collection4.functors.ComparatorPredicate$Criterion`

```java
public final class com.feilong.lib.collection4.functors.ComparatorPredicate$Criterion extends java.lang.Enum<com.feilong.lib.collection4.functors.ComparatorPredicate$Criterion> {
  public static com.feilong.lib.collection4.functors.ComparatorPredicate$Criterion[] values();
  public static com.feilong.lib.collection4.functors.ComparatorPredicate$Criterion valueOf(java.lang.String);
}
```

## `com.feilong.lib.collection4.functors.ConstantTransformer`

```java
public class com.feilong.lib.collection4.functors.ConstantTransformer<I, O> implements org.apache.commons.collections4.Transformer<I, O>, java.io.Serializable {
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> nullTransformer();
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> constantTransformer(O);
  public com.feilong.lib.collection4.functors.ConstantTransformer(O);
  public O transform(I);
  public O getConstant();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.feilong.lib.collection4.functors.DefaultEquator`

```java
public class com.feilong.lib.collection4.functors.DefaultEquator<T> implements org.apache.commons.collections4.Equator<T>, java.io.Serializable {
  public static <T> com.feilong.lib.collection4.functors.DefaultEquator<T> defaultEquator();
  public boolean equate(T, T);
  public int hash(T);
}
```

## `com.feilong.lib.collection4.functors.EqualPredicate`

```java
public final class com.feilong.lib.collection4.functors.EqualPredicate<T> implements org.apache.commons.collections4.Predicate<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> equalPredicate(T);
  public static <T> org.apache.commons.collections4.Predicate<T> equalPredicate(T, org.apache.commons.collections4.Equator<T>);
  public com.feilong.lib.collection4.functors.EqualPredicate(T);
  public com.feilong.lib.collection4.functors.EqualPredicate(T, org.apache.commons.collections4.Equator<T>);
  public boolean evaluate(T);
  public java.lang.Object getValue();
}
```

## `com.feilong.lib.collection4.functors.ExceptionClosure`

```java
public final class com.feilong.lib.collection4.functors.ExceptionClosure<E> implements org.apache.commons.collections4.Closure<E>, java.io.Serializable {
  public static <E> org.apache.commons.collections4.Closure<E> exceptionClosure();
  public void execute(E);
}
```

## `com.feilong.lib.collection4.functors.ExceptionPredicate`

```java
public final class com.feilong.lib.collection4.functors.ExceptionPredicate<T> implements org.apache.commons.collections4.Predicate<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> exceptionPredicate();
  public boolean evaluate(T);
}
```

## `com.feilong.lib.collection4.functors.ExceptionTransformer`

```java
public final class com.feilong.lib.collection4.functors.ExceptionTransformer<I, O> implements org.apache.commons.collections4.Transformer<I, O>, java.io.Serializable {
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> exceptionTransformer();
  public O transform(I);
}
```

## `com.feilong.lib.collection4.functors.FalsePredicate`

```java
public final class com.feilong.lib.collection4.functors.FalsePredicate<T> implements org.apache.commons.collections4.Predicate<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> falsePredicate();
  public boolean evaluate(T);
}
```

## `com.feilong.lib.collection4.functors.ForClosure`

```java
public class com.feilong.lib.collection4.functors.ForClosure<E> implements org.apache.commons.collections4.Closure<E> {
  public static <E> org.apache.commons.collections4.Closure<E> forClosure(int, org.apache.commons.collections4.Closure<? super E>);
  public com.feilong.lib.collection4.functors.ForClosure(int, org.apache.commons.collections4.Closure<? super E>);
  public void execute(E);
  public org.apache.commons.collections4.Closure<? super E> getClosure();
  public int getCount();
}
```

## `com.feilong.lib.collection4.functors.IdentityPredicate`

```java
public final class com.feilong.lib.collection4.functors.IdentityPredicate<T> implements org.apache.commons.collections4.Predicate<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> identityPredicate(T);
  public com.feilong.lib.collection4.functors.IdentityPredicate(T);
  public boolean evaluate(T);
  public T getValue();
}
```

## `com.feilong.lib.collection4.functors.IfClosure`

```java
public class com.feilong.lib.collection4.functors.IfClosure<E> implements org.apache.commons.collections4.Closure<E>, java.io.Serializable {
  public static <E> org.apache.commons.collections4.Closure<E> ifClosure(org.apache.commons.collections4.Predicate<? super E>, org.apache.commons.collections4.Closure<? super E>);
  public static <E> org.apache.commons.collections4.Closure<E> ifClosure(org.apache.commons.collections4.Predicate<? super E>, org.apache.commons.collections4.Closure<? super E>, org.apache.commons.collections4.Closure<? super E>);
  public com.feilong.lib.collection4.functors.IfClosure(org.apache.commons.collections4.Predicate<? super E>, org.apache.commons.collections4.Closure<? super E>);
  public com.feilong.lib.collection4.functors.IfClosure(org.apache.commons.collections4.Predicate<? super E>, org.apache.commons.collections4.Closure<? super E>, org.apache.commons.collections4.Closure<? super E>);
  public void execute(E);
  public org.apache.commons.collections4.Predicate<? super E> getPredicate();
  public org.apache.commons.collections4.Closure<? super E> getTrueClosure();
  public org.apache.commons.collections4.Closure<? super E> getFalseClosure();
}
```

## `com.feilong.lib.collection4.functors.IfTransformer`

```java
public class com.feilong.lib.collection4.functors.IfTransformer<I, O> implements org.apache.commons.collections4.Transformer<I, O>, java.io.Serializable {
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> ifTransformer(org.apache.commons.collections4.Predicate<? super I>, org.apache.commons.collections4.Transformer<? super I, ? extends O>, org.apache.commons.collections4.Transformer<? super I, ? extends O>);
  public static <T> org.apache.commons.collections4.Transformer<T, T> ifTransformer(org.apache.commons.collections4.Predicate<? super T>, org.apache.commons.collections4.Transformer<? super T, ? extends T>);
  public com.feilong.lib.collection4.functors.IfTransformer(org.apache.commons.collections4.Predicate<? super I>, org.apache.commons.collections4.Transformer<? super I, ? extends O>, org.apache.commons.collections4.Transformer<? super I, ? extends O>);
  public O transform(I);
  public org.apache.commons.collections4.Predicate<? super I> getPredicate();
  public org.apache.commons.collections4.Transformer<? super I, ? extends O> getTrueTransformer();
  public org.apache.commons.collections4.Transformer<? super I, ? extends O> getFalseTransformer();
}
```

## `com.feilong.lib.collection4.functors.InstanceofPredicate`

```java
public final class com.feilong.lib.collection4.functors.InstanceofPredicate implements org.apache.commons.collections4.Predicate<java.lang.Object>, java.io.Serializable {
  public static org.apache.commons.collections4.Predicate<java.lang.Object> instanceOfPredicate(java.lang.Class<?>);
  public com.feilong.lib.collection4.functors.InstanceofPredicate(java.lang.Class<?>);
  public boolean evaluate(java.lang.Object);
  public java.lang.Class<?> getType();
}
```

## `com.feilong.lib.collection4.functors.InstantiateTransformer`

```java
public class com.feilong.lib.collection4.functors.InstantiateTransformer<T> implements org.apache.commons.collections4.Transformer<java.lang.Class<? extends T>, T> {
  public static <T> org.apache.commons.collections4.Transformer<java.lang.Class<? extends T>, T> instantiateTransformer();
  public static <T> org.apache.commons.collections4.Transformer<java.lang.Class<? extends T>, T> instantiateTransformer(java.lang.Class<?>[], java.lang.Object[]);
  public com.feilong.lib.collection4.functors.InstantiateTransformer(java.lang.Class<?>[], java.lang.Object[]);
  public T transform(java.lang.Class<? extends T>);
  public java.lang.Object transform(java.lang.Object);
}
```

## `com.feilong.lib.collection4.functors.InvokerTransformer`

```java
public class com.feilong.lib.collection4.functors.InvokerTransformer<I, O> implements org.apache.commons.collections4.Transformer<I, O> {
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> invokerTransformer(java.lang.String);
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> invokerTransformer(java.lang.String, java.lang.Class<?>[], java.lang.Object[]);
  public com.feilong.lib.collection4.functors.InvokerTransformer(java.lang.String, java.lang.Class<?>[], java.lang.Object[]);
  public O transform(java.lang.Object);
}
```

## `com.feilong.lib.collection4.functors.MapTransformer`

```java
public final class com.feilong.lib.collection4.functors.MapTransformer<I, O> implements org.apache.commons.collections4.Transformer<I, O>, java.io.Serializable {
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> mapTransformer(java.util.Map<? super I, ? extends O>);
  public O transform(I);
  public java.util.Map<? super I, ? extends O> getMap();
}
```

## `com.feilong.lib.collection4.functors.NOPClosure`

```java
public final class com.feilong.lib.collection4.functors.NOPClosure<E> implements org.apache.commons.collections4.Closure<E>, java.io.Serializable {
  public static <E> org.apache.commons.collections4.Closure<E> nopClosure();
  public void execute(E);
}
```

## `com.feilong.lib.collection4.functors.NOPTransformer`

```java
public class com.feilong.lib.collection4.functors.NOPTransformer<T> implements org.apache.commons.collections4.Transformer<T, T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Transformer<T, T> nopTransformer();
  public T transform(T);
}
```

## `com.feilong.lib.collection4.functors.NonePredicate`

```java
public final class com.feilong.lib.collection4.functors.NonePredicate<T> extends com.feilong.lib.collection4.functors.AbstractQuantifierPredicate<T> {
  public static <T> org.apache.commons.collections4.Predicate<T> nonePredicate(org.apache.commons.collections4.Predicate<? super T>...);
  public static <T> org.apache.commons.collections4.Predicate<T> nonePredicate(java.util.Collection<? extends org.apache.commons.collections4.Predicate<? super T>>);
  public com.feilong.lib.collection4.functors.NonePredicate(org.apache.commons.collections4.Predicate<? super T>...);
  public boolean evaluate(T);
}
```

## `com.feilong.lib.collection4.functors.NotNullPredicate`

```java
public final class com.feilong.lib.collection4.functors.NotNullPredicate<T> implements org.apache.commons.collections4.Predicate<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> notNullPredicate();
  public boolean evaluate(T);
}
```

## `com.feilong.lib.collection4.functors.NotPredicate`

```java
public final class com.feilong.lib.collection4.functors.NotPredicate<T> implements com.feilong.lib.collection4.functors.PredicateDecorator<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> notPredicate(org.apache.commons.collections4.Predicate<? super T>);
  public com.feilong.lib.collection4.functors.NotPredicate(org.apache.commons.collections4.Predicate<? super T>);
  public boolean evaluate(T);
  public org.apache.commons.collections4.Predicate<? super T>[] getPredicates();
}
```

## `com.feilong.lib.collection4.functors.NullIsExceptionPredicate`

```java
public final class com.feilong.lib.collection4.functors.NullIsExceptionPredicate<T> implements com.feilong.lib.collection4.functors.PredicateDecorator<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> nullIsExceptionPredicate(org.apache.commons.collections4.Predicate<? super T>);
  public com.feilong.lib.collection4.functors.NullIsExceptionPredicate(org.apache.commons.collections4.Predicate<? super T>);
  public boolean evaluate(T);
  public org.apache.commons.collections4.Predicate<? super T>[] getPredicates();
}
```

## `com.feilong.lib.collection4.functors.NullIsFalsePredicate`

```java
public final class com.feilong.lib.collection4.functors.NullIsFalsePredicate<T> implements com.feilong.lib.collection4.functors.PredicateDecorator<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> nullIsFalsePredicate(org.apache.commons.collections4.Predicate<? super T>);
  public com.feilong.lib.collection4.functors.NullIsFalsePredicate(org.apache.commons.collections4.Predicate<? super T>);
  public boolean evaluate(T);
  public org.apache.commons.collections4.Predicate<? super T>[] getPredicates();
}
```

## `com.feilong.lib.collection4.functors.NullIsTruePredicate`

```java
public final class com.feilong.lib.collection4.functors.NullIsTruePredicate<T> implements com.feilong.lib.collection4.functors.PredicateDecorator<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> nullIsTruePredicate(org.apache.commons.collections4.Predicate<? super T>);
  public com.feilong.lib.collection4.functors.NullIsTruePredicate(org.apache.commons.collections4.Predicate<? super T>);
  public boolean evaluate(T);
  public org.apache.commons.collections4.Predicate<? super T>[] getPredicates();
}
```

## `com.feilong.lib.collection4.functors.NullPredicate`

```java
public final class com.feilong.lib.collection4.functors.NullPredicate<T> implements org.apache.commons.collections4.Predicate<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> nullPredicate();
  public boolean evaluate(T);
}
```

## `com.feilong.lib.collection4.functors.OnePredicate`

```java
public final class com.feilong.lib.collection4.functors.OnePredicate<T> extends com.feilong.lib.collection4.functors.AbstractQuantifierPredicate<T> {
  public static <T> org.apache.commons.collections4.Predicate<T> onePredicate(org.apache.commons.collections4.Predicate<? super T>...);
  public static <T> org.apache.commons.collections4.Predicate<T> onePredicate(java.util.Collection<? extends org.apache.commons.collections4.Predicate<? super T>>);
  public com.feilong.lib.collection4.functors.OnePredicate(org.apache.commons.collections4.Predicate<? super T>...);
  public boolean evaluate(T);
}
```

## `com.feilong.lib.collection4.functors.OrPredicate`

```java
public final class com.feilong.lib.collection4.functors.OrPredicate<T> implements com.feilong.lib.collection4.functors.PredicateDecorator<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> orPredicate(org.apache.commons.collections4.Predicate<? super T>, org.apache.commons.collections4.Predicate<? super T>);
  public com.feilong.lib.collection4.functors.OrPredicate(org.apache.commons.collections4.Predicate<? super T>, org.apache.commons.collections4.Predicate<? super T>);
  public boolean evaluate(T);
  public org.apache.commons.collections4.Predicate<? super T>[] getPredicates();
}
```

## `com.feilong.lib.collection4.functors.PredicateDecorator`

```java
public interface com.feilong.lib.collection4.functors.PredicateDecorator<T> extends org.apache.commons.collections4.Predicate<T> {
  public abstract org.apache.commons.collections4.Predicate<? super T>[] getPredicates();
}
```

## `com.feilong.lib.collection4.functors.PredicateTransformer`

```java
public class com.feilong.lib.collection4.functors.PredicateTransformer<T> implements org.apache.commons.collections4.Transformer<T, java.lang.Boolean>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Transformer<T, java.lang.Boolean> predicateTransformer(org.apache.commons.collections4.Predicate<? super T>);
  public com.feilong.lib.collection4.functors.PredicateTransformer(org.apache.commons.collections4.Predicate<? super T>);
  public java.lang.Boolean transform(T);
  public org.apache.commons.collections4.Predicate<? super T> getPredicate();
  public java.lang.Object transform(java.lang.Object);
}
```

## `com.feilong.lib.collection4.functors.StringValueTransformer`

```java
public final class com.feilong.lib.collection4.functors.StringValueTransformer<T> implements org.apache.commons.collections4.Transformer<T, java.lang.String>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Transformer<T, java.lang.String> stringValueTransformer();
  public java.lang.String transform(T);
  public java.lang.Object transform(java.lang.Object);
}
```

## `com.feilong.lib.collection4.functors.SwitchClosure`

```java
public class com.feilong.lib.collection4.functors.SwitchClosure<E> implements org.apache.commons.collections4.Closure<E>, java.io.Serializable {
  public static <E> org.apache.commons.collections4.Closure<E> switchClosure(org.apache.commons.collections4.Predicate<? super E>[], org.apache.commons.collections4.Closure<? super E>[], org.apache.commons.collections4.Closure<? super E>);
  public static <E> org.apache.commons.collections4.Closure<E> switchClosure(java.util.Map<org.apache.commons.collections4.Predicate<E>, org.apache.commons.collections4.Closure<E>>);
  public com.feilong.lib.collection4.functors.SwitchClosure(org.apache.commons.collections4.Predicate<? super E>[], org.apache.commons.collections4.Closure<? super E>[], org.apache.commons.collections4.Closure<? super E>);
  public void execute(E);
  public org.apache.commons.collections4.Predicate<? super E>[] getPredicates();
  public org.apache.commons.collections4.Closure<? super E>[] getClosures();
  public org.apache.commons.collections4.Closure<? super E> getDefaultClosure();
}
```

## `com.feilong.lib.collection4.functors.SwitchTransformer`

```java
public class com.feilong.lib.collection4.functors.SwitchTransformer<I, O> implements org.apache.commons.collections4.Transformer<I, O>, java.io.Serializable {
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> switchTransformer(org.apache.commons.collections4.Predicate<? super I>[], org.apache.commons.collections4.Transformer<? super I, ? extends O>[], org.apache.commons.collections4.Transformer<? super I, ? extends O>);
  public static <I, O> org.apache.commons.collections4.Transformer<I, O> switchTransformer(java.util.Map<? extends org.apache.commons.collections4.Predicate<? super I>, ? extends org.apache.commons.collections4.Transformer<? super I, ? extends O>>);
  public com.feilong.lib.collection4.functors.SwitchTransformer(org.apache.commons.collections4.Predicate<? super I>[], org.apache.commons.collections4.Transformer<? super I, ? extends O>[], org.apache.commons.collections4.Transformer<? super I, ? extends O>);
  public O transform(I);
  public org.apache.commons.collections4.Predicate<? super I>[] getPredicates();
  public org.apache.commons.collections4.Transformer<? super I, ? extends O>[] getTransformers();
  public org.apache.commons.collections4.Transformer<? super I, ? extends O> getDefaultTransformer();
}
```

## `com.feilong.lib.collection4.functors.TransformedPredicate`

```java
public final class com.feilong.lib.collection4.functors.TransformedPredicate<T> implements com.feilong.lib.collection4.functors.PredicateDecorator<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> transformedPredicate(org.apache.commons.collections4.Transformer<? super T, ? extends T>, org.apache.commons.collections4.Predicate<? super T>);
  public com.feilong.lib.collection4.functors.TransformedPredicate(org.apache.commons.collections4.Transformer<? super T, ? extends T>, org.apache.commons.collections4.Predicate<? super T>);
  public boolean evaluate(T);
  public org.apache.commons.collections4.Predicate<? super T>[] getPredicates();
  public org.apache.commons.collections4.Transformer<? super T, ? extends T> getTransformer();
}
```

## `com.feilong.lib.collection4.functors.TransformerClosure`

```java
public class com.feilong.lib.collection4.functors.TransformerClosure<E> implements org.apache.commons.collections4.Closure<E>, java.io.Serializable {
  public static <E> org.apache.commons.collections4.Closure<E> transformerClosure(org.apache.commons.collections4.Transformer<? super E, ?>);
  public com.feilong.lib.collection4.functors.TransformerClosure(org.apache.commons.collections4.Transformer<? super E, ?>);
  public void execute(E);
  public org.apache.commons.collections4.Transformer<? super E, ?> getTransformer();
}
```

## `com.feilong.lib.collection4.functors.TransformerPredicate`

```java
public final class com.feilong.lib.collection4.functors.TransformerPredicate<T> implements org.apache.commons.collections4.Predicate<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> transformerPredicate(org.apache.commons.collections4.Transformer<? super T, java.lang.Boolean>);
  public com.feilong.lib.collection4.functors.TransformerPredicate(org.apache.commons.collections4.Transformer<? super T, java.lang.Boolean>);
  public boolean evaluate(T);
  public org.apache.commons.collections4.Transformer<? super T, java.lang.Boolean> getTransformer();
}
```

## `com.feilong.lib.collection4.functors.TruePredicate`

```java
public final class com.feilong.lib.collection4.functors.TruePredicate<T> implements org.apache.commons.collections4.Predicate<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> truePredicate();
  public boolean evaluate(T);
}
```

## `com.feilong.lib.collection4.functors.UniquePredicate`

```java
public final class com.feilong.lib.collection4.functors.UniquePredicate<T> implements org.apache.commons.collections4.Predicate<T>, java.io.Serializable {
  public static <T> org.apache.commons.collections4.Predicate<T> uniquePredicate();
  public com.feilong.lib.collection4.functors.UniquePredicate();
  public boolean evaluate(T);
}
```

## `com.feilong.lib.collection4.functors.WhileClosure`

```java
public class com.feilong.lib.collection4.functors.WhileClosure<E> implements org.apache.commons.collections4.Closure<E> {
  public static <E> org.apache.commons.collections4.Closure<E> whileClosure(org.apache.commons.collections4.Predicate<? super E>, org.apache.commons.collections4.Closure<? super E>, boolean);
  public com.feilong.lib.collection4.functors.WhileClosure(org.apache.commons.collections4.Predicate<? super E>, org.apache.commons.collections4.Closure<? super E>, boolean);
  public void execute(E);
  public org.apache.commons.collections4.Predicate<? super E> getPredicate();
  public org.apache.commons.collections4.Closure<? super E> getClosure();
  public boolean isDoLoop();
}
```
