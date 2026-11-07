# com.baomidou.mybatisplus.extension

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.DynamicTableNameHandler`

```java
public class com.baomidou.mybatisplus.extension.DynamicTableNameHandler extends net.sf.jsqlparser.util.TablesNamesFinder<java.lang.Void> {
  public com.baomidou.mybatisplus.extension.DynamicTableNameHandler(java.lang.String, com.baomidou.mybatisplus.extension.plugins.handler.TableNameHandler);
  public <S> java.lang.Void visit(net.sf.jsqlparser.statement.create.index.CreateIndex, S);
  public <S> java.lang.Void visit(net.sf.jsqlparser.statement.create.view.CreateView, S);
  public <S> java.lang.Void visit(net.sf.jsqlparser.statement.drop.Drop, S);
  public java.lang.Object visit(net.sf.jsqlparser.statement.create.view.CreateView, java.lang.Object);
  public java.lang.Object visit(net.sf.jsqlparser.statement.create.index.CreateIndex, java.lang.Object);
  public java.lang.Object visit(net.sf.jsqlparser.statement.drop.Drop, java.lang.Object);
}
```

## `com.baomidou.mybatisplus.extension.MybatisMapWrapperFactory`

```java
public class com.baomidou.mybatisplus.extension.MybatisMapWrapperFactory implements org.apache.ibatis.reflection.wrapper.ObjectWrapperFactory {
  public com.baomidou.mybatisplus.extension.MybatisMapWrapperFactory();
  public boolean hasWrapperFor(java.lang.Object);
  public org.apache.ibatis.reflection.wrapper.ObjectWrapper getWrapperFor(org.apache.ibatis.reflection.MetaObject, java.lang.Object);
}
```
