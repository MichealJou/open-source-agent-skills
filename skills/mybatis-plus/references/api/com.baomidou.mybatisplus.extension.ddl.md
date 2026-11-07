# com.baomidou.mybatisplus.extension.ddl

版本：3.5.16。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `com.baomidou.mybatisplus.extension.ddl.DdlHelper`

```java
public class com.baomidou.mybatisplus.extension.ddl.DdlHelper {
  public com.baomidou.mybatisplus.extension.ddl.DdlHelper();
  public static void runScript(com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator, java.sql.Connection, java.util.List<java.lang.String>, boolean) throws java.sql.SQLException;
  public static void runScript(com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator, java.sql.Connection, java.util.List<java.lang.String>, boolean, com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler) throws java.sql.SQLException;
  public static void runScript(com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator, java.sql.Connection, java.util.List<java.lang.String>, java.util.function.Consumer<org.apache.ibatis.jdbc.ScriptRunner>, com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler) throws java.sql.SQLException;
  public static void runScript(com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator, java.sql.Connection, java.util.List<java.lang.String>, java.util.function.Consumer<org.apache.ibatis.jdbc.ScriptRunner>, boolean, com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler) throws java.sql.SQLException;
  public static void runScript(com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator, javax.sql.DataSource, java.util.List<java.lang.String>, boolean);
  public static void runScript(com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator, javax.sql.DataSource, java.util.List<java.lang.String>, boolean, com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler) throws java.sql.SQLException;
  public static void runScript(com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator, javax.sql.DataSource, java.util.List<java.lang.String>, java.util.function.Consumer<org.apache.ibatis.jdbc.ScriptRunner>, com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler) throws java.sql.SQLException;
  public static void runScript(com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator, javax.sql.DataSource, java.util.List<java.lang.String>, java.util.function.Consumer<org.apache.ibatis.jdbc.ScriptRunner>, boolean, com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler) throws java.sql.SQLException;
  public static java.io.InputStream getInputStream(java.lang.String) throws java.lang.Exception;
  public static org.apache.ibatis.jdbc.ScriptRunner getScriptRunner(java.sql.Connection, boolean);
  public static java.lang.String getDatabase(java.lang.String);
}
```

## `com.baomidou.mybatisplus.extension.ddl.DdlScript`

```java
public class com.baomidou.mybatisplus.extension.ddl.DdlScript {
  public com.baomidou.mybatisplus.extension.ddl.DdlScript(java.lang.String, java.lang.String, java.lang.String, java.lang.String);
  public com.baomidou.mybatisplus.extension.ddl.DdlScript(java.lang.String, java.lang.String, java.lang.String, java.lang.String, boolean);
  public com.baomidou.mybatisplus.extension.ddl.DdlScript(javax.sql.DataSource);
  public com.baomidou.mybatisplus.extension.ddl.DdlScript(javax.sql.DataSource, com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator);
  public com.baomidou.mybatisplus.extension.ddl.DdlScript(javax.sql.DataSource, com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator, boolean);
  public void run(java.util.List<java.lang.String>);
  public void run(java.util.List<java.lang.String>, boolean);
  public com.baomidou.mybatisplus.extension.ddl.DdlScript scriptRunner(java.util.function.Consumer<org.apache.ibatis.jdbc.ScriptRunner>);
  public void run(java.lang.String) throws java.lang.Exception;
  public void run(java.lang.String, java.lang.String) throws java.lang.Exception;
  public void run(java.io.Reader) throws java.lang.Exception;
  public void run(java.io.Reader, boolean) throws java.lang.Exception;
  public void run(java.io.Reader, boolean, java.lang.String) throws java.lang.Exception;
  public void run(java.sql.Connection, java.io.Reader, boolean, java.lang.String);
  public boolean execute(java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public boolean run(java.lang.String, java.util.function.Consumer<java.lang.String>);
  public boolean execute(java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.util.function.Consumer<java.lang.String>);
  public boolean run(java.lang.String, java.lang.String, java.util.function.Consumer<java.lang.String>);
}
```

## `com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler`

```java
public interface com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler {
  public abstract void handle(java.lang.String, java.lang.Exception) throws java.sql.SQLException;
}
```

## `com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler$PrintlnLogErrorHandler`

```java
public class com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler$PrintlnLogErrorHandler implements com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler {
  public com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler$PrintlnLogErrorHandler();
  public void handle(java.lang.String, java.lang.Exception);
}
```

## `com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler$ThrowsErrorHandler`

```java
public class com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler$ThrowsErrorHandler implements com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler {
  public com.baomidou.mybatisplus.extension.ddl.DdlScriptErrorHandler$ThrowsErrorHandler();
  public void handle(java.lang.String, java.lang.Exception) throws java.sql.SQLException;
}
```

## `com.baomidou.mybatisplus.extension.ddl.IDdl`

```java
public interface com.baomidou.mybatisplus.extension.ddl.IDdl {
  public abstract void runScript(java.util.function.Consumer<javax.sql.DataSource>);
  public default com.baomidou.mybatisplus.extension.ddl.history.IDdlGenerator getDdlGenerator();
  public abstract java.util.List<java.lang.String> getSqlFiles();
}
```

## `com.baomidou.mybatisplus.extension.ddl.SimpleDdl`

```java
public class com.baomidou.mybatisplus.extension.ddl.SimpleDdl implements com.baomidou.mybatisplus.extension.ddl.IDdl {
  public com.baomidou.mybatisplus.extension.ddl.SimpleDdl();
  public void runScript(java.util.function.Consumer<javax.sql.DataSource>);
  public java.util.List<java.lang.String> getSqlFiles();
}
```
