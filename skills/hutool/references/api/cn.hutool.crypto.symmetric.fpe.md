# cn.hutool.crypto.symmetric.fpe

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.crypto.symmetric.fpe.FPE`

```java
public class cn.hutool.crypto.symmetric.fpe.FPE implements java.io.Serializable {
  public cn.hutool.crypto.symmetric.fpe.FPE(cn.hutool.crypto.symmetric.fpe.FPE$FPEMode, byte[], org.bouncycastle.crypto.AlphabetMapper);
  public cn.hutool.crypto.symmetric.fpe.FPE(cn.hutool.crypto.symmetric.fpe.FPE$FPEMode, byte[], org.bouncycastle.crypto.AlphabetMapper, byte[]);
  public java.lang.String encrypt(java.lang.String);
  public char[] encrypt(char[]);
  public java.lang.String decrypt(java.lang.String);
  public char[] decrypt(char[]);
}
```

## `cn.hutool.crypto.symmetric.fpe.FPE$FPEMode`

```java
public final class cn.hutool.crypto.symmetric.fpe.FPE$FPEMode extends java.lang.Enum<cn.hutool.crypto.symmetric.fpe.FPE$FPEMode> {
  public static cn.hutool.crypto.symmetric.fpe.FPE$FPEMode[] values();
  public static cn.hutool.crypto.symmetric.fpe.FPE$FPEMode valueOf(java.lang.String);
  public java.lang.String getValue();
}
```
