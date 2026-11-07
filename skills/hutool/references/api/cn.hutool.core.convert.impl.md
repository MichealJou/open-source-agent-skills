# cn.hutool.core.convert.impl

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.convert.impl.ArrayConverter`

```java
public class cn.hutool.core.convert.impl.ArrayConverter extends cn.hutool.core.convert.AbstractConverter<java.lang.Object> {
  public cn.hutool.core.convert.impl.ArrayConverter(java.lang.Class<?>);
  public cn.hutool.core.convert.impl.ArrayConverter(java.lang.Class<?>, boolean);
  public java.lang.Class getTargetType();
  public void setIgnoreElementError(boolean);
}
```

## `cn.hutool.core.convert.impl.AtomicBooleanConverter`

```java
public class cn.hutool.core.convert.impl.AtomicBooleanConverter extends cn.hutool.core.convert.AbstractConverter<java.util.concurrent.atomic.AtomicBoolean> {
  public cn.hutool.core.convert.impl.AtomicBooleanConverter();
}
```

## `cn.hutool.core.convert.impl.AtomicIntegerArrayConverter`

```java
public class cn.hutool.core.convert.impl.AtomicIntegerArrayConverter extends cn.hutool.core.convert.AbstractConverter<java.util.concurrent.atomic.AtomicIntegerArray> {
  public cn.hutool.core.convert.impl.AtomicIntegerArrayConverter();
}
```

## `cn.hutool.core.convert.impl.AtomicLongArrayConverter`

```java
public class cn.hutool.core.convert.impl.AtomicLongArrayConverter extends cn.hutool.core.convert.AbstractConverter<java.util.concurrent.atomic.AtomicLongArray> {
  public cn.hutool.core.convert.impl.AtomicLongArrayConverter();
}
```

## `cn.hutool.core.convert.impl.AtomicReferenceConverter`

```java
public class cn.hutool.core.convert.impl.AtomicReferenceConverter extends cn.hutool.core.convert.AbstractConverter<java.util.concurrent.atomic.AtomicReference> {
  public cn.hutool.core.convert.impl.AtomicReferenceConverter();
}
```

## `cn.hutool.core.convert.impl.BeanConverter`

```java
public class cn.hutool.core.convert.impl.BeanConverter<T> extends cn.hutool.core.convert.AbstractConverter<T> {
  public cn.hutool.core.convert.impl.BeanConverter(java.lang.reflect.Type);
  public cn.hutool.core.convert.impl.BeanConverter(java.lang.Class<T>);
  public cn.hutool.core.convert.impl.BeanConverter(java.lang.reflect.Type, cn.hutool.core.bean.copier.CopyOptions);
  public java.lang.Class<T> getTargetType();
}
```

## `cn.hutool.core.convert.impl.BooleanConverter`

```java
public class cn.hutool.core.convert.impl.BooleanConverter extends cn.hutool.core.convert.AbstractConverter<java.lang.Boolean> {
  public cn.hutool.core.convert.impl.BooleanConverter();
}
```

## `cn.hutool.core.convert.impl.CalendarConverter`

```java
public class cn.hutool.core.convert.impl.CalendarConverter extends cn.hutool.core.convert.AbstractConverter<java.util.Calendar> {
  public cn.hutool.core.convert.impl.CalendarConverter();
  public java.lang.String getFormat();
  public void setFormat(java.lang.String);
}
```

## `cn.hutool.core.convert.impl.CastConverter`

```java
public class cn.hutool.core.convert.impl.CastConverter<T> extends cn.hutool.core.convert.AbstractConverter<T> {
  public cn.hutool.core.convert.impl.CastConverter();
  public java.lang.Class<T> getTargetType();
}
```

## `cn.hutool.core.convert.impl.CharacterConverter`

```java
public class cn.hutool.core.convert.impl.CharacterConverter extends cn.hutool.core.convert.AbstractConverter<java.lang.Character> {
  public cn.hutool.core.convert.impl.CharacterConverter();
}
```

## `cn.hutool.core.convert.impl.CharsetConverter`

```java
public class cn.hutool.core.convert.impl.CharsetConverter extends cn.hutool.core.convert.AbstractConverter<java.nio.charset.Charset> {
  public cn.hutool.core.convert.impl.CharsetConverter();
}
```

## `cn.hutool.core.convert.impl.ClassConverter`

```java
public class cn.hutool.core.convert.impl.ClassConverter extends cn.hutool.core.convert.AbstractConverter<java.lang.Class<?>> {
  public cn.hutool.core.convert.impl.ClassConverter();
  public cn.hutool.core.convert.impl.ClassConverter(boolean);
}
```

## `cn.hutool.core.convert.impl.CollectionConverter`

```java
public class cn.hutool.core.convert.impl.CollectionConverter implements cn.hutool.core.convert.Converter<java.util.Collection<?>> {
  public cn.hutool.core.convert.impl.CollectionConverter();
  public cn.hutool.core.convert.impl.CollectionConverter(java.lang.reflect.Type);
  public cn.hutool.core.convert.impl.CollectionConverter(java.lang.Class<?>);
  public cn.hutool.core.convert.impl.CollectionConverter(java.lang.reflect.Type, java.lang.reflect.Type);
  public java.util.Collection<?> convert(java.lang.Object, java.util.Collection<?>) throws java.lang.IllegalArgumentException;
  public java.lang.Object convert(java.lang.Object, java.lang.Object) throws java.lang.IllegalArgumentException;
}
```

## `cn.hutool.core.convert.impl.CurrencyConverter`

```java
public class cn.hutool.core.convert.impl.CurrencyConverter extends cn.hutool.core.convert.AbstractConverter<java.util.Currency> {
  public cn.hutool.core.convert.impl.CurrencyConverter();
}
```

## `cn.hutool.core.convert.impl.DateConverter`

```java
public class cn.hutool.core.convert.impl.DateConverter extends cn.hutool.core.convert.AbstractConverter<java.util.Date> {
  public cn.hutool.core.convert.impl.DateConverter(java.lang.Class<? extends java.util.Date>);
  public cn.hutool.core.convert.impl.DateConverter(java.lang.Class<? extends java.util.Date>, java.lang.String);
  public java.lang.String getFormat();
  public void setFormat(java.lang.String);
  public java.lang.Class<java.util.Date> getTargetType();
}
```

## `cn.hutool.core.convert.impl.DurationConverter`

```java
public class cn.hutool.core.convert.impl.DurationConverter extends cn.hutool.core.convert.AbstractConverter<java.time.Duration> {
  public cn.hutool.core.convert.impl.DurationConverter();
}
```

## `cn.hutool.core.convert.impl.EntryConverter`

```java
public class cn.hutool.core.convert.impl.EntryConverter extends cn.hutool.core.convert.AbstractConverter<java.util.Map$Entry<?, ?>> {
  public cn.hutool.core.convert.impl.EntryConverter(java.lang.reflect.Type);
  public cn.hutool.core.convert.impl.EntryConverter(java.lang.reflect.Type, java.lang.reflect.Type, java.lang.reflect.Type);
}
```

## `cn.hutool.core.convert.impl.EnumConverter`

```java
public class cn.hutool.core.convert.impl.EnumConverter extends cn.hutool.core.convert.AbstractConverter<java.lang.Object> {
  public cn.hutool.core.convert.impl.EnumConverter(java.lang.Class);
  public java.lang.Class getTargetType();
}
```

## `cn.hutool.core.convert.impl.LocaleConverter`

```java
public class cn.hutool.core.convert.impl.LocaleConverter extends cn.hutool.core.convert.AbstractConverter<java.util.Locale> {
  public cn.hutool.core.convert.impl.LocaleConverter();
}
```

## `cn.hutool.core.convert.impl.MapConverter`

```java
public class cn.hutool.core.convert.impl.MapConverter extends cn.hutool.core.convert.AbstractConverter<java.util.Map<?, ?>> {
  public cn.hutool.core.convert.impl.MapConverter(java.lang.reflect.Type);
  public cn.hutool.core.convert.impl.MapConverter(java.lang.reflect.Type, java.lang.reflect.Type, java.lang.reflect.Type);
  public java.lang.Class<java.util.Map<?, ?>> getTargetType();
}
```

## `cn.hutool.core.convert.impl.NumberConverter`

```java
public class cn.hutool.core.convert.impl.NumberConverter extends cn.hutool.core.convert.AbstractConverter<java.lang.Number> {
  public cn.hutool.core.convert.impl.NumberConverter();
  public cn.hutool.core.convert.impl.NumberConverter(java.lang.Class<? extends java.lang.Number>);
  public java.lang.Class<java.lang.Number> getTargetType();
}
```

## `cn.hutool.core.convert.impl.OptConverter`

```java
public class cn.hutool.core.convert.impl.OptConverter extends cn.hutool.core.convert.AbstractConverter<cn.hutool.core.lang.Opt<?>> {
  public cn.hutool.core.convert.impl.OptConverter();
}
```

## `cn.hutool.core.convert.impl.OptionalConverter`

```java
public class cn.hutool.core.convert.impl.OptionalConverter extends cn.hutool.core.convert.AbstractConverter<java.util.Optional<?>> {
  public cn.hutool.core.convert.impl.OptionalConverter();
}
```

## `cn.hutool.core.convert.impl.PairConverter`

```java
public class cn.hutool.core.convert.impl.PairConverter extends cn.hutool.core.convert.AbstractConverter<cn.hutool.core.lang.Pair<?, ?>> {
  public cn.hutool.core.convert.impl.PairConverter(java.lang.reflect.Type);
  public cn.hutool.core.convert.impl.PairConverter(java.lang.reflect.Type, java.lang.reflect.Type, java.lang.reflect.Type);
}
```

## `cn.hutool.core.convert.impl.PathConverter`

```java
public class cn.hutool.core.convert.impl.PathConverter extends cn.hutool.core.convert.AbstractConverter<java.nio.file.Path> {
  public cn.hutool.core.convert.impl.PathConverter();
}
```

## `cn.hutool.core.convert.impl.PeriodConverter`

```java
public class cn.hutool.core.convert.impl.PeriodConverter extends cn.hutool.core.convert.AbstractConverter<java.time.Period> {
  public cn.hutool.core.convert.impl.PeriodConverter();
}
```

## `cn.hutool.core.convert.impl.PrimitiveConverter`

```java
public class cn.hutool.core.convert.impl.PrimitiveConverter extends cn.hutool.core.convert.AbstractConverter<java.lang.Object> {
  public cn.hutool.core.convert.impl.PrimitiveConverter(java.lang.Class<?>);
  public java.lang.Class<java.lang.Object> getTargetType();
}
```

## `cn.hutool.core.convert.impl.RecordConverter`

```java
public class cn.hutool.core.convert.impl.RecordConverter implements cn.hutool.core.convert.Converter<java.lang.Object> {
  public cn.hutool.core.convert.impl.RecordConverter(java.lang.Class<?>);
  public java.lang.Object convert(java.lang.Object, java.lang.Object) throws java.lang.IllegalArgumentException;
}
```

## `cn.hutool.core.convert.impl.ReferenceConverter`

```java
public class cn.hutool.core.convert.impl.ReferenceConverter extends cn.hutool.core.convert.AbstractConverter<java.lang.ref.Reference> {
  public cn.hutool.core.convert.impl.ReferenceConverter(java.lang.Class<? extends java.lang.ref.Reference>);
}
```

## `cn.hutool.core.convert.impl.StackTraceElementConverter`

```java
public class cn.hutool.core.convert.impl.StackTraceElementConverter extends cn.hutool.core.convert.AbstractConverter<java.lang.StackTraceElement> {
  public cn.hutool.core.convert.impl.StackTraceElementConverter();
}
```

## `cn.hutool.core.convert.impl.StringConverter`

```java
public class cn.hutool.core.convert.impl.StringConverter extends cn.hutool.core.convert.AbstractConverter<java.lang.String> {
  public cn.hutool.core.convert.impl.StringConverter();
}
```

## `cn.hutool.core.convert.impl.TemporalAccessorConverter`

```java
public class cn.hutool.core.convert.impl.TemporalAccessorConverter extends cn.hutool.core.convert.AbstractConverter<java.time.temporal.TemporalAccessor> {
  public cn.hutool.core.convert.impl.TemporalAccessorConverter(java.lang.Class<?>);
  public cn.hutool.core.convert.impl.TemporalAccessorConverter(java.lang.Class<?>, java.lang.String);
  public java.lang.String getFormat();
  public void setFormat(java.lang.String);
  public java.lang.Class<java.time.temporal.TemporalAccessor> getTargetType();
}
```

## `cn.hutool.core.convert.impl.TimeZoneConverter`

```java
public class cn.hutool.core.convert.impl.TimeZoneConverter extends cn.hutool.core.convert.AbstractConverter<java.util.TimeZone> {
  public cn.hutool.core.convert.impl.TimeZoneConverter();
}
```

## `cn.hutool.core.convert.impl.URIConverter`

```java
public class cn.hutool.core.convert.impl.URIConverter extends cn.hutool.core.convert.AbstractConverter<java.net.URI> {
  public cn.hutool.core.convert.impl.URIConverter();
}
```

## `cn.hutool.core.convert.impl.URLConverter`

```java
public class cn.hutool.core.convert.impl.URLConverter extends cn.hutool.core.convert.AbstractConverter<java.net.URL> {
  public cn.hutool.core.convert.impl.URLConverter();
}
```

## `cn.hutool.core.convert.impl.UUIDConverter`

```java
public class cn.hutool.core.convert.impl.UUIDConverter extends cn.hutool.core.convert.AbstractConverter<java.util.UUID> {
  public cn.hutool.core.convert.impl.UUIDConverter();
}
```
