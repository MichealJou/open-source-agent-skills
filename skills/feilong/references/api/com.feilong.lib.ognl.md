# com.feilong.lib.ognl

版本：4.5.1。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.feilong.lib.ognl.ASTAnd`

```java
public class com.feilong.lib.ognl.ASTAnd extends com.feilong.lib.ognl.BooleanExpression {
  public com.feilong.lib.ognl.ASTAnd(int);
  public com.feilong.lib.ognl.ASTAnd(com.feilong.lib.ognl.OgnlParser, int);
  public void jjtClose();
  public java.lang.String getExpressionOperator(int);
  public java.lang.Class getGetterClass();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ASTChain`

```java
public class com.feilong.lib.ognl.ASTChain extends com.feilong.lib.ognl.SimpleNode implements com.feilong.lib.ognl.NodeType,com.feilong.lib.ognl.enhance.OrderedReturn {
  public com.feilong.lib.ognl.ASTChain(int);
  public com.feilong.lib.ognl.ASTChain(com.feilong.lib.ognl.OgnlParser, int);
  public java.lang.String getLastExpression();
  public java.lang.String getCoreExpression();
  public void jjtClose();
  public boolean isSimpleNavigationChain(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public java.lang.Class getGetterClass();
  public java.lang.Class getSetterClass();
  public java.lang.String toString();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public boolean isChain(com.feilong.lib.ognl.OgnlContext);
}
```

## `com.feilong.lib.ognl.ASTConst`

```java
public class com.feilong.lib.ognl.ASTConst extends com.feilong.lib.ognl.SimpleNode implements com.feilong.lib.ognl.NodeType {
  public com.feilong.lib.ognl.ASTConst(int);
  public com.feilong.lib.ognl.ASTConst(com.feilong.lib.ognl.OgnlParser, int);
  public void setValue(java.lang.Object);
  public java.lang.Object getValue();
  public boolean isNodeConstant(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public java.lang.Class getGetterClass();
  public java.lang.Class getSetterClass();
  public java.lang.String toString();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ASTCtor`

```java
public class com.feilong.lib.ognl.ASTCtor extends com.feilong.lib.ognl.SimpleNode {
  public com.feilong.lib.ognl.ASTCtor(int);
  public com.feilong.lib.ognl.ASTCtor(com.feilong.lib.ognl.OgnlParser, int);
  public boolean isArray();
  public java.lang.String toString();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ASTInstanceof`

```java
public class com.feilong.lib.ognl.ASTInstanceof extends com.feilong.lib.ognl.SimpleNode implements com.feilong.lib.ognl.NodeType {
  public com.feilong.lib.ognl.ASTInstanceof(int);
  public com.feilong.lib.ognl.ASTInstanceof(com.feilong.lib.ognl.OgnlParser, int);
  public java.lang.String toString();
  public java.lang.Class getGetterClass();
  public java.lang.Class getSetterClass();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ASTList`

```java
public class com.feilong.lib.ognl.ASTList extends com.feilong.lib.ognl.SimpleNode implements com.feilong.lib.ognl.NodeType {
  public com.feilong.lib.ognl.ASTList(int);
  public com.feilong.lib.ognl.ASTList(com.feilong.lib.ognl.OgnlParser, int);
  public java.lang.Class getGetterClass();
  public java.lang.Class getSetterClass();
  public java.lang.String toString();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ASTMethod`

```java
public class com.feilong.lib.ognl.ASTMethod extends com.feilong.lib.ognl.SimpleNode implements com.feilong.lib.ognl.enhance.OrderedReturn,com.feilong.lib.ognl.NodeType {
  public com.feilong.lib.ognl.ASTMethod(int);
  public com.feilong.lib.ognl.ASTMethod(com.feilong.lib.ognl.OgnlParser, int);
  public void setMethodName(java.lang.String);
  public java.lang.String getMethodName();
  public java.lang.String getLastExpression();
  public java.lang.String getCoreExpression();
  public java.lang.Class getGetterClass();
  public java.lang.Class getSetterClass();
  public java.lang.String toString();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public boolean isSimpleMethod(com.feilong.lib.ognl.OgnlContext);
}
```

## `com.feilong.lib.ognl.ASTOr`

```java
public class com.feilong.lib.ognl.ASTOr extends com.feilong.lib.ognl.BooleanExpression {
  public com.feilong.lib.ognl.ASTOr(int);
  public com.feilong.lib.ognl.ASTOr(com.feilong.lib.ognl.OgnlParser, int);
  public void jjtClose();
  public java.lang.String getExpressionOperator(int);
  public java.lang.Class getGetterClass();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ASTProperty`

```java
public class com.feilong.lib.ognl.ASTProperty extends com.feilong.lib.ognl.SimpleNode implements com.feilong.lib.ognl.NodeType {
  public com.feilong.lib.ognl.ASTProperty(int);
  public void setIndexedAccess(boolean);
  public boolean isIndexedAccess();
  public int getIndexedPropertyType(com.feilong.lib.ognl.OgnlContext, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public java.lang.Object getProperty(com.feilong.lib.ognl.OgnlContext, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public boolean isNodeSimpleProperty(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public java.lang.Class getGetterClass();
  public java.lang.Class getSetterClass();
  public java.lang.String toString();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ASTRootVarRef`

```java
public class com.feilong.lib.ognl.ASTRootVarRef extends com.feilong.lib.ognl.ASTVarRef {
  public com.feilong.lib.ognl.ASTRootVarRef(int);
  public com.feilong.lib.ognl.ASTRootVarRef(com.feilong.lib.ognl.OgnlParser, int);
  public java.lang.String toString();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ASTSequence`

```java
public class com.feilong.lib.ognl.ASTSequence extends com.feilong.lib.ognl.SimpleNode implements com.feilong.lib.ognl.NodeType,com.feilong.lib.ognl.enhance.OrderedReturn {
  public com.feilong.lib.ognl.ASTSequence(int);
  public com.feilong.lib.ognl.ASTSequence(com.feilong.lib.ognl.OgnlParser, int);
  public void jjtClose();
  public java.lang.Class getGetterClass();
  public java.lang.Class getSetterClass();
  public java.lang.String getLastExpression();
  public java.lang.String getCoreExpression();
  public java.lang.String toString();
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public boolean isSequence(com.feilong.lib.ognl.OgnlContext);
}
```

## `com.feilong.lib.ognl.ASTStaticField`

```java
public class com.feilong.lib.ognl.ASTStaticField extends com.feilong.lib.ognl.SimpleNode implements com.feilong.lib.ognl.NodeType {
  public com.feilong.lib.ognl.ASTStaticField(int);
  public com.feilong.lib.ognl.ASTStaticField(com.feilong.lib.ognl.OgnlParser, int);
  public boolean isNodeConstant(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public java.lang.Class getGetterClass();
  public java.lang.Class getSetterClass();
  public java.lang.String toString();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ASTStaticMethod`

```java
public class com.feilong.lib.ognl.ASTStaticMethod extends com.feilong.lib.ognl.SimpleNode implements com.feilong.lib.ognl.NodeType {
  public com.feilong.lib.ognl.ASTStaticMethod(int);
  public com.feilong.lib.ognl.ASTStaticMethod(com.feilong.lib.ognl.OgnlParser, int);
  public java.lang.Class getGetterClass();
  public java.lang.Class getSetterClass();
  public java.lang.String toString();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ASTThisVarRef`

```java
public class com.feilong.lib.ognl.ASTThisVarRef extends com.feilong.lib.ognl.ASTVarRef {
  public com.feilong.lib.ognl.ASTThisVarRef(int);
  public com.feilong.lib.ognl.ASTThisVarRef(com.feilong.lib.ognl.OgnlParser, int);
  public java.lang.String toString();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ASTVarRef`

```java
public class com.feilong.lib.ognl.ASTVarRef extends com.feilong.lib.ognl.SimpleNode implements com.feilong.lib.ognl.NodeType,com.feilong.lib.ognl.enhance.OrderedReturn {
  public com.feilong.lib.ognl.ASTVarRef(int);
  public com.feilong.lib.ognl.ASTVarRef(com.feilong.lib.ognl.OgnlParser, int);
  public java.lang.Class getGetterClass();
  public java.lang.Class getSetterClass();
  public java.lang.String getCoreExpression();
  public java.lang.String getLastExpression();
  public java.lang.String toString();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.AccessibleObjectHandler`

```java
public interface com.feilong.lib.ognl.AccessibleObjectHandler {
  public abstract void setAccessible(java.lang.reflect.AccessibleObject, boolean);
}
```

## `com.feilong.lib.ognl.ArrayElementsAccessor`

```java
public class com.feilong.lib.ognl.ArrayElementsAccessor implements com.feilong.lib.ognl.ElementsAccessor {
  public com.feilong.lib.ognl.ArrayElementsAccessor();
  public java.util.Enumeration getElements(java.lang.Object);
}
```

## `com.feilong.lib.ognl.ArrayPropertyAccessor`

```java
public class com.feilong.lib.ognl.ArrayPropertyAccessor extends com.feilong.lib.ognl.ObjectPropertyAccessor implements com.feilong.lib.ognl.PropertyAccessor {
  public com.feilong.lib.ognl.ArrayPropertyAccessor();
  public java.lang.Object getProperty(java.util.Map, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public void setProperty(java.util.Map, java.lang.Object, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public java.lang.String getSourceAccessor(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object);
  public java.lang.String getSourceSetter(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.ognl.BooleanExpression`

```java
public abstract class com.feilong.lib.ognl.BooleanExpression extends com.feilong.lib.ognl.ExpressionNode implements com.feilong.lib.ognl.NodeType {
  public com.feilong.lib.ognl.BooleanExpression(int);
  public com.feilong.lib.ognl.BooleanExpression(com.feilong.lib.ognl.OgnlParser, int);
  public java.lang.Class getGetterClass();
  public java.lang.Class getSetterClass();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ClassCacheInspector`

```java
public interface com.feilong.lib.ognl.ClassCacheInspector {
  public abstract boolean shouldCache(java.lang.Class);
}
```

## `com.feilong.lib.ognl.ClassResolver`

```java
public interface com.feilong.lib.ognl.ClassResolver {
  public abstract java.lang.Class classForName(java.lang.String, java.util.Map) throws java.lang.ClassNotFoundException;
}
```

## `com.feilong.lib.ognl.CollectionElementsAccessor`

```java
public class com.feilong.lib.ognl.CollectionElementsAccessor implements com.feilong.lib.ognl.ElementsAccessor {
  public com.feilong.lib.ognl.CollectionElementsAccessor();
  public java.util.Enumeration getElements(java.lang.Object);
}
```

## `com.feilong.lib.ognl.ComparisonExpression`

```java
public abstract class com.feilong.lib.ognl.ComparisonExpression extends com.feilong.lib.ognl.BooleanExpression {
  public com.feilong.lib.ognl.ComparisonExpression(int);
  public com.feilong.lib.ognl.ComparisonExpression(com.feilong.lib.ognl.OgnlParser, int);
  public abstract java.lang.String getComparisonFunction();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.DefaultClassResolver`

```java
public class com.feilong.lib.ognl.DefaultClassResolver implements com.feilong.lib.ognl.ClassResolver {
  public com.feilong.lib.ognl.DefaultClassResolver();
  public java.lang.Class classForName(java.lang.String, java.util.Map) throws java.lang.ClassNotFoundException;
}
```

## `com.feilong.lib.ognl.DefaultTypeConverter`

```java
public class com.feilong.lib.ognl.DefaultTypeConverter implements com.feilong.lib.ognl.TypeConverter {
  public com.feilong.lib.ognl.DefaultTypeConverter();
  public java.lang.Object convertValue(java.util.Map, java.lang.Object, java.lang.Class);
  public java.lang.Object convertValue(java.util.Map, java.lang.Object, java.lang.reflect.Member, java.lang.String, java.lang.Object, java.lang.Class);
}
```

## `com.feilong.lib.ognl.DynamicSubscript`

```java
public class com.feilong.lib.ognl.DynamicSubscript {
  public int getFlag();
  public java.lang.String toString();
}
```

## `com.feilong.lib.ognl.ElementsAccessor`

```java
public interface com.feilong.lib.ognl.ElementsAccessor {
  public abstract java.util.Enumeration getElements(java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
}
```

## `com.feilong.lib.ognl.EnumerationElementsAccessor`

```java
public class com.feilong.lib.ognl.EnumerationElementsAccessor implements com.feilong.lib.ognl.ElementsAccessor {
  public com.feilong.lib.ognl.EnumerationElementsAccessor();
  public java.util.Enumeration getElements(java.lang.Object);
}
```

## `com.feilong.lib.ognl.EnumerationIterator`

```java
public class com.feilong.lib.ognl.EnumerationIterator implements java.util.Iterator {
  public com.feilong.lib.ognl.EnumerationIterator(java.util.Enumeration);
  public boolean hasNext();
  public java.lang.Object next();
  public void remove();
}
```

## `com.feilong.lib.ognl.EnumerationPropertyAccessor`

```java
public class com.feilong.lib.ognl.EnumerationPropertyAccessor extends com.feilong.lib.ognl.ObjectPropertyAccessor implements com.feilong.lib.ognl.PropertyAccessor {
  public com.feilong.lib.ognl.EnumerationPropertyAccessor();
  public java.lang.Object getProperty(java.util.Map, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public void setProperty(java.util.Map, java.lang.Object, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
}
```

## `com.feilong.lib.ognl.Evaluation`

```java
public class com.feilong.lib.ognl.Evaluation {
  public com.feilong.lib.ognl.Evaluation(com.feilong.lib.ognl.SimpleNode, java.lang.Object);
  public com.feilong.lib.ognl.Evaluation(com.feilong.lib.ognl.SimpleNode, java.lang.Object, boolean);
  public com.feilong.lib.ognl.SimpleNode getNode();
  public void setNode(com.feilong.lib.ognl.SimpleNode);
  public java.lang.Object getSource();
  public void setSource(java.lang.Object);
  public boolean isSetOperation();
  public void setSetOperation(boolean);
  public java.lang.Object getResult();
  public void setResult(java.lang.Object);
  public java.lang.Throwable getException();
  public void setException(java.lang.Throwable);
  public com.feilong.lib.ognl.Evaluation getParent();
  public com.feilong.lib.ognl.Evaluation getNext();
  public com.feilong.lib.ognl.Evaluation getPrevious();
  public com.feilong.lib.ognl.Evaluation getFirstChild();
  public com.feilong.lib.ognl.Evaluation getLastChild();
  public com.feilong.lib.ognl.Evaluation getFirstDescendant();
  public com.feilong.lib.ognl.Evaluation getLastDescendant();
  public void addChild(com.feilong.lib.ognl.Evaluation);
  public void init(com.feilong.lib.ognl.SimpleNode, java.lang.Object, boolean);
  public void reset();
  public java.lang.String toString(boolean, boolean, java.lang.String);
  public java.lang.String toString(boolean, java.lang.String);
  public java.lang.String toString();
}
```

## `com.feilong.lib.ognl.EvaluationPool`

```java
public final class com.feilong.lib.ognl.EvaluationPool {
  public com.feilong.lib.ognl.EvaluationPool();
  public com.feilong.lib.ognl.EvaluationPool(int);
  public com.feilong.lib.ognl.Evaluation create(com.feilong.lib.ognl.SimpleNode, java.lang.Object);
  public com.feilong.lib.ognl.Evaluation create(com.feilong.lib.ognl.SimpleNode, java.lang.Object, boolean);
}
```

## `com.feilong.lib.ognl.ExpressionNode`

```java
public abstract class com.feilong.lib.ognl.ExpressionNode extends com.feilong.lib.ognl.SimpleNode {
  public com.feilong.lib.ognl.ExpressionNode(int);
  public com.feilong.lib.ognl.ExpressionNode(com.feilong.lib.ognl.OgnlParser, int);
  public boolean isNodeConstant(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public boolean isConstant(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public java.lang.String getExpressionOperator(int);
  public java.lang.String toString();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public boolean isOperation(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
}
```

## `com.feilong.lib.ognl.ExpressionSyntaxException`

```java
public class com.feilong.lib.ognl.ExpressionSyntaxException extends com.feilong.lib.ognl.OgnlException {
  public com.feilong.lib.ognl.ExpressionSyntaxException(java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.ognl.InappropriateExpressionException`

```java
public class com.feilong.lib.ognl.InappropriateExpressionException extends com.feilong.lib.ognl.OgnlException {
  public com.feilong.lib.ognl.InappropriateExpressionException(com.feilong.lib.ognl.Node);
}
```

## `com.feilong.lib.ognl.IteratorElementsAccessor`

```java
public class com.feilong.lib.ognl.IteratorElementsAccessor implements com.feilong.lib.ognl.ElementsAccessor {
  public com.feilong.lib.ognl.IteratorElementsAccessor();
  public java.util.Enumeration getElements(java.lang.Object);
}
```

## `com.feilong.lib.ognl.IteratorEnumeration`

```java
public class com.feilong.lib.ognl.IteratorEnumeration implements java.util.Enumeration {
  public com.feilong.lib.ognl.IteratorEnumeration(java.util.Iterator);
  public boolean hasMoreElements();
  public java.lang.Object nextElement();
}
```

## `com.feilong.lib.ognl.IteratorPropertyAccessor`

```java
public class com.feilong.lib.ognl.IteratorPropertyAccessor extends com.feilong.lib.ognl.ObjectPropertyAccessor implements com.feilong.lib.ognl.PropertyAccessor {
  public com.feilong.lib.ognl.IteratorPropertyAccessor();
  public java.lang.Object getProperty(java.util.Map, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public void setProperty(java.util.Map, java.lang.Object, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
}
```

## `com.feilong.lib.ognl.JJTOgnlParserState`

```java
public class com.feilong.lib.ognl.JJTOgnlParserState {
  public com.feilong.lib.ognl.JJTOgnlParserState();
  public boolean nodeCreated();
  public void reset();
  public com.feilong.lib.ognl.Node rootNode();
  public void pushNode(com.feilong.lib.ognl.Node);
  public com.feilong.lib.ognl.Node popNode();
  public com.feilong.lib.ognl.Node peekNode();
  public int nodeArity();
  public void clearNodeScope(com.feilong.lib.ognl.Node);
  public void openNodeScope(com.feilong.lib.ognl.Node);
  public void closeNodeScope(com.feilong.lib.ognl.Node, int);
  public void closeNodeScope(com.feilong.lib.ognl.Node, boolean);
}
```

## `com.feilong.lib.ognl.JavaCharStream`

```java
public class com.feilong.lib.ognl.JavaCharStream {
  public char BeginToken() throws java.io.IOException;
  public char readChar() throws java.io.IOException;
  public int getEndColumn();
  public int getEndLine();
  public int getBeginColumn();
  public int getBeginLine();
  public void backup(int);
  public com.feilong.lib.ognl.JavaCharStream(java.io.Reader, int, int, int);
  public com.feilong.lib.ognl.JavaCharStream(java.io.Reader, int, int);
  public com.feilong.lib.ognl.JavaCharStream(java.io.Reader);
  public void ReInit(java.io.Reader, int, int, int);
  public void ReInit(java.io.Reader, int, int);
  public void ReInit(java.io.Reader);
  public com.feilong.lib.ognl.JavaCharStream(java.io.InputStream, java.lang.String, int, int, int) throws java.io.UnsupportedEncodingException;
  public com.feilong.lib.ognl.JavaCharStream(java.io.InputStream, int, int, int);
  public com.feilong.lib.ognl.JavaCharStream(java.io.InputStream, java.lang.String, int, int) throws java.io.UnsupportedEncodingException;
  public com.feilong.lib.ognl.JavaCharStream(java.io.InputStream, int, int);
  public com.feilong.lib.ognl.JavaCharStream(java.io.InputStream, java.lang.String) throws java.io.UnsupportedEncodingException;
  public com.feilong.lib.ognl.JavaCharStream(java.io.InputStream);
  public void ReInit(java.io.InputStream, java.lang.String, int, int, int) throws java.io.UnsupportedEncodingException;
  public void ReInit(java.io.InputStream, int, int, int);
  public void ReInit(java.io.InputStream, java.lang.String, int, int) throws java.io.UnsupportedEncodingException;
  public void ReInit(java.io.InputStream, int, int);
  public void ReInit(java.io.InputStream, java.lang.String) throws java.io.UnsupportedEncodingException;
  public void ReInit(java.io.InputStream);
  public java.lang.String GetImage();
  public char[] GetSuffix(int);
  public void Done();
  public void adjustBeginLineColumn(int, int);
}
```

## `com.feilong.lib.ognl.JavaSource`

```java
public interface com.feilong.lib.ognl.JavaSource {
  public abstract java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public abstract java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ListPropertyAccessor`

```java
public class com.feilong.lib.ognl.ListPropertyAccessor extends com.feilong.lib.ognl.ObjectPropertyAccessor implements com.feilong.lib.ognl.PropertyAccessor {
  public com.feilong.lib.ognl.ListPropertyAccessor();
  public java.lang.Object getProperty(java.util.Map, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public void setProperty(java.util.Map, java.lang.Object, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public java.lang.Class getPropertyClass(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object);
  public java.lang.String getSourceAccessor(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object);
  public java.lang.String getSourceSetter(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.ognl.MapElementsAccessor`

```java
public class com.feilong.lib.ognl.MapElementsAccessor implements com.feilong.lib.ognl.ElementsAccessor {
  public com.feilong.lib.ognl.MapElementsAccessor();
  public java.util.Enumeration getElements(java.lang.Object);
}
```

## `com.feilong.lib.ognl.MapPropertyAccessor`

```java
public class com.feilong.lib.ognl.MapPropertyAccessor implements com.feilong.lib.ognl.PropertyAccessor {
  public com.feilong.lib.ognl.MapPropertyAccessor();
  public java.lang.Object getProperty(java.util.Map, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public void setProperty(java.util.Map, java.lang.Object, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public java.lang.String getSourceAccessor(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object);
  public java.lang.String getSourceSetter(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.ognl.MemberAccess`

```java
public interface com.feilong.lib.ognl.MemberAccess {
  public abstract java.lang.Object setup(java.util.Map, java.lang.Object, java.lang.reflect.Member, java.lang.String);
  public abstract void restore(java.util.Map, java.lang.Object, java.lang.reflect.Member, java.lang.String, java.lang.Object);
  public abstract boolean isAccessible(java.util.Map, java.lang.Object, java.lang.reflect.Member, java.lang.String);
}
```

## `com.feilong.lib.ognl.MethodAccessor`

```java
public interface com.feilong.lib.ognl.MethodAccessor {
  public abstract java.lang.Object callStaticMethod(java.util.Map, java.lang.Class, java.lang.String, java.lang.Object[]) throws com.feilong.lib.ognl.MethodFailedException;
  public abstract java.lang.Object callMethod(java.util.Map, java.lang.Object, java.lang.String, java.lang.Object[]) throws com.feilong.lib.ognl.MethodFailedException;
}
```

## `com.feilong.lib.ognl.MethodFailedException`

```java
public class com.feilong.lib.ognl.MethodFailedException extends com.feilong.lib.ognl.OgnlException {
  public com.feilong.lib.ognl.MethodFailedException(java.lang.Object, java.lang.String);
  public com.feilong.lib.ognl.MethodFailedException(java.lang.Object, java.lang.String, java.lang.Throwable);
}
```

## `com.feilong.lib.ognl.NoSuchPropertyException`

```java
public class com.feilong.lib.ognl.NoSuchPropertyException extends com.feilong.lib.ognl.OgnlException {
  public com.feilong.lib.ognl.NoSuchPropertyException(java.lang.Object, java.lang.Object);
  public com.feilong.lib.ognl.NoSuchPropertyException(java.lang.Object, java.lang.Object, java.lang.Throwable);
  public java.lang.Object getTarget();
  public java.lang.Object getName();
}
```

## `com.feilong.lib.ognl.Node`

```java
public interface com.feilong.lib.ognl.Node extends com.feilong.lib.ognl.JavaSource {
  public abstract void jjtOpen();
  public abstract void jjtClose();
  public abstract void jjtSetParent(com.feilong.lib.ognl.Node);
  public abstract com.feilong.lib.ognl.Node jjtGetParent();
  public abstract void jjtAddChild(com.feilong.lib.ognl.Node, int);
  public abstract com.feilong.lib.ognl.Node jjtGetChild(int);
  public abstract int jjtGetNumChildren();
  public abstract java.lang.Object getValue(com.feilong.lib.ognl.OgnlContext, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public abstract void setValue(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public abstract com.feilong.lib.ognl.enhance.ExpressionAccessor getAccessor();
  public abstract void setAccessor(com.feilong.lib.ognl.enhance.ExpressionAccessor);
}
```

## `com.feilong.lib.ognl.NodeType`

```java
public interface com.feilong.lib.ognl.NodeType {
  public abstract java.lang.Class getGetterClass();
  public abstract java.lang.Class getSetterClass();
}
```

## `com.feilong.lib.ognl.NullHandler`

```java
public interface com.feilong.lib.ognl.NullHandler {
  public abstract java.lang.Object nullMethodResult(java.util.Map, java.lang.Object, java.lang.String, java.lang.Object[]);
  public abstract java.lang.Object nullPropertyValue(java.util.Map, java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.ognl.NumberElementsAccessor`

```java
public class com.feilong.lib.ognl.NumberElementsAccessor implements com.feilong.lib.ognl.ElementsAccessor,com.feilong.lib.ognl.NumericTypes {
  public com.feilong.lib.ognl.NumberElementsAccessor();
  public java.util.Enumeration getElements(java.lang.Object);
}
```

## `com.feilong.lib.ognl.NumericExpression`

```java
public abstract class com.feilong.lib.ognl.NumericExpression extends com.feilong.lib.ognl.ExpressionNode implements com.feilong.lib.ognl.NodeType {
  public com.feilong.lib.ognl.NumericExpression(int);
  public com.feilong.lib.ognl.NumericExpression(com.feilong.lib.ognl.OgnlParser, int);
  public java.lang.Class getGetterClass();
  public java.lang.Class getSetterClass();
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String coerceToNumeric(java.lang.String, com.feilong.lib.ognl.OgnlContext, com.feilong.lib.ognl.Node);
}
```

## `com.feilong.lib.ognl.ObjectArrayPool`

```java
public final class com.feilong.lib.ognl.ObjectArrayPool {
  public com.feilong.lib.ognl.ObjectArrayPool();
  public static java.lang.Object[] create(int);
  public static java.lang.Object[] create(java.lang.Object);
  public static java.lang.Object[] create(java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ObjectElementsAccessor`

```java
public class com.feilong.lib.ognl.ObjectElementsAccessor implements com.feilong.lib.ognl.ElementsAccessor {
  public com.feilong.lib.ognl.ObjectElementsAccessor();
  public java.util.Enumeration getElements(java.lang.Object);
}
```

## `com.feilong.lib.ognl.ObjectIndexedPropertyDescriptor`

```java
public class com.feilong.lib.ognl.ObjectIndexedPropertyDescriptor extends java.beans.PropertyDescriptor {
  public com.feilong.lib.ognl.ObjectIndexedPropertyDescriptor(java.lang.String, java.lang.Class, java.lang.reflect.Method, java.lang.reflect.Method) throws java.beans.IntrospectionException;
  public java.lang.reflect.Method getIndexedReadMethod();
  public java.lang.reflect.Method getIndexedWriteMethod();
  public java.lang.Class getPropertyType();
}
```

## `com.feilong.lib.ognl.ObjectMethodAccessor`

```java
public class com.feilong.lib.ognl.ObjectMethodAccessor implements com.feilong.lib.ognl.MethodAccessor {
  public com.feilong.lib.ognl.ObjectMethodAccessor();
  public java.lang.Object callStaticMethod(java.util.Map, java.lang.Class, java.lang.String, java.lang.Object[]) throws com.feilong.lib.ognl.MethodFailedException;
  public java.lang.Object callMethod(java.util.Map, java.lang.Object, java.lang.String, java.lang.Object[]) throws com.feilong.lib.ognl.MethodFailedException;
}
```

## `com.feilong.lib.ognl.ObjectNullHandler`

```java
public class com.feilong.lib.ognl.ObjectNullHandler implements com.feilong.lib.ognl.NullHandler {
  public com.feilong.lib.ognl.ObjectNullHandler();
  public java.lang.Object nullMethodResult(java.util.Map, java.lang.Object, java.lang.String, java.lang.Object[]);
  public java.lang.Object nullPropertyValue(java.util.Map, java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.ognl.ObjectPropertyAccessor`

```java
public class com.feilong.lib.ognl.ObjectPropertyAccessor implements com.feilong.lib.ognl.PropertyAccessor {
  public com.feilong.lib.ognl.ObjectPropertyAccessor();
  public java.lang.Object getPossibleProperty(java.util.Map, java.lang.Object, java.lang.String) throws com.feilong.lib.ognl.OgnlException;
  public java.lang.Object setPossibleProperty(java.util.Map, java.lang.Object, java.lang.String, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public boolean hasGetProperty(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public boolean hasGetProperty(java.util.Map, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public boolean hasSetProperty(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public boolean hasSetProperty(java.util.Map, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public java.lang.Object getProperty(java.util.Map, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public void setProperty(java.util.Map, java.lang.Object, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public java.lang.Class getPropertyClass(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object);
  public java.lang.String getSourceAccessor(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object);
  public java.lang.String getSourceSetter(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.ognl.Ognl`

```java
public abstract class com.feilong.lib.ognl.Ognl {
  public static java.lang.Object parseExpression(java.lang.String) throws com.feilong.lib.ognl.OgnlException;
  public static java.lang.Object getValue(java.lang.Object, java.util.Map, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public static void setValue(java.lang.Object, java.util.Map, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public static void setValue(java.lang.String, java.util.Map, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
}
```

## `com.feilong.lib.ognl.OgnlContext`

```java
public class com.feilong.lib.ognl.OgnlContext implements java.util.Map {
  public com.feilong.lib.ognl.OgnlContext(com.feilong.lib.ognl.MemberAccess, com.feilong.lib.ognl.ClassResolver, com.feilong.lib.ognl.TypeConverter, java.util.Map);
  public com.feilong.lib.ognl.ClassResolver getClassResolver();
  public com.feilong.lib.ognl.TypeConverter getTypeConverter();
  public com.feilong.lib.ognl.MemberAccess getMemberAccess();
  public void setRoot(java.lang.Object);
  public java.lang.Object getRoot();
  public boolean getTraceEvaluations();
  public void setTraceEvaluations(boolean);
  public com.feilong.lib.ognl.Evaluation getLastEvaluation();
  public void setLastEvaluation(com.feilong.lib.ognl.Evaluation);
  public boolean getKeepLastEvaluation();
  public void setKeepLastEvaluation(boolean);
  public void setCurrentObject(java.lang.Object);
  public java.lang.Object getCurrentObject();
  public void setCurrentAccessor(java.lang.Class);
  public java.lang.Class getCurrentAccessor();
  public java.lang.Class getPreviousAccessor();
  public java.lang.Class getFirstAccessor();
  public java.lang.Class getCurrentType();
  public void setCurrentType(java.lang.Class);
  public java.lang.Class getPreviousType();
  public void setPreviousType(java.lang.Class);
  public java.lang.Class getFirstType();
  public void setCurrentNode(com.feilong.lib.ognl.Node);
  public com.feilong.lib.ognl.Node getCurrentNode();
  public com.feilong.lib.ognl.Evaluation getCurrentEvaluation();
  public void setCurrentEvaluation(com.feilong.lib.ognl.Evaluation);
  public com.feilong.lib.ognl.Evaluation getRootEvaluation();
  public void setRootEvaluation(com.feilong.lib.ognl.Evaluation);
  public com.feilong.lib.ognl.Evaluation getEvaluation(int);
  public void pushEvaluation(com.feilong.lib.ognl.Evaluation);
  public com.feilong.lib.ognl.Evaluation popEvaluation();
  public int incrementLocalReferenceCounter();
  public void addLocalReference(java.lang.String, com.feilong.lib.ognl.enhance.LocalReference);
  public java.util.Map getLocalReferences();
  public int size();
  public boolean isEmpty();
  public boolean containsKey(java.lang.Object);
  public boolean containsValue(java.lang.Object);
  public java.lang.Object get(java.lang.Object);
  public java.lang.Object put(java.lang.Object, java.lang.Object);
  public java.lang.Object remove(java.lang.Object);
  public void putAll(java.util.Map);
  public void clear();
  public java.util.Set keySet();
  public java.util.Collection values();
  public java.util.Set entrySet();
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `com.feilong.lib.ognl.OgnlException`

```java
public class com.feilong.lib.ognl.OgnlException extends java.lang.Exception {
  public com.feilong.lib.ognl.OgnlException(java.lang.String);
  public com.feilong.lib.ognl.OgnlException(java.lang.String, java.lang.Throwable);
  public void setEvaluation(com.feilong.lib.ognl.Evaluation);
  public java.lang.String toString();
  public void printStackTrace();
  public void printStackTrace(java.io.PrintStream);
  public void printStackTrace(java.io.PrintWriter);
}
```

## `com.feilong.lib.ognl.OgnlInvokePermission`

```java
public class com.feilong.lib.ognl.OgnlInvokePermission extends java.security.BasicPermission {
  public com.feilong.lib.ognl.OgnlInvokePermission(java.lang.String);
  public com.feilong.lib.ognl.OgnlInvokePermission(java.lang.String, java.lang.String);
}
```

## `com.feilong.lib.ognl.OgnlOps`

```java
public abstract class com.feilong.lib.ognl.OgnlOps implements com.feilong.lib.ognl.NumericTypes {
  public com.feilong.lib.ognl.OgnlOps();
  public static int compareWithConversion(java.lang.Object, java.lang.Object);
  public static boolean isEqual(java.lang.Object, java.lang.Object);
  public static boolean booleanValue(boolean);
  public static boolean booleanValue(int);
  public static boolean booleanValue(float);
  public static boolean booleanValue(long);
  public static boolean booleanValue(double);
  public static boolean booleanValue(java.lang.Object);
  public static long longValue(java.lang.Object) throws java.lang.NumberFormatException;
  public static double doubleValue(java.lang.Object) throws java.lang.NumberFormatException;
  public static java.math.BigInteger bigIntValue(java.lang.Object) throws java.lang.NumberFormatException;
  public static java.math.BigDecimal bigDecValue(java.lang.Object) throws java.lang.NumberFormatException;
  public static java.lang.String stringValue(java.lang.Object, boolean);
  public static java.lang.String stringValue(java.lang.Object);
  public static int getNumericType(java.lang.Object);
  public static java.lang.Object toArray(char, java.lang.Class);
  public static java.lang.Object toArray(byte, java.lang.Class);
  public static java.lang.Object toArray(int, java.lang.Class);
  public static java.lang.Object toArray(long, java.lang.Class);
  public static java.lang.Object toArray(float, java.lang.Class);
  public static java.lang.Object toArray(double, java.lang.Class);
  public static java.lang.Object toArray(boolean, java.lang.Class);
  public static java.lang.Object convertValue(char, java.lang.Class);
  public static java.lang.Object convertValue(byte, java.lang.Class);
  public static java.lang.Object convertValue(int, java.lang.Class);
  public static java.lang.Object convertValue(long, java.lang.Class);
  public static java.lang.Object convertValue(float, java.lang.Class);
  public static java.lang.Object convertValue(double, java.lang.Class);
  public static java.lang.Object convertValue(boolean, java.lang.Class);
  public static java.lang.Object convertValue(char, java.lang.Class, boolean);
  public static java.lang.Object convertValue(byte, java.lang.Class, boolean);
  public static java.lang.Object convertValue(int, java.lang.Class, boolean);
  public static java.lang.Object convertValue(long, java.lang.Class, boolean);
  public static java.lang.Object convertValue(float, java.lang.Class, boolean);
  public static java.lang.Object convertValue(double, java.lang.Class, boolean);
  public static java.lang.Object convertValue(boolean, java.lang.Class, boolean);
  public static java.lang.Object toArray(char, java.lang.Class, boolean);
  public static java.lang.Object toArray(byte, java.lang.Class, boolean);
  public static java.lang.Object toArray(int, java.lang.Class, boolean);
  public static java.lang.Object toArray(long, java.lang.Class, boolean);
  public static java.lang.Object toArray(float, java.lang.Class, boolean);
  public static java.lang.Object toArray(double, java.lang.Class, boolean);
  public static java.lang.Object toArray(boolean, java.lang.Class, boolean);
  public static java.lang.Object convertValue(java.lang.Object, java.lang.Class);
  public static java.lang.Object toArray(java.lang.Object, java.lang.Class);
  public static java.lang.Object toArray(java.lang.Object, java.lang.Class, boolean);
  public static java.lang.Object convertValue(java.lang.Object, java.lang.Class, boolean);
  public static int getIntValue(java.lang.Object);
  public static int getNumericType(java.lang.Object, java.lang.Object);
  public static int getNumericType(int, int, boolean);
  public static int getNumericType(java.lang.Object, java.lang.Object, boolean);
  public static java.lang.Number newInteger(int, long);
  public static java.lang.Number newReal(int, double);
  public static java.lang.Object binaryOr(java.lang.Object, java.lang.Object);
  public static java.lang.Object binaryXor(java.lang.Object, java.lang.Object);
  public static java.lang.Object binaryAnd(java.lang.Object, java.lang.Object);
  public static boolean equal(java.lang.Object, java.lang.Object);
  public static boolean less(java.lang.Object, java.lang.Object);
  public static boolean greater(java.lang.Object, java.lang.Object);
  public static boolean in(java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public static java.lang.Object shiftLeft(java.lang.Object, java.lang.Object);
  public static java.lang.Object shiftRight(java.lang.Object, java.lang.Object);
  public static java.lang.Object unsignedShiftRight(java.lang.Object, java.lang.Object);
  public static java.lang.Object add(java.lang.Object, java.lang.Object);
  public static java.lang.Object subtract(java.lang.Object, java.lang.Object);
  public static java.lang.Object multiply(java.lang.Object, java.lang.Object);
  public static java.lang.Object divide(java.lang.Object, java.lang.Object);
  public static java.lang.Object remainder(java.lang.Object, java.lang.Object);
  public static java.lang.Object negate(java.lang.Object);
  public static java.lang.Object bitNegate(java.lang.Object);
  public static java.lang.String getEscapeString(java.lang.String);
  public static java.lang.String getEscapedChar(char);
  public static java.lang.Object returnValue(java.lang.Object, java.lang.Object);
  public static java.lang.RuntimeException castToRuntime(java.lang.Throwable);
}
```

## `com.feilong.lib.ognl.OgnlParser`

```java
public class com.feilong.lib.ognl.OgnlParser implements com.feilong.lib.ognl.OgnlParserTreeConstants,com.feilong.lib.ognl.OgnlParserConstants {
  public final com.feilong.lib.ognl.Node topLevelExpression() throws com.feilong.lib.ognl.ParseException;
  public final void expression() throws com.feilong.lib.ognl.ParseException;
  public final void assignmentExpression() throws com.feilong.lib.ognl.ParseException;
  public final void conditionalTestExpression() throws com.feilong.lib.ognl.ParseException;
  public final void logicalOrExpression() throws com.feilong.lib.ognl.ParseException;
  public final void logicalAndExpression() throws com.feilong.lib.ognl.ParseException;
  public final void inclusiveOrExpression() throws com.feilong.lib.ognl.ParseException;
  public final void exclusiveOrExpression() throws com.feilong.lib.ognl.ParseException;
  public final void andExpression() throws com.feilong.lib.ognl.ParseException;
  public final void equalityExpression() throws com.feilong.lib.ognl.ParseException;
  public final void relationalExpression() throws com.feilong.lib.ognl.ParseException;
  public final void shiftExpression() throws com.feilong.lib.ognl.ParseException;
  public final void additiveExpression() throws com.feilong.lib.ognl.ParseException;
  public final void multiplicativeExpression() throws com.feilong.lib.ognl.ParseException;
  public final void unaryExpression() throws com.feilong.lib.ognl.ParseException;
  public final void navigationChain() throws com.feilong.lib.ognl.ParseException;
  public final void primaryExpression() throws com.feilong.lib.ognl.ParseException;
  public final void keyValueExpression() throws com.feilong.lib.ognl.ParseException;
  public final void staticReference() throws com.feilong.lib.ognl.ParseException;
  public final java.lang.String classReference() throws com.feilong.lib.ognl.ParseException;
  public final java.lang.String className() throws com.feilong.lib.ognl.ParseException;
  public final void constructorCall() throws com.feilong.lib.ognl.ParseException;
  public final void propertyName() throws com.feilong.lib.ognl.ParseException;
  public final void staticMethodCall(java.lang.String) throws com.feilong.lib.ognl.ParseException;
  public final void methodCall() throws com.feilong.lib.ognl.ParseException;
  public final void projection() throws com.feilong.lib.ognl.ParseException;
  public final void selection() throws com.feilong.lib.ognl.ParseException;
  public final void selectAll() throws com.feilong.lib.ognl.ParseException;
  public final void selectFirst() throws com.feilong.lib.ognl.ParseException;
  public final void selectLast() throws com.feilong.lib.ognl.ParseException;
  public final void index() throws com.feilong.lib.ognl.ParseException;
  public com.feilong.lib.ognl.OgnlParser(java.io.InputStream);
  public com.feilong.lib.ognl.OgnlParser(java.io.InputStream, java.lang.String);
  public void ReInit(java.io.InputStream);
  public void ReInit(java.io.InputStream, java.lang.String);
  public com.feilong.lib.ognl.OgnlParser(java.io.Reader);
  public void ReInit(java.io.Reader);
  public com.feilong.lib.ognl.OgnlParser(com.feilong.lib.ognl.OgnlParserTokenManager);
  public void ReInit(com.feilong.lib.ognl.OgnlParserTokenManager);
  public final com.feilong.lib.ognl.Token getNextToken();
  public final com.feilong.lib.ognl.Token getToken(int);
  public com.feilong.lib.ognl.ParseException generateParseException();
  public final void enable_tracing();
  public final void disable_tracing();
}
```

## `com.feilong.lib.ognl.OgnlParserTokenManager`

```java
public class com.feilong.lib.ognl.OgnlParserTokenManager implements com.feilong.lib.ognl.OgnlParserConstants {
  public void setDebugStream(java.io.PrintStream);
  public com.feilong.lib.ognl.OgnlParserTokenManager(com.feilong.lib.ognl.JavaCharStream);
  public com.feilong.lib.ognl.OgnlParserTokenManager(com.feilong.lib.ognl.JavaCharStream, int);
  public void ReInit(com.feilong.lib.ognl.JavaCharStream);
  public void ReInit(com.feilong.lib.ognl.JavaCharStream, int);
  public void SwitchTo(int);
  public com.feilong.lib.ognl.Token getNextToken();
}
```

## `com.feilong.lib.ognl.OgnlRuntime`

```java
public class com.feilong.lib.ognl.OgnlRuntime {
  public com.feilong.lib.ognl.OgnlRuntime();
  public static void clearCache();
  public static void clearAdditionalCache();
  public static java.lang.String getNumericValueGetter(java.lang.Class);
  public static java.lang.Class getPrimitiveWrapperClass(java.lang.Class);
  public static java.lang.String getNumericLiteral(java.lang.Class);
  public static com.feilong.lib.ognl.enhance.OgnlExpressionCompiler getCompiler();
  public static java.lang.Class getTargetClass(java.lang.Object);
  public static boolean areArgsCompatible(java.lang.Object[], java.lang.Class[]);
  public static final boolean isMoreSpecific(java.lang.Class[], java.lang.Class[]);
  public static java.lang.Class classForName(com.feilong.lib.ognl.OgnlContext, java.lang.String) throws java.lang.ClassNotFoundException;
  public static boolean isInstance(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.String) throws com.feilong.lib.ognl.OgnlException;
  public static java.lang.Object getPrimitiveDefaultValue(java.lang.Class);
  public static java.lang.Object getNumericDefaultValue(java.lang.Class);
  public static java.lang.reflect.Constructor getConvertedConstructorAndArgs(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.util.List, java.lang.Object[], java.lang.Object[]);
  public static java.lang.Object callAppropriateMethod(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object, java.lang.String, java.lang.String, java.util.List, java.lang.Object[]) throws com.feilong.lib.ognl.MethodFailedException;
  public static java.lang.Object callStaticMethod(com.feilong.lib.ognl.OgnlContext, java.lang.String, java.lang.String, java.lang.Object[]) throws com.feilong.lib.ognl.OgnlException;
  public static java.lang.Object callMethod(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.String, java.lang.Object[]) throws com.feilong.lib.ognl.OgnlException;
  public static java.lang.Object callConstructor(com.feilong.lib.ognl.OgnlContext, java.lang.String, java.lang.Object[]) throws com.feilong.lib.ognl.OgnlException;
  public static final java.lang.Object getMethodValue(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.String, boolean) throws com.feilong.lib.ognl.OgnlException, java.lang.IllegalAccessException, java.lang.NoSuchMethodException, java.beans.IntrospectionException;
  public static boolean setMethodValue(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.String, java.lang.Object, boolean) throws com.feilong.lib.ognl.OgnlException, java.lang.IllegalAccessException, java.lang.NoSuchMethodException, java.beans.IntrospectionException;
  public static java.util.List getConstructors(java.lang.Class);
  public static java.util.List getMethods(java.lang.Class, java.lang.String, boolean);
  public static java.lang.reflect.Field getField(java.lang.Class, java.lang.String);
  public static java.lang.Object getFieldValue(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.String, boolean) throws java.lang.NoSuchFieldException;
  public static boolean setFieldValue(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.String, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public static java.lang.Object getStaticField(com.feilong.lib.ognl.OgnlContext, java.lang.String, java.lang.String) throws com.feilong.lib.ognl.OgnlException;
  public static final boolean hasGetProperty(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object) throws java.beans.IntrospectionException, com.feilong.lib.ognl.OgnlException;
  public static final boolean hasSetProperty(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object) throws java.beans.IntrospectionException, com.feilong.lib.ognl.OgnlException;
  public static java.util.Map getPropertyDescriptors(java.lang.Class) throws java.beans.IntrospectionException, com.feilong.lib.ognl.OgnlException;
  public static java.beans.PropertyDescriptor getPropertyDescriptor(java.lang.Class, java.lang.String) throws java.beans.IntrospectionException, com.feilong.lib.ognl.OgnlException;
  public static void setMethodAccessor(java.lang.Class, com.feilong.lib.ognl.MethodAccessor);
  public static com.feilong.lib.ognl.MethodAccessor getMethodAccessor(java.lang.Class) throws com.feilong.lib.ognl.OgnlException;
  public static void setPropertyAccessor(java.lang.Class, com.feilong.lib.ognl.PropertyAccessor);
  public static com.feilong.lib.ognl.PropertyAccessor getPropertyAccessor(java.lang.Class) throws com.feilong.lib.ognl.OgnlException;
  public static com.feilong.lib.ognl.ElementsAccessor getElementsAccessor(java.lang.Class) throws com.feilong.lib.ognl.OgnlException;
  public static void setElementsAccessor(java.lang.Class, com.feilong.lib.ognl.ElementsAccessor);
  public static com.feilong.lib.ognl.NullHandler getNullHandler(java.lang.Class) throws com.feilong.lib.ognl.OgnlException;
  public static void setNullHandler(java.lang.Class, com.feilong.lib.ognl.NullHandler);
  public static java.lang.Object getProperty(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public static void setProperty(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public static int getIndexedPropertyType(com.feilong.lib.ognl.OgnlContext, java.lang.Class, java.lang.String) throws com.feilong.lib.ognl.OgnlException;
  public static java.lang.Object getIndexedProperty(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.String, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public static void setIndexedProperty(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.String, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public static com.feilong.lib.ognl.EvaluationPool getEvaluationPool();
  public static java.lang.reflect.Method getMethod(com.feilong.lib.ognl.OgnlContext, java.lang.Class, java.lang.String, com.feilong.lib.ognl.Node[], boolean) throws java.lang.Exception;
  public static java.lang.reflect.Method getReadMethod(java.lang.Class, java.lang.String);
  public static java.lang.reflect.Method getReadMethod(java.lang.Class, java.lang.String, java.lang.Class[]);
  public static java.lang.reflect.Method getWriteMethod(java.lang.Class, java.lang.String);
  public static java.lang.reflect.Method getWriteMethod(java.lang.Class, java.lang.String, java.lang.Class[]);
  public static java.beans.PropertyDescriptor getProperty(java.lang.Class, java.lang.String);
  public static boolean isBoolean(java.lang.String);
  public static boolean shouldConvertNumericTypes(com.feilong.lib.ognl.OgnlContext);
  public static java.lang.String getChildSource(com.feilong.lib.ognl.OgnlContext, java.lang.Object, com.feilong.lib.ognl.Node) throws com.feilong.lib.ognl.OgnlException;
  public static java.lang.String getChildSource(com.feilong.lib.ognl.OgnlContext, java.lang.Object, com.feilong.lib.ognl.Node, boolean) throws com.feilong.lib.ognl.OgnlException;
  public static boolean usingJDK9PlusAccessHandler();
}
```

## `com.feilong.lib.ognl.ParseException`

```java
public class com.feilong.lib.ognl.ParseException extends java.lang.Exception {
  public com.feilong.lib.ognl.ParseException(com.feilong.lib.ognl.Token, int[][], java.lang.String[]);
  public com.feilong.lib.ognl.ParseException();
  public com.feilong.lib.ognl.ParseException(java.lang.String);
  public java.lang.String getMessage();
}
```

## `com.feilong.lib.ognl.PropertyAccessor`

```java
public interface com.feilong.lib.ognl.PropertyAccessor {
  public abstract java.lang.Object getProperty(java.util.Map, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public abstract void setProperty(java.util.Map, java.lang.Object, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public abstract java.lang.String getSourceAccessor(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object);
  public abstract java.lang.String getSourceSetter(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object);
}
```

## `com.feilong.lib.ognl.SetPropertyAccessor`

```java
public class com.feilong.lib.ognl.SetPropertyAccessor extends com.feilong.lib.ognl.ObjectPropertyAccessor implements com.feilong.lib.ognl.PropertyAccessor {
  public com.feilong.lib.ognl.SetPropertyAccessor();
  public java.lang.Object getProperty(java.util.Map, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
}
```

## `com.feilong.lib.ognl.SimpleNode`

```java
public abstract class com.feilong.lib.ognl.SimpleNode implements com.feilong.lib.ognl.Node,java.io.Serializable {
  public com.feilong.lib.ognl.SimpleNode(int);
  public com.feilong.lib.ognl.SimpleNode(com.feilong.lib.ognl.OgnlParser, int);
  public void jjtOpen();
  public void jjtClose();
  public void jjtSetParent(com.feilong.lib.ognl.Node);
  public com.feilong.lib.ognl.Node jjtGetParent();
  public void jjtAddChild(com.feilong.lib.ognl.Node, int);
  public com.feilong.lib.ognl.Node jjtGetChild(int);
  public int jjtGetNumChildren();
  public java.lang.String toString();
  public java.lang.String toString(java.lang.String);
  public java.lang.String toGetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public java.lang.String toSetSourceString(com.feilong.lib.ognl.OgnlContext, java.lang.Object);
  public void dump(java.io.PrintWriter, java.lang.String);
  public int getIndexInParent();
  public com.feilong.lib.ognl.Node getNextSibling();
  public final java.lang.Object getValue(com.feilong.lib.ognl.OgnlContext, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public final void setValue(com.feilong.lib.ognl.OgnlContext, java.lang.Object, java.lang.Object) throws com.feilong.lib.ognl.OgnlException;
  public boolean isNodeConstant(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public boolean isConstant(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public boolean isNodeSimpleProperty(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public boolean isSimpleProperty(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public boolean isSimpleNavigationChain(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public boolean isEvalChain(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public boolean isSequence(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public boolean isOperation(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public boolean isChain(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public boolean isSimpleMethod(com.feilong.lib.ognl.OgnlContext) throws com.feilong.lib.ognl.OgnlException;
  public com.feilong.lib.ognl.enhance.ExpressionAccessor getAccessor();
  public void setAccessor(com.feilong.lib.ognl.enhance.ExpressionAccessor);
}
```

## `com.feilong.lib.ognl.Token`

```java
public class com.feilong.lib.ognl.Token {
  public java.lang.Object getValue();
  public com.feilong.lib.ognl.Token();
  public com.feilong.lib.ognl.Token(int);
  public com.feilong.lib.ognl.Token(int, java.lang.String);
  public java.lang.String toString();
  public static com.feilong.lib.ognl.Token newToken(int, java.lang.String);
  public static com.feilong.lib.ognl.Token newToken(int);
}
```

## `com.feilong.lib.ognl.TokenMgrError`

```java
public class com.feilong.lib.ognl.TokenMgrError extends java.lang.Error {
  public java.lang.String getMessage();
  public com.feilong.lib.ognl.TokenMgrError();
  public com.feilong.lib.ognl.TokenMgrError(java.lang.String, int);
  public com.feilong.lib.ognl.TokenMgrError(boolean, int, int, int, java.lang.String, char, int);
}
```

## `com.feilong.lib.ognl.TypeConverter`

```java
public interface com.feilong.lib.ognl.TypeConverter {
  public abstract java.lang.Object convertValue(java.util.Map, java.lang.Object, java.lang.reflect.Member, java.lang.String, java.lang.Object, java.lang.Class);
}
```
