# cn.hutool.crypto.digest.otp

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.crypto.digest.otp.HOTP` | `String generateSecretKey(int numBytes)` | 生成共享密钥的Base32表示形式 |
| `cn.hutool.crypto.digest.otp.HOTP` | `String getAlgorithm()` | 获取HMAC算法 |
| `cn.hutool.crypto.digest.otp.HOTP` | `int generate(long counter)` | 生成一次性密码 |
| `cn.hutool.crypto.digest.otp.HOTP` | `int getPasswordLength()` | 获取密码长度，可以是6,7,8 |
| `cn.hutool.crypto.digest.otp.TOTP` | `Duration getTimeStep()` | 获取步进 |
| `cn.hutool.crypto.digest.otp.TOTP` | `String generateGoogleSecretKey(String account,int numBytes)` | 生成谷歌认证器的字符串（扫码字符串） 基于时间的，计数器不适合 |
| `cn.hutool.crypto.digest.otp.TOTP` | `boolean validate(Instant timestamp,int offsetSize,int code)` | 用于验证code是否正确 |
| `cn.hutool.crypto.digest.otp.TOTP` | `int generate(Instant timestamp)` | 使用给定的时间戳生成一次性密码. |
