# cn.hutool.script

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.script.FullSupportScriptEngine`

```java
public class cn.hutool.script.FullSupportScriptEngine implements javax.script.ScriptEngine,javax.script.Compilable,javax.script.Invocable {
  public cn.hutool.script.FullSupportScriptEngine(javax.script.ScriptEngine);
  public cn.hutool.script.FullSupportScriptEngine(java.lang.String);
  public java.lang.Object invokeMethod(java.lang.Object, java.lang.String, java.lang.Object...) throws javax.script.ScriptException, java.lang.NoSuchMethodException;
  public java.lang.Object invokeFunction(java.lang.String, java.lang.Object...) throws javax.script.ScriptException, java.lang.NoSuchMethodException;
  public <T> T getInterface(java.lang.Class<T>);
  public <T> T getInterface(java.lang.Object, java.lang.Class<T>);
  public javax.script.CompiledScript compile(java.lang.String) throws javax.script.ScriptException;
  public javax.script.CompiledScript compile(java.io.Reader) throws javax.script.ScriptException;
  public java.lang.Object eval(java.lang.String, javax.script.ScriptContext) throws javax.script.ScriptException;
  public java.lang.Object eval(java.io.Reader, javax.script.ScriptContext) throws javax.script.ScriptException;
  public java.lang.Object eval(java.lang.String) throws javax.script.ScriptException;
  public java.lang.Object eval(java.io.Reader) throws javax.script.ScriptException;
  public java.lang.Object eval(java.lang.String, javax.script.Bindings) throws javax.script.ScriptException;
  public java.lang.Object eval(java.io.Reader, javax.script.Bindings) throws javax.script.ScriptException;
  public void put(java.lang.String, java.lang.Object);
  public java.lang.Object get(java.lang.String);
  public javax.script.Bindings getBindings(int);
  public void setBindings(javax.script.Bindings, int);
  public javax.script.Bindings createBindings();
  public javax.script.ScriptContext getContext();
  public void setContext(javax.script.ScriptContext);
  public javax.script.ScriptEngineFactory getFactory();
}
```

## `cn.hutool.script.JavaScriptEngine`

```java
public class cn.hutool.script.JavaScriptEngine extends cn.hutool.script.FullSupportScriptEngine {
  public cn.hutool.script.JavaScriptEngine();
  public static cn.hutool.script.JavaScriptEngine instance();
  public java.lang.Object invokeMethod(java.lang.Object, java.lang.String, java.lang.Object...) throws javax.script.ScriptException, java.lang.NoSuchMethodException;
  public java.lang.Object invokeFunction(java.lang.String, java.lang.Object...) throws javax.script.ScriptException, java.lang.NoSuchMethodException;
  public <T> T getInterface(java.lang.Class<T>);
  public <T> T getInterface(java.lang.Object, java.lang.Class<T>);
  public javax.script.CompiledScript compile(java.lang.String) throws javax.script.ScriptException;
  public javax.script.CompiledScript compile(java.io.Reader) throws javax.script.ScriptException;
  public java.lang.Object eval(java.lang.String, javax.script.ScriptContext) throws javax.script.ScriptException;
  public java.lang.Object eval(java.io.Reader, javax.script.ScriptContext) throws javax.script.ScriptException;
  public java.lang.Object eval(java.lang.String) throws javax.script.ScriptException;
  public java.lang.Object eval(java.io.Reader) throws javax.script.ScriptException;
  public java.lang.Object eval(java.lang.String, javax.script.Bindings) throws javax.script.ScriptException;
  public java.lang.Object eval(java.io.Reader, javax.script.Bindings) throws javax.script.ScriptException;
  public void put(java.lang.String, java.lang.Object);
  public java.lang.Object get(java.lang.String);
  public javax.script.Bindings getBindings(int);
  public void setBindings(javax.script.Bindings, int);
  public javax.script.Bindings createBindings();
  public javax.script.ScriptContext getContext();
  public void setContext(javax.script.ScriptContext);
  public javax.script.ScriptEngineFactory getFactory();
}
```

## `cn.hutool.script.ScriptRuntimeException`

```java
public class cn.hutool.script.ScriptRuntimeException extends java.lang.RuntimeException {
  public cn.hutool.script.ScriptRuntimeException(java.lang.Throwable);
  public cn.hutool.script.ScriptRuntimeException(java.lang.String);
  public cn.hutool.script.ScriptRuntimeException(java.lang.String, java.lang.Object...);
  public cn.hutool.script.ScriptRuntimeException(java.lang.String, java.lang.Throwable);
  public cn.hutool.script.ScriptRuntimeException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.script.ScriptRuntimeException(java.lang.Throwable, java.lang.String, java.lang.Object...);
  public cn.hutool.script.ScriptRuntimeException(java.lang.String, java.lang.String, int);
  public cn.hutool.script.ScriptRuntimeException(java.lang.String, java.lang.String, int, int);
  public cn.hutool.script.ScriptRuntimeException(javax.script.ScriptException);
  public java.lang.String getMessage();
  public int getLineNumber();
  public int getColumnNumber();
  public java.lang.String getFileName();
}
```

## `cn.hutool.script.ScriptUtil`

```java
public class cn.hutool.script.ScriptUtil {
  public cn.hutool.script.ScriptUtil();
  public static javax.script.ScriptEngine getScript(java.lang.String);
  public static javax.script.ScriptEngine createScript(java.lang.String);
  public static cn.hutool.script.JavaScriptEngine getJavaScriptEngine();
  public static javax.script.ScriptEngine getJsEngine();
  public static javax.script.ScriptEngine createJsEngine();
  public static javax.script.ScriptEngine getPythonEngine();
  public static javax.script.ScriptEngine createPythonEngine();
  public static javax.script.ScriptEngine getLuaEngine();
  public static javax.script.ScriptEngine createLuaEngine();
  public static javax.script.ScriptEngine getGroovyEngine();
  public static javax.script.ScriptEngine createGroovyEngine();
  public static javax.script.Invocable evalInvocable(java.lang.String) throws cn.hutool.script.ScriptRuntimeException;
  public static java.lang.Object eval(java.lang.String) throws cn.hutool.script.ScriptRuntimeException;
  public static java.lang.Object eval(java.lang.String, javax.script.ScriptContext) throws cn.hutool.script.ScriptRuntimeException;
  public static java.lang.Object eval(java.lang.String, javax.script.Bindings) throws cn.hutool.script.ScriptRuntimeException;
  public static java.lang.Object invoke(java.lang.String, java.lang.String, java.lang.Object...);
  public static javax.script.CompiledScript compile(java.lang.String) throws cn.hutool.script.ScriptRuntimeException;
  public static javax.script.CompiledScript compile(javax.script.ScriptEngine, java.lang.String) throws javax.script.ScriptException;
}
```
