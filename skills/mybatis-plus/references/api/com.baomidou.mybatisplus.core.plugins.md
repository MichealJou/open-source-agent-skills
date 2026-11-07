# com.baomidou.mybatisplus.core.plugins

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.core.plugins.IgnoreStrategy`

```java
public class com.baomidou.mybatisplus.core.plugins.IgnoreStrategy {
  public static com.baomidou.mybatisplus.core.plugins.IgnoreStrategy$IgnoreStrategyBuilder builder();
  public java.lang.Boolean getTenantLine();
  public java.lang.Boolean getDynamicTableName();
  public java.lang.Boolean getBlockAttack();
  public java.lang.Boolean getIllegalSql();
  public java.lang.Boolean getDataPermission();
  public java.util.Map<java.lang.String, java.lang.Boolean> getOthers();
  public void setTenantLine(java.lang.Boolean);
  public void setDynamicTableName(java.lang.Boolean);
  public void setBlockAttack(java.lang.Boolean);
  public void setIllegalSql(java.lang.Boolean);
  public void setDataPermission(java.lang.Boolean);
  public void setOthers(java.util.Map<java.lang.String, java.lang.Boolean>);
}
```

## `com.baomidou.mybatisplus.core.plugins.IgnoreStrategy$IgnoreStrategyBuilder`

```java
public class com.baomidou.mybatisplus.core.plugins.IgnoreStrategy$IgnoreStrategyBuilder {
  public com.baomidou.mybatisplus.core.plugins.IgnoreStrategy$IgnoreStrategyBuilder tenantLine(java.lang.Boolean);
  public com.baomidou.mybatisplus.core.plugins.IgnoreStrategy$IgnoreStrategyBuilder dynamicTableName(java.lang.Boolean);
  public com.baomidou.mybatisplus.core.plugins.IgnoreStrategy$IgnoreStrategyBuilder blockAttack(java.lang.Boolean);
  public com.baomidou.mybatisplus.core.plugins.IgnoreStrategy$IgnoreStrategyBuilder illegalSql(java.lang.Boolean);
  public com.baomidou.mybatisplus.core.plugins.IgnoreStrategy$IgnoreStrategyBuilder dataPermission(java.lang.Boolean);
  public com.baomidou.mybatisplus.core.plugins.IgnoreStrategy$IgnoreStrategyBuilder others(java.util.Map<java.lang.String, java.lang.Boolean>);
  public com.baomidou.mybatisplus.core.plugins.IgnoreStrategy build();
  public java.lang.String toString();
}
```

## `com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper`

```java
public abstract class com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper {
  public com.baomidou.mybatisplus.core.plugins.InterceptorIgnoreHelper();
  public static void handle(com.baomidou.mybatisplus.core.plugins.IgnoreStrategy);
  public static void clearIgnoreStrategy();
  public static boolean hasIgnoreStrategy();
  public static synchronized com.baomidou.mybatisplus.core.plugins.IgnoreStrategy initSqlParserInfoCache(java.lang.Class<?>);
  public static com.baomidou.mybatisplus.core.plugins.IgnoreStrategy getIgnoreStrategy(java.lang.String);
  public static <T> T execute(com.baomidou.mybatisplus.core.plugins.IgnoreStrategy, java.util.function.Supplier<T>);
  public static void execute(com.baomidou.mybatisplus.core.plugins.IgnoreStrategy, java.lang.Runnable);
  public static com.baomidou.mybatisplus.core.plugins.IgnoreStrategy findIgnoreStrategy(java.lang.Class<?>, java.lang.reflect.Method);
  public static void initSqlParserInfoCache(com.baomidou.mybatisplus.core.plugins.IgnoreStrategy, java.lang.String, java.lang.reflect.Method);
  public static boolean willIgnoreTenantLine(java.lang.String);
  public static boolean willIgnoreDynamicTableName(java.lang.String);
  public static boolean willIgnoreBlockAttack(java.lang.String);
  public static boolean willIgnoreIllegalSql(java.lang.String);
  public static boolean willIgnoreDataPermission(java.lang.String);
  public static boolean willIgnoreOthersByKey(java.lang.String, java.lang.String);
  public static boolean willIgnore(java.lang.String, java.util.function.Function<com.baomidou.mybatisplus.core.plugins.IgnoreStrategy, java.lang.Boolean>);
}
```
