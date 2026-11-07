# com.baomidou.mybatisplus.extension.scripting

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.scripting.MybatisFreeMarkerLanguageDriver`

```java
public class com.baomidou.mybatisplus.extension.scripting.MybatisFreeMarkerLanguageDriver extends org.mybatis.scripting.freemarker.FreeMarkerLanguageDriver {
  public com.baomidou.mybatisplus.extension.scripting.MybatisFreeMarkerLanguageDriver(org.mybatis.scripting.freemarker.FreeMarkerLanguageDriverConfig);
  public org.apache.ibatis.executor.parameter.ParameterHandler createParameterHandler(org.apache.ibatis.mapping.MappedStatement, java.lang.Object, org.apache.ibatis.mapping.BoundSql);
  public com.baomidou.mybatisplus.extension.scripting.MybatisFreeMarkerLanguageDriver();
}
```

## `com.baomidou.mybatisplus.extension.scripting.MybatisThymeleafLanguageDriver`

```java
public class com.baomidou.mybatisplus.extension.scripting.MybatisThymeleafLanguageDriver extends org.mybatis.scripting.thymeleaf.ThymeleafLanguageDriver {
  public com.baomidou.mybatisplus.extension.scripting.MybatisThymeleafLanguageDriver(org.mybatis.scripting.thymeleaf.ThymeleafLanguageDriverConfig);
  public com.baomidou.mybatisplus.extension.scripting.MybatisThymeleafLanguageDriver(org.thymeleaf.ITemplateEngine);
  public org.apache.ibatis.executor.parameter.ParameterHandler createParameterHandler(org.apache.ibatis.mapping.MappedStatement, java.lang.Object, org.apache.ibatis.mapping.BoundSql);
  public com.baomidou.mybatisplus.extension.scripting.MybatisThymeleafLanguageDriver();
}
```

## `com.baomidou.mybatisplus.extension.scripting.MybatisVelocityLanguageDriver`

```java
public class com.baomidou.mybatisplus.extension.scripting.MybatisVelocityLanguageDriver extends org.mybatis.scripting.velocity.VelocityLanguageDriver {
  public com.baomidou.mybatisplus.extension.scripting.MybatisVelocityLanguageDriver(org.mybatis.scripting.velocity.VelocityLanguageDriverConfig);
  public org.apache.ibatis.executor.parameter.ParameterHandler createParameterHandler(org.apache.ibatis.mapping.MappedStatement, java.lang.Object, org.apache.ibatis.mapping.BoundSql);
  public com.baomidou.mybatisplus.extension.scripting.MybatisVelocityLanguageDriver();
}
```
