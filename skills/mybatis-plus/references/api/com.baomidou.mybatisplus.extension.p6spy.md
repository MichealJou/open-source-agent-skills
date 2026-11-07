# com.baomidou.mybatisplus.extension.p6spy

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.p6spy.MybatisPlusLogFactory`

```java
public class com.baomidou.mybatisplus.extension.p6spy.MybatisPlusLogFactory implements com.p6spy.engine.spy.P6Factory {
  public com.baomidou.mybatisplus.extension.p6spy.MybatisPlusLogFactory();
  public com.p6spy.engine.spy.P6LoadableOptions getOptions(com.p6spy.engine.spy.option.P6OptionsRepository);
  public com.p6spy.engine.event.JdbcEventListener getJdbcEventListener();
}
```

## `com.baomidou.mybatisplus.extension.p6spy.MybatisPlusLoggingEventListener`

```java
public class com.baomidou.mybatisplus.extension.p6spy.MybatisPlusLoggingEventListener extends com.p6spy.engine.logging.LoggingEventListener {
  public com.baomidou.mybatisplus.extension.p6spy.MybatisPlusLoggingEventListener();
  public static com.baomidou.mybatisplus.extension.p6spy.MybatisPlusLoggingEventListener getInstance();
  public void onAfterExecuteBatch(com.p6spy.engine.common.StatementInformation, long, int[], java.sql.SQLException);
}
```

## `com.baomidou.mybatisplus.extension.p6spy.P6SpyLogger`

```java
public class com.baomidou.mybatisplus.extension.p6spy.P6SpyLogger implements com.p6spy.engine.spy.appender.MessageFormattingStrategy {
  public com.baomidou.mybatisplus.extension.p6spy.P6SpyLogger();
  public java.lang.String formatMessage(int, java.lang.String, long, java.lang.String, java.lang.String, java.lang.String, java.lang.String);
}
```

## `com.baomidou.mybatisplus.extension.p6spy.StdoutLogger`

```java
public class com.baomidou.mybatisplus.extension.p6spy.StdoutLogger extends com.p6spy.engine.spy.appender.StdoutLogger {
  public com.baomidou.mybatisplus.extension.p6spy.StdoutLogger();
  public void logText(java.lang.String);
}
```
