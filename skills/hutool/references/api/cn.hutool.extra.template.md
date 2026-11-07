# cn.hutool.extra.template

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.template.AbstractTemplate`

```java
public abstract class cn.hutool.extra.template.AbstractTemplate implements cn.hutool.extra.template.Template {
  public cn.hutool.extra.template.AbstractTemplate();
  public void render(java.util.Map<?, ?>, java.io.File);
  public java.lang.String render(java.util.Map<?, ?>);
}
```

## `cn.hutool.extra.template.Template`

```java
public interface cn.hutool.extra.template.Template {
  public abstract void render(java.util.Map<?, ?>, java.io.Writer);
  public abstract void render(java.util.Map<?, ?>, java.io.OutputStream);
  public abstract void render(java.util.Map<?, ?>, java.io.File);
  public abstract java.lang.String render(java.util.Map<?, ?>);
}
```

## `cn.hutool.extra.template.TemplateConfig`

```java
public class cn.hutool.extra.template.TemplateConfig implements java.io.Serializable {
  public cn.hutool.extra.template.TemplateConfig();
  public cn.hutool.extra.template.TemplateConfig(java.lang.String);
  public cn.hutool.extra.template.TemplateConfig(java.lang.String, cn.hutool.extra.template.TemplateConfig$ResourceMode);
  public cn.hutool.extra.template.TemplateConfig(java.nio.charset.Charset, java.lang.String, cn.hutool.extra.template.TemplateConfig$ResourceMode);
  public java.nio.charset.Charset getCharset();
  public java.lang.String getCharsetStr();
  public void setCharset(java.nio.charset.Charset);
  public java.lang.String getPath();
  public void setPath(java.lang.String);
  public cn.hutool.extra.template.TemplateConfig$ResourceMode getResourceMode();
  public void setResourceMode(cn.hutool.extra.template.TemplateConfig$ResourceMode);
  public java.lang.Class<? extends cn.hutool.extra.template.TemplateEngine> getCustomEngine();
  public cn.hutool.extra.template.TemplateConfig setCustomEngine(java.lang.Class<? extends cn.hutool.extra.template.TemplateEngine>);
  public boolean isUseCache();
  public cn.hutool.extra.template.TemplateConfig setUseCache(boolean);
  public boolean equals(java.lang.Object);
  public int hashCode();
}
```

## `cn.hutool.extra.template.TemplateConfig$ResourceMode`

```java
public final class cn.hutool.extra.template.TemplateConfig$ResourceMode extends java.lang.Enum<cn.hutool.extra.template.TemplateConfig$ResourceMode> {
  public static cn.hutool.extra.template.TemplateConfig$ResourceMode[] values();
  public static cn.hutool.extra.template.TemplateConfig$ResourceMode valueOf(java.lang.String);
}
```

## `cn.hutool.extra.template.TemplateEngine`

```java
public interface cn.hutool.extra.template.TemplateEngine {
  public abstract cn.hutool.extra.template.TemplateEngine init(cn.hutool.extra.template.TemplateConfig);
  public abstract cn.hutool.extra.template.Template getTemplate(java.lang.String);
}
```

## `cn.hutool.extra.template.TemplateException`

```java
public class cn.hutool.extra.template.TemplateException extends java.lang.RuntimeException {
  public cn.hutool.extra.template.TemplateException(java.lang.Throwable);
  public cn.hutool.extra.template.TemplateException(java.lang.String);
  public cn.hutool.extra.template.TemplateException(java.lang.String, java.lang.Object...);
  public cn.hutool.extra.template.TemplateException(java.lang.String, java.lang.Throwable);
  public cn.hutool.extra.template.TemplateException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.extra.template.TemplateException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.extra.template.TemplateUtil`

```java
public class cn.hutool.extra.template.TemplateUtil {
  public cn.hutool.extra.template.TemplateUtil();
  public static cn.hutool.extra.template.TemplateEngine createEngine();
  public static cn.hutool.extra.template.TemplateEngine createEngine(cn.hutool.extra.template.TemplateConfig);
}
```
