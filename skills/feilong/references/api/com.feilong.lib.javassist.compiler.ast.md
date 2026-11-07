# com.feilong.lib.javassist.compiler.ast

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.javassist.compiler.ast.ASTList`

```java
public class com.feilong.lib.javassist.compiler.ast.ASTList extends com.feilong.lib.javassist.compiler.ast.ASTree {
  public com.feilong.lib.javassist.compiler.ast.ASTList(com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTList);
  public com.feilong.lib.javassist.compiler.ast.ASTList(com.feilong.lib.javassist.compiler.ast.ASTree);
  public static com.feilong.lib.javassist.compiler.ast.ASTList make(com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree);
  public com.feilong.lib.javassist.compiler.ast.ASTree getLeft();
  public com.feilong.lib.javassist.compiler.ast.ASTree getRight();
  public void setLeft(com.feilong.lib.javassist.compiler.ast.ASTree);
  public void setRight(com.feilong.lib.javassist.compiler.ast.ASTree);
  public com.feilong.lib.javassist.compiler.ast.ASTree head();
  public void setHead(com.feilong.lib.javassist.compiler.ast.ASTree);
  public com.feilong.lib.javassist.compiler.ast.ASTList tail();
  public void setTail(com.feilong.lib.javassist.compiler.ast.ASTList);
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
  public java.lang.String toString();
  public int length();
  public static int length(com.feilong.lib.javassist.compiler.ast.ASTList);
  public com.feilong.lib.javassist.compiler.ast.ASTList sublist(int);
  public boolean subst(com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree);
  public static com.feilong.lib.javassist.compiler.ast.ASTList append(com.feilong.lib.javassist.compiler.ast.ASTList, com.feilong.lib.javassist.compiler.ast.ASTree);
  public static com.feilong.lib.javassist.compiler.ast.ASTList concat(com.feilong.lib.javassist.compiler.ast.ASTList, com.feilong.lib.javassist.compiler.ast.ASTList);
}
```

## `com.feilong.lib.javassist.compiler.ast.ASTree`

```java
public abstract class com.feilong.lib.javassist.compiler.ast.ASTree implements java.io.Serializable {
  public com.feilong.lib.javassist.compiler.ast.ASTree();
  public com.feilong.lib.javassist.compiler.ast.ASTree getLeft();
  public com.feilong.lib.javassist.compiler.ast.ASTree getRight();
  public void setLeft(com.feilong.lib.javassist.compiler.ast.ASTree);
  public void setRight(com.feilong.lib.javassist.compiler.ast.ASTree);
  public abstract void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
  public java.lang.String toString();
}
```

## `com.feilong.lib.javassist.compiler.ast.ArrayInit`

```java
public class com.feilong.lib.javassist.compiler.ast.ArrayInit extends com.feilong.lib.javassist.compiler.ast.ASTList {
  public com.feilong.lib.javassist.compiler.ast.ArrayInit(com.feilong.lib.javassist.compiler.ast.ASTree);
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
  public java.lang.String getTag();
}
```

## `com.feilong.lib.javassist.compiler.ast.AssignExpr`

```java
public class com.feilong.lib.javassist.compiler.ast.AssignExpr extends com.feilong.lib.javassist.compiler.ast.Expr {
  public static com.feilong.lib.javassist.compiler.ast.AssignExpr makeAssign(int, com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree);
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ast.BinExpr`

```java
public class com.feilong.lib.javassist.compiler.ast.BinExpr extends com.feilong.lib.javassist.compiler.ast.Expr {
  public static com.feilong.lib.javassist.compiler.ast.BinExpr makeBin(int, com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree);
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ast.CallExpr`

```java
public class com.feilong.lib.javassist.compiler.ast.CallExpr extends com.feilong.lib.javassist.compiler.ast.Expr {
  public void setMethod(com.feilong.lib.javassist.compiler.MemberResolver$Method);
  public com.feilong.lib.javassist.compiler.MemberResolver$Method getMethod();
  public static com.feilong.lib.javassist.compiler.ast.CallExpr makeCall(com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree);
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ast.CastExpr`

```java
public class com.feilong.lib.javassist.compiler.ast.CastExpr extends com.feilong.lib.javassist.compiler.ast.ASTList implements com.feilong.lib.javassist.compiler.TokenId {
  public com.feilong.lib.javassist.compiler.ast.CastExpr(com.feilong.lib.javassist.compiler.ast.ASTList, int, com.feilong.lib.javassist.compiler.ast.ASTree);
  public com.feilong.lib.javassist.compiler.ast.CastExpr(int, int, com.feilong.lib.javassist.compiler.ast.ASTree);
  public int getType();
  public int getArrayDim();
  public com.feilong.lib.javassist.compiler.ast.ASTList getClassName();
  public com.feilong.lib.javassist.compiler.ast.ASTree getOprand();
  public void setOprand(com.feilong.lib.javassist.compiler.ast.ASTree);
  public java.lang.String getTag();
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ast.CondExpr`

```java
public class com.feilong.lib.javassist.compiler.ast.CondExpr extends com.feilong.lib.javassist.compiler.ast.ASTList {
  public com.feilong.lib.javassist.compiler.ast.CondExpr(com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree);
  public com.feilong.lib.javassist.compiler.ast.ASTree condExpr();
  public void setCond(com.feilong.lib.javassist.compiler.ast.ASTree);
  public com.feilong.lib.javassist.compiler.ast.ASTree thenExpr();
  public void setThen(com.feilong.lib.javassist.compiler.ast.ASTree);
  public com.feilong.lib.javassist.compiler.ast.ASTree elseExpr();
  public void setElse(com.feilong.lib.javassist.compiler.ast.ASTree);
  public java.lang.String getTag();
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ast.Declarator`

```java
public class com.feilong.lib.javassist.compiler.ast.Declarator extends com.feilong.lib.javassist.compiler.ast.ASTList implements com.feilong.lib.javassist.compiler.TokenId {
  public com.feilong.lib.javassist.compiler.ast.Declarator(int, int);
  public com.feilong.lib.javassist.compiler.ast.Declarator(com.feilong.lib.javassist.compiler.ast.ASTList, int);
  public com.feilong.lib.javassist.compiler.ast.Declarator(int, java.lang.String, int, int, com.feilong.lib.javassist.compiler.ast.Symbol);
  public com.feilong.lib.javassist.compiler.ast.Declarator make(com.feilong.lib.javassist.compiler.ast.Symbol, int, com.feilong.lib.javassist.compiler.ast.ASTree);
  public int getType();
  public int getArrayDim();
  public void addArrayDim(int);
  public java.lang.String getClassName();
  public void setClassName(java.lang.String);
  public com.feilong.lib.javassist.compiler.ast.Symbol getVariable();
  public void setVariable(com.feilong.lib.javassist.compiler.ast.Symbol);
  public com.feilong.lib.javassist.compiler.ast.ASTree getInitializer();
  public void setLocalVar(int);
  public int getLocalVar();
  public java.lang.String getTag();
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
  public static java.lang.String astToClassName(com.feilong.lib.javassist.compiler.ast.ASTList, char);
}
```

## `com.feilong.lib.javassist.compiler.ast.DoubleConst`

```java
public class com.feilong.lib.javassist.compiler.ast.DoubleConst extends com.feilong.lib.javassist.compiler.ast.ASTree {
  public com.feilong.lib.javassist.compiler.ast.DoubleConst(double, int);
  public double get();
  public void set(double);
  public int getType();
  public java.lang.String toString();
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.compiler.ast.ASTree compute(int, com.feilong.lib.javassist.compiler.ast.ASTree);
}
```

## `com.feilong.lib.javassist.compiler.ast.Expr`

```java
public class com.feilong.lib.javassist.compiler.ast.Expr extends com.feilong.lib.javassist.compiler.ast.ASTList implements com.feilong.lib.javassist.compiler.TokenId {
  public static com.feilong.lib.javassist.compiler.ast.Expr make(int, com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree);
  public static com.feilong.lib.javassist.compiler.ast.Expr make(int, com.feilong.lib.javassist.compiler.ast.ASTree);
  public int getOperator();
  public void setOperator(int);
  public com.feilong.lib.javassist.compiler.ast.ASTree oprand1();
  public void setOprand1(com.feilong.lib.javassist.compiler.ast.ASTree);
  public com.feilong.lib.javassist.compiler.ast.ASTree oprand2();
  public void setOprand2(com.feilong.lib.javassist.compiler.ast.ASTree);
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
  public java.lang.String getName();
}
```

## `com.feilong.lib.javassist.compiler.ast.FieldDecl`

```java
public class com.feilong.lib.javassist.compiler.ast.FieldDecl extends com.feilong.lib.javassist.compiler.ast.ASTList {
  public com.feilong.lib.javassist.compiler.ast.FieldDecl(com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTList);
  public com.feilong.lib.javassist.compiler.ast.ASTList getModifiers();
  public com.feilong.lib.javassist.compiler.ast.Declarator getDeclarator();
  public com.feilong.lib.javassist.compiler.ast.ASTree getInit();
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ast.InstanceOfExpr`

```java
public class com.feilong.lib.javassist.compiler.ast.InstanceOfExpr extends com.feilong.lib.javassist.compiler.ast.CastExpr {
  public com.feilong.lib.javassist.compiler.ast.InstanceOfExpr(com.feilong.lib.javassist.compiler.ast.ASTList, int, com.feilong.lib.javassist.compiler.ast.ASTree);
  public com.feilong.lib.javassist.compiler.ast.InstanceOfExpr(int, int, com.feilong.lib.javassist.compiler.ast.ASTree);
  public java.lang.String getTag();
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ast.IntConst`

```java
public class com.feilong.lib.javassist.compiler.ast.IntConst extends com.feilong.lib.javassist.compiler.ast.ASTree {
  public com.feilong.lib.javassist.compiler.ast.IntConst(long, int);
  public long get();
  public void set(long);
  public int getType();
  public java.lang.String toString();
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
  public com.feilong.lib.javassist.compiler.ast.ASTree compute(int, com.feilong.lib.javassist.compiler.ast.ASTree);
}
```

## `com.feilong.lib.javassist.compiler.ast.Keyword`

```java
public class com.feilong.lib.javassist.compiler.ast.Keyword extends com.feilong.lib.javassist.compiler.ast.ASTree {
  public com.feilong.lib.javassist.compiler.ast.Keyword(int);
  public int get();
  public java.lang.String toString();
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ast.Member`

```java
public class com.feilong.lib.javassist.compiler.ast.Member extends com.feilong.lib.javassist.compiler.ast.Symbol {
  public com.feilong.lib.javassist.compiler.ast.Member(java.lang.String);
  public void setField(com.feilong.lib.javassist.CtField);
  public com.feilong.lib.javassist.CtField getField();
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ast.MethodDecl`

```java
public class com.feilong.lib.javassist.compiler.ast.MethodDecl extends com.feilong.lib.javassist.compiler.ast.ASTList {
  public com.feilong.lib.javassist.compiler.ast.MethodDecl(com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTList);
  public boolean isConstructor();
  public com.feilong.lib.javassist.compiler.ast.ASTList getModifiers();
  public com.feilong.lib.javassist.compiler.ast.Declarator getReturn();
  public com.feilong.lib.javassist.compiler.ast.ASTList getParams();
  public com.feilong.lib.javassist.compiler.ast.ASTList getThrows();
  public com.feilong.lib.javassist.compiler.ast.Stmnt getBody();
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ast.NewExpr`

```java
public class com.feilong.lib.javassist.compiler.ast.NewExpr extends com.feilong.lib.javassist.compiler.ast.ASTList implements com.feilong.lib.javassist.compiler.TokenId {
  public com.feilong.lib.javassist.compiler.ast.NewExpr(com.feilong.lib.javassist.compiler.ast.ASTList, com.feilong.lib.javassist.compiler.ast.ASTList);
  public com.feilong.lib.javassist.compiler.ast.NewExpr(int, com.feilong.lib.javassist.compiler.ast.ASTList, com.feilong.lib.javassist.compiler.ast.ArrayInit);
  public static com.feilong.lib.javassist.compiler.ast.NewExpr makeObjectArray(com.feilong.lib.javassist.compiler.ast.ASTList, com.feilong.lib.javassist.compiler.ast.ASTList, com.feilong.lib.javassist.compiler.ast.ArrayInit);
  public boolean isArray();
  public int getArrayType();
  public com.feilong.lib.javassist.compiler.ast.ASTList getClassName();
  public com.feilong.lib.javassist.compiler.ast.ASTList getArguments();
  public com.feilong.lib.javassist.compiler.ast.ASTList getArraySize();
  public com.feilong.lib.javassist.compiler.ast.ArrayInit getInitializer();
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ast.Pair`

```java
public class com.feilong.lib.javassist.compiler.ast.Pair extends com.feilong.lib.javassist.compiler.ast.ASTree {
  public com.feilong.lib.javassist.compiler.ast.Pair(com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree);
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
  public java.lang.String toString();
  public com.feilong.lib.javassist.compiler.ast.ASTree getLeft();
  public com.feilong.lib.javassist.compiler.ast.ASTree getRight();
  public void setLeft(com.feilong.lib.javassist.compiler.ast.ASTree);
  public void setRight(com.feilong.lib.javassist.compiler.ast.ASTree);
}
```

## `com.feilong.lib.javassist.compiler.ast.Stmnt`

```java
public class com.feilong.lib.javassist.compiler.ast.Stmnt extends com.feilong.lib.javassist.compiler.ast.ASTList implements com.feilong.lib.javassist.compiler.TokenId {
  public com.feilong.lib.javassist.compiler.ast.Stmnt(int, com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTList);
  public com.feilong.lib.javassist.compiler.ast.Stmnt(int, com.feilong.lib.javassist.compiler.ast.ASTree);
  public com.feilong.lib.javassist.compiler.ast.Stmnt(int);
  public static com.feilong.lib.javassist.compiler.ast.Stmnt make(int, com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree);
  public static com.feilong.lib.javassist.compiler.ast.Stmnt make(int, com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree, com.feilong.lib.javassist.compiler.ast.ASTree);
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
  public int getOperator();
}
```

## `com.feilong.lib.javassist.compiler.ast.StringL`

```java
public class com.feilong.lib.javassist.compiler.ast.StringL extends com.feilong.lib.javassist.compiler.ast.ASTree {
  public com.feilong.lib.javassist.compiler.ast.StringL(java.lang.String);
  public java.lang.String get();
  public java.lang.String toString();
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ast.Symbol`

```java
public class com.feilong.lib.javassist.compiler.ast.Symbol extends com.feilong.lib.javassist.compiler.ast.ASTree {
  public com.feilong.lib.javassist.compiler.ast.Symbol(java.lang.String);
  public java.lang.String get();
  public java.lang.String toString();
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ast.Variable`

```java
public class com.feilong.lib.javassist.compiler.ast.Variable extends com.feilong.lib.javassist.compiler.ast.Symbol {
  public com.feilong.lib.javassist.compiler.ast.Variable(java.lang.String, com.feilong.lib.javassist.compiler.ast.Declarator);
  public com.feilong.lib.javassist.compiler.ast.Declarator getDeclarator();
  public java.lang.String toString();
  public void accept(com.feilong.lib.javassist.compiler.ast.Visitor) throws com.feilong.lib.javassist.compiler.CompileError;
}
```

## `com.feilong.lib.javassist.compiler.ast.Visitor`

```java
public class com.feilong.lib.javassist.compiler.ast.Visitor {
  public com.feilong.lib.javassist.compiler.ast.Visitor();
  public void atASTList(com.feilong.lib.javassist.compiler.ast.ASTList) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atPair(com.feilong.lib.javassist.compiler.ast.Pair) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atFieldDecl(com.feilong.lib.javassist.compiler.ast.FieldDecl) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atMethodDecl(com.feilong.lib.javassist.compiler.ast.MethodDecl) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atStmnt(com.feilong.lib.javassist.compiler.ast.Stmnt) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atDeclarator(com.feilong.lib.javassist.compiler.ast.Declarator) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atAssignExpr(com.feilong.lib.javassist.compiler.ast.AssignExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atCondExpr(com.feilong.lib.javassist.compiler.ast.CondExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atBinExpr(com.feilong.lib.javassist.compiler.ast.BinExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atExpr(com.feilong.lib.javassist.compiler.ast.Expr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atCallExpr(com.feilong.lib.javassist.compiler.ast.CallExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atCastExpr(com.feilong.lib.javassist.compiler.ast.CastExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atInstanceOfExpr(com.feilong.lib.javassist.compiler.ast.InstanceOfExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atNewExpr(com.feilong.lib.javassist.compiler.ast.NewExpr) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atSymbol(com.feilong.lib.javassist.compiler.ast.Symbol) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atMember(com.feilong.lib.javassist.compiler.ast.Member) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atVariable(com.feilong.lib.javassist.compiler.ast.Variable) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atKeyword(com.feilong.lib.javassist.compiler.ast.Keyword) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atStringL(com.feilong.lib.javassist.compiler.ast.StringL) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atIntConst(com.feilong.lib.javassist.compiler.ast.IntConst) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atDoubleConst(com.feilong.lib.javassist.compiler.ast.DoubleConst) throws com.feilong.lib.javassist.compiler.CompileError;
  public void atArrayInit(com.feilong.lib.javassist.compiler.ast.ArrayInit) throws com.feilong.lib.javassist.compiler.CompileError;
}
```
