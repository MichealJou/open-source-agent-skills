# com.feilong.lib.javassist.bytecode.annotation

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.javassist.bytecode.annotation.Annotation`

```java
public class com.feilong.lib.javassist.bytecode.annotation.Annotation {
  public com.feilong.lib.javassist.bytecode.annotation.Annotation(int, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.Annotation(java.lang.String, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.Annotation(com.feilong.lib.javassist.bytecode.ConstPool, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.NotFoundException;
  public static com.feilong.lib.javassist.bytecode.annotation.MemberValue createMemberValue(com.feilong.lib.javassist.bytecode.ConstPool, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.NotFoundException;
  public void addMemberValue(int, com.feilong.lib.javassist.bytecode.annotation.MemberValue);
  public void addMemberValue(java.lang.String, com.feilong.lib.javassist.bytecode.annotation.MemberValue);
  public java.lang.String toString();
  public java.lang.String getTypeName();
  public java.util.Set<java.lang.String> getMemberNames();
  public com.feilong.lib.javassist.bytecode.annotation.MemberValue getMemberValue(java.lang.String);
  public java.lang.Object toAnnotationType(java.lang.ClassLoader, com.feilong.lib.javassist.ClassPool) throws java.lang.ClassNotFoundException, com.feilong.lib.javassist.bytecode.annotation.NoSuchClassError;
  public void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
  public int hashCode();
  public boolean equals(java.lang.Object);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.AnnotationImpl`

```java
public class com.feilong.lib.javassist.bytecode.annotation.AnnotationImpl implements java.lang.reflect.InvocationHandler {
  public static java.lang.Object make(java.lang.ClassLoader, java.lang.Class<?>, com.feilong.lib.javassist.ClassPool, com.feilong.lib.javassist.bytecode.annotation.Annotation) throws java.lang.IllegalArgumentException;
  public java.lang.String getTypeName();
  public com.feilong.lib.javassist.bytecode.annotation.Annotation getAnnotation();
  public java.lang.Object invoke(java.lang.Object, java.lang.reflect.Method, java.lang.Object[]) throws java.lang.Throwable;
  public int hashCode();
}
```

## `com.feilong.lib.javassist.bytecode.annotation.AnnotationMemberValue`

```java
public class com.feilong.lib.javassist.bytecode.annotation.AnnotationMemberValue extends com.feilong.lib.javassist.bytecode.annotation.MemberValue {
  public com.feilong.lib.javassist.bytecode.annotation.AnnotationMemberValue(com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.AnnotationMemberValue(com.feilong.lib.javassist.bytecode.annotation.Annotation, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.Annotation getValue();
  public void setValue(com.feilong.lib.javassist.bytecode.annotation.Annotation);
  public java.lang.String toString();
  public void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
  public void accept(com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter`

```java
public class com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter {
  public com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter(java.io.OutputStream, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.ConstPool getConstPool();
  public void close() throws java.io.IOException;
  public void numParameters(int) throws java.io.IOException;
  public void numAnnotations(int) throws java.io.IOException;
  public void annotation(java.lang.String, int) throws java.io.IOException;
  public void annotation(int, int) throws java.io.IOException;
  public void memberValuePair(java.lang.String) throws java.io.IOException;
  public void memberValuePair(int) throws java.io.IOException;
  public void constValueIndex(boolean) throws java.io.IOException;
  public void constValueIndex(byte) throws java.io.IOException;
  public void constValueIndex(char) throws java.io.IOException;
  public void constValueIndex(short) throws java.io.IOException;
  public void constValueIndex(int) throws java.io.IOException;
  public void constValueIndex(long) throws java.io.IOException;
  public void constValueIndex(float) throws java.io.IOException;
  public void constValueIndex(double) throws java.io.IOException;
  public void constValueIndex(java.lang.String) throws java.io.IOException;
  public void constValueIndex(int, int) throws java.io.IOException;
  public void enumConstValue(java.lang.String, java.lang.String) throws java.io.IOException;
  public void enumConstValue(int, int) throws java.io.IOException;
  public void classInfoIndex(java.lang.String) throws java.io.IOException;
  public void classInfoIndex(int) throws java.io.IOException;
  public void annotationValue() throws java.io.IOException;
  public void arrayValue(int) throws java.io.IOException;
}
```

## `com.feilong.lib.javassist.bytecode.annotation.ArrayMemberValue`

```java
public class com.feilong.lib.javassist.bytecode.annotation.ArrayMemberValue extends com.feilong.lib.javassist.bytecode.annotation.MemberValue {
  public com.feilong.lib.javassist.bytecode.annotation.ArrayMemberValue(com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.ArrayMemberValue(com.feilong.lib.javassist.bytecode.annotation.MemberValue, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.MemberValue getType();
  public com.feilong.lib.javassist.bytecode.annotation.MemberValue[] getValue();
  public void setValue(com.feilong.lib.javassist.bytecode.annotation.MemberValue[]);
  public java.lang.String toString();
  public void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
  public void accept(com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.BooleanMemberValue`

```java
public class com.feilong.lib.javassist.bytecode.annotation.BooleanMemberValue extends com.feilong.lib.javassist.bytecode.annotation.MemberValue {
  public com.feilong.lib.javassist.bytecode.annotation.BooleanMemberValue(int, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.BooleanMemberValue(boolean, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.BooleanMemberValue(com.feilong.lib.javassist.bytecode.ConstPool);
  public boolean getValue();
  public void setValue(boolean);
  public java.lang.String toString();
  public void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
  public void accept(com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.ByteMemberValue`

```java
public class com.feilong.lib.javassist.bytecode.annotation.ByteMemberValue extends com.feilong.lib.javassist.bytecode.annotation.MemberValue {
  public com.feilong.lib.javassist.bytecode.annotation.ByteMemberValue(int, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.ByteMemberValue(byte, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.ByteMemberValue(com.feilong.lib.javassist.bytecode.ConstPool);
  public byte getValue();
  public void setValue(byte);
  public java.lang.String toString();
  public void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
  public void accept(com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.CharMemberValue`

```java
public class com.feilong.lib.javassist.bytecode.annotation.CharMemberValue extends com.feilong.lib.javassist.bytecode.annotation.MemberValue {
  public com.feilong.lib.javassist.bytecode.annotation.CharMemberValue(int, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.CharMemberValue(char, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.CharMemberValue(com.feilong.lib.javassist.bytecode.ConstPool);
  public char getValue();
  public void setValue(char);
  public java.lang.String toString();
  public void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
  public void accept(com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.ClassMemberValue`

```java
public class com.feilong.lib.javassist.bytecode.annotation.ClassMemberValue extends com.feilong.lib.javassist.bytecode.annotation.MemberValue {
  public com.feilong.lib.javassist.bytecode.annotation.ClassMemberValue(int, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.ClassMemberValue(java.lang.String, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.ClassMemberValue(com.feilong.lib.javassist.bytecode.ConstPool);
  public java.lang.String getValue();
  public void setValue(java.lang.String);
  public java.lang.String toString();
  public void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
  public void accept(com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.DoubleMemberValue`

```java
public class com.feilong.lib.javassist.bytecode.annotation.DoubleMemberValue extends com.feilong.lib.javassist.bytecode.annotation.MemberValue {
  public com.feilong.lib.javassist.bytecode.annotation.DoubleMemberValue(int, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.DoubleMemberValue(double, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.DoubleMemberValue(com.feilong.lib.javassist.bytecode.ConstPool);
  public double getValue();
  public void setValue(double);
  public java.lang.String toString();
  public void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
  public void accept(com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.EnumMemberValue`

```java
public class com.feilong.lib.javassist.bytecode.annotation.EnumMemberValue extends com.feilong.lib.javassist.bytecode.annotation.MemberValue {
  public com.feilong.lib.javassist.bytecode.annotation.EnumMemberValue(int, int, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.EnumMemberValue(com.feilong.lib.javassist.bytecode.ConstPool);
  public java.lang.String getType();
  public void setType(java.lang.String);
  public java.lang.String getValue();
  public void setValue(java.lang.String);
  public java.lang.String toString();
  public void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
  public void accept(com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.FloatMemberValue`

```java
public class com.feilong.lib.javassist.bytecode.annotation.FloatMemberValue extends com.feilong.lib.javassist.bytecode.annotation.MemberValue {
  public com.feilong.lib.javassist.bytecode.annotation.FloatMemberValue(int, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.FloatMemberValue(float, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.FloatMemberValue(com.feilong.lib.javassist.bytecode.ConstPool);
  public float getValue();
  public void setValue(float);
  public java.lang.String toString();
  public void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
  public void accept(com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.IntegerMemberValue`

```java
public class com.feilong.lib.javassist.bytecode.annotation.IntegerMemberValue extends com.feilong.lib.javassist.bytecode.annotation.MemberValue {
  public com.feilong.lib.javassist.bytecode.annotation.IntegerMemberValue(int, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.IntegerMemberValue(com.feilong.lib.javassist.bytecode.ConstPool, int);
  public com.feilong.lib.javassist.bytecode.annotation.IntegerMemberValue(com.feilong.lib.javassist.bytecode.ConstPool);
  public int getValue();
  public void setValue(int);
  public java.lang.String toString();
  public void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
  public void accept(com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.LongMemberValue`

```java
public class com.feilong.lib.javassist.bytecode.annotation.LongMemberValue extends com.feilong.lib.javassist.bytecode.annotation.MemberValue {
  public com.feilong.lib.javassist.bytecode.annotation.LongMemberValue(int, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.LongMemberValue(long, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.LongMemberValue(com.feilong.lib.javassist.bytecode.ConstPool);
  public long getValue();
  public void setValue(long);
  public java.lang.String toString();
  public void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
  public void accept(com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.MemberValue`

```java
public abstract class com.feilong.lib.javassist.bytecode.annotation.MemberValue {
  public abstract void accept(com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor);
  public abstract void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
}
```

## `com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor`

```java
public interface com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor {
  public abstract void visitAnnotationMemberValue(com.feilong.lib.javassist.bytecode.annotation.AnnotationMemberValue);
  public abstract void visitArrayMemberValue(com.feilong.lib.javassist.bytecode.annotation.ArrayMemberValue);
  public abstract void visitBooleanMemberValue(com.feilong.lib.javassist.bytecode.annotation.BooleanMemberValue);
  public abstract void visitByteMemberValue(com.feilong.lib.javassist.bytecode.annotation.ByteMemberValue);
  public abstract void visitCharMemberValue(com.feilong.lib.javassist.bytecode.annotation.CharMemberValue);
  public abstract void visitDoubleMemberValue(com.feilong.lib.javassist.bytecode.annotation.DoubleMemberValue);
  public abstract void visitEnumMemberValue(com.feilong.lib.javassist.bytecode.annotation.EnumMemberValue);
  public abstract void visitFloatMemberValue(com.feilong.lib.javassist.bytecode.annotation.FloatMemberValue);
  public abstract void visitIntegerMemberValue(com.feilong.lib.javassist.bytecode.annotation.IntegerMemberValue);
  public abstract void visitLongMemberValue(com.feilong.lib.javassist.bytecode.annotation.LongMemberValue);
  public abstract void visitShortMemberValue(com.feilong.lib.javassist.bytecode.annotation.ShortMemberValue);
  public abstract void visitStringMemberValue(com.feilong.lib.javassist.bytecode.annotation.StringMemberValue);
  public abstract void visitClassMemberValue(com.feilong.lib.javassist.bytecode.annotation.ClassMemberValue);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.NoSuchClassError`

```java
public class com.feilong.lib.javassist.bytecode.annotation.NoSuchClassError extends java.lang.Error {
  public com.feilong.lib.javassist.bytecode.annotation.NoSuchClassError(java.lang.String, java.lang.Error);
  public java.lang.String getClassName();
}
```

## `com.feilong.lib.javassist.bytecode.annotation.ShortMemberValue`

```java
public class com.feilong.lib.javassist.bytecode.annotation.ShortMemberValue extends com.feilong.lib.javassist.bytecode.annotation.MemberValue {
  public com.feilong.lib.javassist.bytecode.annotation.ShortMemberValue(int, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.ShortMemberValue(short, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.ShortMemberValue(com.feilong.lib.javassist.bytecode.ConstPool);
  public short getValue();
  public void setValue(short);
  public java.lang.String toString();
  public void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
  public void accept(com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.StringMemberValue`

```java
public class com.feilong.lib.javassist.bytecode.annotation.StringMemberValue extends com.feilong.lib.javassist.bytecode.annotation.MemberValue {
  public com.feilong.lib.javassist.bytecode.annotation.StringMemberValue(int, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.StringMemberValue(java.lang.String, com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.annotation.StringMemberValue(com.feilong.lib.javassist.bytecode.ConstPool);
  public java.lang.String getValue();
  public void setValue(java.lang.String);
  public java.lang.String toString();
  public void write(com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter) throws java.io.IOException;
  public void accept(com.feilong.lib.javassist.bytecode.annotation.MemberValueVisitor);
}
```

## `com.feilong.lib.javassist.bytecode.annotation.TypeAnnotationsWriter`

```java
public class com.feilong.lib.javassist.bytecode.annotation.TypeAnnotationsWriter extends com.feilong.lib.javassist.bytecode.annotation.AnnotationsWriter {
  public com.feilong.lib.javassist.bytecode.annotation.TypeAnnotationsWriter(java.io.OutputStream, com.feilong.lib.javassist.bytecode.ConstPool);
  public void numAnnotations(int) throws java.io.IOException;
  public void typeParameterTarget(int, int) throws java.io.IOException;
  public void supertypeTarget(int) throws java.io.IOException;
  public void typeParameterBoundTarget(int, int, int) throws java.io.IOException;
  public void emptyTarget(int) throws java.io.IOException;
  public void formalParameterTarget(int) throws java.io.IOException;
  public void throwsTarget(int) throws java.io.IOException;
  public void localVarTarget(int, int) throws java.io.IOException;
  public void localVarTargetTable(int, int, int) throws java.io.IOException;
  public void catchTarget(int) throws java.io.IOException;
  public void offsetTarget(int, int) throws java.io.IOException;
  public void typeArgumentTarget(int, int, int) throws java.io.IOException;
  public void typePath(int) throws java.io.IOException;
  public void typePathPath(int, int) throws java.io.IOException;
}
```
