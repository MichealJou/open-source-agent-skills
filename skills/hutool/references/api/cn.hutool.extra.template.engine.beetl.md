# cn.hutool.extra.template.engine.beetl

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.template.engine.beetl.BeetlEngine`

```java
public class cn.hutool.extra.template.engine.beetl.BeetlEngine implements cn.hutool.extra.template.TemplateEngine {
  public cn.hutool.extra.template.engine.beetl.BeetlEngine();
  public cn.hutool.extra.template.engine.beetl.BeetlEngine(cn.hutool.extra.template.TemplateConfig);
  public cn.hutool.extra.template.engine.beetl.BeetlEngine(org.beetl.core.GroupTemplate);
  public cn.hutool.extra.template.TemplateEngine init(cn.hutool.extra.template.TemplateConfig);
  public cn.hutool.extra.template.Template getTemplate(java.lang.String);
  public org.beetl.core.GroupTemplate getRawEngine();
}
```

## `cn.hutool.extra.template.engine.beetl.BeetlTemplate`

```java
public class cn.hutool.extra.template.engine.beetl.BeetlTemplate extends cn.hutool.extra.template.AbstractTemplate implements java.io.Serializable {
  public static cn.hutool.extra.template.engine.beetl.BeetlTemplate wrap(org.beetl.core.Template);
  public cn.hutool.extra.template.engine.beetl.BeetlTemplate(org.beetl.core.Template);
  public void render(java.util.Map<?, ?>, java.io.Writer);
  public void render(java.util.Map<?, ?>, java.io.OutputStream);
}
```
