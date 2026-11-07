# cn.hutool.extra.template.engine.rythm

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.template.engine.rythm.RythmEngine`

```java
public class cn.hutool.extra.template.engine.rythm.RythmEngine implements cn.hutool.extra.template.TemplateEngine {
  public cn.hutool.extra.template.engine.rythm.RythmEngine();
  public cn.hutool.extra.template.engine.rythm.RythmEngine(cn.hutool.extra.template.TemplateConfig);
  public cn.hutool.extra.template.engine.rythm.RythmEngine(org.rythmengine.RythmEngine);
  public cn.hutool.extra.template.TemplateEngine init(cn.hutool.extra.template.TemplateConfig);
  public org.rythmengine.RythmEngine getRawEngine();
  public cn.hutool.extra.template.Template getTemplate(java.lang.String);
}
```

## `cn.hutool.extra.template.engine.rythm.RythmTemplate`

```java
public class cn.hutool.extra.template.engine.rythm.RythmTemplate extends cn.hutool.extra.template.AbstractTemplate implements java.io.Serializable {
  public static cn.hutool.extra.template.engine.rythm.RythmTemplate wrap(org.rythmengine.template.ITemplate);
  public cn.hutool.extra.template.engine.rythm.RythmTemplate(org.rythmengine.template.ITemplate);
  public void render(java.util.Map<?, ?>, java.io.Writer);
  public void render(java.util.Map<?, ?>, java.io.OutputStream);
}
```
