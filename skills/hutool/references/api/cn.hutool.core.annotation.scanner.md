# cn.hutool.core.annotation.scanner

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner`

```java
public abstract class cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner<T extends cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner<T>> implements cn.hutool.core.annotation.scanner.AnnotationScanner {
  public boolean isIncludeSuperClass();
  public boolean isIncludeInterfaces();
  public T setFilter(java.util.function.Predicate<java.lang.Class<?>>);
  public T addExcludeTypes(java.lang.Class<?>...);
  public T addConverters(java.util.function.UnaryOperator<java.lang.Class<?>>);
  public void scan(java.util.function.BiConsumer<java.lang.Integer, java.lang.annotation.Annotation>, java.lang.reflect.AnnotatedElement, java.util.function.Predicate<java.lang.annotation.Annotation>);
}
```

## `cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner$JdkProxyClassConverter`

```java
public class cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner$JdkProxyClassConverter implements java.util.function.UnaryOperator<java.lang.Class<?>> {
  public cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner$JdkProxyClassConverter();
  public java.lang.Class<?> apply(java.lang.Class<?>);
  public java.lang.Object apply(java.lang.Object);
}
```

## `cn.hutool.core.annotation.scanner.AnnotationScanner`

```java
public interface cn.hutool.core.annotation.scanner.AnnotationScanner {
  public static java.util.List<java.lang.annotation.Annotation> scanByAnySupported(java.lang.reflect.AnnotatedElement, cn.hutool.core.annotation.scanner.AnnotationScanner...);
  public static java.util.List<java.lang.annotation.Annotation> scanByAllSupported(java.lang.reflect.AnnotatedElement, cn.hutool.core.annotation.scanner.AnnotationScanner...);
  public default boolean support(java.lang.reflect.AnnotatedElement);
  public default java.util.List<java.lang.annotation.Annotation> getAnnotations(java.lang.reflect.AnnotatedElement);
  public default java.util.List<java.lang.annotation.Annotation> getAnnotationsIfSupport(java.lang.reflect.AnnotatedElement);
  public default void scan(java.util.function.BiConsumer<java.lang.Integer, java.lang.annotation.Annotation>, java.lang.reflect.AnnotatedElement, java.util.function.Predicate<java.lang.annotation.Annotation>);
  public default void scanIfSupport(java.util.function.BiConsumer<java.lang.Integer, java.lang.annotation.Annotation>, java.lang.reflect.AnnotatedElement, java.util.function.Predicate<java.lang.annotation.Annotation>);
}
```

## `cn.hutool.core.annotation.scanner.ElementAnnotationScanner`

```java
public class cn.hutool.core.annotation.scanner.ElementAnnotationScanner implements cn.hutool.core.annotation.scanner.AnnotationScanner {
  public cn.hutool.core.annotation.scanner.ElementAnnotationScanner();
  public boolean support(java.lang.reflect.AnnotatedElement);
  public void scan(java.util.function.BiConsumer<java.lang.Integer, java.lang.annotation.Annotation>, java.lang.reflect.AnnotatedElement, java.util.function.Predicate<java.lang.annotation.Annotation>);
}
```

## `cn.hutool.core.annotation.scanner.EmptyAnnotationScanner`

```java
public class cn.hutool.core.annotation.scanner.EmptyAnnotationScanner implements cn.hutool.core.annotation.scanner.AnnotationScanner {
  public cn.hutool.core.annotation.scanner.EmptyAnnotationScanner();
  public boolean support(java.lang.reflect.AnnotatedElement);
  public java.util.List<java.lang.annotation.Annotation> getAnnotations(java.lang.reflect.AnnotatedElement);
  public void scan(java.util.function.BiConsumer<java.lang.Integer, java.lang.annotation.Annotation>, java.lang.reflect.AnnotatedElement, java.util.function.Predicate<java.lang.annotation.Annotation>);
}
```

## `cn.hutool.core.annotation.scanner.FieldAnnotationScanner`

```java
public class cn.hutool.core.annotation.scanner.FieldAnnotationScanner implements cn.hutool.core.annotation.scanner.AnnotationScanner {
  public cn.hutool.core.annotation.scanner.FieldAnnotationScanner();
  public boolean support(java.lang.reflect.AnnotatedElement);
  public void scan(java.util.function.BiConsumer<java.lang.Integer, java.lang.annotation.Annotation>, java.lang.reflect.AnnotatedElement, java.util.function.Predicate<java.lang.annotation.Annotation>);
}
```

## `cn.hutool.core.annotation.scanner.GenericAnnotationScanner`

```java
public class cn.hutool.core.annotation.scanner.GenericAnnotationScanner implements cn.hutool.core.annotation.scanner.AnnotationScanner {
  public boolean support(java.lang.reflect.AnnotatedElement);
  public cn.hutool.core.annotation.scanner.GenericAnnotationScanner(boolean, boolean, boolean);
  public void scan(java.util.function.BiConsumer<java.lang.Integer, java.lang.annotation.Annotation>, java.lang.reflect.AnnotatedElement, java.util.function.Predicate<java.lang.annotation.Annotation>);
}
```

## `cn.hutool.core.annotation.scanner.MetaAnnotationScanner`

```java
public class cn.hutool.core.annotation.scanner.MetaAnnotationScanner implements cn.hutool.core.annotation.scanner.AnnotationScanner {
  public cn.hutool.core.annotation.scanner.MetaAnnotationScanner(boolean);
  public cn.hutool.core.annotation.scanner.MetaAnnotationScanner();
  public boolean support(java.lang.reflect.AnnotatedElement);
  public java.util.List<java.lang.annotation.Annotation> getAnnotations(java.lang.reflect.AnnotatedElement);
  public void scan(java.util.function.BiConsumer<java.lang.Integer, java.lang.annotation.Annotation>, java.lang.reflect.AnnotatedElement, java.util.function.Predicate<java.lang.annotation.Annotation>);
}
```

## `cn.hutool.core.annotation.scanner.MethodAnnotationScanner`

```java
public class cn.hutool.core.annotation.scanner.MethodAnnotationScanner extends cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner<cn.hutool.core.annotation.scanner.MethodAnnotationScanner> implements cn.hutool.core.annotation.scanner.AnnotationScanner {
  public cn.hutool.core.annotation.scanner.MethodAnnotationScanner();
  public cn.hutool.core.annotation.scanner.MethodAnnotationScanner(boolean);
  public cn.hutool.core.annotation.scanner.MethodAnnotationScanner(boolean, java.util.function.Predicate<java.lang.Class<?>>, java.util.Set<java.lang.Class<?>>);
  public cn.hutool.core.annotation.scanner.MethodAnnotationScanner(boolean, boolean, java.util.function.Predicate<java.lang.Class<?>>, java.util.Set<java.lang.Class<?>>);
  public boolean support(java.lang.reflect.AnnotatedElement);
  public cn.hutool.core.annotation.scanner.MethodAnnotationScanner setScanSameSignatureMethod(boolean);
}
```

## `cn.hutool.core.annotation.scanner.TypeAnnotationScanner`

```java
public class cn.hutool.core.annotation.scanner.TypeAnnotationScanner extends cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner<cn.hutool.core.annotation.scanner.TypeAnnotationScanner> implements cn.hutool.core.annotation.scanner.AnnotationScanner {
  public cn.hutool.core.annotation.scanner.TypeAnnotationScanner(boolean, boolean, java.util.function.Predicate<java.lang.Class<?>>, java.util.Set<java.lang.Class<?>>);
  public cn.hutool.core.annotation.scanner.TypeAnnotationScanner();
  public boolean support(java.lang.reflect.AnnotatedElement);
  public cn.hutool.core.annotation.scanner.TypeAnnotationScanner setIncludeSuperClass(boolean);
  public cn.hutool.core.annotation.scanner.TypeAnnotationScanner setIncludeInterfaces(boolean);
  public cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner setIncludeInterfaces(boolean);
  public cn.hutool.core.annotation.scanner.AbstractTypeAnnotationScanner setIncludeSuperClass(boolean);
}
```

## `cn.hutool.core.annotation.scanner.TypeAnnotationScanner$JdkProxyClassConverter`

```java
public class cn.hutool.core.annotation.scanner.TypeAnnotationScanner$JdkProxyClassConverter implements java.util.function.UnaryOperator<java.lang.Class<?>> {
  public cn.hutool.core.annotation.scanner.TypeAnnotationScanner$JdkProxyClassConverter();
  public java.lang.Class<?> apply(java.lang.Class<?>);
  public java.lang.Object apply(java.lang.Object);
}
```
