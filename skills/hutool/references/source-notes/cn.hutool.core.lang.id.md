# cn.hutool.core.lang.id

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.lang.id.NanoId` | `String randomNanoId()` | 生成伪随机的NanoId字符串，长度为默认的#DEFAULT_SIZE，使用密码安全的伪随机生成器 |
| `cn.hutool.core.lang.id.NanoId` | `String randomNanoId(Random random,char[] alphabet,int size)` | 生成伪随机的NanoId字符串 |
| `cn.hutool.core.lang.id.NanoId` | `String randomNanoId(int size)` | 生成伪随机的NanoId字符串 |
