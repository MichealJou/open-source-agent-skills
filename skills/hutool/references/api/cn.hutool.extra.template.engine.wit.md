# cn.hutool.extra.template.engine.wit

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.template.engine.wit.WitEngine`

```java
public class cn.hutool.extra.template.engine.wit.WitEngine implements cn.hutool.extra.template.TemplateEngine {
  public cn.hutool.extra.template.engine.wit.WitEngine();
  public cn.hutool.extra.template.engine.wit.WitEngine(cn.hutool.extra.template.TemplateConfig);
  public cn.hutool.extra.template.engine.wit.WitEngine(org.febit.wit.Engine);
  public cn.hutool.extra.template.TemplateEngine init(cn.hutool.extra.template.TemplateConfig);
  public cn.hutool.extra.template.Template getTemplate(java.lang.String);
  public org.febit.wit.Engine getRawEngine();
}
```

## `cn.hutool.extra.template.engine.wit.WitTemplate`

```java
public class cn.hutool.extra.template.engine.wit.WitTemplate extends cn.hutool.extra.template.AbstractTemplate implements java.io.Serializable {
  public static cn.hutool.extra.template.engine.wit.WitTemplate wrap(org.febit.wit.Template);
  public cn.hutool.extra.template.engine.wit.WitTemplate(org.febit.wit.Template);
  public void render(java.util.Map<?, ?>, java.io.Writer);
  public void render(java.util.Map<?, ?>, java.io.OutputStream);
}
```
