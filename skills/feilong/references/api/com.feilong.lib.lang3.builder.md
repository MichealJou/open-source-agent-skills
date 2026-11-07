# com.feilong.lib.lang3.builder

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.lang3.builder.Builder`

```java
public interface com.feilong.lib.lang3.builder.Builder<T> {
  public abstract T build();
}
```

## `com.feilong.lib.lang3.builder.CompareToBuilder`

```java
public class com.feilong.lib.lang3.builder.CompareToBuilder implements com.feilong.lib.lang3.builder.Builder<java.lang.Integer> {
  public com.feilong.lib.lang3.builder.CompareToBuilder();
  public static int reflectionCompare(java.lang.Object, java.lang.Object);
  public static int reflectionCompare(java.lang.Object, java.lang.Object, boolean);
  public static int reflectionCompare(java.lang.Object, java.lang.Object, java.util.Collection<java.lang.String>);
  public static int reflectionCompare(java.lang.Object, java.lang.Object, java.lang.String...);
  public static int reflectionCompare(java.lang.Object, java.lang.Object, boolean, java.lang.Class<?>, java.lang.String...);
  public com.feilong.lib.lang3.builder.CompareToBuilder appendSuper(int);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(java.lang.Object, java.lang.Object);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(java.lang.Object, java.lang.Object, java.util.Comparator<?>);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(long, long);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(int, int);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(short, short);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(char, char);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(byte, byte);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(double, double);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(float, float);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(boolean, boolean);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(java.lang.Object[], java.lang.Object[]);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(java.lang.Object[], java.lang.Object[], java.util.Comparator<?>);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(long[], long[]);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(int[], int[]);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(short[], short[]);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(char[], char[]);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(byte[], byte[]);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(double[], double[]);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(float[], float[]);
  public com.feilong.lib.lang3.builder.CompareToBuilder append(boolean[], boolean[]);
  public int toComparison();
  public java.lang.Integer build();
  public java.lang.Object build();
}
```

## `com.feilong.lib.lang3.builder.EqualsBuilder`

```java
public class com.feilong.lib.lang3.builder.EqualsBuilder implements com.feilong.lib.lang3.builder.Builder<java.lang.Boolean> {
  public com.feilong.lib.lang3.builder.EqualsBuilder();
  public com.feilong.lib.lang3.builder.EqualsBuilder setTestTransients(boolean);
  public com.feilong.lib.lang3.builder.EqualsBuilder setTestRecursive(boolean);
  public com.feilong.lib.lang3.builder.EqualsBuilder setBypassReflectionClasses(java.util.List<java.lang.Class<?>>);
  public com.feilong.lib.lang3.builder.EqualsBuilder setReflectUpToClass(java.lang.Class<?>);
  public com.feilong.lib.lang3.builder.EqualsBuilder setExcludeFields(java.lang.String...);
  public static boolean reflectionEquals(java.lang.Object, java.lang.Object, java.util.Collection<java.lang.String>);
  public static boolean reflectionEquals(java.lang.Object, java.lang.Object, java.lang.String...);
  public static boolean reflectionEquals(java.lang.Object, java.lang.Object, boolean);
  public static boolean reflectionEquals(java.lang.Object, java.lang.Object, boolean, java.lang.Class<?>, java.lang.String...);
  public static boolean reflectionEquals(java.lang.Object, java.lang.Object, boolean, java.lang.Class<?>, boolean, java.lang.String...);
  public com.feilong.lib.lang3.builder.EqualsBuilder reflectionAppend(java.lang.Object, java.lang.Object);
  public com.feilong.lib.lang3.builder.EqualsBuilder appendSuper(boolean);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(java.lang.Object, java.lang.Object);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(long, long);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(int, int);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(short, short);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(char, char);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(byte, byte);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(double, double);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(float, float);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(boolean, boolean);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(java.lang.Object[], java.lang.Object[]);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(long[], long[]);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(int[], int[]);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(short[], short[]);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(char[], char[]);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(byte[], byte[]);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(double[], double[]);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(float[], float[]);
  public com.feilong.lib.lang3.builder.EqualsBuilder append(boolean[], boolean[]);
  public boolean isEquals();
  public java.lang.Boolean build();
  public void reset();
  public java.lang.Object build();
}
```

## `com.feilong.lib.lang3.builder.HashCodeBuilder`

```java
public class com.feilong.lib.lang3.builder.HashCodeBuilder implements com.feilong.lib.lang3.builder.Builder<java.lang.Integer> {
  public static int reflectionHashCode(int, int, java.lang.Object);
  public static int reflectionHashCode(int, int, java.lang.Object, boolean);
  public static <T> int reflectionHashCode(int, int, T, boolean, java.lang.Class<? super T>, java.lang.String...);
  public static int reflectionHashCode(java.lang.Object, boolean);
  public static int reflectionHashCode(java.lang.Object, java.util.Collection<java.lang.String>);
  public static int reflectionHashCode(java.lang.Object, java.lang.String...);
  public com.feilong.lib.lang3.builder.HashCodeBuilder();
  public com.feilong.lib.lang3.builder.HashCodeBuilder(int, int);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(boolean);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(boolean[]);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(byte);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(byte[]);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(char);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(char[]);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(double);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(double[]);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(float);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(float[]);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(int);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(int[]);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(long);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(long[]);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(java.lang.Object);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(java.lang.Object[]);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(short);
  public com.feilong.lib.lang3.builder.HashCodeBuilder append(short[]);
  public com.feilong.lib.lang3.builder.HashCodeBuilder appendSuper(int);
  public int toHashCode();
  public java.lang.Integer build();
  public int hashCode();
  public java.lang.Object build();
}
```

## `com.feilong.lib.lang3.builder.RecursiveToStringStyle`

```java
public class com.feilong.lib.lang3.builder.RecursiveToStringStyle extends com.feilong.lib.lang3.builder.ToStringStyle {
  public com.feilong.lib.lang3.builder.RecursiveToStringStyle();
  public void appendDetail(java.lang.StringBuffer, java.lang.String, java.lang.Object);
}
```

## `com.feilong.lib.lang3.builder.ReflectionToStringBuilder`

```java
public class com.feilong.lib.lang3.builder.ReflectionToStringBuilder extends com.feilong.lib.lang3.builder.ToStringBuilder {
  public static java.lang.String toString(java.lang.Object);
  public static java.lang.String toString(java.lang.Object, com.feilong.lib.lang3.builder.ToStringStyle);
  public static java.lang.String toString(java.lang.Object, com.feilong.lib.lang3.builder.ToStringStyle, boolean);
  public static java.lang.String toString(java.lang.Object, com.feilong.lib.lang3.builder.ToStringStyle, boolean, boolean);
  public static <T> java.lang.String toString(T, com.feilong.lib.lang3.builder.ToStringStyle, boolean, boolean, java.lang.Class<? super T>);
  public static <T> java.lang.String toString(T, com.feilong.lib.lang3.builder.ToStringStyle, boolean, boolean, boolean, java.lang.Class<? super T>);
  public static java.lang.String toStringExclude(java.lang.Object, java.util.Collection<java.lang.String>);
  public static java.lang.String toStringExclude(java.lang.Object, java.lang.String...);
  public com.feilong.lib.lang3.builder.ReflectionToStringBuilder(java.lang.Object);
  public com.feilong.lib.lang3.builder.ReflectionToStringBuilder(java.lang.Object, com.feilong.lib.lang3.builder.ToStringStyle);
  public com.feilong.lib.lang3.builder.ReflectionToStringBuilder(java.lang.Object, com.feilong.lib.lang3.builder.ToStringStyle, java.lang.StringBuffer);
  public <T> com.feilong.lib.lang3.builder.ReflectionToStringBuilder(T, com.feilong.lib.lang3.builder.ToStringStyle, java.lang.StringBuffer, java.lang.Class<? super T>, boolean, boolean);
  public <T> com.feilong.lib.lang3.builder.ReflectionToStringBuilder(T, com.feilong.lib.lang3.builder.ToStringStyle, java.lang.StringBuffer, java.lang.Class<? super T>, boolean, boolean, boolean);
  public java.lang.String[] getExcludeFieldNames();
  public java.lang.Class<?> getUpToClass();
  public boolean isAppendStatics();
  public boolean isAppendTransients();
  public boolean isExcludeNullValues();
  public com.feilong.lib.lang3.builder.ReflectionToStringBuilder reflectionAppendArray(java.lang.Object);
  public void setAppendStatics(boolean);
  public void setAppendTransients(boolean);
  public void setExcludeNullValues(boolean);
  public com.feilong.lib.lang3.builder.ReflectionToStringBuilder setExcludeFieldNames(java.lang.String...);
  public void setUpToClass(java.lang.Class<?>);
  public java.lang.String toString();
}
```

## `com.feilong.lib.lang3.builder.StandardToStringStyle`

```java
public class com.feilong.lib.lang3.builder.StandardToStringStyle extends com.feilong.lib.lang3.builder.ToStringStyle {
  public com.feilong.lib.lang3.builder.StandardToStringStyle();
  public boolean isUseClassName();
  public void setUseClassName(boolean);
  public boolean isUseShortClassName();
  public void setUseShortClassName(boolean);
  public boolean isUseIdentityHashCode();
  public void setUseIdentityHashCode(boolean);
  public boolean isUseFieldNames();
  public void setUseFieldNames(boolean);
  public boolean isDefaultFullDetail();
  public void setDefaultFullDetail(boolean);
  public boolean isArrayContentDetail();
  public void setArrayContentDetail(boolean);
  public java.lang.String getArrayStart();
  public void setArrayStart(java.lang.String);
  public java.lang.String getArrayEnd();
  public void setArrayEnd(java.lang.String);
  public java.lang.String getArraySeparator();
  public void setArraySeparator(java.lang.String);
  public java.lang.String getContentStart();
  public void setContentStart(java.lang.String);
  public java.lang.String getContentEnd();
  public void setContentEnd(java.lang.String);
  public java.lang.String getFieldNameValueSeparator();
  public void setFieldNameValueSeparator(java.lang.String);
  public java.lang.String getFieldSeparator();
  public void setFieldSeparator(java.lang.String);
  public boolean isFieldSeparatorAtStart();
  public void setFieldSeparatorAtStart(boolean);
  public boolean isFieldSeparatorAtEnd();
  public void setFieldSeparatorAtEnd(boolean);
  public java.lang.String getNullText();
  public void setNullText(java.lang.String);
  public java.lang.String getSizeStartText();
  public void setSizeStartText(java.lang.String);
  public java.lang.String getSizeEndText();
  public void setSizeEndText(java.lang.String);
  public java.lang.String getSummaryObjectStartText();
  public void setSummaryObjectStartText(java.lang.String);
  public java.lang.String getSummaryObjectEndText();
  public void setSummaryObjectEndText(java.lang.String);
}
```

## `com.feilong.lib.lang3.builder.ToStringBuilder`

```java
public class com.feilong.lib.lang3.builder.ToStringBuilder implements com.feilong.lib.lang3.builder.Builder<java.lang.String> {
  public static com.feilong.lib.lang3.builder.ToStringStyle getDefaultStyle();
  public static void setDefaultStyle(com.feilong.lib.lang3.builder.ToStringStyle);
  public static java.lang.String reflectionToString(java.lang.Object);
  public static java.lang.String reflectionToString(java.lang.Object, com.feilong.lib.lang3.builder.ToStringStyle);
  public static java.lang.String reflectionToString(java.lang.Object, com.feilong.lib.lang3.builder.ToStringStyle, boolean);
  public static <T> java.lang.String reflectionToString(T, com.feilong.lib.lang3.builder.ToStringStyle, boolean, java.lang.Class<? super T>);
  public com.feilong.lib.lang3.builder.ToStringBuilder(java.lang.Object);
  public com.feilong.lib.lang3.builder.ToStringBuilder(java.lang.Object, com.feilong.lib.lang3.builder.ToStringStyle);
  public com.feilong.lib.lang3.builder.ToStringBuilder(java.lang.Object, com.feilong.lib.lang3.builder.ToStringStyle, java.lang.StringBuffer);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(boolean);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(boolean[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(byte);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(byte[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(char);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(char[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(double);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(double[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(float);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(float[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(int);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(int[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(long);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(long[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.Object);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.Object[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(short);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(short[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, boolean);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, boolean[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, boolean[], boolean);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, byte);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, byte[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, byte[], boolean);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, char);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, char[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, char[], boolean);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, double);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, double[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, double[], boolean);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, float);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, float[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, float[], boolean);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, int);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, int[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, int[], boolean);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, long);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, long[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, long[], boolean);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, java.lang.Object);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, java.lang.Object, boolean);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, java.lang.Object[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, java.lang.Object[], boolean);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, short);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, short[]);
  public com.feilong.lib.lang3.builder.ToStringBuilder append(java.lang.String, short[], boolean);
  public com.feilong.lib.lang3.builder.ToStringBuilder appendSuper(java.lang.String);
  public com.feilong.lib.lang3.builder.ToStringBuilder appendToString(java.lang.String);
  public java.lang.Object getObject();
  public java.lang.StringBuffer getStringBuffer();
  public com.feilong.lib.lang3.builder.ToStringStyle getStyle();
  public java.lang.String toString();
  public java.lang.String build();
  public java.lang.Object build();
}
```

## `com.feilong.lib.lang3.builder.ToStringStyle`

```java
public abstract class com.feilong.lib.lang3.builder.ToStringStyle implements java.io.Serializable {
  public void appendSuper(java.lang.StringBuffer, java.lang.String);
  public void appendToString(java.lang.StringBuffer, java.lang.String);
  public void appendStart(java.lang.StringBuffer, java.lang.Object);
  public void appendEnd(java.lang.StringBuffer, java.lang.Object);
  public void append(java.lang.StringBuffer, java.lang.String, java.lang.Object, java.lang.Boolean);
  public void append(java.lang.StringBuffer, java.lang.String, long);
  public void append(java.lang.StringBuffer, java.lang.String, int);
  public void append(java.lang.StringBuffer, java.lang.String, short);
  public void append(java.lang.StringBuffer, java.lang.String, byte);
  public void append(java.lang.StringBuffer, java.lang.String, char);
  public void append(java.lang.StringBuffer, java.lang.String, double);
  public void append(java.lang.StringBuffer, java.lang.String, float);
  public void append(java.lang.StringBuffer, java.lang.String, boolean);
  public void append(java.lang.StringBuffer, java.lang.String, java.lang.Object[], java.lang.Boolean);
  public void append(java.lang.StringBuffer, java.lang.String, long[], java.lang.Boolean);
  public void append(java.lang.StringBuffer, java.lang.String, int[], java.lang.Boolean);
  public void append(java.lang.StringBuffer, java.lang.String, short[], java.lang.Boolean);
  public void append(java.lang.StringBuffer, java.lang.String, byte[], java.lang.Boolean);
  public void append(java.lang.StringBuffer, java.lang.String, char[], java.lang.Boolean);
  public void append(java.lang.StringBuffer, java.lang.String, double[], java.lang.Boolean);
  public void append(java.lang.StringBuffer, java.lang.String, float[], java.lang.Boolean);
  public void append(java.lang.StringBuffer, java.lang.String, boolean[], java.lang.Boolean);
}
```
