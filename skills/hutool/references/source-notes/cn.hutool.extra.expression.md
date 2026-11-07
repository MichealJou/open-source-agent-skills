# cn.hutool.extra.expression

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.expression.ExpressionEngine` | `Object eval(String expression,Map<String, Object> context,Collection<Class<?>> allowClassSet)` | 执行表达式 |
| `cn.hutool.extra.expression.ExpressionUtil` | `ExpressionEngine getEngine()` | 获得全局单例的表达式引擎 |
| `cn.hutool.extra.expression.ExpressionUtil` | `Object eval(String expression,Map<String, Object> context)` | 执行表达式 |
| `cn.hutool.extra.expression.ExpressionUtil` | `Object eval(String expression,Map<String, Object> context,Collection<Class<?>> allowClassSet)` | 执行表达式 |
