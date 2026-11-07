# cn.hutool.extra.template.engine.enjoy

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.template.engine.enjoy.EnjoyEngine`

```java
public class cn.hutool.extra.template.engine.enjoy.EnjoyEngine implements cn.hutool.extra.template.TemplateEngine {
  public cn.hutool.extra.template.engine.enjoy.EnjoyEngine();
  public cn.hutool.extra.template.engine.enjoy.EnjoyEngine(cn.hutool.extra.template.TemplateConfig);
  public cn.hutool.extra.template.engine.enjoy.EnjoyEngine(com.jfinal.template.Engine);
  public cn.hutool.extra.template.TemplateEngine init(cn.hutool.extra.template.TemplateConfig);
  public cn.hutool.extra.template.Template getTemplate(java.lang.String);
  public com.jfinal.template.Engine getRawEngine();
}
```

## `cn.hutool.extra.template.engine.enjoy.EnjoyTemplate`

```java
public class cn.hutool.extra.template.engine.enjoy.EnjoyTemplate extends cn.hutool.extra.template.AbstractTemplate implements java.io.Serializable {
  public static cn.hutool.extra.template.engine.enjoy.EnjoyTemplate wrap(com.jfinal.template.Template);
  public cn.hutool.extra.template.engine.enjoy.EnjoyTemplate(com.jfinal.template.Template);
  public void render(java.util.Map<?, ?>, java.io.Writer);
  public void render(java.util.Map<?, ?>, java.io.OutputStream);
}
```
