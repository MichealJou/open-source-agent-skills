# cn.hutool.core.annotation

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.annotation.AbstractAnnotationSynthesizer`

```java
public abstract class cn.hutool.core.annotation.AbstractAnnotationSynthesizer<T> implements cn.hutool.core.annotation.AnnotationSynthesizer {
  public T getSource();
  public cn.hutool.core.annotation.SynthesizedAnnotationSelector getAnnotationSelector();
  public java.util.Collection<cn.hutool.core.annotation.SynthesizedAnnotationPostProcessor> getAnnotationPostProcessors();
  public cn.hutool.core.annotation.SynthesizedAnnotation getSynthesizedAnnotation(java.lang.Class<?>);
  public java.util.Map<java.lang.Class<? extends java.lang.annotation.Annotation>, cn.hutool.core.annotation.SynthesizedAnnotation> getAllSynthesizedAnnotation();
  public <A extends java.lang.annotation.Annotation> A synthesize(java.lang.Class<A>);
}
```

## `cn.hutool.core.annotation.AbstractLinkAnnotationPostProcessor`

```java
public abstract class cn.hutool.core.annotation.AbstractLinkAnnotationPostProcessor implements cn.hutool.core.annotation.SynthesizedAnnotationPostProcessor {
  public cn.hutool.core.annotation.AbstractLinkAnnotationPostProcessor();
  public void process(cn.hutool.core.annotation.SynthesizedAnnotation, cn.hutool.core.annotation.AnnotationSynthesizer);
}
```

## `cn.hutool.core.annotation.AbstractWrappedAnnotationAttribute`

```java
public abstract class cn.hutool.core.annotation.AbstractWrappedAnnotationAttribute implements cn.hutool.core.annotation.WrappedAnnotationAttribute {
  public cn.hutool.core.annotation.AnnotationAttribute getOriginal();
  public cn.hutool.core.annotation.AnnotationAttribute getLinked();
  public cn.hutool.core.annotation.AnnotationAttribute getNonWrappedOriginal();
  public java.util.Collection<cn.hutool.core.annotation.AnnotationAttribute> getAllLinkedNonWrappedAttributes();
}
```

## `cn.hutool.core.annotation.AggregateAnnotation`

```java
public interface cn.hutool.core.annotation.AggregateAnnotation extends java.lang.annotation.Annotation {
  public abstract boolean isAnnotationPresent(java.lang.Class<? extends java.lang.annotation.Annotation>);
  public abstract java.lang.annotation.Annotation[] getAnnotations();
}
```

## `cn.hutool.core.annotation.Alias`

```java
public interface cn.hutool.core.annotation.Alias extends java.lang.annotation.Annotation {
  public abstract java.lang.String value();
}
```

## `cn.hutool.core.annotation.AliasAnnotationPostProcessor`

```java
public class cn.hutool.core.annotation.AliasAnnotationPostProcessor implements cn.hutool.core.annotation.SynthesizedAnnotationPostProcessor {
  public cn.hutool.core.annotation.AliasAnnotationPostProcessor();
  public int order();
  public void process(cn.hutool.core.annotation.SynthesizedAnnotation, cn.hutool.core.annotation.AnnotationSynthesizer);
}
```

## `cn.hutool.core.annotation.AliasFor`

```java
public interface cn.hutool.core.annotation.AliasFor extends java.lang.annotation.Annotation {
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation> annotation();
  public abstract java.lang.String attribute();
}
```

## `cn.hutool.core.annotation.AliasLinkAnnotationPostProcessor`

```java
public class cn.hutool.core.annotation.AliasLinkAnnotationPostProcessor extends cn.hutool.core.annotation.AbstractLinkAnnotationPostProcessor {
  public cn.hutool.core.annotation.AliasLinkAnnotationPostProcessor();
  public int order();
}
```

## `cn.hutool.core.annotation.AliasedAnnotationAttribute`

```java
public class cn.hutool.core.annotation.AliasedAnnotationAttribute extends cn.hutool.core.annotation.AbstractWrappedAnnotationAttribute {
  public java.lang.Object getValue();
  public boolean isValueEquivalentToDefaultValue();
}
```

## `cn.hutool.core.annotation.AnnotationAttribute`

```java
public interface cn.hutool.core.annotation.AnnotationAttribute {
  public abstract java.lang.annotation.Annotation getAnnotation();
  public abstract java.lang.reflect.Method getAttribute();
  public default java.lang.Class<?> getAnnotationType();
  public default java.lang.String getAttributeName();
  public default java.lang.Object getValue();
  public abstract boolean isValueEquivalentToDefaultValue();
  public default java.lang.Class<?> getAttributeType();
  public default <T extends java.lang.annotation.Annotation> T getAnnotation(java.lang.Class<T>);
  public default boolean isWrapped();
}
```

## `cn.hutool.core.annotation.AnnotationAttributeValueProvider`

```java
public interface cn.hutool.core.annotation.AnnotationAttributeValueProvider {
  public abstract java.lang.Object getAttributeValue(java.lang.String, java.lang.Class<?>);
}
```

## `cn.hutool.core.annotation.AnnotationProxy`

```java
public class cn.hutool.core.annotation.AnnotationProxy<T extends java.lang.annotation.Annotation> implements java.lang.annotation.Annotation, java.lang.reflect.InvocationHandler, java.io.Serializable {
  public cn.hutool.core.annotation.AnnotationProxy(T);
  public java.lang.Class<? extends java.lang.annotation.Annotation> annotationType();
  public java.lang.Object invoke(java.lang.Object, java.lang.reflect.Method, java.lang.Object[]) throws java.lang.Throwable;
}
```

## `cn.hutool.core.annotation.AnnotationSynthesizer`

```java
public interface cn.hutool.core.annotation.AnnotationSynthesizer {
  public abstract java.lang.Object getSource();
  public abstract cn.hutool.core.annotation.SynthesizedAnnotationSelector getAnnotationSelector();
  public abstract java.util.Collection<cn.hutool.core.annotation.SynthesizedAnnotationPostProcessor> getAnnotationPostProcessors();
  public abstract cn.hutool.core.annotation.SynthesizedAnnotation getSynthesizedAnnotation(java.lang.Class<?>);
  public abstract java.util.Map<java.lang.Class<? extends java.lang.annotation.Annotation>, cn.hutool.core.annotation.SynthesizedAnnotation> getAllSynthesizedAnnotation();
  public abstract <T extends java.lang.annotation.Annotation> T synthesize(java.lang.Class<T>);
}
```

## `cn.hutool.core.annotation.AnnotationUtil`

```java
public class cn.hutool.core.annotation.AnnotationUtil {
  public cn.hutool.core.annotation.AnnotationUtil();
  public static boolean isJdkMetaAnnotation(java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static boolean isNotJdkMateAnnotation(java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static cn.hutool.core.annotation.CombinationAnnotationElement toCombination(java.lang.reflect.AnnotatedElement);
  public static java.lang.annotation.Annotation[] getAnnotations(java.lang.reflect.AnnotatedElement, boolean);
  public static <T> T[] getCombinationAnnotations(java.lang.reflect.AnnotatedElement, java.lang.Class<T>);
  public static <T> T[] getAnnotations(java.lang.reflect.AnnotatedElement, boolean, java.lang.Class<T>);
  public static java.lang.annotation.Annotation[] getAnnotations(java.lang.reflect.AnnotatedElement, boolean, java.util.function.Predicate<java.lang.annotation.Annotation>);
  public static <A extends java.lang.annotation.Annotation> A getAnnotation(java.lang.reflect.AnnotatedElement, java.lang.Class<A>);
  public static boolean hasAnnotation(java.lang.reflect.AnnotatedElement, java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static boolean hasAnnotation(java.lang.reflect.AnnotatedElement, java.lang.String);
  public static <T> T getAnnotationValue(java.lang.reflect.AnnotatedElement, java.lang.Class<? extends java.lang.annotation.Annotation>) throws cn.hutool.core.exceptions.UtilException;
  public static <T> T getAnnotationValue(java.lang.reflect.AnnotatedElement, java.lang.Class<? extends java.lang.annotation.Annotation>, java.lang.String) throws cn.hutool.core.exceptions.UtilException;
  public static <A extends java.lang.annotation.Annotation, R> R getAnnotationValue(java.lang.reflect.AnnotatedElement, cn.hutool.core.lang.func.Func1<A, R>);
  public static java.util.Map<java.lang.String, java.lang.Object> getAnnotationValueMap(java.lang.reflect.AnnotatedElement, java.lang.Class<? extends java.lang.annotation.Annotation>) throws cn.hutool.core.exceptions.UtilException;
  public static java.lang.annotation.RetentionPolicy getRetentionPolicy(java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static java.lang.annotation.ElementType[] getTargetType(java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static boolean isDocumented(java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static boolean isInherited(java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static java.util.List<java.lang.annotation.Annotation> scanMetaAnnotation(java.lang.Class<? extends java.lang.annotation.Annotation>);
  public static java.util.List<java.lang.annotation.Annotation> scanClass(java.lang.Class<?>);
  public static java.util.List<java.lang.annotation.Annotation> scanMethod(java.lang.reflect.Method);
  public static void setValue(java.lang.annotation.Annotation, java.lang.String, java.lang.Object);
  public static boolean isSynthesizedAnnotation(java.lang.annotation.Annotation);
  public static <T extends java.lang.annotation.Annotation> T getAnnotationAlias(java.lang.reflect.AnnotatedElement, java.lang.Class<T>);
  public static <T extends java.lang.annotation.Annotation> T getSynthesizedAnnotation(java.lang.Class<T>, java.lang.annotation.Annotation...);
  public static <T extends java.lang.annotation.Annotation> T getSynthesizedAnnotation(java.lang.reflect.AnnotatedElement, java.lang.Class<T>);
  public static <T extends java.lang.annotation.Annotation> java.util.List<T> getAllSynthesizedAnnotations(java.lang.reflect.AnnotatedElement, java.lang.Class<T>);
  public static cn.hutool.core.annotation.SynthesizedAggregateAnnotation aggregatingFromAnnotation(java.lang.annotation.Annotation...);
  public static cn.hutool.core.annotation.SynthesizedAggregateAnnotation aggregatingFromAnnotationWithMeta(java.lang.annotation.Annotation...);
}
```

## `cn.hutool.core.annotation.CacheableAnnotationAttribute`

```java
public class cn.hutool.core.annotation.CacheableAnnotationAttribute implements cn.hutool.core.annotation.AnnotationAttribute {
  public cn.hutool.core.annotation.CacheableAnnotationAttribute(java.lang.annotation.Annotation, java.lang.reflect.Method);
  public java.lang.annotation.Annotation getAnnotation();
  public java.lang.reflect.Method getAttribute();
  public java.lang.Object getValue();
  public boolean isValueEquivalentToDefaultValue();
}
```

## `cn.hutool.core.annotation.CacheableSynthesizedAnnotationAttributeProcessor`

```java
public class cn.hutool.core.annotation.CacheableSynthesizedAnnotationAttributeProcessor implements cn.hutool.core.annotation.SynthesizedAnnotationAttributeProcessor {
  public cn.hutool.core.annotation.CacheableSynthesizedAnnotationAttributeProcessor(java.util.Comparator<cn.hutool.core.annotation.Hierarchical>);
  public cn.hutool.core.annotation.CacheableSynthesizedAnnotationAttributeProcessor();
  public <T> T getAttributeValue(java.lang.String, java.lang.Class<T>, java.util.Collection<? extends cn.hutool.core.annotation.SynthesizedAnnotation>);
}
```

## `cn.hutool.core.annotation.CombinationAnnotationElement`

```java
public class cn.hutool.core.annotation.CombinationAnnotationElement implements java.lang.reflect.AnnotatedElement,java.io.Serializable {
  public static cn.hutool.core.annotation.CombinationAnnotationElement of(java.lang.reflect.AnnotatedElement, java.util.function.Predicate<java.lang.annotation.Annotation>);
  public cn.hutool.core.annotation.CombinationAnnotationElement(java.lang.reflect.AnnotatedElement);
  public cn.hutool.core.annotation.CombinationAnnotationElement(java.lang.reflect.AnnotatedElement, java.util.function.Predicate<java.lang.annotation.Annotation>);
  public boolean isAnnotationPresent(java.lang.Class<? extends java.lang.annotation.Annotation>);
  public <T extends java.lang.annotation.Annotation> T getAnnotation(java.lang.Class<T>);
  public java.lang.annotation.Annotation[] getAnnotations();
  public java.lang.annotation.Annotation[] getDeclaredAnnotations();
}
```

## `cn.hutool.core.annotation.ForceAliasFor`

```java
public interface cn.hutool.core.annotation.ForceAliasFor extends java.lang.annotation.Annotation {
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation> annotation();
  public abstract java.lang.String attribute();
}
```

## `cn.hutool.core.annotation.ForceAliasedAnnotationAttribute`

```java
public class cn.hutool.core.annotation.ForceAliasedAnnotationAttribute extends cn.hutool.core.annotation.AbstractWrappedAnnotationAttribute {
  public java.lang.Object getValue();
  public boolean isValueEquivalentToDefaultValue();
  public java.lang.Class<?> getAttributeType();
}
```

## `cn.hutool.core.annotation.GenericSynthesizedAggregateAnnotation`

```java
public class cn.hutool.core.annotation.GenericSynthesizedAggregateAnnotation extends cn.hutool.core.annotation.AbstractAnnotationSynthesizer<java.util.List<java.lang.annotation.Annotation>> implements cn.hutool.core.annotation.SynthesizedAggregateAnnotation {
  public cn.hutool.core.annotation.GenericSynthesizedAggregateAnnotation(java.lang.annotation.Annotation...);
  public cn.hutool.core.annotation.GenericSynthesizedAggregateAnnotation(java.util.List<java.lang.annotation.Annotation>, cn.hutool.core.annotation.scanner.AnnotationScanner);
  public cn.hutool.core.annotation.GenericSynthesizedAggregateAnnotation(java.util.List<java.lang.annotation.Annotation>, cn.hutool.core.annotation.SynthesizedAnnotationSelector, cn.hutool.core.annotation.SynthesizedAnnotationAttributeProcessor, java.util.Collection<cn.hutool.core.annotation.SynthesizedAnnotationPostProcessor>, cn.hutool.core.annotation.scanner.AnnotationScanner);
  public java.lang.Object getRoot();
  public int getVerticalDistance();
  public int getHorizontalDistance();
  public cn.hutool.core.annotation.SynthesizedAnnotationAttributeProcessor getAnnotationAttributeProcessor();
  public java.lang.Object getAttributeValue(java.lang.String, java.lang.Class<?>);
  public <T extends java.lang.annotation.Annotation> T getAnnotation(java.lang.Class<T>);
  public boolean isAnnotationPresent(java.lang.Class<? extends java.lang.annotation.Annotation>);
  public java.lang.annotation.Annotation[] getAnnotations();
  public <T extends java.lang.annotation.Annotation> T synthesize(java.lang.Class<T>, cn.hutool.core.annotation.SynthesizedAnnotation);
}
```

## `cn.hutool.core.annotation.GenericSynthesizedAnnotation`

```java
public class cn.hutool.core.annotation.GenericSynthesizedAnnotation<R, T extends java.lang.annotation.Annotation> implements cn.hutool.core.annotation.SynthesizedAnnotation {
  public boolean hasAttribute(java.lang.String);
  public boolean hasAttribute(java.lang.String, java.lang.Class<?>);
  public java.util.Map<java.lang.String, cn.hutool.core.annotation.AnnotationAttribute> getAttributes();
  public void setAttribute(java.lang.String, cn.hutool.core.annotation.AnnotationAttribute);
  public void replaceAttribute(java.lang.String, java.util.function.UnaryOperator<cn.hutool.core.annotation.AnnotationAttribute>);
  public java.lang.Object getAttributeValue(java.lang.String);
  public R getRoot();
  public T getAnnotation();
  public int getVerticalDistance();
  public int getHorizontalDistance();
  public java.lang.Class<? extends java.lang.annotation.Annotation> annotationType();
  public java.lang.Object getAttributeValue(java.lang.String, java.lang.Class<?>);
}
```

## `cn.hutool.core.annotation.Hierarchical`

```java
public interface cn.hutool.core.annotation.Hierarchical extends java.lang.Comparable<cn.hutool.core.annotation.Hierarchical> {
  public default int compareTo(cn.hutool.core.annotation.Hierarchical);
  public abstract java.lang.Object getRoot();
  public abstract int getVerticalDistance();
  public abstract int getHorizontalDistance();
  public default int compareTo(java.lang.Object);
}
```

## `cn.hutool.core.annotation.Hierarchical$Selector`

```java
public interface cn.hutool.core.annotation.Hierarchical$Selector {
  public abstract <T extends cn.hutool.core.annotation.Hierarchical> T choose(T, T);
}
```

## `cn.hutool.core.annotation.Hierarchical$Selector$FarthestAndNewestPrioritySelector`

```java
public class cn.hutool.core.annotation.Hierarchical$Selector$FarthestAndNewestPrioritySelector implements cn.hutool.core.annotation.Hierarchical$Selector {
  public cn.hutool.core.annotation.Hierarchical$Selector$FarthestAndNewestPrioritySelector();
  public <T extends cn.hutool.core.annotation.Hierarchical> T choose(T, T);
}
```

## `cn.hutool.core.annotation.Hierarchical$Selector$FarthestAndOldestPrioritySelector`

```java
public class cn.hutool.core.annotation.Hierarchical$Selector$FarthestAndOldestPrioritySelector implements cn.hutool.core.annotation.Hierarchical$Selector {
  public cn.hutool.core.annotation.Hierarchical$Selector$FarthestAndOldestPrioritySelector();
  public <T extends cn.hutool.core.annotation.Hierarchical> T choose(T, T);
}
```

## `cn.hutool.core.annotation.Hierarchical$Selector$NearestAndNewestPrioritySelector`

```java
public class cn.hutool.core.annotation.Hierarchical$Selector$NearestAndNewestPrioritySelector implements cn.hutool.core.annotation.Hierarchical$Selector {
  public cn.hutool.core.annotation.Hierarchical$Selector$NearestAndNewestPrioritySelector();
  public <T extends cn.hutool.core.annotation.Hierarchical> T choose(T, T);
}
```

## `cn.hutool.core.annotation.Hierarchical$Selector$NearestAndOldestPrioritySelector`

```java
public class cn.hutool.core.annotation.Hierarchical$Selector$NearestAndOldestPrioritySelector implements cn.hutool.core.annotation.Hierarchical$Selector {
  public cn.hutool.core.annotation.Hierarchical$Selector$NearestAndOldestPrioritySelector();
  public <T extends cn.hutool.core.annotation.Hierarchical> T choose(T, T);
}
```

## `cn.hutool.core.annotation.Link`

```java
public interface cn.hutool.core.annotation.Link extends java.lang.annotation.Annotation {
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation> annotation();
  public abstract java.lang.String attribute();
  public abstract cn.hutool.core.annotation.RelationType type();
}
```

## `cn.hutool.core.annotation.MirrorFor`

```java
public interface cn.hutool.core.annotation.MirrorFor extends java.lang.annotation.Annotation {
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation> annotation();
  public abstract java.lang.String attribute();
}
```

## `cn.hutool.core.annotation.MirrorLinkAnnotationPostProcessor`

```java
public class cn.hutool.core.annotation.MirrorLinkAnnotationPostProcessor extends cn.hutool.core.annotation.AbstractLinkAnnotationPostProcessor {
  public cn.hutool.core.annotation.MirrorLinkAnnotationPostProcessor();
  public int order();
}
```

## `cn.hutool.core.annotation.MirroredAnnotationAttribute`

```java
public class cn.hutool.core.annotation.MirroredAnnotationAttribute extends cn.hutool.core.annotation.AbstractWrappedAnnotationAttribute {
  public cn.hutool.core.annotation.MirroredAnnotationAttribute(cn.hutool.core.annotation.AnnotationAttribute, cn.hutool.core.annotation.AnnotationAttribute);
  public java.lang.Object getValue();
  public boolean isValueEquivalentToDefaultValue();
}
```

## `cn.hutool.core.annotation.RelationType`

```java
public final class cn.hutool.core.annotation.RelationType extends java.lang.Enum<cn.hutool.core.annotation.RelationType> {
  public static cn.hutool.core.annotation.RelationType[] values();
  public static cn.hutool.core.annotation.RelationType valueOf(java.lang.String);
}
```

## `cn.hutool.core.annotation.SynthesizedAggregateAnnotation`

```java
public interface cn.hutool.core.annotation.SynthesizedAggregateAnnotation extends cn.hutool.core.annotation.AggregateAnnotation,cn.hutool.core.annotation.Hierarchical,cn.hutool.core.annotation.AnnotationSynthesizer,cn.hutool.core.annotation.AnnotationAttributeValueProvider {
  public default int getVerticalDistance();
  public default int getHorizontalDistance();
  public abstract <T extends java.lang.annotation.Annotation> T getAnnotation(java.lang.Class<T>);
  public abstract cn.hutool.core.annotation.SynthesizedAnnotationAttributeProcessor getAnnotationAttributeProcessor();
  public default java.lang.Class<? extends java.lang.annotation.Annotation> annotationType();
  public abstract java.lang.Object getAttributeValue(java.lang.String, java.lang.Class<?>);
}
```

## `cn.hutool.core.annotation.SynthesizedAnnotation`

```java
public interface cn.hutool.core.annotation.SynthesizedAnnotation extends java.lang.annotation.Annotation,cn.hutool.core.annotation.Hierarchical,cn.hutool.core.annotation.AnnotationAttributeValueProvider {
  public abstract java.lang.annotation.Annotation getAnnotation();
  public abstract int getVerticalDistance();
  public abstract int getHorizontalDistance();
  public abstract boolean hasAttribute(java.lang.String, java.lang.Class<?>);
  public abstract java.util.Map<java.lang.String, cn.hutool.core.annotation.AnnotationAttribute> getAttributes();
  public default void setAttributes(java.util.Map<java.lang.String, cn.hutool.core.annotation.AnnotationAttribute>);
  public abstract void setAttribute(java.lang.String, cn.hutool.core.annotation.AnnotationAttribute);
  public abstract void replaceAttribute(java.lang.String, java.util.function.UnaryOperator<cn.hutool.core.annotation.AnnotationAttribute>);
  public abstract java.lang.Object getAttributeValue(java.lang.String);
}
```

## `cn.hutool.core.annotation.SynthesizedAnnotationAttributeProcessor`

```java
public interface cn.hutool.core.annotation.SynthesizedAnnotationAttributeProcessor {
  public abstract <R> R getAttributeValue(java.lang.String, java.lang.Class<R>, java.util.Collection<? extends cn.hutool.core.annotation.SynthesizedAnnotation>);
}
```

## `cn.hutool.core.annotation.SynthesizedAnnotationPostProcessor`

```java
public interface cn.hutool.core.annotation.SynthesizedAnnotationPostProcessor extends java.lang.Comparable<cn.hutool.core.annotation.SynthesizedAnnotationPostProcessor> {
  public default int order();
  public default int compareTo(cn.hutool.core.annotation.SynthesizedAnnotationPostProcessor);
  public abstract void process(cn.hutool.core.annotation.SynthesizedAnnotation, cn.hutool.core.annotation.AnnotationSynthesizer);
  public default int compareTo(java.lang.Object);
}
```

## `cn.hutool.core.annotation.SynthesizedAnnotationProxy`

```java
public class cn.hutool.core.annotation.SynthesizedAnnotationProxy implements java.lang.reflect.InvocationHandler {
  public static <T extends java.lang.annotation.Annotation> T create(java.lang.Class<T>, cn.hutool.core.annotation.AnnotationAttributeValueProvider, cn.hutool.core.annotation.SynthesizedAnnotation);
  public static <T extends java.lang.annotation.Annotation> T create(java.lang.Class<T>, cn.hutool.core.annotation.SynthesizedAnnotation);
  public static boolean isProxyAnnotation(java.lang.Class<?>);
  public java.lang.Object invoke(java.lang.Object, java.lang.reflect.Method, java.lang.Object[]) throws java.lang.Throwable;
}
```

## `cn.hutool.core.annotation.SynthesizedAnnotationSelector`

```java
public interface cn.hutool.core.annotation.SynthesizedAnnotationSelector {
  public abstract <T extends cn.hutool.core.annotation.SynthesizedAnnotation> T choose(T, T);
}
```

## `cn.hutool.core.annotation.SynthesizedAnnotationSelector$FarthestAndNewestPrioritySelector`

```java
public class cn.hutool.core.annotation.SynthesizedAnnotationSelector$FarthestAndNewestPrioritySelector implements cn.hutool.core.annotation.SynthesizedAnnotationSelector {
  public cn.hutool.core.annotation.SynthesizedAnnotationSelector$FarthestAndNewestPrioritySelector();
  public <T extends cn.hutool.core.annotation.SynthesizedAnnotation> T choose(T, T);
}
```

## `cn.hutool.core.annotation.SynthesizedAnnotationSelector$FarthestAndOldestPrioritySelector`

```java
public class cn.hutool.core.annotation.SynthesizedAnnotationSelector$FarthestAndOldestPrioritySelector implements cn.hutool.core.annotation.SynthesizedAnnotationSelector {
  public cn.hutool.core.annotation.SynthesizedAnnotationSelector$FarthestAndOldestPrioritySelector();
  public <T extends cn.hutool.core.annotation.SynthesizedAnnotation> T choose(T, T);
}
```

## `cn.hutool.core.annotation.SynthesizedAnnotationSelector$NearestAndNewestPrioritySelector`

```java
public class cn.hutool.core.annotation.SynthesizedAnnotationSelector$NearestAndNewestPrioritySelector implements cn.hutool.core.annotation.SynthesizedAnnotationSelector {
  public cn.hutool.core.annotation.SynthesizedAnnotationSelector$NearestAndNewestPrioritySelector();
  public <T extends cn.hutool.core.annotation.SynthesizedAnnotation> T choose(T, T);
}
```

## `cn.hutool.core.annotation.SynthesizedAnnotationSelector$NearestAndOldestPrioritySelector`

```java
public class cn.hutool.core.annotation.SynthesizedAnnotationSelector$NearestAndOldestPrioritySelector implements cn.hutool.core.annotation.SynthesizedAnnotationSelector {
  public cn.hutool.core.annotation.SynthesizedAnnotationSelector$NearestAndOldestPrioritySelector();
  public <T extends cn.hutool.core.annotation.SynthesizedAnnotation> T choose(T, T);
}
```

## `cn.hutool.core.annotation.WrappedAnnotationAttribute`

```java
public interface cn.hutool.core.annotation.WrappedAnnotationAttribute extends cn.hutool.core.annotation.AnnotationAttribute {
  public abstract cn.hutool.core.annotation.AnnotationAttribute getOriginal();
  public abstract cn.hutool.core.annotation.AnnotationAttribute getNonWrappedOriginal();
  public abstract cn.hutool.core.annotation.AnnotationAttribute getLinked();
  public abstract java.util.Collection<cn.hutool.core.annotation.AnnotationAttribute> getAllLinkedNonWrappedAttributes();
  public default java.lang.annotation.Annotation getAnnotation();
  public default java.lang.reflect.Method getAttribute();
  public abstract boolean isValueEquivalentToDefaultValue();
  public default java.lang.Class<?> getAttributeType();
  public default <T extends java.lang.annotation.Annotation> T getAnnotation(java.lang.Class<T>);
  public default boolean isWrapped();
}
```
