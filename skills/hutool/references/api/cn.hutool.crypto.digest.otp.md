# cn.hutool.crypto.digest.otp

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.crypto.digest.otp.HOTP`

```java
public class cn.hutool.crypto.digest.otp.HOTP {
  public cn.hutool.crypto.digest.otp.HOTP(byte[]);
  public cn.hutool.crypto.digest.otp.HOTP(int, byte[]);
  public cn.hutool.crypto.digest.otp.HOTP(int, cn.hutool.crypto.digest.HmacAlgorithm, byte[]);
  public synchronized int generate(long);
  public static java.lang.String generateSecretKey(int);
  public int getPasswordLength();
  public java.lang.String getAlgorithm();
}
```

## `cn.hutool.crypto.digest.otp.TOTP`

```java
public class cn.hutool.crypto.digest.otp.TOTP extends cn.hutool.crypto.digest.otp.HOTP {
  public cn.hutool.crypto.digest.otp.TOTP(byte[]);
  public cn.hutool.crypto.digest.otp.TOTP(java.time.Duration, byte[]);
  public cn.hutool.crypto.digest.otp.TOTP(java.time.Duration, int, byte[]);
  public cn.hutool.crypto.digest.otp.TOTP(java.time.Duration, int, cn.hutool.crypto.digest.HmacAlgorithm, byte[]);
  public int generate(java.time.Instant);
  public boolean validate(java.time.Instant, int, int);
  public static java.lang.String generateGoogleSecretKey(java.lang.String, int);
  public java.time.Duration getTimeStep();
}
```
