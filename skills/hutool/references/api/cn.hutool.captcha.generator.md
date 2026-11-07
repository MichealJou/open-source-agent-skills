# cn.hutool.captcha.generator

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.captcha.generator.AbstractGenerator`

```java
public abstract class cn.hutool.captcha.generator.AbstractGenerator implements cn.hutool.captcha.generator.CodeGenerator {
  public cn.hutool.captcha.generator.AbstractGenerator(int);
  public cn.hutool.captcha.generator.AbstractGenerator(java.lang.String, int);
  public int getLength();
}
```

## `cn.hutool.captcha.generator.CodeGenerator`

```java
public interface cn.hutool.captcha.generator.CodeGenerator extends java.io.Serializable {
  public abstract java.lang.String generate();
  public abstract boolean verify(java.lang.String, java.lang.String);
}
```

## `cn.hutool.captcha.generator.MathGenerator`

```java
public class cn.hutool.captcha.generator.MathGenerator implements cn.hutool.captcha.generator.CodeGenerator {
  public cn.hutool.captcha.generator.MathGenerator();
  public cn.hutool.captcha.generator.MathGenerator(boolean);
  public cn.hutool.captcha.generator.MathGenerator(int);
  public cn.hutool.captcha.generator.MathGenerator(int, boolean);
  public java.lang.String generate();
  public boolean verify(java.lang.String, java.lang.String);
  public int getLength();
}
```

## `cn.hutool.captcha.generator.RandomGenerator`

```java
public class cn.hutool.captcha.generator.RandomGenerator extends cn.hutool.captcha.generator.AbstractGenerator {
  public cn.hutool.captcha.generator.RandomGenerator(int);
  public cn.hutool.captcha.generator.RandomGenerator(java.lang.String, int);
  public java.lang.String generate();
  public boolean verify(java.lang.String, java.lang.String);
}
```
