# cn.hutool.extra.template.engine.freemarker

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.template.engine.freemarker.FreemarkerEngine`

```java
public class cn.hutool.extra.template.engine.freemarker.FreemarkerEngine implements cn.hutool.extra.template.TemplateEngine {
  public cn.hutool.extra.template.engine.freemarker.FreemarkerEngine();
  public cn.hutool.extra.template.engine.freemarker.FreemarkerEngine(cn.hutool.extra.template.TemplateConfig);
  public cn.hutool.extra.template.engine.freemarker.FreemarkerEngine(freemarker.template.Configuration);
  public cn.hutool.extra.template.TemplateEngine init(cn.hutool.extra.template.TemplateConfig);
  public cn.hutool.extra.template.Template getTemplate(java.lang.String);
  public freemarker.template.Configuration getConfiguration();
}
```

## `cn.hutool.extra.template.engine.freemarker.FreemarkerTemplate`

```java
public class cn.hutool.extra.template.engine.freemarker.FreemarkerTemplate extends cn.hutool.extra.template.AbstractTemplate implements java.io.Serializable {
  public static cn.hutool.extra.template.engine.freemarker.FreemarkerTemplate wrap(freemarker.template.Template);
  public cn.hutool.extra.template.engine.freemarker.FreemarkerTemplate(freemarker.template.Template);
  public void render(java.util.Map<?, ?>, java.io.Writer);
  public void render(java.util.Map<?, ?>, java.io.OutputStream);
}
```

## `cn.hutool.extra.template.engine.freemarker.SimpleStringTemplateLoader`

```java
public class cn.hutool.extra.template.engine.freemarker.SimpleStringTemplateLoader implements freemarker.cache.TemplateLoader {
  public cn.hutool.extra.template.engine.freemarker.SimpleStringTemplateLoader();
  public java.lang.Object findTemplateSource(java.lang.String);
  public long getLastModified(java.lang.Object);
  public java.io.Reader getReader(java.lang.Object, java.lang.String);
  public void closeTemplateSource(java.lang.Object);
}
```
