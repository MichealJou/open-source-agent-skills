# com.baomidou.mybatisplus.core.injector

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.injector.AbstractMethod`

```java
public abstract class com.baomidou.mybatisplus.core.injector.AbstractMethod implements com.baomidou.mybatisplus.core.toolkit.Constants {
  public void inject(org.apache.ibatis.builder.MapperBuilderAssistant, java.lang.Class<?>, java.lang.Class<?>, com.baomidou.mybatisplus.core.metadata.TableInfo);
  public abstract org.apache.ibatis.mapping.MappedStatement injectMappedStatement(java.lang.Class<?>, java.lang.Class<?>, com.baomidou.mybatisplus.core.metadata.TableInfo);
  public org.apache.ibatis.mapping.SqlSource createSqlSource(org.apache.ibatis.session.Configuration, java.lang.String, java.lang.Class<?>);
}
```

## `com.baomidou.mybatisplus.core.injector.AbstractSqlInjector`

```java
public abstract class com.baomidou.mybatisplus.core.injector.AbstractSqlInjector implements com.baomidou.mybatisplus.core.injector.ISqlInjector {
  public com.baomidou.mybatisplus.core.injector.AbstractSqlInjector();
  public void inspectInject(org.apache.ibatis.builder.MapperBuilderAssistant, java.lang.Class<?>);
  public java.util.List<com.baomidou.mybatisplus.core.injector.AbstractMethod> getMethodList(java.lang.Class<?>, com.baomidou.mybatisplus.core.metadata.TableInfo);
  public java.util.List<com.baomidou.mybatisplus.core.injector.AbstractMethod> getMethodList(org.apache.ibatis.session.Configuration, java.lang.Class<?>, com.baomidou.mybatisplus.core.metadata.TableInfo);
}
```

## `com.baomidou.mybatisplus.core.injector.DefaultSqlInjector`

```java
public class com.baomidou.mybatisplus.core.injector.DefaultSqlInjector extends com.baomidou.mybatisplus.core.injector.AbstractSqlInjector {
  public com.baomidou.mybatisplus.core.injector.DefaultSqlInjector();
  public java.util.List<com.baomidou.mybatisplus.core.injector.AbstractMethod> getMethodList(org.apache.ibatis.session.Configuration, java.lang.Class<?>, com.baomidou.mybatisplus.core.metadata.TableInfo);
}
```

## `com.baomidou.mybatisplus.core.injector.ISqlInjector`

```java
public interface com.baomidou.mybatisplus.core.injector.ISqlInjector {
  public abstract void inspectInject(org.apache.ibatis.builder.MapperBuilderAssistant, java.lang.Class<?>);
}
```

## `com.baomidou.mybatisplus.core.injector.SqlRunnerInjector`

```java
public class com.baomidou.mybatisplus.core.injector.SqlRunnerInjector {
  public com.baomidou.mybatisplus.core.injector.SqlRunnerInjector();
  public void inject(org.apache.ibatis.session.Configuration);
}
```
