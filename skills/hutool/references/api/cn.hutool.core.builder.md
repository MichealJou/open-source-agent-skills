# cn.hutool.core.builder

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.builder.Builder`

```java
public interface cn.hutool.core.builder.Builder<T> extends java.io.Serializable {
  public abstract T build();
}
```

## `cn.hutool.core.builder.CompareToBuilder`

```java
public class cn.hutool.core.builder.CompareToBuilder implements cn.hutool.core.builder.Builder<java.lang.Integer> {
  public cn.hutool.core.builder.CompareToBuilder();
  public static int reflectionCompare(java.lang.Object, java.lang.Object);
  public static int reflectionCompare(java.lang.Object, java.lang.Object, boolean);
  public static int reflectionCompare(java.lang.Object, java.lang.Object, java.util.Collection<java.lang.String>);
  public static int reflectionCompare(java.lang.Object, java.lang.Object, java.lang.String...);
  public static int reflectionCompare(java.lang.Object, java.lang.Object, boolean, java.lang.Class<?>, java.lang.String...);
  public cn.hutool.core.builder.CompareToBuilder appendSuper(int);
  public cn.hutool.core.builder.CompareToBuilder append(java.lang.Object, java.lang.Object);
  public cn.hutool.core.builder.CompareToBuilder append(java.lang.Object, java.lang.Object, java.util.Comparator<?>);
  public cn.hutool.core.builder.CompareToBuilder append(long, long);
  public cn.hutool.core.builder.CompareToBuilder append(int, int);
  public cn.hutool.core.builder.CompareToBuilder append(short, short);
  public cn.hutool.core.builder.CompareToBuilder append(char, char);
  public cn.hutool.core.builder.CompareToBuilder append(byte, byte);
  public cn.hutool.core.builder.CompareToBuilder append(double, double);
  public cn.hutool.core.builder.CompareToBuilder append(float, float);
  public cn.hutool.core.builder.CompareToBuilder append(boolean, boolean);
  public cn.hutool.core.builder.CompareToBuilder append(java.lang.Object[], java.lang.Object[]);
  public cn.hutool.core.builder.CompareToBuilder append(java.lang.Object[], java.lang.Object[], java.util.Comparator<?>);
  public cn.hutool.core.builder.CompareToBuilder append(long[], long[]);
  public cn.hutool.core.builder.CompareToBuilder append(int[], int[]);
  public cn.hutool.core.builder.CompareToBuilder append(short[], short[]);
  public cn.hutool.core.builder.CompareToBuilder append(char[], char[]);
  public cn.hutool.core.builder.CompareToBuilder append(byte[], byte[]);
  public cn.hutool.core.builder.CompareToBuilder append(double[], double[]);
  public cn.hutool.core.builder.CompareToBuilder append(float[], float[]);
  public cn.hutool.core.builder.CompareToBuilder append(boolean[], boolean[]);
  public int toComparison();
  public java.lang.Integer build();
  public java.lang.Object build();
}
```

## `cn.hutool.core.builder.EqualsBuilder`

```java
public class cn.hutool.core.builder.EqualsBuilder implements cn.hutool.core.builder.Builder<java.lang.Boolean> {
  public cn.hutool.core.builder.EqualsBuilder();
  public static boolean reflectionEquals(java.lang.Object, java.lang.Object, java.util.Collection<java.lang.String>);
  public static boolean reflectionEquals(java.lang.Object, java.lang.Object, java.lang.String...);
  public static boolean reflectionEquals(java.lang.Object, java.lang.Object, boolean);
  public static boolean reflectionEquals(java.lang.Object, java.lang.Object, boolean, java.lang.Class<?>, java.lang.String...);
  public cn.hutool.core.builder.EqualsBuilder appendSuper(boolean);
  public cn.hutool.core.builder.EqualsBuilder append(java.lang.Object, java.lang.Object);
  public cn.hutool.core.builder.EqualsBuilder append(long, long);
  public cn.hutool.core.builder.EqualsBuilder append(int, int);
  public cn.hutool.core.builder.EqualsBuilder append(short, short);
  public cn.hutool.core.builder.EqualsBuilder append(char, char);
  public cn.hutool.core.builder.EqualsBuilder append(byte, byte);
  public cn.hutool.core.builder.EqualsBuilder append(double, double);
  public cn.hutool.core.builder.EqualsBuilder append(float, float);
  public cn.hutool.core.builder.EqualsBuilder append(boolean, boolean);
  public boolean isEquals();
  public java.lang.Boolean build();
  public void reset();
  public java.lang.Object build();
}
```

## `cn.hutool.core.builder.GenericBuilder`

```java
public class cn.hutool.core.builder.GenericBuilder<T> implements cn.hutool.core.builder.Builder<T> {
  public cn.hutool.core.builder.GenericBuilder(java.util.function.Supplier<T>);
  public static <T> cn.hutool.core.builder.GenericBuilder<T> of(java.util.function.Supplier<T>);
  public static <T, P1> cn.hutool.core.builder.GenericBuilder<T> of(cn.hutool.core.lang.func.Supplier1<T, P1>, P1);
  public static <T, P1, P2> cn.hutool.core.builder.GenericBuilder<T> of(cn.hutool.core.lang.func.Supplier2<T, P1, P2>, P1, P2);
  public static <T, P1, P2, P3> cn.hutool.core.builder.GenericBuilder<T> of(cn.hutool.core.lang.func.Supplier3<T, P1, P2, P3>, P1, P2, P3);
  public static <T, P1, P2, P3, P4> cn.hutool.core.builder.GenericBuilder<T> of(cn.hutool.core.lang.func.Supplier4<T, P1, P2, P3, P4>, P1, P2, P3, P4);
  public static <T, P1, P2, P3, P4, P5> cn.hutool.core.builder.GenericBuilder<T> of(cn.hutool.core.lang.func.Supplier5<T, P1, P2, P3, P4, P5>, P1, P2, P3, P4, P5);
  public cn.hutool.core.builder.GenericBuilder<T> with(java.util.function.Consumer<T>);
  public <P1> cn.hutool.core.builder.GenericBuilder<T> with(java.util.function.BiConsumer<T, P1>, P1);
  public <P1, P2> cn.hutool.core.builder.GenericBuilder<T> with(cn.hutool.core.lang.func.Consumer3<T, P1, P2>, P1, P2);
  public T build();
}
```

## `cn.hutool.core.builder.HashCodeBuilder`

```java
public class cn.hutool.core.builder.HashCodeBuilder implements cn.hutool.core.builder.Builder<java.lang.Integer> {
  public static int reflectionHashCode(int, int, java.lang.Object);
  public static int reflectionHashCode(int, int, java.lang.Object, boolean);
  public static <T> int reflectionHashCode(int, int, T, boolean, java.lang.Class<? super T>, java.lang.String...);
  public static int reflectionHashCode(java.lang.Object, boolean);
  public static int reflectionHashCode(java.lang.Object, java.util.Collection<java.lang.String>);
  public static int reflectionHashCode(java.lang.Object, java.lang.String...);
  public cn.hutool.core.builder.HashCodeBuilder();
  public cn.hutool.core.builder.HashCodeBuilder(int, int);
  public cn.hutool.core.builder.HashCodeBuilder append(boolean);
  public cn.hutool.core.builder.HashCodeBuilder append(boolean[]);
  public cn.hutool.core.builder.HashCodeBuilder append(byte);
  public cn.hutool.core.builder.HashCodeBuilder append(byte[]);
  public cn.hutool.core.builder.HashCodeBuilder append(char);
  public cn.hutool.core.builder.HashCodeBuilder append(char[]);
  public cn.hutool.core.builder.HashCodeBuilder append(double);
  public cn.hutool.core.builder.HashCodeBuilder append(double[]);
  public cn.hutool.core.builder.HashCodeBuilder append(float);
  public cn.hutool.core.builder.HashCodeBuilder append(float[]);
  public cn.hutool.core.builder.HashCodeBuilder append(int);
  public cn.hutool.core.builder.HashCodeBuilder append(int[]);
  public cn.hutool.core.builder.HashCodeBuilder append(long);
  public cn.hutool.core.builder.HashCodeBuilder append(long[]);
  public cn.hutool.core.builder.HashCodeBuilder append(java.lang.Object);
  public cn.hutool.core.builder.HashCodeBuilder append(java.lang.Object[]);
  public cn.hutool.core.builder.HashCodeBuilder append(short);
  public cn.hutool.core.builder.HashCodeBuilder append(short[]);
  public cn.hutool.core.builder.HashCodeBuilder appendSuper(int);
  public int toHashCode();
  public java.lang.Integer build();
  public int hashCode();
  public java.lang.Object build();
}
```
