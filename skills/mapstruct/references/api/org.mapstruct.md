# org.mapstruct

版本：1.6.3。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `org.mapstruct.AnnotateWith`

```java
public interface org.mapstruct.AnnotateWith extends java.lang.annotation.Annotation {
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation> value();
  public abstract org.mapstruct.AnnotateWith$Element[] elements();
}
```

## `org.mapstruct.AnnotateWith$Element`

```java
public interface org.mapstruct.AnnotateWith$Element extends java.lang.annotation.Annotation {
  public abstract java.lang.String name();
  public abstract short[] shorts();
  public abstract byte[] bytes();
  public abstract int[] ints();
  public abstract long[] longs();
  public abstract float[] floats();
  public abstract double[] doubles();
  public abstract char[] chars();
  public abstract boolean[] booleans();
  public abstract java.lang.String[] strings();
  public abstract java.lang.Class<?>[] classes();
  public abstract java.lang.Class<? extends java.lang.Enum<?>> enumClass();
  public abstract java.lang.String[] enums();
}
```

## `org.mapstruct.AnnotateWiths`

```java
public interface org.mapstruct.AnnotateWiths extends java.lang.annotation.Annotation {
  public abstract org.mapstruct.AnnotateWith[] value();
}
```

## `org.mapstruct.BeanMapping`

```java
public interface org.mapstruct.BeanMapping extends java.lang.annotation.Annotation {
  public abstract java.lang.Class<?> resultType();
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation>[] qualifiedBy();
  public abstract java.lang.String[] qualifiedByName();
  public abstract org.mapstruct.NullValueMappingStrategy nullValueMappingStrategy();
  public abstract org.mapstruct.NullValuePropertyMappingStrategy nullValuePropertyMappingStrategy();
  public abstract org.mapstruct.NullValueCheckStrategy nullValueCheckStrategy();
  public abstract org.mapstruct.SubclassExhaustiveStrategy subclassExhaustiveStrategy();
  public abstract boolean ignoreByDefault();
  public abstract java.lang.String[] ignoreUnmappedSourceProperties();
  public abstract org.mapstruct.ReportingPolicy unmappedSourcePolicy();
  public abstract org.mapstruct.ReportingPolicy unmappedTargetPolicy();
  public abstract org.mapstruct.Builder builder();
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation> mappingControl();
}
```

## `org.mapstruct.Builder`

```java
public interface org.mapstruct.Builder extends java.lang.annotation.Annotation {
  public abstract java.lang.String buildMethod();
  public abstract boolean disableBuilder();
}
```

## `org.mapstruct.CollectionMappingStrategy`

```java
public final class org.mapstruct.CollectionMappingStrategy extends java.lang.Enum<org.mapstruct.CollectionMappingStrategy> {
  public static org.mapstruct.CollectionMappingStrategy[] values();
  public static org.mapstruct.CollectionMappingStrategy valueOf(java.lang.String);
}
```

## `org.mapstruct.Condition`

```java
public interface org.mapstruct.Condition extends java.lang.annotation.Annotation {
  public abstract org.mapstruct.ConditionStrategy[] appliesTo();
}
```

## `org.mapstruct.ConditionStrategy`

```java
public final class org.mapstruct.ConditionStrategy extends java.lang.Enum<org.mapstruct.ConditionStrategy> {
  public static org.mapstruct.ConditionStrategy[] values();
  public static org.mapstruct.ConditionStrategy valueOf(java.lang.String);
}
```

## `org.mapstruct.DecoratedWith`

```java
public interface org.mapstruct.DecoratedWith extends java.lang.annotation.Annotation {
  public abstract java.lang.Class<?> value();
}
```

## `org.mapstruct.EnumMapping`

```java
public interface org.mapstruct.EnumMapping extends java.lang.annotation.Annotation {
  public abstract java.lang.String nameTransformationStrategy();
  public abstract java.lang.String configuration();
  public abstract java.lang.Class<? extends java.lang.Exception> unexpectedValueMappingException();
}
```

## `org.mapstruct.InheritConfiguration`

```java
public interface org.mapstruct.InheritConfiguration extends java.lang.annotation.Annotation {
  public abstract java.lang.String name();
}
```

## `org.mapstruct.InheritInverseConfiguration`

```java
public interface org.mapstruct.InheritInverseConfiguration extends java.lang.annotation.Annotation {
  public abstract java.lang.String name();
}
```

## `org.mapstruct.InjectionStrategy`

```java
public final class org.mapstruct.InjectionStrategy extends java.lang.Enum<org.mapstruct.InjectionStrategy> {
  public static org.mapstruct.InjectionStrategy[] values();
  public static org.mapstruct.InjectionStrategy valueOf(java.lang.String);
}
```

## `org.mapstruct.IterableMapping`

```java
public interface org.mapstruct.IterableMapping extends java.lang.annotation.Annotation {
  public abstract java.lang.String dateFormat();
  public abstract java.lang.String numberFormat();
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation>[] qualifiedBy();
  public abstract java.lang.String[] qualifiedByName();
  public abstract java.lang.Class<?> elementTargetType();
  public abstract org.mapstruct.NullValueMappingStrategy nullValueMappingStrategy();
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation> elementMappingControl();
}
```

## `org.mapstruct.Javadoc`

```java
public interface org.mapstruct.Javadoc extends java.lang.annotation.Annotation {
  public abstract java.lang.String value();
  public abstract java.lang.String[] authors();
  public abstract java.lang.String deprecated();
  public abstract java.lang.String since();
}
```

## `org.mapstruct.MapMapping`

```java
public interface org.mapstruct.MapMapping extends java.lang.annotation.Annotation {
  public abstract java.lang.String keyDateFormat();
  public abstract java.lang.String valueDateFormat();
  public abstract java.lang.String keyNumberFormat();
  public abstract java.lang.String valueNumberFormat();
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation>[] keyQualifiedBy();
  public abstract java.lang.String[] keyQualifiedByName();
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation>[] valueQualifiedBy();
  public abstract java.lang.String[] valueQualifiedByName();
  public abstract java.lang.Class<?> keyTargetType();
  public abstract java.lang.Class<?> valueTargetType();
  public abstract org.mapstruct.NullValueMappingStrategy nullValueMappingStrategy();
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation> keyMappingControl();
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation> valueMappingControl();
}
```

## `org.mapstruct.Mapper`

```java
public interface org.mapstruct.Mapper extends java.lang.annotation.Annotation {
  public abstract java.lang.Class<?>[] uses();
  public abstract java.lang.Class<?>[] imports();
  public abstract org.mapstruct.ReportingPolicy unmappedSourcePolicy();
  public abstract org.mapstruct.ReportingPolicy unmappedTargetPolicy();
  public abstract org.mapstruct.ReportingPolicy typeConversionPolicy();
  public abstract java.lang.String componentModel();
  public abstract java.lang.String implementationName();
  public abstract java.lang.String implementationPackage();
  public abstract java.lang.Class<?> config();
  public abstract org.mapstruct.CollectionMappingStrategy collectionMappingStrategy();
  public abstract org.mapstruct.NullValueMappingStrategy nullValueMappingStrategy();
  public abstract org.mapstruct.NullValueMappingStrategy nullValueIterableMappingStrategy();
  public abstract org.mapstruct.NullValueMappingStrategy nullValueMapMappingStrategy();
  public abstract org.mapstruct.NullValuePropertyMappingStrategy nullValuePropertyMappingStrategy();
  public abstract org.mapstruct.MappingInheritanceStrategy mappingInheritanceStrategy();
  public abstract org.mapstruct.NullValueCheckStrategy nullValueCheckStrategy();
  public abstract org.mapstruct.SubclassExhaustiveStrategy subclassExhaustiveStrategy();
  public abstract org.mapstruct.InjectionStrategy injectionStrategy();
  public abstract boolean disableSubMappingMethodsGeneration();
  public abstract org.mapstruct.Builder builder();
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation> mappingControl();
  public abstract java.lang.Class<? extends java.lang.Exception> unexpectedValueMappingException();
  public abstract boolean suppressTimestampInGenerated();
}
```

## `org.mapstruct.MapperConfig`

```java
public interface org.mapstruct.MapperConfig extends java.lang.annotation.Annotation {
  public abstract java.lang.Class<?>[] uses();
  public abstract java.lang.Class<?>[] imports();
  public abstract org.mapstruct.ReportingPolicy unmappedSourcePolicy();
  public abstract org.mapstruct.ReportingPolicy unmappedTargetPolicy();
  public abstract org.mapstruct.ReportingPolicy typeConversionPolicy();
  public abstract java.lang.String componentModel();
  public abstract java.lang.String implementationName();
  public abstract java.lang.String implementationPackage();
  public abstract org.mapstruct.CollectionMappingStrategy collectionMappingStrategy();
  public abstract org.mapstruct.NullValueMappingStrategy nullValueMappingStrategy();
  public abstract org.mapstruct.NullValueMappingStrategy nullValueIterableMappingStrategy();
  public abstract org.mapstruct.NullValueMappingStrategy nullValueMapMappingStrategy();
  public abstract org.mapstruct.NullValuePropertyMappingStrategy nullValuePropertyMappingStrategy();
  public abstract org.mapstruct.MappingInheritanceStrategy mappingInheritanceStrategy();
  public abstract org.mapstruct.NullValueCheckStrategy nullValueCheckStrategy();
  public abstract org.mapstruct.SubclassExhaustiveStrategy subclassExhaustiveStrategy();
  public abstract org.mapstruct.InjectionStrategy injectionStrategy();
  public abstract boolean disableSubMappingMethodsGeneration();
  public abstract org.mapstruct.Builder builder();
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation> mappingControl();
  public abstract java.lang.Class<? extends java.lang.Exception> unexpectedValueMappingException();
  public abstract boolean suppressTimestampInGenerated();
}
```

## `org.mapstruct.Mapping`

```java
public interface org.mapstruct.Mapping extends java.lang.annotation.Annotation {
  public abstract java.lang.String target();
  public abstract java.lang.String source();
  public abstract java.lang.String dateFormat();
  public abstract java.lang.String numberFormat();
  public abstract java.lang.String constant();
  public abstract java.lang.String expression();
  public abstract java.lang.String defaultExpression();
  public abstract boolean ignore();
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation>[] qualifiedBy();
  public abstract java.lang.String[] qualifiedByName();
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation>[] conditionQualifiedBy();
  public abstract java.lang.String[] conditionQualifiedByName();
  public abstract java.lang.String conditionExpression();
  public abstract java.lang.Class<?> resultType();
  public abstract java.lang.String[] dependsOn();
  public abstract java.lang.String defaultValue();
  public abstract org.mapstruct.NullValueCheckStrategy nullValueCheckStrategy();
  public abstract org.mapstruct.NullValuePropertyMappingStrategy nullValuePropertyMappingStrategy();
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation> mappingControl();
}
```

## `org.mapstruct.MappingInheritanceStrategy`

```java
public final class org.mapstruct.MappingInheritanceStrategy extends java.lang.Enum<org.mapstruct.MappingInheritanceStrategy> {
  public static org.mapstruct.MappingInheritanceStrategy[] values();
  public static org.mapstruct.MappingInheritanceStrategy valueOf(java.lang.String);
}
```

## `org.mapstruct.Mappings`

```java
public interface org.mapstruct.Mappings extends java.lang.annotation.Annotation {
  public abstract org.mapstruct.Mapping[] value();
}
```

## `org.mapstruct.Named`

```java
public interface org.mapstruct.Named extends java.lang.annotation.Annotation {
  public abstract java.lang.String value();
}
```

## `org.mapstruct.NullValueCheckStrategy`

```java
public final class org.mapstruct.NullValueCheckStrategy extends java.lang.Enum<org.mapstruct.NullValueCheckStrategy> {
  public static org.mapstruct.NullValueCheckStrategy[] values();
  public static org.mapstruct.NullValueCheckStrategy valueOf(java.lang.String);
}
```

## `org.mapstruct.NullValueMappingStrategy`

```java
public final class org.mapstruct.NullValueMappingStrategy extends java.lang.Enum<org.mapstruct.NullValueMappingStrategy> {
  public static org.mapstruct.NullValueMappingStrategy[] values();
  public static org.mapstruct.NullValueMappingStrategy valueOf(java.lang.String);
}
```

## `org.mapstruct.NullValuePropertyMappingStrategy`

```java
public final class org.mapstruct.NullValuePropertyMappingStrategy extends java.lang.Enum<org.mapstruct.NullValuePropertyMappingStrategy> {
  public static org.mapstruct.NullValuePropertyMappingStrategy[] values();
  public static org.mapstruct.NullValuePropertyMappingStrategy valueOf(java.lang.String);
}
```

## `org.mapstruct.ReportingPolicy`

```java
public final class org.mapstruct.ReportingPolicy extends java.lang.Enum<org.mapstruct.ReportingPolicy> {
  public static org.mapstruct.ReportingPolicy[] values();
  public static org.mapstruct.ReportingPolicy valueOf(java.lang.String);
}
```

## `org.mapstruct.SubclassExhaustiveStrategy`

```java
public final class org.mapstruct.SubclassExhaustiveStrategy extends java.lang.Enum<org.mapstruct.SubclassExhaustiveStrategy> {
  public static org.mapstruct.SubclassExhaustiveStrategy[] values();
  public static org.mapstruct.SubclassExhaustiveStrategy valueOf(java.lang.String);
}
```

## `org.mapstruct.SubclassMapping`

```java
public interface org.mapstruct.SubclassMapping extends java.lang.annotation.Annotation {
  public abstract java.lang.Class<?> source();
  public abstract java.lang.Class<?> target();
  public abstract java.lang.Class<? extends java.lang.annotation.Annotation>[] qualifiedBy();
  public abstract java.lang.String[] qualifiedByName();
}
```

## `org.mapstruct.SubclassMappings`

```java
public interface org.mapstruct.SubclassMappings extends java.lang.annotation.Annotation {
  public abstract org.mapstruct.SubclassMapping[] value();
}
```

## `org.mapstruct.ValueMapping`

```java
public interface org.mapstruct.ValueMapping extends java.lang.annotation.Annotation {
  public abstract java.lang.String source();
  public abstract java.lang.String target();
}
```

## `org.mapstruct.ValueMappings`

```java
public interface org.mapstruct.ValueMappings extends java.lang.annotation.Annotation {
  public abstract org.mapstruct.ValueMapping[] value();
}
```
