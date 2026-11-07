# com.baomidou.mybatisplus.extension.injector.methods

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.injector.methods.AlwaysUpdateSomeColumnById`

```java
public class com.baomidou.mybatisplus.extension.injector.methods.AlwaysUpdateSomeColumnById extends com.baomidou.mybatisplus.core.injector.AbstractMethod {
  public com.baomidou.mybatisplus.extension.injector.methods.AlwaysUpdateSomeColumnById(java.lang.String, java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public com.baomidou.mybatisplus.extension.injector.methods.AlwaysUpdateSomeColumnById();
  public com.baomidou.mybatisplus.extension.injector.methods.AlwaysUpdateSomeColumnById(java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public org.apache.ibatis.mapping.MappedStatement injectMappedStatement(java.lang.Class<?>, java.lang.Class<?>, com.baomidou.mybatisplus.core.metadata.TableInfo);
  public com.baomidou.mybatisplus.extension.injector.methods.AlwaysUpdateSomeColumnById setPredicate(java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
}
```

## `com.baomidou.mybatisplus.extension.injector.methods.InsertBatchSomeColumn`

```java
public class com.baomidou.mybatisplus.extension.injector.methods.InsertBatchSomeColumn extends com.baomidou.mybatisplus.core.injector.AbstractMethod {
  public com.baomidou.mybatisplus.extension.injector.methods.InsertBatchSomeColumn();
  public com.baomidou.mybatisplus.extension.injector.methods.InsertBatchSomeColumn(java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public com.baomidou.mybatisplus.extension.injector.methods.InsertBatchSomeColumn(java.lang.String, java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
  public org.apache.ibatis.mapping.MappedStatement injectMappedStatement(java.lang.Class<?>, java.lang.Class<?>, com.baomidou.mybatisplus.core.metadata.TableInfo);
  public com.baomidou.mybatisplus.extension.injector.methods.InsertBatchSomeColumn setPredicate(java.util.function.Predicate<com.baomidou.mybatisplus.core.metadata.TableFieldInfo>);
}
```

## `com.baomidou.mybatisplus.extension.injector.methods.LogicDeleteBatchByIds`

```java
public class com.baomidou.mybatisplus.extension.injector.methods.LogicDeleteBatchByIds extends com.baomidou.mybatisplus.core.injector.methods.DeleteByIds {
  public com.baomidou.mybatisplus.extension.injector.methods.LogicDeleteBatchByIds();
  public com.baomidou.mybatisplus.extension.injector.methods.LogicDeleteBatchByIds(java.lang.String);
  public java.lang.String logicDeleteScript(com.baomidou.mybatisplus.core.metadata.TableInfo, com.baomidou.mybatisplus.core.enums.SqlMethod);
}
```

## `com.baomidou.mybatisplus.extension.injector.methods.LogicDeleteByIdWithFill`

```java
public class com.baomidou.mybatisplus.extension.injector.methods.LogicDeleteByIdWithFill extends com.baomidou.mybatisplus.core.injector.AbstractMethod {
  public com.baomidou.mybatisplus.extension.injector.methods.LogicDeleteByIdWithFill();
  public com.baomidou.mybatisplus.extension.injector.methods.LogicDeleteByIdWithFill(java.lang.String);
  public org.apache.ibatis.mapping.MappedStatement injectMappedStatement(java.lang.Class<?>, java.lang.Class<?>, com.baomidou.mybatisplus.core.metadata.TableInfo);
}
```

## `com.baomidou.mybatisplus.extension.injector.methods.Upsert`

```java
public class com.baomidou.mybatisplus.extension.injector.methods.Upsert extends com.baomidou.mybatisplus.core.injector.AbstractMethod {
  public com.baomidou.mybatisplus.extension.injector.methods.Upsert();
  public com.baomidou.mybatisplus.extension.injector.methods.Upsert(java.lang.String);
  public org.apache.ibatis.mapping.MappedStatement injectMappedStatement(java.lang.Class<?>, java.lang.Class<?>, com.baomidou.mybatisplus.core.metadata.TableInfo);
}
```
