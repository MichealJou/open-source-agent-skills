# com.feilong.lib.javassist.bytecode

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.javassist.bytecode.AccessFlag`

```java
public class com.feilong.lib.javassist.bytecode.AccessFlag {
  public com.feilong.lib.javassist.bytecode.AccessFlag();
  public static int setPublic(int);
  public static int setProtected(int);
  public static int setPrivate(int);
  public static int setPackage(int);
  public static boolean isPublic(int);
  public static boolean isProtected(int);
  public static boolean isPrivate(int);
  public static boolean isPackage(int);
  public static int clear(int, int);
  public static int of(int);
  public static int toModifier(int);
}
```

## `com.feilong.lib.javassist.bytecode.AnnotationDefaultAttribute`

```java
public class com.feilong.lib.javassist.bytecode.AnnotationDefaultAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.AnnotationDefaultAttribute(com.feilong.lib.javassist.bytecode.ConstPool, byte[]);
  public com.feilong.lib.javassist.bytecode.AnnotationDefaultAttribute(com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
  public com.feilong.lib.javassist.bytecode.annotation.MemberValue getDefaultValue();
  public void setDefaultValue(com.feilong.lib.javassist.bytecode.annotation.MemberValue);
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.bytecode.AnnotationsAttribute`

```java
public class com.feilong.lib.javassist.bytecode.AnnotationsAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.AnnotationsAttribute(com.feilong.lib.javassist.bytecode.ConstPool, java.lang.String, byte[]);
  public int numAnnotations();
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
  public com.feilong.lib.javassist.bytecode.annotation.Annotation getAnnotation(java.lang.String);
  public void addAnnotation(com.feilong.lib.javassist.bytecode.annotation.Annotation);
  public boolean removeAnnotation(java.lang.String);
  public com.feilong.lib.javassist.bytecode.annotation.Annotation[] getAnnotations();
  public void setAnnotations(com.feilong.lib.javassist.bytecode.annotation.Annotation[]);
  public void setAnnotation(com.feilong.lib.javassist.bytecode.annotation.Annotation);
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.bytecode.AttributeInfo`

```java
public class com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.AttributeInfo(com.feilong.lib.javassist.bytecode.ConstPool, java.lang.String, byte[]);
  public java.lang.String getName();
  public com.feilong.lib.javassist.bytecode.ConstPool getConstPool();
  public int length();
  public byte[] get();
  public void set(byte[]);
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
}
```

## `com.feilong.lib.javassist.bytecode.BadBytecode`

```java
public class com.feilong.lib.javassist.bytecode.BadBytecode extends java.lang.Exception {
  public com.feilong.lib.javassist.bytecode.BadBytecode(int);
  public com.feilong.lib.javassist.bytecode.BadBytecode(java.lang.String);
  public com.feilong.lib.javassist.bytecode.BadBytecode(java.lang.String, java.lang.Throwable);
  public com.feilong.lib.javassist.bytecode.BadBytecode(com.feilong.lib.javassist.bytecode.MethodInfo, java.lang.Throwable);
}
```

## `com.feilong.lib.javassist.bytecode.BootstrapMethodsAttribute`

```java
public class com.feilong.lib.javassist.bytecode.BootstrapMethodsAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.BootstrapMethodsAttribute(com.feilong.lib.javassist.bytecode.ConstPool, com.feilong.lib.javassist.bytecode.BootstrapMethodsAttribute$BootstrapMethod[]);
  public com.feilong.lib.javassist.bytecode.BootstrapMethodsAttribute$BootstrapMethod[] getMethods();
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
}
```

## `com.feilong.lib.javassist.bytecode.BootstrapMethodsAttribute$BootstrapMethod`

```java
public class com.feilong.lib.javassist.bytecode.BootstrapMethodsAttribute$BootstrapMethod {
  public com.feilong.lib.javassist.bytecode.BootstrapMethodsAttribute$BootstrapMethod(int, int[]);
}
```

## `com.feilong.lib.javassist.bytecode.ByteArray`

```java
public class com.feilong.lib.javassist.bytecode.ByteArray {
  public com.feilong.lib.javassist.bytecode.ByteArray();
  public static int readU16bit(byte[], int);
  public static int readS16bit(byte[], int);
  public static void write16bit(int, byte[], int);
  public static int read32bit(byte[], int);
  public static void write32bit(int, byte[], int);
}
```

## `com.feilong.lib.javassist.bytecode.Bytecode`

```java
public class com.feilong.lib.javassist.bytecode.Bytecode extends com.feilong.lib.javassist.bytecode.ByteVector implements java.lang.Cloneable,com.feilong.lib.javassist.bytecode.Opcode {
  public com.feilong.lib.javassist.bytecode.Bytecode(com.feilong.lib.javassist.bytecode.ConstPool, int, int);
  public com.feilong.lib.javassist.bytecode.Bytecode(com.feilong.lib.javassist.bytecode.ConstPool);
  public java.lang.Object clone();
  public com.feilong.lib.javassist.bytecode.ConstPool getConstPool();
  public com.feilong.lib.javassist.bytecode.ExceptionTable getExceptionTable();
  public com.feilong.lib.javassist.bytecode.CodeAttribute toCodeAttribute();
  public int length();
  public byte[] get();
  public int getMaxStack();
  public void setMaxStack(int);
  public int getMaxLocals();
  public void setMaxLocals(int);
  public void setMaxLocals(boolean, com.feilong.lib.javassist.CtClass[], int);
  public void incMaxLocals(int);
  public void addExceptionHandler(int, int, int, com.feilong.lib.javassist.CtClass);
  public void addExceptionHandler(int, int, int, java.lang.String);
  public void addExceptionHandler(int, int, int, int);
  public int currentPc();
  public int read(int);
  public int read16bit(int);
  public int read32bit(int);
  public void write(int, int);
  public void write16bit(int, int);
  public void write32bit(int, int);
  public void add(int);
  public void add32bit(int);
  public void addGap(int);
  public void addOpcode(int);
  public void growStack(int);
  public int getStackDepth();
  public void setStackDepth(int);
  public void addIndex(int);
  public void addAload(int);
  public void addAstore(int);
  public void addIconst(int);
  public void addConstZero(com.feilong.lib.javassist.CtClass);
  public void addIload(int);
  public void addIstore(int);
  public void addLconst(long);
  public void addLload(int);
  public void addLstore(int);
  public void addDconst(double);
  public void addDload(int);
  public void addDstore(int);
  public void addFconst(float);
  public void addFload(int);
  public void addFstore(int);
  public int addLoad(int, com.feilong.lib.javassist.CtClass);
  public int addStore(int, com.feilong.lib.javassist.CtClass);
  public int addLoadParameters(com.feilong.lib.javassist.CtClass[], int);
  public void addCheckcast(com.feilong.lib.javassist.CtClass);
  public void addCheckcast(java.lang.String);
  public void addInstanceof(java.lang.String);
  public void addGetfield(com.feilong.lib.javassist.CtClass, java.lang.String, java.lang.String);
  public void addGetfield(java.lang.String, java.lang.String, java.lang.String);
  public void addGetstatic(com.feilong.lib.javassist.CtClass, java.lang.String, java.lang.String);
  public void addGetstatic(java.lang.String, java.lang.String, java.lang.String);
  public void addInvokespecial(com.feilong.lib.javassist.CtClass, java.lang.String, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.CtClass[]);
  public void addInvokespecial(com.feilong.lib.javassist.CtClass, java.lang.String, java.lang.String);
  public void addInvokespecial(java.lang.String, java.lang.String, java.lang.String);
  public void addInvokespecial(int, java.lang.String, java.lang.String);
  public void addInvokespecial(boolean, int, java.lang.String, java.lang.String);
  public void addInvokespecial(int, java.lang.String);
  public void addInvokestatic(com.feilong.lib.javassist.CtClass, java.lang.String, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.CtClass[]);
  public void addInvokestatic(com.feilong.lib.javassist.CtClass, java.lang.String, java.lang.String);
  public void addInvokestatic(java.lang.String, java.lang.String, java.lang.String);
  public void addInvokestatic(int, java.lang.String, java.lang.String);
  public void addInvokevirtual(com.feilong.lib.javassist.CtClass, java.lang.String, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.CtClass[]);
  public void addInvokevirtual(com.feilong.lib.javassist.CtClass, java.lang.String, java.lang.String);
  public void addInvokevirtual(java.lang.String, java.lang.String, java.lang.String);
  public void addInvokevirtual(int, java.lang.String, java.lang.String);
  public void addInvokeinterface(com.feilong.lib.javassist.CtClass, java.lang.String, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.CtClass[], int);
  public void addInvokeinterface(com.feilong.lib.javassist.CtClass, java.lang.String, java.lang.String, int);
  public void addInvokeinterface(java.lang.String, java.lang.String, java.lang.String, int);
  public void addInvokeinterface(int, java.lang.String, java.lang.String, int);
  public void addInvokedynamic(int, java.lang.String, java.lang.String);
  public void addLdc(java.lang.String);
  public void addLdc(int);
  public void addLdc2w(long);
  public void addLdc2w(double);
  public void addNew(com.feilong.lib.javassist.CtClass);
  public void addNew(java.lang.String);
  public void addAnewarray(java.lang.String);
  public void addAnewarray(com.feilong.lib.javassist.CtClass, int);
  public void addNewarray(int, int);
  public int addMultiNewarray(com.feilong.lib.javassist.CtClass, int[]);
  public int addMultiNewarray(com.feilong.lib.javassist.CtClass, int);
  public int addMultiNewarray(java.lang.String, int);
  public void addPutfield(com.feilong.lib.javassist.CtClass, java.lang.String, java.lang.String);
  public void addPutfield(java.lang.String, java.lang.String, java.lang.String);
  public void addPutstatic(com.feilong.lib.javassist.CtClass, java.lang.String, java.lang.String);
  public void addPutstatic(java.lang.String, java.lang.String, java.lang.String);
  public void addReturn(com.feilong.lib.javassist.CtClass);
  public void addRet(int);
  public void addPrintln(java.lang.String);
  public void add(int, int, int, int);
  public void add(int, int);
}
```

## `com.feilong.lib.javassist.bytecode.ClassFile`

```java
public final class com.feilong.lib.javassist.bytecode.ClassFile {
  public com.feilong.lib.javassist.bytecode.ClassFile(java.io.DataInputStream) throws java.io.IOException;
  public com.feilong.lib.javassist.bytecode.ClassFile(boolean, java.lang.String, java.lang.String);
  public void compact();
  public void prune();
  public com.feilong.lib.javassist.bytecode.ConstPool getConstPool();
  public boolean isInterface();
  public boolean isFinal();
  public boolean isAbstract();
  public int getAccessFlags();
  public void setAccessFlags(int);
  public int getInnerAccessFlags();
  public java.lang.String getName();
  public void setName(java.lang.String);
  public java.lang.String getSuperclass();
  public int getSuperclassId();
  public void setSuperclass(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
  public void renameClass(java.lang.String, java.lang.String);
  public void renameClass(java.util.Map<java.lang.String, java.lang.String>);
  public void getRefClasses(java.util.Map<java.lang.String, java.lang.String>);
  public java.lang.String[] getInterfaces();
  public void setInterfaces(java.lang.String[]);
  public void addInterface(java.lang.String);
  public java.util.List<com.feilong.lib.javassist.bytecode.FieldInfo> getFields();
  public void addField(com.feilong.lib.javassist.bytecode.FieldInfo) throws com.feilong.lib.javassist.bytecode.DuplicateMemberException;
  public void addField2(com.feilong.lib.javassist.bytecode.FieldInfo);
  public java.util.List<com.feilong.lib.javassist.bytecode.MethodInfo> getMethods();
  public com.feilong.lib.javassist.bytecode.MethodInfo getMethod(java.lang.String);
  public com.feilong.lib.javassist.bytecode.MethodInfo getStaticInitializer();
  public void addMethod(com.feilong.lib.javassist.bytecode.MethodInfo) throws com.feilong.lib.javassist.bytecode.DuplicateMemberException;
  public void addMethod2(com.feilong.lib.javassist.bytecode.MethodInfo);
  public java.util.List<com.feilong.lib.javassist.bytecode.AttributeInfo> getAttributes();
  public com.feilong.lib.javassist.bytecode.AttributeInfo getAttribute(java.lang.String);
  public com.feilong.lib.javassist.bytecode.AttributeInfo removeAttribute(java.lang.String);
  public void addAttribute(com.feilong.lib.javassist.bytecode.AttributeInfo);
  public java.lang.String getSourceFile();
  public void write(java.io.DataOutputStream) throws java.io.IOException;
  public int getMajorVersion();
  public void setMajorVersion(int);
  public int getMinorVersion();
  public void setMinorVersion(int);
  public void setVersionToJava5();
}
```

## `com.feilong.lib.javassist.bytecode.ClassFilePrinter`

```java
public class com.feilong.lib.javassist.bytecode.ClassFilePrinter {
  public com.feilong.lib.javassist.bytecode.ClassFilePrinter();
  public static void print(com.feilong.lib.javassist.bytecode.ClassFile);
  public static void print(com.feilong.lib.javassist.bytecode.ClassFile, java.io.PrintWriter);
}
```

## `com.feilong.lib.javassist.bytecode.ClassFileWriter`

```java
public class com.feilong.lib.javassist.bytecode.ClassFileWriter {
  public com.feilong.lib.javassist.bytecode.ClassFileWriter(int, int);
  public com.feilong.lib.javassist.bytecode.ClassFileWriter$ConstPoolWriter getConstPool();
  public com.feilong.lib.javassist.bytecode.ClassFileWriter$FieldWriter getFieldWriter();
  public com.feilong.lib.javassist.bytecode.ClassFileWriter$MethodWriter getMethodWriter();
  public byte[] end(int, int, int, int[], com.feilong.lib.javassist.bytecode.ClassFileWriter$AttributeWriter);
  public void end(java.io.DataOutputStream, int, int, int, int[], com.feilong.lib.javassist.bytecode.ClassFileWriter$AttributeWriter) throws java.io.IOException;
}
```

## `com.feilong.lib.javassist.bytecode.ClassFileWriter$AttributeWriter`

```java
public interface com.feilong.lib.javassist.bytecode.ClassFileWriter$AttributeWriter {
  public abstract int size();
  public abstract void write(java.io.DataOutputStream) throws java.io.IOException;
}
```

## `com.feilong.lib.javassist.bytecode.ClassFileWriter$ConstPoolWriter`

```java
public final class com.feilong.lib.javassist.bytecode.ClassFileWriter$ConstPoolWriter {
  public int[] addClassInfo(java.lang.String[]);
  public int addClassInfo(java.lang.String);
  public int addClassInfo(int);
  public int addNameAndTypeInfo(java.lang.String, java.lang.String);
  public int addNameAndTypeInfo(int, int);
  public int addFieldrefInfo(int, int);
  public int addMethodrefInfo(int, int);
  public int addInterfaceMethodrefInfo(int, int);
  public int addMethodHandleInfo(int, int);
  public int addMethodTypeInfo(int);
  public int addInvokeDynamicInfo(int, int);
  public int addStringInfo(java.lang.String);
  public int addIntegerInfo(int);
  public int addFloatInfo(float);
  public int addLongInfo(long);
  public int addDoubleInfo(double);
  public int addUtf8Info(java.lang.String);
}
```

## `com.feilong.lib.javassist.bytecode.ClassFileWriter$FieldWriter`

```java
public final class com.feilong.lib.javassist.bytecode.ClassFileWriter$FieldWriter {
  public void add(int, java.lang.String, java.lang.String, com.feilong.lib.javassist.bytecode.ClassFileWriter$AttributeWriter);
  public void add(int, int, int, com.feilong.lib.javassist.bytecode.ClassFileWriter$AttributeWriter);
}
```

## `com.feilong.lib.javassist.bytecode.ClassFileWriter$MethodWriter`

```java
public final class com.feilong.lib.javassist.bytecode.ClassFileWriter$MethodWriter {
  public void begin(int, java.lang.String, java.lang.String, java.lang.String[], com.feilong.lib.javassist.bytecode.ClassFileWriter$AttributeWriter);
  public void begin(int, int, int, int[], com.feilong.lib.javassist.bytecode.ClassFileWriter$AttributeWriter);
  public void add(int);
  public void add16(int);
  public void add32(int);
  public void addInvoke(int, java.lang.String, java.lang.String, java.lang.String);
  public void codeEnd(int, int);
  public void addCatch(int, int, int, int);
  public void end(com.feilong.lib.javassist.bytecode.StackMapTable$Writer, com.feilong.lib.javassist.bytecode.ClassFileWriter$AttributeWriter);
  public int size();
}
```

## `com.feilong.lib.javassist.bytecode.CodeAttribute`

```java
public class com.feilong.lib.javassist.bytecode.CodeAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo implements com.feilong.lib.javassist.bytecode.Opcode {
  public com.feilong.lib.javassist.bytecode.CodeAttribute(com.feilong.lib.javassist.bytecode.ConstPool, int, int, byte[], com.feilong.lib.javassist.bytecode.ExceptionTable);
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>) throws com.feilong.lib.javassist.bytecode.CodeAttribute$RuntimeCopyException;
  public int length();
  public byte[] get();
  public void set(byte[]);
  public java.lang.String getDeclaringClass();
  public int getMaxStack();
  public void setMaxStack(int);
  public int computeMaxStack() throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public int getMaxLocals();
  public void setMaxLocals(int);
  public int getCodeLength();
  public byte[] getCode();
  public com.feilong.lib.javassist.bytecode.CodeIterator iterator();
  public com.feilong.lib.javassist.bytecode.ExceptionTable getExceptionTable();
  public java.util.List<com.feilong.lib.javassist.bytecode.AttributeInfo> getAttributes();
  public com.feilong.lib.javassist.bytecode.AttributeInfo getAttribute(java.lang.String);
  public void setAttribute(com.feilong.lib.javassist.bytecode.StackMapTable);
  public void setAttribute(com.feilong.lib.javassist.bytecode.StackMap);
  public void insertLocalVar(int, int) throws com.feilong.lib.javassist.bytecode.BadBytecode;
}
```

## `com.feilong.lib.javassist.bytecode.CodeAttribute$RuntimeCopyException`

```java
public class com.feilong.lib.javassist.bytecode.CodeAttribute$RuntimeCopyException extends java.lang.RuntimeException {
  public com.feilong.lib.javassist.bytecode.CodeAttribute$RuntimeCopyException(java.lang.String);
}
```

## `com.feilong.lib.javassist.bytecode.CodeIterator`

```java
public class com.feilong.lib.javassist.bytecode.CodeIterator implements com.feilong.lib.javassist.bytecode.Opcode {
  public void begin();
  public void move(int);
  public void setMark(int);
  public int getMark();
  public com.feilong.lib.javassist.bytecode.CodeAttribute get();
  public int getCodeLength();
  public int byteAt(int);
  public int signedByteAt(int);
  public void writeByte(int, int);
  public int u16bitAt(int);
  public int s16bitAt(int);
  public void write16bit(int, int);
  public int s32bitAt(int);
  public void write32bit(int, int);
  public void write(byte[], int);
  public boolean hasNext();
  public int next() throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public int lookAhead();
  public int skipConstructor() throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public int skipSuperConstructor() throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public int skipThisConstructor() throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public int insert(byte[]) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void insert(int, byte[]) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public int insertAt(int, byte[]) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public int insertEx(byte[]) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void insertEx(int, byte[]) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public int insertExAt(int, byte[]) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public int insertGap(int) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public int insertGap(int, int) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public int insertExGap(int) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public int insertExGap(int, int) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public com.feilong.lib.javassist.bytecode.CodeIterator$Gap insertGapAt(int, int, boolean) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void insert(com.feilong.lib.javassist.bytecode.ExceptionTable, int);
  public int append(byte[]);
  public void appendGap(int);
  public void append(com.feilong.lib.javassist.bytecode.ExceptionTable, int);
}
```

## `com.feilong.lib.javassist.bytecode.CodeIterator$Gap`

```java
public class com.feilong.lib.javassist.bytecode.CodeIterator$Gap {
  public com.feilong.lib.javassist.bytecode.CodeIterator$Gap();
}
```

## `com.feilong.lib.javassist.bytecode.ConstPool`

```java
public final class com.feilong.lib.javassist.bytecode.ConstPool {
  public com.feilong.lib.javassist.bytecode.ConstPool(java.lang.String);
  public com.feilong.lib.javassist.bytecode.ConstPool(java.io.DataInputStream) throws java.io.IOException;
  public int getSize();
  public java.lang.String getClassName();
  public int getThisClassInfo();
  public int getTag(int);
  public java.lang.String getClassInfo(int);
  public java.lang.String getClassInfoByDescriptor(int);
  public int getNameAndTypeName(int);
  public int getNameAndTypeDescriptor(int);
  public int getMemberClass(int);
  public int getMemberNameAndType(int);
  public int getFieldrefClass(int);
  public java.lang.String getFieldrefClassName(int);
  public int getFieldrefNameAndType(int);
  public java.lang.String getFieldrefName(int);
  public java.lang.String getFieldrefType(int);
  public int getMethodrefClass(int);
  public java.lang.String getMethodrefClassName(int);
  public int getMethodrefNameAndType(int);
  public java.lang.String getMethodrefName(int);
  public java.lang.String getMethodrefType(int);
  public int getInterfaceMethodrefClass(int);
  public java.lang.String getInterfaceMethodrefClassName(int);
  public int getInterfaceMethodrefNameAndType(int);
  public java.lang.String getInterfaceMethodrefName(int);
  public java.lang.String getInterfaceMethodrefType(int);
  public java.lang.Object getLdcValue(int);
  public int getIntegerInfo(int);
  public float getFloatInfo(int);
  public long getLongInfo(int);
  public double getDoubleInfo(int);
  public java.lang.String getStringInfo(int);
  public java.lang.String getUtf8Info(int);
  public int getMethodHandleKind(int);
  public int getMethodHandleIndex(int);
  public int getMethodTypeInfo(int);
  public int getInvokeDynamicBootstrap(int);
  public int getInvokeDynamicNameAndType(int);
  public java.lang.String getInvokeDynamicType(int);
  public java.lang.String getModuleInfo(int);
  public java.lang.String getPackageInfo(int);
  public int isConstructor(java.lang.String, int);
  public int isMember(java.lang.String, java.lang.String, int);
  public java.lang.String eqMember(java.lang.String, java.lang.String, int);
  public int copy(int, com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
  public int addClassInfo(com.feilong.lib.javassist.CtClass);
  public int addClassInfo(java.lang.String);
  public int addNameAndTypeInfo(java.lang.String, java.lang.String);
  public int addNameAndTypeInfo(int, int);
  public int addFieldrefInfo(int, java.lang.String, java.lang.String);
  public int addFieldrefInfo(int, int);
  public int addMethodrefInfo(int, java.lang.String, java.lang.String);
  public int addMethodrefInfo(int, int);
  public int addInterfaceMethodrefInfo(int, java.lang.String, java.lang.String);
  public int addInterfaceMethodrefInfo(int, int);
  public int addStringInfo(java.lang.String);
  public int addIntegerInfo(int);
  public int addFloatInfo(float);
  public int addLongInfo(long);
  public int addDoubleInfo(double);
  public int addUtf8Info(java.lang.String);
  public int addMethodHandleInfo(int, int);
  public int addMethodTypeInfo(int);
  public int addInvokeDynamicInfo(int, int);
  public int addModuleInfo(int);
  public int addPackageInfo(int);
  public java.util.Set<java.lang.String> getClassNames();
  public void renameClass(java.lang.String, java.lang.String);
  public void renameClass(java.util.Map<java.lang.String, java.lang.String>);
  public void write(java.io.DataOutputStream) throws java.io.IOException;
  public void print();
  public void print(java.io.PrintWriter);
}
```

## `com.feilong.lib.javassist.bytecode.ConstantAttribute`

```java
public class com.feilong.lib.javassist.bytecode.ConstantAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.ConstantAttribute(com.feilong.lib.javassist.bytecode.ConstPool, int);
  public int getConstantValue();
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
}
```

## `com.feilong.lib.javassist.bytecode.DeprecatedAttribute`

```java
public class com.feilong.lib.javassist.bytecode.DeprecatedAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.DeprecatedAttribute(com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
}
```

## `com.feilong.lib.javassist.bytecode.Descriptor`

```java
public class com.feilong.lib.javassist.bytecode.Descriptor {
  public com.feilong.lib.javassist.bytecode.Descriptor();
  public static java.lang.String toJvmName(java.lang.String);
  public static java.lang.String toJavaName(java.lang.String);
  public static java.lang.String toJvmName(com.feilong.lib.javassist.CtClass);
  public static java.lang.String toClassName(java.lang.String);
  public static java.lang.String of(java.lang.String);
  public static java.lang.String rename(java.lang.String, java.lang.String, java.lang.String);
  public static java.lang.String rename(java.lang.String, java.util.Map<java.lang.String, java.lang.String>);
  public static java.lang.String of(com.feilong.lib.javassist.CtClass);
  public static java.lang.String ofConstructor(com.feilong.lib.javassist.CtClass[]);
  public static java.lang.String ofMethod(com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.CtClass[]);
  public static java.lang.String ofParameters(com.feilong.lib.javassist.CtClass[]);
  public static java.lang.String appendParameter(java.lang.String, java.lang.String);
  public static java.lang.String insertParameter(java.lang.String, java.lang.String);
  public static java.lang.String appendParameter(com.feilong.lib.javassist.CtClass, java.lang.String);
  public static java.lang.String insertParameter(com.feilong.lib.javassist.CtClass, java.lang.String);
  public static java.lang.String changeReturnType(java.lang.String, java.lang.String);
  public static com.feilong.lib.javassist.CtClass[] getParameterTypes(java.lang.String, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.NotFoundException;
  public static boolean eqParamTypes(java.lang.String, java.lang.String);
  public static java.lang.String getParamDescriptor(java.lang.String);
  public static com.feilong.lib.javassist.CtClass getReturnType(java.lang.String, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.NotFoundException;
  public static int numOfParameters(java.lang.String);
  public static com.feilong.lib.javassist.CtClass toCtClass(java.lang.String, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.NotFoundException;
  public static int arrayDimension(java.lang.String);
  public static java.lang.String toArrayComponent(java.lang.String, int);
  public static int dataSize(java.lang.String);
  public static int paramSize(java.lang.String);
  public static java.lang.String toString(java.lang.String);
}
```

## `com.feilong.lib.javassist.bytecode.Descriptor$Iterator`

```java
public class com.feilong.lib.javassist.bytecode.Descriptor$Iterator {
  public com.feilong.lib.javassist.bytecode.Descriptor$Iterator(java.lang.String);
  public boolean hasNext();
  public boolean isParameter();
  public char currentChar();
  public boolean is2byte();
  public int next();
}
```

## `com.feilong.lib.javassist.bytecode.DuplicateMemberException`

```java
public class com.feilong.lib.javassist.bytecode.DuplicateMemberException extends com.feilong.lib.javassist.CannotCompileException {
  public com.feilong.lib.javassist.bytecode.DuplicateMemberException(java.lang.String);
}
```

## `com.feilong.lib.javassist.bytecode.EnclosingMethodAttribute`

```java
public class com.feilong.lib.javassist.bytecode.EnclosingMethodAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.EnclosingMethodAttribute(com.feilong.lib.javassist.bytecode.ConstPool, java.lang.String, java.lang.String, java.lang.String);
  public com.feilong.lib.javassist.bytecode.EnclosingMethodAttribute(com.feilong.lib.javassist.bytecode.ConstPool, java.lang.String);
  public int classIndex();
  public int methodIndex();
  public java.lang.String className();
  public java.lang.String methodName();
  public java.lang.String methodDescriptor();
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
}
```

## `com.feilong.lib.javassist.bytecode.ExceptionTable`

```java
public class com.feilong.lib.javassist.bytecode.ExceptionTable implements java.lang.Cloneable {
  public com.feilong.lib.javassist.bytecode.ExceptionTable(com.feilong.lib.javassist.bytecode.ConstPool);
  public java.lang.Object clone() throws java.lang.CloneNotSupportedException;
  public int size();
  public int startPc(int);
  public void setStartPc(int, int);
  public int endPc(int);
  public void setEndPc(int, int);
  public int handlerPc(int);
  public void setHandlerPc(int, int);
  public int catchType(int);
  public void setCatchType(int, int);
  public void add(int, com.feilong.lib.javassist.bytecode.ExceptionTable, int);
  public void add(int, int, int, int, int);
  public void add(int, int, int, int);
  public void remove(int);
  public com.feilong.lib.javassist.bytecode.ExceptionTable copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
}
```

## `com.feilong.lib.javassist.bytecode.ExceptionsAttribute`

```java
public class com.feilong.lib.javassist.bytecode.ExceptionsAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.ExceptionsAttribute(com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
  public int[] getExceptionIndexes();
  public java.lang.String[] getExceptions();
  public void setExceptionIndexes(int[]);
  public void setExceptions(java.lang.String[]);
  public int tableLength();
  public int getException(int);
}
```

## `com.feilong.lib.javassist.bytecode.FieldInfo`

```java
public final class com.feilong.lib.javassist.bytecode.FieldInfo {
  public com.feilong.lib.javassist.bytecode.FieldInfo(com.feilong.lib.javassist.bytecode.ConstPool, java.lang.String, java.lang.String);
  public java.lang.String toString();
  public com.feilong.lib.javassist.bytecode.ConstPool getConstPool();
  public java.lang.String getName();
  public void setName(java.lang.String);
  public int getAccessFlags();
  public void setAccessFlags(int);
  public java.lang.String getDescriptor();
  public void setDescriptor(java.lang.String);
  public int getConstantValue();
  public java.util.List<com.feilong.lib.javassist.bytecode.AttributeInfo> getAttributes();
  public com.feilong.lib.javassist.bytecode.AttributeInfo getAttribute(java.lang.String);
  public com.feilong.lib.javassist.bytecode.AttributeInfo removeAttribute(java.lang.String);
  public void addAttribute(com.feilong.lib.javassist.bytecode.AttributeInfo);
}
```

## `com.feilong.lib.javassist.bytecode.InnerClassesAttribute`

```java
public class com.feilong.lib.javassist.bytecode.InnerClassesAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.InnerClassesAttribute(com.feilong.lib.javassist.bytecode.ConstPool);
  public int tableLength();
  public int innerClassIndex(int);
  public java.lang.String innerClass(int);
  public void setInnerClassIndex(int, int);
  public int outerClassIndex(int);
  public java.lang.String outerClass(int);
  public void setOuterClassIndex(int, int);
  public int innerNameIndex(int);
  public java.lang.String innerName(int);
  public void setInnerNameIndex(int, int);
  public int accessFlags(int);
  public void setAccessFlags(int, int);
  public int find(java.lang.String);
  public void append(java.lang.String, java.lang.String, java.lang.String, int);
  public void append(int, int, int, int);
  public int remove(int);
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
}
```

## `com.feilong.lib.javassist.bytecode.InstructionPrinter`

```java
public class com.feilong.lib.javassist.bytecode.InstructionPrinter implements com.feilong.lib.javassist.bytecode.Opcode {
  public com.feilong.lib.javassist.bytecode.InstructionPrinter(java.io.PrintStream);
  public static void print(com.feilong.lib.javassist.CtMethod, java.io.PrintStream);
  public void print(com.feilong.lib.javassist.CtMethod);
  public static java.lang.String instructionString(com.feilong.lib.javassist.bytecode.CodeIterator, int, com.feilong.lib.javassist.bytecode.ConstPool);
}
```

## `com.feilong.lib.javassist.bytecode.LineNumberAttribute`

```java
public class com.feilong.lib.javassist.bytecode.LineNumberAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public int tableLength();
  public int startPc(int);
  public int lineNumber(int);
  public int toLineNumber(int);
  public int toStartPc(int);
  public com.feilong.lib.javassist.bytecode.LineNumberAttribute$Pc toNearPc(int);
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
}
```

## `com.feilong.lib.javassist.bytecode.LineNumberAttribute$Pc`

```java
public class com.feilong.lib.javassist.bytecode.LineNumberAttribute$Pc {
  public com.feilong.lib.javassist.bytecode.LineNumberAttribute$Pc();
}
```

## `com.feilong.lib.javassist.bytecode.LocalVariableAttribute`

```java
public class com.feilong.lib.javassist.bytecode.LocalVariableAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.LocalVariableAttribute(com.feilong.lib.javassist.bytecode.ConstPool);
  public void addEntry(int, int, int, int, int);
  public void shiftIndex(int, int);
  public int tableLength();
  public int startPc(int);
  public int codeLength(int);
  public int nameIndex(int);
  public java.lang.String variableName(int);
  public int descriptorIndex(int);
  public int signatureIndex(int);
  public java.lang.String descriptor(int);
  public java.lang.String signature(int);
  public int index(int);
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
}
```

## `com.feilong.lib.javassist.bytecode.LocalVariableTypeAttribute`

```java
public class com.feilong.lib.javassist.bytecode.LocalVariableTypeAttribute extends com.feilong.lib.javassist.bytecode.LocalVariableAttribute {
  public com.feilong.lib.javassist.bytecode.LocalVariableTypeAttribute(com.feilong.lib.javassist.bytecode.ConstPool);
}
```

## `com.feilong.lib.javassist.bytecode.MethodInfo`

```java
public class com.feilong.lib.javassist.bytecode.MethodInfo {
  public com.feilong.lib.javassist.bytecode.MethodInfo(com.feilong.lib.javassist.bytecode.ConstPool, java.lang.String, java.lang.String);
  public com.feilong.lib.javassist.bytecode.MethodInfo(com.feilong.lib.javassist.bytecode.ConstPool, java.lang.String, com.feilong.lib.javassist.bytecode.MethodInfo, java.util.Map<java.lang.String, java.lang.String>) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public java.lang.String toString();
  public java.lang.String getName();
  public void setName(java.lang.String);
  public boolean isMethod();
  public com.feilong.lib.javassist.bytecode.ConstPool getConstPool();
  public boolean isConstructor();
  public boolean isStaticInitializer();
  public int getAccessFlags();
  public void setAccessFlags(int);
  public java.lang.String getDescriptor();
  public void setDescriptor(java.lang.String);
  public java.util.List<com.feilong.lib.javassist.bytecode.AttributeInfo> getAttributes();
  public com.feilong.lib.javassist.bytecode.AttributeInfo getAttribute(java.lang.String);
  public com.feilong.lib.javassist.bytecode.AttributeInfo removeAttribute(java.lang.String);
  public void addAttribute(com.feilong.lib.javassist.bytecode.AttributeInfo);
  public com.feilong.lib.javassist.bytecode.ExceptionsAttribute getExceptionsAttribute();
  public com.feilong.lib.javassist.bytecode.CodeAttribute getCodeAttribute();
  public void removeExceptionsAttribute();
  public void setExceptionsAttribute(com.feilong.lib.javassist.bytecode.ExceptionsAttribute);
  public void removeCodeAttribute();
  public void setCodeAttribute(com.feilong.lib.javassist.bytecode.CodeAttribute);
  public void rebuildStackMapIf6(com.feilong.lib.javassist.ClassPool, com.feilong.lib.javassist.bytecode.ClassFile) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void rebuildStackMap(com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void rebuildStackMapForME(com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public int getLineNumber(int);
  public void setSuperclass(java.lang.String) throws com.feilong.lib.javassist.bytecode.BadBytecode;
}
```

## `com.feilong.lib.javassist.bytecode.MethodParametersAttribute`

```java
public class com.feilong.lib.javassist.bytecode.MethodParametersAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.MethodParametersAttribute(com.feilong.lib.javassist.bytecode.ConstPool, java.lang.String[], int[]);
  public int size();
  public int name(int);
  public int accessFlags(int);
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
}
```

## `com.feilong.lib.javassist.bytecode.NestHostAttribute`

```java
public class com.feilong.lib.javassist.bytecode.NestHostAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
  public int hostClassIndex();
}
```

## `com.feilong.lib.javassist.bytecode.NestMembersAttribute`

```java
public class com.feilong.lib.javassist.bytecode.NestMembersAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
  public int numberOfClasses();
  public int memberClass(int);
}
```

## `com.feilong.lib.javassist.bytecode.ParameterAnnotationsAttribute`

```java
public class com.feilong.lib.javassist.bytecode.ParameterAnnotationsAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.ParameterAnnotationsAttribute(com.feilong.lib.javassist.bytecode.ConstPool, java.lang.String, byte[]);
  public com.feilong.lib.javassist.bytecode.ParameterAnnotationsAttribute(com.feilong.lib.javassist.bytecode.ConstPool, java.lang.String);
  public int numParameters();
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
  public com.feilong.lib.javassist.bytecode.annotation.Annotation[][] getAnnotations();
  public void setAnnotations(com.feilong.lib.javassist.bytecode.annotation.Annotation[][]);
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.bytecode.SignatureAttribute`

```java
public class com.feilong.lib.javassist.bytecode.SignatureAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.SignatureAttribute(com.feilong.lib.javassist.bytecode.ConstPool, java.lang.String);
  public java.lang.String getSignature();
  public void setSignature(java.lang.String);
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
  public static com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassSignature toClassSignature(java.lang.String) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public static com.feilong.lib.javassist.bytecode.SignatureAttribute$MethodSignature toMethodSignature(java.lang.String) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public static com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType toFieldSignature(java.lang.String) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public static com.feilong.lib.javassist.bytecode.SignatureAttribute$Type toTypeSignature(java.lang.String) throws com.feilong.lib.javassist.bytecode.BadBytecode;
}
```

## `com.feilong.lib.javassist.bytecode.SignatureAttribute$ArrayType`

```java
public class com.feilong.lib.javassist.bytecode.SignatureAttribute$ArrayType extends com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType {
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$ArrayType(int, com.feilong.lib.javassist.bytecode.SignatureAttribute$Type);
  public int getDimension();
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$Type getComponentType();
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.bytecode.SignatureAttribute$BaseType`

```java
public class com.feilong.lib.javassist.bytecode.SignatureAttribute$BaseType extends com.feilong.lib.javassist.bytecode.SignatureAttribute$Type {
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$BaseType(java.lang.String);
  public char getDescriptor();
  public com.feilong.lib.javassist.CtClass getCtlass();
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassSignature`

```java
public class com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassSignature {
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassSignature(com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeParameter[], com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassType, com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassType[]);
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassSignature(com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeParameter[]);
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeParameter[] getParameters();
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassType getSuperClass();
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassType[] getInterfaces();
  public java.lang.String toString();
  public java.lang.String encode();
}
```

## `com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassType`

```java
public class com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassType extends com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType {
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassType(java.lang.String, com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeArgument[]);
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassType(java.lang.String);
  public java.lang.String getName();
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeArgument[] getTypeArguments();
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassType getDeclaringClass();
  public java.lang.String toString();
  public java.lang.String jvmTypeName();
}
```

## `com.feilong.lib.javassist.bytecode.SignatureAttribute$MethodSignature`

```java
public class com.feilong.lib.javassist.bytecode.SignatureAttribute$MethodSignature {
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$MethodSignature(com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeParameter[], com.feilong.lib.javassist.bytecode.SignatureAttribute$Type[], com.feilong.lib.javassist.bytecode.SignatureAttribute$Type, com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType[]);
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeParameter[] getTypeParameters();
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$Type[] getParameterTypes();
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$Type getReturnType();
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType[] getExceptionTypes();
  public java.lang.String toString();
  public java.lang.String encode();
}
```

## `com.feilong.lib.javassist.bytecode.SignatureAttribute$NestedClassType`

```java
public class com.feilong.lib.javassist.bytecode.SignatureAttribute$NestedClassType extends com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassType {
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$NestedClassType(com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassType, java.lang.String, com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeArgument[]);
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$ClassType getDeclaringClass();
}
```

## `com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType`

```java
public abstract class com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType extends com.feilong.lib.javassist.bytecode.SignatureAttribute$Type {
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType();
  public java.lang.String encode();
}
```

## `com.feilong.lib.javassist.bytecode.SignatureAttribute$Type`

```java
public abstract class com.feilong.lib.javassist.bytecode.SignatureAttribute$Type {
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$Type();
  public java.lang.String jvmTypeName();
}
```

## `com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeArgument`

```java
public class com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeArgument {
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeArgument(com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType);
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeArgument();
  public static com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeArgument subclassOf(com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType);
  public static com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeArgument superOf(com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType);
  public char getKind();
  public boolean isWildcard();
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType getType();
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeParameter`

```java
public class com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeParameter {
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeParameter(java.lang.String, com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType, com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType[]);
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeParameter(java.lang.String);
  public java.lang.String getName();
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType getClassBound();
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType[] getInterfaceBound();
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeVariable`

```java
public class com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeVariable extends com.feilong.lib.javassist.bytecode.SignatureAttribute$ObjectType {
  public com.feilong.lib.javassist.bytecode.SignatureAttribute$TypeVariable(java.lang.String);
  public java.lang.String getName();
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.bytecode.SourceFileAttribute`

```java
public class com.feilong.lib.javassist.bytecode.SourceFileAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.SourceFileAttribute(com.feilong.lib.javassist.bytecode.ConstPool, java.lang.String);
  public java.lang.String getFileName();
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
}
```

## `com.feilong.lib.javassist.bytecode.StackMap`

```java
public class com.feilong.lib.javassist.bytecode.StackMap extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public int numOfEntries();
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
  public void insertLocal(int, int, int) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void removeNew(int) throws com.feilong.lib.javassist.CannotCompileException;
  public void print(java.io.PrintWriter);
}
```

## `com.feilong.lib.javassist.bytecode.StackMap$Walker`

```java
public class com.feilong.lib.javassist.bytecode.StackMap$Walker {
  public com.feilong.lib.javassist.bytecode.StackMap$Walker(com.feilong.lib.javassist.bytecode.StackMap);
  public void visit();
  public int locals(int, int, int);
  public int stack(int, int, int);
  public int typeInfoArray(int, int, int, boolean);
  public void typeInfo(int, byte);
  public void objectVariable(int, int);
  public void uninitialized(int, int);
}
```

## `com.feilong.lib.javassist.bytecode.StackMap$Writer`

```java
public class com.feilong.lib.javassist.bytecode.StackMap$Writer {
  public com.feilong.lib.javassist.bytecode.StackMap$Writer();
  public byte[] toByteArray();
  public com.feilong.lib.javassist.bytecode.StackMap toStackMap(com.feilong.lib.javassist.bytecode.ConstPool);
  public void writeVerifyTypeInfo(int, int);
  public void write16bit(int);
}
```

## `com.feilong.lib.javassist.bytecode.StackMapTable`

```java
public class com.feilong.lib.javassist.bytecode.StackMapTable extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>) throws com.feilong.lib.javassist.bytecode.StackMapTable$RuntimeCopyException;
  public void insertLocal(int, int, int) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public static int typeTagOf(char);
  public void println(java.io.PrintWriter);
  public void println(java.io.PrintStream);
  public void removeNew(int) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.bytecode.StackMapTable$RuntimeCopyException`

```java
public class com.feilong.lib.javassist.bytecode.StackMapTable$RuntimeCopyException extends java.lang.RuntimeException {
  public com.feilong.lib.javassist.bytecode.StackMapTable$RuntimeCopyException(java.lang.String);
}
```

## `com.feilong.lib.javassist.bytecode.StackMapTable$Walker`

```java
public class com.feilong.lib.javassist.bytecode.StackMapTable$Walker {
  public com.feilong.lib.javassist.bytecode.StackMapTable$Walker(com.feilong.lib.javassist.bytecode.StackMapTable);
  public com.feilong.lib.javassist.bytecode.StackMapTable$Walker(byte[]);
  public final int size();
  public void parse() throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void sameFrame(int, int) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void sameLocals(int, int, int, int) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void chopFrame(int, int, int) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void appendFrame(int, int, int[], int[]) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void fullFrame(int, int, int[], int[], int[], int[]) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void objectOrUninitialized(int, int, int);
}
```

## `com.feilong.lib.javassist.bytecode.StackMapTable$Writer`

```java
public class com.feilong.lib.javassist.bytecode.StackMapTable$Writer {
  public com.feilong.lib.javassist.bytecode.StackMapTable$Writer(int);
  public byte[] toByteArray();
  public com.feilong.lib.javassist.bytecode.StackMapTable toStackMapTable(com.feilong.lib.javassist.bytecode.ConstPool);
  public void sameFrame(int);
  public void sameLocals(int, int, int);
  public void chopFrame(int, int);
  public void appendFrame(int, int[], int[]);
  public void fullFrame(int, int[], int[], int[], int[]);
}
```

## `com.feilong.lib.javassist.bytecode.SyntheticAttribute`

```java
public class com.feilong.lib.javassist.bytecode.SyntheticAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.SyntheticAttribute(com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
}
```

## `com.feilong.lib.javassist.bytecode.TypeAnnotationsAttribute`

```java
public class com.feilong.lib.javassist.bytecode.TypeAnnotationsAttribute extends com.feilong.lib.javassist.bytecode.AttributeInfo {
  public com.feilong.lib.javassist.bytecode.TypeAnnotationsAttribute(com.feilong.lib.javassist.bytecode.ConstPool, java.lang.String, byte[]);
  public int numAnnotations();
  public com.feilong.lib.javassist.bytecode.AttributeInfo copy(com.feilong.lib.javassist.bytecode.ConstPool, java.util.Map<java.lang.String, java.lang.String>);
}
```
