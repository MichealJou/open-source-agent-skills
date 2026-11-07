# cn.hutool.extra.template.engine.velocity

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.template.engine.velocity.SimpleStringResourceLoader`

```java
public class cn.hutool.extra.template.engine.velocity.SimpleStringResourceLoader extends org.apache.velocity.runtime.resource.loader.ResourceLoader {
  public cn.hutool.extra.template.engine.velocity.SimpleStringResourceLoader();
  public void init(org.apache.velocity.util.ExtProperties);
  public java.io.InputStream getResourceStream(java.lang.String) throws org.apache.velocity.exception.ResourceNotFoundException;
  public java.io.Reader getResourceReader(java.lang.String, java.lang.String) throws org.apache.velocity.exception.ResourceNotFoundException;
  public boolean isSourceModified(org.apache.velocity.runtime.resource.Resource);
  public long getLastModified(org.apache.velocity.runtime.resource.Resource);
}
```

## `cn.hutool.extra.template.engine.velocity.VelocityEngine`

```java
public class cn.hutool.extra.template.engine.velocity.VelocityEngine implements cn.hutool.extra.template.TemplateEngine {
  public cn.hutool.extra.template.engine.velocity.VelocityEngine();
  public cn.hutool.extra.template.engine.velocity.VelocityEngine(cn.hutool.extra.template.TemplateConfig);
  public cn.hutool.extra.template.engine.velocity.VelocityEngine(org.apache.velocity.app.VelocityEngine);
  public cn.hutool.extra.template.TemplateEngine init(cn.hutool.extra.template.TemplateConfig);
  public org.apache.velocity.app.VelocityEngine getRawEngine();
  public cn.hutool.extra.template.Template getTemplate(java.lang.String);
}
```

## `cn.hutool.extra.template.engine.velocity.VelocityTemplate`

```java
public class cn.hutool.extra.template.engine.velocity.VelocityTemplate extends cn.hutool.extra.template.AbstractTemplate implements java.io.Serializable {
  public static cn.hutool.extra.template.engine.velocity.VelocityTemplate wrap(org.apache.velocity.Template);
  public cn.hutool.extra.template.engine.velocity.VelocityTemplate(org.apache.velocity.Template);
  public void render(java.util.Map<?, ?>, java.io.Writer);
  public void render(java.util.Map<?, ?>, java.io.OutputStream);
}
```
