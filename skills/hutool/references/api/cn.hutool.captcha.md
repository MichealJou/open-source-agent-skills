# cn.hutool.captcha

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.captcha.AbstractCaptcha`

```java
public abstract class cn.hutool.captcha.AbstractCaptcha implements cn.hutool.captcha.ICaptcha {
  public cn.hutool.captcha.AbstractCaptcha(int, int, int, int);
  public cn.hutool.captcha.AbstractCaptcha(int, int, cn.hutool.captcha.generator.CodeGenerator, int);
  public cn.hutool.captcha.AbstractCaptcha(int, int, cn.hutool.captcha.generator.CodeGenerator, int, float);
  public void createCode();
  public java.lang.String getCode();
  public boolean verify(java.lang.String);
  public void write(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public void write(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public void write(java.io.OutputStream);
  public byte[] getImageBytes();
  public java.awt.image.BufferedImage getImage();
  public java.lang.String getImageBase64();
  public java.lang.String getImageBase64Data();
  public void setFont(java.awt.Font);
  public cn.hutool.captcha.generator.CodeGenerator getGenerator();
  public void setGenerator(cn.hutool.captcha.generator.CodeGenerator);
  public void setBackground(java.awt.Color);
  public void setTextAlpha(float);
  public void setStroke(java.awt.Stroke);
}
```

## `cn.hutool.captcha.CaptchaUtil`

```java
public class cn.hutool.captcha.CaptchaUtil {
  public cn.hutool.captcha.CaptchaUtil();
  public static cn.hutool.captcha.LineCaptcha createLineCaptcha(int, int);
  public static cn.hutool.captcha.LineCaptcha createLineCaptcha(int, int, int, int);
  public static cn.hutool.captcha.LineCaptcha createLineCaptcha(int, int, cn.hutool.captcha.generator.CodeGenerator, int);
  public static cn.hutool.captcha.LineCaptcha createLineCaptcha(int, int, int, int, float);
  public static cn.hutool.captcha.CircleCaptcha createCircleCaptcha(int, int);
  public static cn.hutool.captcha.CircleCaptcha createCircleCaptcha(int, int, int, int);
  public static cn.hutool.captcha.CircleCaptcha createCircleCaptcha(int, int, cn.hutool.captcha.generator.CodeGenerator, int);
  public static cn.hutool.captcha.CircleCaptcha createCircleCaptcha(int, int, int, int, float);
  public static cn.hutool.captcha.ShearCaptcha createShearCaptcha(int, int);
  public static cn.hutool.captcha.ShearCaptcha createShearCaptcha(int, int, int, int);
  public static cn.hutool.captcha.ShearCaptcha createShearCaptcha(int, int, cn.hutool.captcha.generator.CodeGenerator, int);
  public static cn.hutool.captcha.ShearCaptcha createShearCaptcha(int, int, int, int, float);
  public static cn.hutool.captcha.GifCaptcha createGifCaptcha(int, int);
  public static cn.hutool.captcha.GifCaptcha createGifCaptcha(int, int, int);
  public static cn.hutool.captcha.GifCaptcha createGifCaptcha(int, int, cn.hutool.captcha.generator.CodeGenerator, int);
  public static cn.hutool.captcha.GifCaptcha createGifCaptcha(int, int, int, int, float);
}
```

## `cn.hutool.captcha.CircleCaptcha`

```java
public class cn.hutool.captcha.CircleCaptcha extends cn.hutool.captcha.AbstractCaptcha {
  public cn.hutool.captcha.CircleCaptcha(int, int);
  public cn.hutool.captcha.CircleCaptcha(int, int, int);
  public cn.hutool.captcha.CircleCaptcha(int, int, int, int);
  public cn.hutool.captcha.CircleCaptcha(int, int, cn.hutool.captcha.generator.CodeGenerator, int);
  public cn.hutool.captcha.CircleCaptcha(int, int, int, int, float);
  public java.awt.Image createImage(java.lang.String);
}
```

## `cn.hutool.captcha.GifCaptcha`

```java
public class cn.hutool.captcha.GifCaptcha extends cn.hutool.captcha.AbstractCaptcha {
  public cn.hutool.captcha.GifCaptcha(int, int);
  public cn.hutool.captcha.GifCaptcha(int, int, int);
  public cn.hutool.captcha.GifCaptcha(int, int, int, int);
  public cn.hutool.captcha.GifCaptcha(int, int, cn.hutool.captcha.generator.CodeGenerator, int);
  public cn.hutool.captcha.GifCaptcha(int, int, int, int, float);
  public cn.hutool.captcha.GifCaptcha setQuality(int);
  public cn.hutool.captcha.GifCaptcha setRepeat(int);
  public cn.hutool.captcha.GifCaptcha setMaxColor(int);
  public cn.hutool.captcha.GifCaptcha setMinColor(int);
  public void createCode();
}
```

## `cn.hutool.captcha.ICaptcha`

```java
public interface cn.hutool.captcha.ICaptcha extends java.io.Serializable {
  public abstract void createCode();
  public abstract java.lang.String getCode();
  public abstract boolean verify(java.lang.String);
  public abstract void write(java.io.OutputStream);
}
```

## `cn.hutool.captcha.LineCaptcha`

```java
public class cn.hutool.captcha.LineCaptcha extends cn.hutool.captcha.AbstractCaptcha {
  public cn.hutool.captcha.LineCaptcha(int, int);
  public cn.hutool.captcha.LineCaptcha(int, int, int, int);
  public cn.hutool.captcha.LineCaptcha(int, int, cn.hutool.captcha.generator.CodeGenerator, int);
  public cn.hutool.captcha.LineCaptcha(int, int, int, int, float);
  public java.awt.Image createImage(java.lang.String);
}
```

## `cn.hutool.captcha.ShearCaptcha`

```java
public class cn.hutool.captcha.ShearCaptcha extends cn.hutool.captcha.AbstractCaptcha {
  public cn.hutool.captcha.ShearCaptcha(int, int);
  public cn.hutool.captcha.ShearCaptcha(int, int, int);
  public cn.hutool.captcha.ShearCaptcha(int, int, int, int);
  public cn.hutool.captcha.ShearCaptcha(int, int, cn.hutool.captcha.generator.CodeGenerator, int);
  public cn.hutool.captcha.ShearCaptcha(int, int, int, int, float);
  public java.awt.Image createImage(java.lang.String);
}
```
