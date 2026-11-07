# com.feilong.lib.javassist

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.javassist.ByteArrayClassPath`

```java
public class com.feilong.lib.javassist.ByteArrayClassPath implements com.feilong.lib.javassist.ClassPath {
  public com.feilong.lib.javassist.ByteArrayClassPath(java.lang.String, byte[]);
  public java.lang.String toString();
  public java.io.InputStream openClassfile(java.lang.String);
  public java.net.URL find(java.lang.String);
}
```

## `com.feilong.lib.javassist.CannotCompileException`

```java
public class com.feilong.lib.javassist.CannotCompileException extends java.lang.Exception {
  public synchronized java.lang.Throwable getCause();
  public synchronized java.lang.Throwable initCause(java.lang.Throwable);
  public java.lang.String getReason();
  public com.feilong.lib.javassist.CannotCompileException(java.lang.String);
  public com.feilong.lib.javassist.CannotCompileException(java.lang.Throwable);
  public com.feilong.lib.javassist.CannotCompileException(java.lang.String, java.lang.Throwable);
  public com.feilong.lib.javassist.CannotCompileException(com.feilong.lib.javassist.NotFoundException);
  public com.feilong.lib.javassist.CannotCompileException(com.feilong.lib.javassist.compiler.CompileError);
  public com.feilong.lib.javassist.CannotCompileException(java.lang.ClassNotFoundException, java.lang.String);
  public com.feilong.lib.javassist.CannotCompileException(java.lang.ClassFormatError, java.lang.String);
}
```

## `com.feilong.lib.javassist.ClassClassPath`

```java
public class com.feilong.lib.javassist.ClassClassPath implements com.feilong.lib.javassist.ClassPath {
  public com.feilong.lib.javassist.ClassClassPath(java.lang.Class<?>);
  public java.io.InputStream openClassfile(java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public java.net.URL find(java.lang.String);
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.ClassMap`

```java
public class com.feilong.lib.javassist.ClassMap extends java.util.HashMap<java.lang.String, java.lang.String> {
  public com.feilong.lib.javassist.ClassMap();
  public void put(com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.CtClass);
  public java.lang.String put(java.lang.String, java.lang.String);
  public void putIfNone(java.lang.String, java.lang.String);
  public java.lang.String get(java.lang.Object);
  public void fix(com.feilong.lib.javassist.CtClass);
  public void fix(java.lang.String);
  public static java.lang.String toJvmName(java.lang.String);
  public static java.lang.String toJavaName(java.lang.String);
  public java.lang.Object put(java.lang.Object, java.lang.Object);
  public java.lang.Object get(java.lang.Object);
}
```

## `com.feilong.lib.javassist.ClassPath`

```java
public interface com.feilong.lib.javassist.ClassPath {
  public abstract java.io.InputStream openClassfile(java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public abstract java.net.URL find(java.lang.String);
}
```

## `com.feilong.lib.javassist.ClassPool`

```java
public class com.feilong.lib.javassist.ClassPool {
  public com.feilong.lib.javassist.ClassPool(com.feilong.lib.javassist.ClassPool);
  public static synchronized com.feilong.lib.javassist.ClassPool getDefault();
  public java.lang.String toString();
  public java.util.Iterator<java.lang.String> getImportedPackages();
  public java.lang.Object[] lookupCflow(java.lang.String);
  public com.feilong.lib.javassist.CtClass get(java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtClass getCtClass(java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public java.net.URL find(java.lang.String);
  public com.feilong.lib.javassist.CtClass[] get(java.lang.String[]) throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtClass makeClass(java.io.InputStream) throws java.io.IOException, java.lang.RuntimeException;
  public com.feilong.lib.javassist.CtClass makeClass(java.io.InputStream, boolean) throws java.io.IOException, java.lang.RuntimeException;
  public com.feilong.lib.javassist.CtClass makeClass(com.feilong.lib.javassist.bytecode.ClassFile) throws java.lang.RuntimeException;
  public com.feilong.lib.javassist.CtClass makeClassIfNew(java.io.InputStream) throws java.io.IOException, java.lang.RuntimeException;
  public synchronized com.feilong.lib.javassist.CtClass makeClass(java.lang.String, com.feilong.lib.javassist.CtClass) throws java.lang.RuntimeException;
  public com.feilong.lib.javassist.ClassPath appendSystemPath();
  public com.feilong.lib.javassist.ClassPath insertClassPath(com.feilong.lib.javassist.ClassPath);
  public com.feilong.lib.javassist.ClassPath appendClassPath(com.feilong.lib.javassist.ClassPath);
  public com.feilong.lib.javassist.ClassPath appendClassPath(java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public void removeClassPath(com.feilong.lib.javassist.ClassPath);
  public java.lang.Class toClass(com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public java.lang.ClassLoader getClassLoader();
  public java.lang.Class toClass(com.feilong.lib.javassist.CtClass, java.lang.ClassLoader) throws com.feilong.lib.javassist.CannotCompileException;
  public java.lang.Class toClass(com.feilong.lib.javassist.CtClass, java.lang.ClassLoader, java.security.ProtectionDomain) throws com.feilong.lib.javassist.CannotCompileException;
  public java.lang.Class toClass(com.feilong.lib.javassist.CtClass, java.lang.Class<?>, java.lang.ClassLoader, java.security.ProtectionDomain) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.CodeConverter`

```java
public class com.feilong.lib.javassist.CodeConverter {
  public com.feilong.lib.javassist.CodeConverter();
  public void replaceFieldRead(com.feilong.lib.javassist.CtField, com.feilong.lib.javassist.CtClass, java.lang.String);
  public void replaceFieldWrite(com.feilong.lib.javassist.CtField, com.feilong.lib.javassist.CtClass, java.lang.String);
}
```

## `com.feilong.lib.javassist.CodeConverter$ArrayAccessReplacementMethodNames`

```java
public interface com.feilong.lib.javassist.CodeConverter$ArrayAccessReplacementMethodNames {
  public abstract java.lang.String byteOrBooleanRead();
  public abstract java.lang.String byteOrBooleanWrite();
  public abstract java.lang.String charRead();
  public abstract java.lang.String charWrite();
  public abstract java.lang.String doubleRead();
  public abstract java.lang.String doubleWrite();
  public abstract java.lang.String floatRead();
  public abstract java.lang.String floatWrite();
  public abstract java.lang.String intRead();
  public abstract java.lang.String intWrite();
  public abstract java.lang.String longRead();
  public abstract java.lang.String longWrite();
  public abstract java.lang.String objectRead();
  public abstract java.lang.String objectWrite();
  public abstract java.lang.String shortRead();
  public abstract java.lang.String shortWrite();
}
```

## `com.feilong.lib.javassist.CtBehavior`

```java
public abstract class com.feilong.lib.javassist.CtBehavior extends com.feilong.lib.javassist.CtMember {
  public abstract java.lang.String getLongName();
  public com.feilong.lib.javassist.bytecode.MethodInfo getMethodInfo();
  public com.feilong.lib.javassist.bytecode.MethodInfo getMethodInfo2();
  public int getModifiers();
  public void setModifiers(int);
  public boolean hasAnnotation(java.lang.String);
  public java.lang.Object getAnnotation(java.lang.Class<?>) throws java.lang.ClassNotFoundException;
  public java.lang.Object[] getAnnotations() throws java.lang.ClassNotFoundException;
  public java.lang.Object[] getAvailableAnnotations();
  public java.lang.Object[][] getParameterAnnotations() throws java.lang.ClassNotFoundException;
  public java.lang.Object[][] getAvailableParameterAnnotations();
  public com.feilong.lib.javassist.CtClass[] getParameterTypes() throws com.feilong.lib.javassist.NotFoundException;
  public java.lang.String getSignature();
  public java.lang.String getGenericSignature();
  public void setGenericSignature(java.lang.String);
  public com.feilong.lib.javassist.CtClass[] getExceptionTypes() throws com.feilong.lib.javassist.NotFoundException;
  public void setExceptionTypes(com.feilong.lib.javassist.CtClass[]) throws com.feilong.lib.javassist.NotFoundException;
  public abstract boolean isEmpty();
  public void setBody(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
  public void setBody(java.lang.String, java.lang.String, java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
  public byte[] getAttribute(java.lang.String);
  public void setAttribute(java.lang.String, byte[]);
  public void useCflow(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
  public void addLocalVariable(java.lang.String, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public void insertParameter(com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public void addParameter(com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public void instrument(com.feilong.lib.javassist.CodeConverter) throws com.feilong.lib.javassist.CannotCompileException;
  public void instrument(com.feilong.lib.javassist.expr.ExprEditor) throws com.feilong.lib.javassist.CannotCompileException;
  public void insertBefore(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
  public void insertAfter(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
  public void insertAfter(java.lang.String, boolean) throws com.feilong.lib.javassist.CannotCompileException;
  public void addCatch(java.lang.String, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public void addCatch(java.lang.String, com.feilong.lib.javassist.CtClass, java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
  public int insertAt(int, java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
  public int insertAt(int, boolean, java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.CtClass`

```java
public abstract class com.feilong.lib.javassist.CtClass {
  public java.lang.String toString();
  public com.feilong.lib.javassist.ClassPool getClassPool();
  public com.feilong.lib.javassist.bytecode.ClassFile getClassFile();
  public com.feilong.lib.javassist.bytecode.ClassFile getClassFile2();
  public com.feilong.lib.javassist.compiler.AccessorMaker getAccessorMaker();
  public java.net.URL getURL() throws com.feilong.lib.javassist.NotFoundException;
  public boolean isModified();
  public boolean isFrozen();
  public void freeze();
  public void defrost();
  public boolean isPrimitive();
  public boolean isArray();
  public com.feilong.lib.javassist.CtClass getComponentType() throws com.feilong.lib.javassist.NotFoundException;
  public boolean subtypeOf(com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.NotFoundException;
  public java.lang.String getName();
  public final java.lang.String getSimpleName();
  public final java.lang.String getPackageName();
  public void setName(java.lang.String);
  public java.lang.String getGenericSignature();
  public void setGenericSignature(java.lang.String);
  public void replaceClassName(java.lang.String, java.lang.String);
  public void replaceClassName(com.feilong.lib.javassist.ClassMap);
  public synchronized java.util.Collection<java.lang.String> getRefClasses();
  public boolean isInterface();
  public boolean isAnnotation();
  public boolean isEnum();
  public int getModifiers();
  public boolean hasAnnotation(java.lang.Class<?>);
  public boolean hasAnnotation(java.lang.String);
  public java.lang.Object getAnnotation(java.lang.Class<?>) throws java.lang.ClassNotFoundException;
  public java.lang.Object[] getAnnotations() throws java.lang.ClassNotFoundException;
  public java.lang.Object[] getAvailableAnnotations();
  public com.feilong.lib.javassist.CtClass[] getDeclaredClasses() throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtClass[] getNestedClasses() throws com.feilong.lib.javassist.NotFoundException;
  public void setModifiers(int);
  public boolean subclassOf(com.feilong.lib.javassist.CtClass);
  public com.feilong.lib.javassist.CtClass getSuperclass() throws com.feilong.lib.javassist.NotFoundException;
  public void setSuperclass(com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public com.feilong.lib.javassist.CtClass[] getInterfaces() throws com.feilong.lib.javassist.NotFoundException;
  public void setInterfaces(com.feilong.lib.javassist.CtClass[]);
  public void addInterface(com.feilong.lib.javassist.CtClass);
  public com.feilong.lib.javassist.CtClass getDeclaringClass() throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtBehavior getEnclosingBehavior() throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtClass makeNestedClass(java.lang.String, boolean);
  public com.feilong.lib.javassist.CtField[] getFields();
  public com.feilong.lib.javassist.CtField getField(java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtField getField(java.lang.String, java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtField[] getDeclaredFields();
  public com.feilong.lib.javassist.CtField getDeclaredField(java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtField getDeclaredField(java.lang.String, java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtBehavior[] getDeclaredBehaviors();
  public com.feilong.lib.javassist.CtConstructor[] getConstructors();
  public com.feilong.lib.javassist.CtConstructor getConstructor(java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtConstructor[] getDeclaredConstructors();
  public com.feilong.lib.javassist.CtConstructor getDeclaredConstructor(com.feilong.lib.javassist.CtClass[]) throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtConstructor getClassInitializer();
  public com.feilong.lib.javassist.CtMethod[] getMethods();
  public com.feilong.lib.javassist.CtMethod getMethod(java.lang.String, java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtMethod[] getDeclaredMethods();
  public com.feilong.lib.javassist.CtMethod getDeclaredMethod(java.lang.String, com.feilong.lib.javassist.CtClass[]) throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtMethod[] getDeclaredMethods(java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtMethod getDeclaredMethod(java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public com.feilong.lib.javassist.CtConstructor makeClassInitializer() throws com.feilong.lib.javassist.CannotCompileException;
  public void addConstructor(com.feilong.lib.javassist.CtConstructor) throws com.feilong.lib.javassist.CannotCompileException;
  public void removeConstructor(com.feilong.lib.javassist.CtConstructor) throws com.feilong.lib.javassist.NotFoundException;
  public void addMethod(com.feilong.lib.javassist.CtMethod) throws com.feilong.lib.javassist.CannotCompileException;
  public void removeMethod(com.feilong.lib.javassist.CtMethod) throws com.feilong.lib.javassist.NotFoundException;
  public void addField(com.feilong.lib.javassist.CtField) throws com.feilong.lib.javassist.CannotCompileException;
  public void addField(com.feilong.lib.javassist.CtField, java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
  public void addField(com.feilong.lib.javassist.CtField, com.feilong.lib.javassist.CtField$Initializer) throws com.feilong.lib.javassist.CannotCompileException;
  public void removeField(com.feilong.lib.javassist.CtField) throws com.feilong.lib.javassist.NotFoundException;
  public byte[] getAttribute(java.lang.String);
  public void setAttribute(java.lang.String, byte[]);
  public void instrument(com.feilong.lib.javassist.CodeConverter) throws com.feilong.lib.javassist.CannotCompileException;
  public void instrument(com.feilong.lib.javassist.expr.ExprEditor) throws com.feilong.lib.javassist.CannotCompileException;
  public java.lang.Class<?> toClass() throws com.feilong.lib.javassist.CannotCompileException;
  public void detach();
  public boolean stopPruning(boolean);
  public void prune();
  public void rebuildClassFile();
  public byte[] toBytecode() throws java.io.IOException, com.feilong.lib.javassist.CannotCompileException;
  public void writeFile() throws com.feilong.lib.javassist.NotFoundException, java.io.IOException, com.feilong.lib.javassist.CannotCompileException;
  public void writeFile(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException, java.io.IOException;
  public void debugWriteFile();
  public void debugWriteFile(java.lang.String);
  public void toBytecode(java.io.DataOutputStream) throws com.feilong.lib.javassist.CannotCompileException, java.io.IOException;
  public java.lang.String makeUniqueName(java.lang.String);
}
```

## `com.feilong.lib.javassist.CtConstructor`

```java
public final class com.feilong.lib.javassist.CtConstructor extends com.feilong.lib.javassist.CtBehavior {
  public com.feilong.lib.javassist.CtConstructor(com.feilong.lib.javassist.CtClass[], com.feilong.lib.javassist.CtClass);
  public com.feilong.lib.javassist.CtConstructor(com.feilong.lib.javassist.CtConstructor, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.ClassMap) throws com.feilong.lib.javassist.CannotCompileException;
  public boolean isConstructor();
  public boolean isClassInitializer();
  public java.lang.String getLongName();
  public java.lang.String getName();
  public boolean isEmpty();
  public boolean callsSuper() throws com.feilong.lib.javassist.CannotCompileException;
  public void setBody(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
  public void setBody(com.feilong.lib.javassist.CtConstructor, com.feilong.lib.javassist.ClassMap) throws com.feilong.lib.javassist.CannotCompileException;
  public void insertBeforeBody(java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
  public com.feilong.lib.javassist.CtMethod toMethod(java.lang.String, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public com.feilong.lib.javassist.CtMethod toMethod(java.lang.String, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.ClassMap) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.CtField`

```java
public class com.feilong.lib.javassist.CtField extends com.feilong.lib.javassist.CtMember {
  public com.feilong.lib.javassist.CtField(com.feilong.lib.javassist.CtClass, java.lang.String, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public com.feilong.lib.javassist.CtField(com.feilong.lib.javassist.CtField, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public java.lang.String toString();
  public static com.feilong.lib.javassist.CtField make(java.lang.String, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public com.feilong.lib.javassist.bytecode.FieldInfo getFieldInfo();
  public com.feilong.lib.javassist.bytecode.FieldInfo getFieldInfo2();
  public com.feilong.lib.javassist.CtClass getDeclaringClass();
  public java.lang.String getName();
  public void setName(java.lang.String);
  public int getModifiers();
  public void setModifiers(int);
  public boolean hasAnnotation(java.lang.String);
  public java.lang.Object getAnnotation(java.lang.Class<?>) throws java.lang.ClassNotFoundException;
  public java.lang.Object[] getAnnotations() throws java.lang.ClassNotFoundException;
  public java.lang.Object[] getAvailableAnnotations();
  public java.lang.String getSignature();
  public java.lang.String getGenericSignature();
  public void setGenericSignature(java.lang.String);
  public com.feilong.lib.javassist.CtClass getType() throws com.feilong.lib.javassist.NotFoundException;
  public void setType(com.feilong.lib.javassist.CtClass);
  public java.lang.Object getConstantValue();
  public byte[] getAttribute(java.lang.String);
  public void setAttribute(java.lang.String, byte[]);
}
```

## `com.feilong.lib.javassist.CtField$Initializer`

```java
public abstract class com.feilong.lib.javassist.CtField$Initializer {
  public com.feilong.lib.javassist.CtField$Initializer();
  public static com.feilong.lib.javassist.CtField$Initializer constant(int);
  public static com.feilong.lib.javassist.CtField$Initializer constant(boolean);
  public static com.feilong.lib.javassist.CtField$Initializer constant(long);
  public static com.feilong.lib.javassist.CtField$Initializer constant(float);
  public static com.feilong.lib.javassist.CtField$Initializer constant(double);
  public static com.feilong.lib.javassist.CtField$Initializer constant(java.lang.String);
  public static com.feilong.lib.javassist.CtField$Initializer byParameter(int);
  public static com.feilong.lib.javassist.CtField$Initializer byNew(com.feilong.lib.javassist.CtClass);
  public static com.feilong.lib.javassist.CtField$Initializer byNew(com.feilong.lib.javassist.CtClass, java.lang.String[]);
  public static com.feilong.lib.javassist.CtField$Initializer byNewWithParams(com.feilong.lib.javassist.CtClass);
  public static com.feilong.lib.javassist.CtField$Initializer byNewWithParams(com.feilong.lib.javassist.CtClass, java.lang.String[]);
  public static com.feilong.lib.javassist.CtField$Initializer byCall(com.feilong.lib.javassist.CtClass, java.lang.String);
  public static com.feilong.lib.javassist.CtField$Initializer byCall(com.feilong.lib.javassist.CtClass, java.lang.String, java.lang.String[]);
  public static com.feilong.lib.javassist.CtField$Initializer byCallWithParams(com.feilong.lib.javassist.CtClass, java.lang.String);
  public static com.feilong.lib.javassist.CtField$Initializer byCallWithParams(com.feilong.lib.javassist.CtClass, java.lang.String, java.lang.String[]);
  public static com.feilong.lib.javassist.CtField$Initializer byNewArray(com.feilong.lib.javassist.CtClass, int) throws com.feilong.lib.javassist.NotFoundException;
  public static com.feilong.lib.javassist.CtField$Initializer byNewArray(com.feilong.lib.javassist.CtClass, int[]);
  public static com.feilong.lib.javassist.CtField$Initializer byExpr(java.lang.String);
}
```

## `com.feilong.lib.javassist.CtMember`

```java
public abstract class com.feilong.lib.javassist.CtMember {
  public java.lang.String toString();
  public com.feilong.lib.javassist.CtClass getDeclaringClass();
  public boolean visibleFrom(com.feilong.lib.javassist.CtClass);
  public abstract int getModifiers();
  public abstract void setModifiers(int);
  public boolean hasAnnotation(java.lang.Class<?>);
  public abstract boolean hasAnnotation(java.lang.String);
  public abstract java.lang.Object getAnnotation(java.lang.Class<?>) throws java.lang.ClassNotFoundException;
  public abstract java.lang.Object[] getAnnotations() throws java.lang.ClassNotFoundException;
  public abstract java.lang.Object[] getAvailableAnnotations();
  public abstract java.lang.String getName();
  public abstract java.lang.String getSignature();
  public abstract java.lang.String getGenericSignature();
  public abstract void setGenericSignature(java.lang.String);
  public abstract byte[] getAttribute(java.lang.String);
  public abstract void setAttribute(java.lang.String, byte[]);
}
```

## `com.feilong.lib.javassist.CtMethod`

```java
public final class com.feilong.lib.javassist.CtMethod extends com.feilong.lib.javassist.CtBehavior {
  public com.feilong.lib.javassist.CtMethod(com.feilong.lib.javassist.CtClass, java.lang.String, com.feilong.lib.javassist.CtClass[], com.feilong.lib.javassist.CtClass);
  public com.feilong.lib.javassist.CtMethod(com.feilong.lib.javassist.CtMethod, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.ClassMap) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtMethod make(java.lang.String, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtMethod make(com.feilong.lib.javassist.bytecode.MethodInfo, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public int hashCode();
  public boolean equals(java.lang.Object);
  public java.lang.String getLongName();
  public java.lang.String getName();
  public void setName(java.lang.String);
  public com.feilong.lib.javassist.CtClass getReturnType() throws com.feilong.lib.javassist.NotFoundException;
  public boolean isEmpty();
  public void setBody(com.feilong.lib.javassist.CtMethod, com.feilong.lib.javassist.ClassMap) throws com.feilong.lib.javassist.CannotCompileException;
  public void setWrappedBody(com.feilong.lib.javassist.CtMethod, com.feilong.lib.javassist.CtMethod$ConstParameter) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.CtMethod$ConstParameter`

```java
public class com.feilong.lib.javassist.CtMethod$ConstParameter {
  public static com.feilong.lib.javassist.CtMethod$ConstParameter integer(int);
  public static com.feilong.lib.javassist.CtMethod$ConstParameter integer(long);
  public static com.feilong.lib.javassist.CtMethod$ConstParameter string(java.lang.String);
}
```

## `com.feilong.lib.javassist.CtNewConstructor`

```java
public class com.feilong.lib.javassist.CtNewConstructor {
  public com.feilong.lib.javassist.CtNewConstructor();
  public static com.feilong.lib.javassist.CtConstructor make(java.lang.String, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtConstructor make(com.feilong.lib.javassist.CtClass[], com.feilong.lib.javassist.CtClass[], java.lang.String, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtConstructor copy(com.feilong.lib.javassist.CtConstructor, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.ClassMap) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtConstructor defaultConstructor(com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtConstructor skeleton(com.feilong.lib.javassist.CtClass[], com.feilong.lib.javassist.CtClass[], com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtConstructor make(com.feilong.lib.javassist.CtClass[], com.feilong.lib.javassist.CtClass[], com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtConstructor make(com.feilong.lib.javassist.CtClass[], com.feilong.lib.javassist.CtClass[], int, com.feilong.lib.javassist.CtMethod, com.feilong.lib.javassist.CtMethod$ConstParameter, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.CtNewMethod`

```java
public class com.feilong.lib.javassist.CtNewMethod {
  public com.feilong.lib.javassist.CtNewMethod();
  public static com.feilong.lib.javassist.CtMethod make(java.lang.String, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtMethod make(java.lang.String, com.feilong.lib.javassist.CtClass, java.lang.String, java.lang.String) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtMethod make(com.feilong.lib.javassist.CtClass, java.lang.String, com.feilong.lib.javassist.CtClass[], com.feilong.lib.javassist.CtClass[], java.lang.String, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtMethod make(int, com.feilong.lib.javassist.CtClass, java.lang.String, com.feilong.lib.javassist.CtClass[], com.feilong.lib.javassist.CtClass[], java.lang.String, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtMethod copy(com.feilong.lib.javassist.CtMethod, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.ClassMap) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtMethod copy(com.feilong.lib.javassist.CtMethod, java.lang.String, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.ClassMap) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtMethod abstractMethod(com.feilong.lib.javassist.CtClass, java.lang.String, com.feilong.lib.javassist.CtClass[], com.feilong.lib.javassist.CtClass[], com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.NotFoundException;
  public static com.feilong.lib.javassist.CtMethod getter(java.lang.String, com.feilong.lib.javassist.CtField) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtMethod setter(java.lang.String, com.feilong.lib.javassist.CtField) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtMethod delegator(com.feilong.lib.javassist.CtMethod, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
  public static com.feilong.lib.javassist.CtMethod wrapped(com.feilong.lib.javassist.CtClass, java.lang.String, com.feilong.lib.javassist.CtClass[], com.feilong.lib.javassist.CtClass[], com.feilong.lib.javassist.CtMethod, com.feilong.lib.javassist.CtMethod$ConstParameter, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.CtPrimitiveType`

```java
public final class com.feilong.lib.javassist.CtPrimitiveType extends com.feilong.lib.javassist.CtClass {
  public boolean isPrimitive();
  public int getModifiers();
  public char getDescriptor();
  public java.lang.String getWrapperName();
  public java.lang.String getGetMethodName();
  public java.lang.String getGetMethodDescriptor();
  public int getReturnOp();
  public int getArrayType();
  public int getDataSize();
}
```

## `com.feilong.lib.javassist.Loader`

```java
public class com.feilong.lib.javassist.Loader extends java.lang.ClassLoader {
  public com.feilong.lib.javassist.Loader();
  public com.feilong.lib.javassist.Loader(com.feilong.lib.javassist.ClassPool);
  public com.feilong.lib.javassist.Loader(java.lang.ClassLoader, com.feilong.lib.javassist.ClassPool);
  public void delegateLoadingOf(java.lang.String);
  public void setDomain(java.security.ProtectionDomain);
  public void setClassPool(com.feilong.lib.javassist.ClassPool);
  public void addTranslator(com.feilong.lib.javassist.ClassPool, com.feilong.lib.javassist.Translator) throws com.feilong.lib.javassist.NotFoundException, com.feilong.lib.javassist.CannotCompileException;
  public void run(java.lang.String[]) throws java.lang.Throwable;
  public void run(java.lang.String, java.lang.String[]) throws java.lang.Throwable;
}
```

## `com.feilong.lib.javassist.Loader$Simple`

```java
public class com.feilong.lib.javassist.Loader$Simple extends java.lang.ClassLoader {
  public com.feilong.lib.javassist.Loader$Simple();
  public com.feilong.lib.javassist.Loader$Simple(java.lang.ClassLoader);
  public java.lang.Class<?> invokeDefineClass(com.feilong.lib.javassist.CtClass) throws java.io.IOException, com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.LoaderClassPath`

```java
public class com.feilong.lib.javassist.LoaderClassPath implements com.feilong.lib.javassist.ClassPath {
  public com.feilong.lib.javassist.LoaderClassPath(java.lang.ClassLoader);
  public java.lang.String toString();
  public java.io.InputStream openClassfile(java.lang.String) throws com.feilong.lib.javassist.NotFoundException;
  public java.net.URL find(java.lang.String);
}
```

## `com.feilong.lib.javassist.Modifier`

```java
public class com.feilong.lib.javassist.Modifier {
  public com.feilong.lib.javassist.Modifier();
  public static boolean isPublic(int);
  public static boolean isPrivate(int);
  public static boolean isProtected(int);
  public static boolean isPackage(int);
  public static boolean isStatic(int);
  public static boolean isFinal(int);
  public static boolean isSynchronized(int);
  public static boolean isVolatile(int);
  public static boolean isTransient(int);
  public static boolean isNative(int);
  public static boolean isInterface(int);
  public static boolean isAnnotation(int);
  public static boolean isEnum(int);
  public static boolean isAbstract(int);
  public static boolean isStrict(int);
  public static boolean isVarArgs(int);
  public static int setPublic(int);
  public static int setProtected(int);
  public static int setPrivate(int);
  public static int setPackage(int);
  public static int clear(int, int);
  public static java.lang.String toString(int);
}
```

## `com.feilong.lib.javassist.NotFoundException`

```java
public class com.feilong.lib.javassist.NotFoundException extends java.lang.Exception {
  public com.feilong.lib.javassist.NotFoundException(java.lang.String);
}
```

## `com.feilong.lib.javassist.Translator`

```java
public interface com.feilong.lib.javassist.Translator {
  public abstract void start(com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.NotFoundException, com.feilong.lib.javassist.CannotCompileException;
  public abstract void onLoad(com.feilong.lib.javassist.ClassPool, java.lang.String) throws com.feilong.lib.javassist.NotFoundException, com.feilong.lib.javassist.CannotCompileException;
}
```

## `com.feilong.lib.javassist.URLClassPath`

```java
public class com.feilong.lib.javassist.URLClassPath implements com.feilong.lib.javassist.ClassPath {
  public com.feilong.lib.javassist.URLClassPath(java.lang.String, int, java.lang.String, java.lang.String);
  public java.lang.String toString();
  public java.io.InputStream openClassfile(java.lang.String);
  public java.net.URL find(java.lang.String);
  public static byte[] fetchClass(java.lang.String, int, java.lang.String, java.lang.String) throws java.io.IOException;
}
```
