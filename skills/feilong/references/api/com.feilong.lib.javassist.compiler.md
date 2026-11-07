# com.feilong.lib.javassist.compiler

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.javassist.compiler.AccessorMaker`

```java
public class com.feilong.lib.javassist.compiler.AccessorMaker {
  public com.feilong.lib.javassist.compiler.AccessorMaker(com.feilong.lib.javassist.CtClass);
  public java.lang.String getConstructor(com.feilong.lib.javassist.CtClass, java.lang.String, com.feilong.lib.javassist.bytecode.MethodInfo) throws com.feilong.lib.javassist.compiler.CompileError;
  public java.lang.String getMethodAccessor(java.lang.String, java.lang.String, java.lang.String, com.feilong.lib.javassist.bytecode.MethodInfo) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.bytecode.MethodInfo getFieldGetter(com.feilong.lib.javassist.bytecode.FieldInfo, boolean) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.bytecode.MethodInfo getFieldSetter(com.feilong.lib.javassist.bytecode.FieldInfo, boolean) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.CodeGen`

```java
public abstract class com.feilong.lib.javassist.compiler.CodeGen extends com.feilong.lib.javassist.compiler.ast.Visitor implements com.feilong.lib.javassist.bytecode.Opcode,com.feilong.lib.javassist.compiler.TokenId {
  public com.feilong.lib.javassist.compiler.CodeGen(com.feilong.lib.javassist.bytecode.Bytecode);
  public void setTypeChecker(com.feilong.lib.javassist.compiler.TypeChecker);
  public static boolean is2word(int, int);
  public int getMaxLocals();
  public void setMaxLocals(int);
  public void compileExpr(com.feilong.lib.javassist.compiler.ast.ASTree) throws com.feilong.lib.javassist.compiler.CompileError;
  public boolean compileBooleanExpr(boolean, com.feilong.lib.javassist.compiler.ast.ASTree) throws com.feilong.lib.javassist.compiler.CompileError;
  public void doTypeCheck(com.feilong.lib.javassist.compiler.ast.ASTree) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atASTList(com.feilong.lib.javassist.compiler.ast.ASTList) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atPair(com.feilong.lib.javassist.compiler.ast.Pair) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atSymbol(com.feilong.lib.javassist.compiler.ast.Symbol) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atFieldDecl(com.feilong.lib.javassist.compiler.ast.FieldDecl) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atMethodDecl(com.feilong.lib.javassist.compiler.ast.MethodDecl) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atMethodBody(com.feilong.lib.javassist.compiler.ast.Stmnt, boolean, boolean) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atStmnt(com.feilong.lib.javassist.compiler.ast.Stmnt) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atDeclarator(com.feilong.lib.javassist.compiler.ast.Declarator) throws com.feilong.lib.javassist.compiler.CompileError;
  public abstract void atNewExpr(com.feilong.lib.javassist.compiler.ast.NewExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public abstract void atArrayInit(com.feilong.lib.javassist.compiler.ast.ArrayInit) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atAssignExpr(com.feilong.lib.javassist.compiler.ast.AssignExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atCondExpr(com.feilong.lib.javassist.compiler.ast.CondExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atBinExpr(com.feilong.lib.javassist.compiler.ast.BinExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atCastExpr(com.feilong.lib.javassist.compiler.ast.CastExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atInstanceOfExpr(com.feilong.lib.javassist.compiler.ast.InstanceOfExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atExpr(com.feilong.lib.javassist.compiler.ast.Expr) throws com.feilong.lib.javassist.compiler.CompileError;
  public abstract void atCallExpr(com.feilong.lib.javassist.compiler.ast.CallExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atClassObject(com.feilong.lib.javassist.compiler.ast.Expr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atArrayRead(com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atArrayPlusPlus(int, boolean, com.feilong.lib.javassist.compiler.ast.Expr, boolean) throws com.feilong.lib.javassist.compiler.CompileError;
  public abstract void atMember(com.feilong.lib.javassist.compiler.ast.Member) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atVariable(com.feilong.lib.javassist.compiler.ast.Variable) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atKeyword(com.feilong.lib.javassist.compiler.ast.Keyword) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atStringL(com.feilong.lib.javassist.compiler.ast.StringL) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atIntConst(com.feilong.lib.javassist.compiler.ast.IntConst) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atDoubleConst(com.feilong.lib.javassist.compiler.ast.DoubleConst) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.CompileError`

```java
public class com.feilong.lib.javassist.compiler.CompileError extends java.lang.Exception {
  public com.feilong.lib.javassist.compiler.CompileError(java.lang.String, com.feilong.lib.javassist.compiler.Lex);
  public com.feilong.lib.javassist.compiler.CompileError(java.lang.String);
  public com.feilong.lib.javassist.compiler.CompileError(com.feilong.lib.javassist.CannotCompileException);
  public com.feilong.lib.javassist.compiler.CompileError(com.feilong.lib.javassist.NotFoundException);
  public com.feilong.lib.javassist.compiler.Lex getLex();
  public java.lang.String getMessage();
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.compiler.Javac`

```java
public class com.feilong.lib.javassist.compiler.Javac {
  public com.feilong.lib.javassist.compiler.Javac(com.feilong.lib.javassist.CtClass);
  public com.feilong.lib.javassist.compiler.Javac(com.feilong.lib.javassist.bytecode.Bytecode, com.feilong.lib.javassist.CtClass);
  public com.feilong.lib.javassist.bytecode.Bytecode getBytecode();
  public com.feilong.lib.javassist.CtMember compile(java.lang.String) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.bytecode.Bytecode compileBody(com.feilong.lib.javassist.CtBehavior, java.lang.String) throws com.feilong.lib.javassist.compiler.CompileError;
  public boolean recordLocalVariables(com.feilong.lib.javassist.bytecode.CodeAttribute, int) throws com.feilong.lib.javassist.compiler.CompileError;
  public boolean recordParamNames(com.feilong.lib.javassist.bytecode.CodeAttribute, int) throws com.feilong.lib.javassist.compiler.CompileError;
  public int recordParams(com.feilong.lib.javassist.CtClass[], boolean) throws com.feilong.lib.javassist.compiler.CompileError;
  public int recordParams(java.lang.String, com.feilong.lib.javassist.CtClass[], boolean, int, boolean) throws com.feilong.lib.javassist.compiler.CompileError;
  public void setMaxLocals(int);
  public int recordReturnType(com.feilong.lib.javassist.CtClass, boolean) throws com.feilong.lib.javassist.compiler.CompileError;
  public void recordType(com.feilong.lib.javassist.CtClass);
  public int recordVariable(com.feilong.lib.javassist.CtClass, java.lang.String) throws com.feilong.lib.javassist.compiler.CompileError;
  public void recordProceed(java.lang.String, java.lang.String) throws com.feilong.lib.javassist.compiler.CompileError;
  public void recordStaticProceed(java.lang.String, java.lang.String) throws com.feilong.lib.javassist.compiler.CompileError;
  public void recordSpecialProceed(java.lang.String, java.lang.String, java.lang.String, java.lang.String, int) throws com.feilong.lib.javassist.compiler.CompileError;
  public void recordProceed(com.feilong.lib.javassist.compiler.ProceedHandler);
  public void compileStmnt(java.lang.String) throws com.feilong.lib.javassist.compiler.CompileError;
  public void compileExpr(java.lang.String) throws com.feilong.lib.javassist.compiler.CompileError;
  public static com.feilong.lib.javassist.compiler.ast.ASTree parseExpr(java.lang.String, com.feilong.lib.javassist.compiler.SymbolTable) throws com.feilong.lib.javassist.compiler.CompileError;
  public void compileExpr(com.feilong.lib.javassist.compiler.ast.ASTree) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.JvstCodeGen`

```java
public class com.feilong.lib.javassist.compiler.JvstCodeGen extends com.feilong.lib.javassist.compiler.MemberCodeGen {
  public com.feilong.lib.javassist.compiler.JvstCodeGen(com.feilong.lib.javassist.bytecode.Bytecode, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.ClassPool);
  public void setProceedHandler(com.feilong.lib.javassist.compiler.ProceedHandler, java.lang.String);
  public void addNullIfVoid();
  public void atMember(com.feilong.lib.javassist.compiler.ast.Member) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atCastExpr(com.feilong.lib.javassist.compiler.ast.CastExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atCallExpr(com.feilong.lib.javassist.compiler.ast.CallExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public boolean isParamListName(com.feilong.lib.javassist.compiler.ast.ASTList);
  public int getMethodArgsLength(com.feilong.lib.javassist.compiler.ast.ASTList);
  public void atMethodArgs(com.feilong.lib.javassist.compiler.ast.ASTList, int[], int[], java.lang.String[]) throws com.feilong.lib.javassist.compiler.CompileError;
  public int recordReturnType(com.feilong.lib.javassist.CtClass, java.lang.String, java.lang.String, com.feilong.lib.javassist.compiler.SymbolTable) throws com.feilong.lib.javassist.compiler.CompileError;
  public void recordType(com.feilong.lib.javassist.CtClass);
  public int recordParams(com.feilong.lib.javassist.CtClass[], boolean, java.lang.String, java.lang.String, java.lang.String, com.feilong.lib.javassist.compiler.SymbolTable) throws com.feilong.lib.javassist.compiler.CompileError;
  public int recordParams(com.feilong.lib.javassist.CtClass[], boolean, java.lang.String, java.lang.String, java.lang.String, boolean, int, java.lang.String, com.feilong.lib.javassist.compiler.SymbolTable) throws com.feilong.lib.javassist.compiler.CompileError;
  public int recordVariable(com.feilong.lib.javassist.CtClass, java.lang.String, com.feilong.lib.javassist.compiler.SymbolTable) throws com.feilong.lib.javassist.compiler.CompileError;
  public void recordVariable(java.lang.String, java.lang.String, int, com.feilong.lib.javassist.compiler.SymbolTable) throws com.feilong.lib.javassist.compiler.CompileError;
  public static int compileParameterList(com.feilong.lib.javassist.bytecode.Bytecode, com.feilong.lib.javassist.CtClass[], int);
  public void setType(com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.compiler.CompileError;
  public void doNumCast(com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.JvstTypeChecker`

```java
public class com.feilong.lib.javassist.compiler.JvstTypeChecker extends com.feilong.lib.javassist.compiler.TypeChecker {
  public com.feilong.lib.javassist.compiler.JvstTypeChecker(com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.ClassPool, com.feilong.lib.javassist.compiler.JvstCodeGen);
  public void addNullIfVoid();
  public void atMember(com.feilong.lib.javassist.compiler.ast.Member) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atCastExpr(com.feilong.lib.javassist.compiler.ast.CastExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atCallExpr(com.feilong.lib.javassist.compiler.ast.CallExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public boolean isParamListName(com.feilong.lib.javassist.compiler.ast.ASTList);
  public int getMethodArgsLength(com.feilong.lib.javassist.compiler.ast.ASTList);
  public void atMethodArgs(com.feilong.lib.javassist.compiler.ast.ASTList, int[], int[], java.lang.String[]) throws com.feilong.lib.javassist.compiler.CompileError;
  public void setType(com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.KeywordTable`

```java
public final class com.feilong.lib.javassist.compiler.KeywordTable extends java.util.HashMap<java.lang.String, java.lang.Integer> {
  public com.feilong.lib.javassist.compiler.KeywordTable();
  public int lookup(java.lang.String);
  public void append(java.lang.String, int);
}
```

## `com.feilong.lib.javassist.compiler.Lex`

```java
public class com.feilong.lib.javassist.compiler.Lex implements com.feilong.lib.javassist.compiler.TokenId {
  public com.feilong.lib.javassist.compiler.Lex(java.lang.String);
  public int get();
  public int lookAhead();
  public int lookAhead(int);
  public java.lang.String getString();
  public long getLong();
  public double getDouble();
  public java.lang.String getTextAround();
}
```

## `com.feilong.lib.javassist.compiler.MemberCodeGen`

```java
public class com.feilong.lib.javassist.compiler.MemberCodeGen extends com.feilong.lib.javassist.compiler.CodeGen {
  public com.feilong.lib.javassist.compiler.MemberCodeGen(com.feilong.lib.javassist.bytecode.Bytecode, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.ClassPool);
  public int getMajorVersion();
  public void setThisMethod(com.feilong.lib.javassist.CtMethod);
  public com.feilong.lib.javassist.CtClass getThisClass();
  public void atNewExpr(com.feilong.lib.javassist.compiler.ast.NewExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atNewArrayExpr(com.feilong.lib.javassist.compiler.ast.NewExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atArrayInit(com.feilong.lib.javassist.compiler.ast.ArrayInit) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atCallExpr(com.feilong.lib.javassist.compiler.ast.CallExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atMethodCallCore(com.feilong.lib.javassist.CtClass, java.lang.String, com.feilong.lib.javassist.compiler.ast.ASTList, boolean, boolean, int, com.feilong.lib.javassist.compiler.MemberResolver$Method) throws com.feilong.lib.javassist.compiler.CompileError;
  public int getMethodArgsLength(com.feilong.lib.javassist.compiler.ast.ASTList);
  public void atMethodArgs(com.feilong.lib.javassist.compiler.ast.ASTList, int[], int[], java.lang.String[]) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atMember(com.feilong.lib.javassist.compiler.ast.Member) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.CtClass[] makeParamList(com.feilong.lib.javassist.compiler.ast.MethodDecl) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.CtClass[] makeThrowsList(com.feilong.lib.javassist.compiler.ast.MethodDecl) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.MemberResolver`

```java
public class com.feilong.lib.javassist.compiler.MemberResolver implements com.feilong.lib.javassist.compiler.TokenId {
  public com.feilong.lib.javassist.compiler.MemberResolver(com.feilong.lib.javassist.ClassPool);
  public com.feilong.lib.javassist.ClassPool getClassPool();
  public com.feilong.lib.javassist.compiler.MemberResolver$Method lookupMethod(com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.bytecode.MethodInfo, java.lang.String, int[], int[], java.lang.String[]) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.CtField lookupFieldByJvmName2(java.lang.String, com.feilong.lib.javassist.compiler.ast.Symbol, com.feilong.lib.javassist.compiler.ast.ASTree) throws com.feilong.lib.javassist.compiler.NoFieldException;
  public com.feilong.lib.javassist.CtField lookupFieldByJvmName(java.lang.String, com.feilong.lib.javassist.compiler.ast.Symbol) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.CtField lookupField(java.lang.String, com.feilong.lib.javassist.compiler.ast.Symbol) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.CtClass lookupClassByName(com.feilong.lib.javassist.compiler.ast.ASTList) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.CtClass lookupClassByJvmName(java.lang.String) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.CtClass lookupClass(com.feilong.lib.javassist.compiler.ast.Declarator) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.CtClass lookupClass(int, int, java.lang.String) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.CtClass lookupClass(java.lang.String, boolean) throws com.feilong.lib.javassist.compiler.CompileError;
  public static int getInvalidMapSize();
  public java.lang.String resolveClassName(com.feilong.lib.javassist.compiler.ast.ASTList) throws com.feilong.lib.javassist.compiler.CompileError;
  public java.lang.String resolveJvmClassName(java.lang.String) throws com.feilong.lib.javassist.compiler.CompileError;
  public static com.feilong.lib.javassist.CtClass getSuperclass(com.feilong.lib.javassist.CtClass) throws com.feilong.lib.javassist.compiler.CompileError;
  public static com.feilong.lib.javassist.CtClass getSuperInterface(com.feilong.lib.javassist.CtClass, java.lang.String) throws com.feilong.lib.javassist.compiler.CompileError;
  public static java.lang.String javaToJvmName(java.lang.String);
  public static java.lang.String jvmToJavaName(java.lang.String);
  public static int descToType(char) throws com.feilong.lib.javassist.compiler.CompileError;
  public static int getModifiers(com.feilong.lib.javassist.compiler.ast.ASTList);
}
```

## `com.feilong.lib.javassist.compiler.MemberResolver$Method`

```java
public class com.feilong.lib.javassist.compiler.MemberResolver$Method {
  public com.feilong.lib.javassist.compiler.MemberResolver$Method(com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.bytecode.MethodInfo, int);
  public boolean isStatic();
}
```

## `com.feilong.lib.javassist.compiler.NoFieldException`

```java
public class com.feilong.lib.javassist.compiler.NoFieldException extends com.feilong.lib.javassist.compiler.CompileError {
  public com.feilong.lib.javassist.compiler.NoFieldException(java.lang.String, com.feilong.lib.javassist.compiler.ast.ASTree);
  public java.lang.String getField();
  public com.feilong.lib.javassist.compiler.ast.ASTree getExpr();
}
```

## `com.feilong.lib.javassist.compiler.Parser`

```java
public final class com.feilong.lib.javassist.compiler.Parser implements com.feilong.lib.javassist.compiler.TokenId {
  public com.feilong.lib.javassist.compiler.Parser(com.feilong.lib.javassist.compiler.Lex);
  public boolean hasMore();
  public com.feilong.lib.javassist.compiler.ast.ASTList parseMember(com.feilong.lib.javassist.compiler.SymbolTable) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.compiler.ast.ASTList parseMember1(com.feilong.lib.javassist.compiler.SymbolTable) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.compiler.ast.MethodDecl parseMethod2(com.feilong.lib.javassist.compiler.SymbolTable, com.feilong.lib.javassist.compiler.ast.MethodDecl) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.compiler.ast.Stmnt parseStatement(com.feilong.lib.javassist.compiler.SymbolTable) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.compiler.ast.ASTree parseExpression(com.feilong.lib.javassist.compiler.SymbolTable) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ProceedHandler`

```java
public interface com.feilong.lib.javassist.compiler.ProceedHandler {
  public abstract void doit(com.feilong.lib.javassist.compiler.JvstCodeGen, com.feilong.lib.javassist.bytecode.Bytecode, com.feilong.lib.javassist.compiler.ast.ASTList) throws com.feilong.lib.javassist.compiler.CompileError;
  public abstract void setReturnType(com.feilong.lib.javassist.compiler.JvstTypeChecker, com.feilong.lib.javassist.compiler.ast.ASTList) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.SymbolTable`

```java
public final class com.feilong.lib.javassist.compiler.SymbolTable extends java.util.HashMap<java.lang.String, com.feilong.lib.javassist.compiler.ast.Declarator> {
  public com.feilong.lib.javassist.compiler.SymbolTable();
  public com.feilong.lib.javassist.compiler.SymbolTable(com.feilong.lib.javassist.compiler.SymbolTable);
  public com.feilong.lib.javassist.compiler.SymbolTable getParent();
  public com.feilong.lib.javassist.compiler.ast.Declarator lookup(java.lang.String);
  public void append(java.lang.String, com.feilong.lib.javassist.compiler.ast.Declarator);
}
```

## `com.feilong.lib.javassist.compiler.SyntaxError`

```java
public class com.feilong.lib.javassist.compiler.SyntaxError extends com.feilong.lib.javassist.compiler.CompileError {
  public com.feilong.lib.javassist.compiler.SyntaxError(com.feilong.lib.javassist.compiler.Lex);
}
```

## `com.feilong.lib.javassist.compiler.TypeChecker`

```java
public class com.feilong.lib.javassist.compiler.TypeChecker extends com.feilong.lib.javassist.compiler.ast.Visitor implements com.feilong.lib.javassist.bytecode.Opcode,com.feilong.lib.javassist.compiler.TokenId {
  public com.feilong.lib.javassist.compiler.TypeChecker(com.feilong.lib.javassist.CtClass, com.feilong.lib.javassist.ClassPool);
  public void setThisMethod(com.feilong.lib.javassist.bytecode.MethodInfo);
  public void atNewExpr(com.feilong.lib.javassist.compiler.ast.NewExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atNewArrayExpr(com.feilong.lib.javassist.compiler.ast.NewExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atArrayInit(com.feilong.lib.javassist.compiler.ast.ArrayInit) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atAssignExpr(com.feilong.lib.javassist.compiler.ast.AssignExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atCondExpr(com.feilong.lib.javassist.compiler.ast.CondExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atBinExpr(com.feilong.lib.javassist.compiler.ast.BinExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public static com.feilong.lib.javassist.compiler.ast.ASTree getConstantFieldValue(com.feilong.lib.javassist.CtField);
  public void atCastExpr(com.feilong.lib.javassist.compiler.ast.CastExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atInstanceOfExpr(com.feilong.lib.javassist.compiler.ast.InstanceOfExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atExpr(com.feilong.lib.javassist.compiler.ast.Expr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atCallExpr(com.feilong.lib.javassist.compiler.ast.CallExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.compiler.MemberResolver$Method atMethodCallCore(com.feilong.lib.javassist.CtClass, java.lang.String, com.feilong.lib.javassist.compiler.ast.ASTList) throws com.feilong.lib.javassist.compiler.CompileError;
  public int getMethodArgsLength(com.feilong.lib.javassist.compiler.ast.ASTList);
  public void atMethodArgs(com.feilong.lib.javassist.compiler.ast.ASTList, int[], int[], java.lang.String[]) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atClassObject(com.feilong.lib.javassist.compiler.ast.Expr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atArrayLength(com.feilong.lib.javassist.compiler.ast.Expr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atArrayRead(com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atMember(com.feilong.lib.javassist.compiler.ast.Member) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atVariable(com.feilong.lib.javassist.compiler.ast.Variable) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atKeyword(com.feilong.lib.javassist.compiler.ast.Keyword) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atStringL(com.feilong.lib.javassist.compiler.ast.StringL) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atIntConst(com.feilong.lib.javassist.compiler.ast.IntConst) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atDoubleConst(com.feilong.lib.javassist.compiler.ast.DoubleConst) throws com.feilong.lib.javassist.compiler.CompileError;
}
```
