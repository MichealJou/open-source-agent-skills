# cn.hutool.extra.template.engine

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.template.engine.TemplateFactory` | `TemplateEngine create()` | 根据用户引入的模板引擎jar，自动创建对应的模板引擎对象 推荐创建的引擎单例使用，此方法每次调用会返回新的引擎 |
| `cn.hutool.extra.template.engine.TemplateFactory` | `TemplateEngine create(TemplateConfig config)` | 根据用户引入的模板引擎jar，自动创建对应的模板引擎对象 推荐创建的引擎单例使用，此方法每次调用会返回新的引擎 |
| `cn.hutool.extra.template.engine.TemplateFactory` | `TemplateEngine get()` | 根据用户引入的模板引擎jar，自动创建对应的模板引擎对象 获得的是单例的TemplateEngine |
