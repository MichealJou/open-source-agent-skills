# cn.hutool.extra.template

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.template.AbstractTemplate` | `String render(Map<?, ?> bindingMap)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.template.AbstractTemplate` | `void render(Map<?, ?> bindingMap,File file)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.template.Template` | `String render(Map<?, ?> bindingMap)` | 将模板与绑定参数融合后返回为字符串 |
| `cn.hutool.extra.template.Template` | `void render(Map<?, ?> bindingMap,File file)` | 写出到文件 |
| `cn.hutool.extra.template.Template` | `void render(Map<?, ?> bindingMap,OutputStream out)` | 将模板与绑定参数融合后输出到流 |
| `cn.hutool.extra.template.Template` | `void render(Map<?, ?> bindingMap,Writer writer)` | 将模板与绑定参数融合后输出到Writer |
| `cn.hutool.extra.template.TemplateConfig` | `Charset getCharset()` | 获取编码 |
| `cn.hutool.extra.template.TemplateConfig` | `Class<? extends TemplateEngine> getCustomEngine()` | 获取自定义引擎，null表示系统自动判断 |
| `cn.hutool.extra.template.TemplateConfig` | `ResourceMode getResourceMode()` | 获取模板资源加载方式 |
| `cn.hutool.extra.template.TemplateConfig` | `String getCharsetStr()` | 获取编码 |
| `cn.hutool.extra.template.TemplateConfig` | `String getPath()` | 获取模板路径，如果ClassPath或者WebRoot模式，则表示相对路径 |
| `cn.hutool.extra.template.TemplateConfig` | `TemplateConfig setCustomEngine(Class<? extends TemplateEngine> customEngine)` | 设置自定义引擎，null表示系统自动判断 |
| `cn.hutool.extra.template.TemplateConfig` | `TemplateConfig setUseCache(boolean useCache)` | 设置是否使用缓存 |
| `cn.hutool.extra.template.TemplateConfig` | `boolean equals(Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.template.TemplateConfig` | `boolean isUseCache()` | 是否使用缓存 |
| `cn.hutool.extra.template.TemplateConfig` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.template.TemplateConfig` | `void setCharset(Charset charset)` | 设置编码 |
| `cn.hutool.extra.template.TemplateConfig` | `void setPath(String path)` | 设置模板路径，如果ClassPath或者WebRoot模式，则表示相对路径 |
| `cn.hutool.extra.template.TemplateConfig` | `void setResourceMode(ResourceMode resourceMode)` | 设置模板资源加载方式 |
| `cn.hutool.extra.template.TemplateEngine` | `Template getTemplate(String resource)` | 获取模板 |
| `cn.hutool.extra.template.TemplateEngine` | `TemplateEngine init(TemplateConfig config)` | 使用指定配置文件初始化模板引擎 |
| `cn.hutool.extra.template.TemplateUtil` | `TemplateEngine createEngine()` | 根据用户引入的模板引擎jar，自动创建对应的模板引擎对象，使用默认配置 推荐创建的引擎单例使用，此方法每次调用会返回新的引擎 |
| `cn.hutool.extra.template.TemplateUtil` | `TemplateEngine createEngine(TemplateConfig config)` | 根据用户引入的模板引擎jar，自动创建对应的模板引擎对象 推荐创建的引擎单例使用，此方法每次调用会返回新的引擎 |
