# cn.hutool.captcha.generator

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.captcha.generator.AbstractGenerator` | `int getLength()` | 获取长度验证码 |
| `cn.hutool.captcha.generator.CodeGenerator` | `String generate()` | 生成验证码 |
| `cn.hutool.captcha.generator.CodeGenerator` | `boolean verify(String code,String userInputCode)` | 验证用户输入的字符串是否与生成的验证码匹配 用户通过实现此方法定义验证码匹配方式 |
| `cn.hutool.captcha.generator.MathGenerator` | `String generate()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.captcha.generator.MathGenerator` | `boolean verify(String code,String userInputCode)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.captcha.generator.MathGenerator` | `int getLength()` | 获取验证码长度 |
| `cn.hutool.captcha.generator.RandomGenerator` | `String generate()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.captcha.generator.RandomGenerator` | `boolean verify(String code,String userInputCode)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
