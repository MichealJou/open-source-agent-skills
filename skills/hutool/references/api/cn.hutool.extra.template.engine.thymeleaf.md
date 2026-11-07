# cn.hutool.extra.template.engine.thymeleaf

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.template.engine.thymeleaf.ThymeleafEngine`

```java
public class cn.hutool.extra.template.engine.thymeleaf.ThymeleafEngine implements cn.hutool.extra.template.TemplateEngine {
  public cn.hutool.extra.template.engine.thymeleaf.ThymeleafEngine();
  public cn.hutool.extra.template.engine.thymeleaf.ThymeleafEngine(cn.hutool.extra.template.TemplateConfig);
  public cn.hutool.extra.template.engine.thymeleaf.ThymeleafEngine(org.thymeleaf.TemplateEngine);
  public cn.hutool.extra.template.TemplateEngine init(cn.hutool.extra.template.TemplateConfig);
  public cn.hutool.extra.template.Template getTemplate(java.lang.String);
  public org.thymeleaf.TemplateEngine getRawEngine();
}
```

## `cn.hutool.extra.template.engine.thymeleaf.ThymeleafTemplate`

```java
public class cn.hutool.extra.template.engine.thymeleaf.ThymeleafTemplate extends cn.hutool.extra.template.AbstractTemplate implements java.io.Serializable {
  public static cn.hutool.extra.template.engine.thymeleaf.ThymeleafTemplate wrap(org.thymeleaf.TemplateEngine, java.lang.String, java.nio.charset.Charset);
  public cn.hutool.extra.template.engine.thymeleaf.ThymeleafTemplate(org.thymeleaf.TemplateEngine, java.lang.String, java.nio.charset.Charset);
  public void render(java.util.Map<?, ?>, java.io.Writer);
  public void render(java.util.Map<?, ?>, java.io.OutputStream);
}
```
