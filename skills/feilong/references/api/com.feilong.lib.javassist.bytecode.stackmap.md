# com.feilong.lib.javassist.bytecode.stackmap

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.javassist.bytecode.stackmap.BasicBlock`

```java
public class com.feilong.lib.javassist.bytecode.stackmap.BasicBlock {
  public static com.feilong.lib.javassist.bytecode.stackmap.BasicBlock find(com.feilong.lib.javassist.bytecode.stackmap.BasicBlock[], int) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.BasicBlock$Maker`

```java
public class com.feilong.lib.javassist.bytecode.stackmap.BasicBlock$Maker {
  public com.feilong.lib.javassist.bytecode.stackmap.BasicBlock$Maker();
  public com.feilong.lib.javassist.bytecode.stackmap.BasicBlock[] make(com.feilong.lib.javassist.bytecode.MethodInfo) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public com.feilong.lib.javassist.bytecode.stackmap.BasicBlock[] make(com.feilong.lib.javassist.bytecode.CodeIterator, int, int, com.feilong.lib.javassist.bytecode.ExceptionTable) throws com.feilong.lib.javassist.bytecode.BadBytecode;
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.MapMaker`

```java
public class com.feilong.lib.javassist.bytecode.stackmap.MapMaker extends com.feilong.lib.javassist.bytecode.stackmap.Tracer {
  public static com.feilong.lib.javassist.bytecode.StackMapTable make(com.feilong.lib.javassist.ClassPool, com.feilong.lib.javassist.bytecode.MethodInfo) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public static com.feilong.lib.javassist.bytecode.StackMap make2(com.feilong.lib.javassist.ClassPool, com.feilong.lib.javassist.bytecode.MethodInfo) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public com.feilong.lib.javassist.bytecode.stackmap.MapMaker(com.feilong.lib.javassist.ClassPool, com.feilong.lib.javassist.bytecode.MethodInfo, com.feilong.lib.javassist.bytecode.CodeAttribute);
  public com.feilong.lib.javassist.bytecode.StackMapTable toStackMap(com.feilong.lib.javassist.bytecode.stackmap.TypedBlock[]);
  public com.feilong.lib.javassist.bytecode.StackMap toStackMap2(com.feilong.lib.javassist.bytecode.ConstPool, com.feilong.lib.javassist.bytecode.stackmap.TypedBlock[]);
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.Tracer`

```java
public abstract class com.feilong.lib.javassist.bytecode.stackmap.Tracer implements com.feilong.lib.javassist.bytecode.stackmap.TypeTag {
  public com.feilong.lib.javassist.bytecode.stackmap.Tracer(com.feilong.lib.javassist.ClassPool, com.feilong.lib.javassist.bytecode.ConstPool, int, int, java.lang.String);
  public com.feilong.lib.javassist.bytecode.stackmap.Tracer(com.feilong.lib.javassist.bytecode.stackmap.Tracer);
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.TypeData`

```java
public abstract class com.feilong.lib.javassist.bytecode.stackmap.TypeData {
  public static com.feilong.lib.javassist.bytecode.stackmap.TypeData[] make(int);
  public abstract int getTypeTag();
  public abstract int getTypeData(com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData join();
  public abstract com.feilong.lib.javassist.bytecode.stackmap.TypeData$BasicType isBasicType();
  public abstract boolean is2WordType();
  public boolean isNullType();
  public boolean isUninit();
  public abstract boolean eq(com.feilong.lib.javassist.bytecode.stackmap.TypeData);
  public abstract java.lang.String getName();
  public abstract void setType(java.lang.String, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public abstract com.feilong.lib.javassist.bytecode.stackmap.TypeData getArrayType(int) throws com.feilong.lib.javassist.NotFoundException;
  public int dfs(java.util.List<com.feilong.lib.javassist.bytecode.stackmap.TypeData>, int, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.NotFoundException;
  public void constructorCalled(int);
  public java.lang.String toString();
  public static com.feilong.lib.javassist.CtClass commonSuperClassEx(com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.NotFoundException;
  public static com.feilong.lib.javassist.CtClass commonSuperClass(com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.NotFoundException;
  public static void aastore(com.feilong.lib.javassist.bytecode.stackmap.TypeData, com.feilong.lib.javassist.bytecode.stackmap.TypeData, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.bytecode.BadBytecode;
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.TypeData$AbsTypeVar`

```java
public abstract class com.feilong.lib.javassist.bytecode.stackmap.TypeData$AbsTypeVar extends com.feilong.lib.javassist.bytecode.stackmap.TypeData {
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$AbsTypeVar();
  public abstract void merge(com.feilong.lib.javassist.bytecode.stackmap.TypeData);
  public int getTypeTag();
  public int getTypeData(com.feilong.lib.javassist.bytecode.ConstPool);
  public boolean eq(com.feilong.lib.javassist.bytecode.stackmap.TypeData);
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.TypeData$ArrayElement`

```java
public class com.feilong.lib.javassist.bytecode.stackmap.TypeData$ArrayElement extends com.feilong.lib.javassist.bytecode.stackmap.TypeData$AbsTypeVar {
  public static com.feilong.lib.javassist.bytecode.stackmap.TypeData make(com.feilong.lib.javassist.bytecode.stackmap.TypeData) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void merge(com.feilong.lib.javassist.bytecode.stackmap.TypeData);
  public java.lang.String getName();
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$AbsTypeVar arrayType();
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$BasicType isBasicType();
  public boolean is2WordType();
  public void setType(java.lang.String, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData getArrayType(int) throws com.feilong.lib.javassist.NotFoundException;
  public int dfs(java.util.List<com.feilong.lib.javassist.bytecode.stackmap.TypeData>, int, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.NotFoundException;
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.TypeData$ArrayType`

```java
public class com.feilong.lib.javassist.bytecode.stackmap.TypeData$ArrayType extends com.feilong.lib.javassist.bytecode.stackmap.TypeData$AbsTypeVar {
  public void merge(com.feilong.lib.javassist.bytecode.stackmap.TypeData);
  public java.lang.String getName();
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$AbsTypeVar elementType();
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$BasicType isBasicType();
  public boolean is2WordType();
  public static java.lang.String typeName(java.lang.String);
  public void setType(java.lang.String, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData getArrayType(int) throws com.feilong.lib.javassist.NotFoundException;
  public int dfs(java.util.List<com.feilong.lib.javassist.bytecode.stackmap.TypeData>, int, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.NotFoundException;
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.TypeData$BasicType`

```java
public class com.feilong.lib.javassist.bytecode.stackmap.TypeData$BasicType extends com.feilong.lib.javassist.bytecode.stackmap.TypeData {
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$BasicType(java.lang.String, int, char);
  public int getTypeTag();
  public int getTypeData(com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData join();
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$BasicType isBasicType();
  public boolean is2WordType();
  public boolean eq(com.feilong.lib.javassist.bytecode.stackmap.TypeData);
  public java.lang.String getName();
  public char getDecodedName();
  public void setType(java.lang.String, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData getArrayType(int) throws com.feilong.lib.javassist.NotFoundException;
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.TypeData$ClassName`

```java
public class com.feilong.lib.javassist.bytecode.stackmap.TypeData$ClassName extends com.feilong.lib.javassist.bytecode.stackmap.TypeData {
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$ClassName(java.lang.String);
  public java.lang.String getName();
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$BasicType isBasicType();
  public boolean is2WordType();
  public int getTypeTag();
  public int getTypeData(com.feilong.lib.javassist.bytecode.ConstPool);
  public boolean eq(com.feilong.lib.javassist.bytecode.stackmap.TypeData);
  public void setType(java.lang.String, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData getArrayType(int) throws com.feilong.lib.javassist.NotFoundException;
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.TypeData$NullType`

```java
public class com.feilong.lib.javassist.bytecode.stackmap.TypeData$NullType extends com.feilong.lib.javassist.bytecode.stackmap.TypeData$ClassName {
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$NullType();
  public int getTypeTag();
  public boolean isNullType();
  public int getTypeData(com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData getArrayType(int);
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.TypeData$TypeVar`

```java
public class com.feilong.lib.javassist.bytecode.stackmap.TypeData$TypeVar extends com.feilong.lib.javassist.bytecode.stackmap.TypeData$AbsTypeVar {
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$TypeVar(com.feilong.lib.javassist.bytecode.stackmap.TypeData);
  public java.lang.String getName();
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$BasicType isBasicType();
  public boolean is2WordType();
  public boolean isNullType();
  public boolean isUninit();
  public void merge(com.feilong.lib.javassist.bytecode.stackmap.TypeData);
  public int getTypeTag();
  public int getTypeData(com.feilong.lib.javassist.bytecode.ConstPool);
  public void setType(java.lang.String, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData getArrayType(int) throws com.feilong.lib.javassist.NotFoundException;
  public int dfs(java.util.List<com.feilong.lib.javassist.bytecode.stackmap.TypeData>, int, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.NotFoundException;
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.TypeData$UninitData`

```java
public class com.feilong.lib.javassist.bytecode.stackmap.TypeData$UninitData extends com.feilong.lib.javassist.bytecode.stackmap.TypeData$ClassName {
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$UninitData copy();
  public int getTypeTag();
  public int getTypeData(com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData join();
  public boolean isUninit();
  public boolean eq(com.feilong.lib.javassist.bytecode.stackmap.TypeData);
  public int offset();
  public void constructorCalled(int);
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.TypeData$UninitThis`

```java
public class com.feilong.lib.javassist.bytecode.stackmap.TypeData$UninitThis extends com.feilong.lib.javassist.bytecode.stackmap.TypeData$UninitData {
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$UninitData copy();
  public int getTypeTag();
  public int getTypeData(com.feilong.lib.javassist.bytecode.ConstPool);
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.TypeData$UninitTypeVar`

```java
public class com.feilong.lib.javassist.bytecode.stackmap.TypeData$UninitTypeVar extends com.feilong.lib.javassist.bytecode.stackmap.TypeData$AbsTypeVar {
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$UninitTypeVar(com.feilong.lib.javassist.bytecode.stackmap.TypeData$UninitData);
  public int getTypeTag();
  public int getTypeData(com.feilong.lib.javassist.bytecode.ConstPool);
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData$BasicType isBasicType();
  public boolean is2WordType();
  public boolean isUninit();
  public boolean eq(com.feilong.lib.javassist.bytecode.stackmap.TypeData);
  public java.lang.String getName();
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData join();
  public void setType(java.lang.String, com.feilong.lib.javassist.ClassPool) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void merge(com.feilong.lib.javassist.bytecode.stackmap.TypeData);
  public void constructorCalled(int);
  public int offset();
  public com.feilong.lib.javassist.bytecode.stackmap.TypeData getArrayType(int) throws com.feilong.lib.javassist.NotFoundException;
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.TypedBlock`

```java
public class com.feilong.lib.javassist.bytecode.stackmap.TypedBlock extends com.feilong.lib.javassist.bytecode.stackmap.BasicBlock {
  public static com.feilong.lib.javassist.bytecode.stackmap.TypedBlock[] makeBlocks(com.feilong.lib.javassist.bytecode.MethodInfo, com.feilong.lib.javassist.bytecode.CodeAttribute, boolean) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public boolean alreadySet();
  public void setStackMap(int, com.feilong.lib.javassist.bytecode.stackmap.TypeData[], int, com.feilong.lib.javassist.bytecode.stackmap.TypeData[]) throws com.feilong.lib.javassist.bytecode.BadBytecode;
  public void resetNumLocals();
  public static java.lang.String getRetType(java.lang.String);
}
```

## `com.feilong.lib.javassist.bytecode.stackmap.TypedBlock$Maker`

```java
public class com.feilong.lib.javassist.bytecode.stackmap.TypedBlock$Maker extends com.feilong.lib.javassist.bytecode.stackmap.BasicBlock$Maker {
  public com.feilong.lib.javassist.bytecode.stackmap.TypedBlock$Maker();
}
```
