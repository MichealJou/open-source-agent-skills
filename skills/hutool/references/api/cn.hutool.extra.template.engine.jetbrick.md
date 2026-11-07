# cn.hutool.extra.template.engine.jetbrick

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.template.engine.jetbrick.JetbrickEngine`

```java
public class cn.hutool.extra.template.engine.jetbrick.JetbrickEngine implements cn.hutool.extra.template.TemplateEngine {
  public cn.hutool.extra.template.engine.jetbrick.JetbrickEngine();
  public cn.hutool.extra.template.engine.jetbrick.JetbrickEngine(cn.hutool.extra.template.TemplateConfig);
  public cn.hutool.extra.template.engine.jetbrick.JetbrickEngine(jetbrick.template.JetEngine);
  public cn.hutool.extra.template.TemplateEngine init(cn.hutool.extra.template.TemplateConfig);
  public cn.hutool.extra.template.Template getTemplate(java.lang.String);
  public jetbrick.template.JetEngine getRawEngine();
}
```

## `cn.hutool.extra.template.engine.jetbrick.JetbrickTemplate`

```java
public class cn.hutool.extra.template.engine.jetbrick.JetbrickTemplate extends cn.hutool.extra.template.AbstractTemplate implements java.io.Serializable {
  public static cn.hutool.extra.template.engine.jetbrick.JetbrickTemplate wrap(jetbrick.template.JetTemplate);
  public cn.hutool.extra.template.engine.jetbrick.JetbrickTemplate(jetbrick.template.JetTemplate);
  public void render(java.util.Map<?, ?>, java.io.Writer);
  public void render(java.util.Map<?, ?>, java.io.OutputStream);
}
```
