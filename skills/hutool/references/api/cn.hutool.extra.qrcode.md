# cn.hutool.extra.qrcode

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.extra.qrcode.BufferedImageLuminanceSource`

```java
public final class cn.hutool.extra.qrcode.BufferedImageLuminanceSource extends com.google.zxing.LuminanceSource {
  public cn.hutool.extra.qrcode.BufferedImageLuminanceSource(java.awt.image.BufferedImage);
  public cn.hutool.extra.qrcode.BufferedImageLuminanceSource(java.awt.image.BufferedImage, int, int, int, int);
  public byte[] getRow(int, byte[]);
  public byte[] getMatrix();
  public boolean isCropSupported();
  public com.google.zxing.LuminanceSource crop(int, int, int, int);
  public boolean isRotateSupported();
  public com.google.zxing.LuminanceSource rotateCounterClockwise();
}
```

## `cn.hutool.extra.qrcode.QrCodeException`

```java
public class cn.hutool.extra.qrcode.QrCodeException extends java.lang.RuntimeException {
  public cn.hutool.extra.qrcode.QrCodeException(java.lang.Throwable);
  public cn.hutool.extra.qrcode.QrCodeException(java.lang.String);
  public cn.hutool.extra.qrcode.QrCodeException(java.lang.String, java.lang.Object...);
  public cn.hutool.extra.qrcode.QrCodeException(java.lang.String, java.lang.Throwable);
  public cn.hutool.extra.qrcode.QrCodeException(java.lang.String, java.lang.Throwable, boolean, boolean);
  public cn.hutool.extra.qrcode.QrCodeException(java.lang.Throwable, java.lang.String, java.lang.Object...);
}
```

## `cn.hutool.extra.qrcode.QrCodeUtil`

```java
public class cn.hutool.extra.qrcode.QrCodeUtil {
  public cn.hutool.extra.qrcode.QrCodeUtil();
  public static java.lang.String generateAsBase64(java.lang.String, cn.hutool.extra.qrcode.QrConfig, java.lang.String, java.lang.String);
  public static java.lang.String generateAsBase64(java.lang.String, cn.hutool.extra.qrcode.QrConfig, java.lang.String, byte[]);
  public static java.lang.String generateAsBase64(java.lang.String, cn.hutool.extra.qrcode.QrConfig, java.lang.String, java.awt.Image);
  public static java.lang.String generateAsBase64(java.lang.String, cn.hutool.extra.qrcode.QrConfig, java.lang.String);
  public static java.lang.String generateAsSvg(java.lang.String, cn.hutool.extra.qrcode.QrConfig);
  public static java.lang.String generateAsAsciiArt(java.lang.String);
  public static java.lang.String generateAsAsciiArt(java.lang.String, cn.hutool.extra.qrcode.QrConfig);
  public static java.lang.String generateAsAsciiArt(java.lang.String, int, int, int);
  public static byte[] generatePng(java.lang.String, int, int);
  public static byte[] generatePng(java.lang.String, cn.hutool.extra.qrcode.QrConfig);
  public static java.io.File generate(java.lang.String, int, int, java.io.File);
  public static java.io.File generate(java.lang.String, cn.hutool.extra.qrcode.QrConfig, java.io.File);
  public static void generate(java.lang.String, int, int, java.lang.String, java.io.OutputStream);
  public static void generate(java.lang.String, cn.hutool.extra.qrcode.QrConfig, java.lang.String, java.io.OutputStream);
  public static java.awt.image.BufferedImage generate(java.lang.String, int, int);
  public static java.awt.image.BufferedImage generate(java.lang.String, com.google.zxing.BarcodeFormat, int, int);
  public static java.awt.image.BufferedImage generate(java.lang.String, cn.hutool.extra.qrcode.QrConfig);
  public static java.awt.image.BufferedImage generate(java.lang.String, com.google.zxing.BarcodeFormat, cn.hutool.extra.qrcode.QrConfig);
  public static com.google.zxing.common.BitMatrix encode(java.lang.String, int, int);
  public static com.google.zxing.common.BitMatrix encode(java.lang.String, cn.hutool.extra.qrcode.QrConfig);
  public static com.google.zxing.common.BitMatrix encode(java.lang.String, com.google.zxing.BarcodeFormat, int, int);
  public static com.google.zxing.common.BitMatrix encode(java.lang.String, com.google.zxing.BarcodeFormat, cn.hutool.extra.qrcode.QrConfig);
  public static java.lang.String decode(java.io.InputStream);
  public static java.lang.String decode(java.io.File);
  public static java.lang.String decode(java.awt.Image);
  public static java.lang.String decode(java.awt.Image, boolean, boolean);
  public static java.lang.String decode(java.awt.Image, java.util.Map<com.google.zxing.DecodeHintType, java.lang.Object>);
  public static java.awt.image.BufferedImage toImage(com.google.zxing.common.BitMatrix, int, java.lang.Integer);
  public static java.lang.String toSVG(com.google.zxing.common.BitMatrix, cn.hutool.extra.qrcode.QrConfig);
  public static java.lang.String toSVG(com.google.zxing.common.BitMatrix, java.lang.Integer, java.lang.Integer, java.awt.Image, int);
  public static java.lang.String toAsciiArt(com.google.zxing.common.BitMatrix, cn.hutool.extra.qrcode.QrConfig);
}
```

## `cn.hutool.extra.qrcode.QrConfig`

```java
public class cn.hutool.extra.qrcode.QrConfig {
  public static cn.hutool.extra.qrcode.QrConfig create();
  public cn.hutool.extra.qrcode.QrConfig();
  public cn.hutool.extra.qrcode.QrConfig(int, int);
  public int getWidth();
  public cn.hutool.extra.qrcode.QrConfig setWidth(int);
  public int getHeight();
  public cn.hutool.extra.qrcode.QrConfig setHeight(int);
  public int getForeColor();
  public cn.hutool.extra.qrcode.QrConfig setForeColor(int);
  public cn.hutool.extra.qrcode.QrConfig setForeColor(java.awt.Color);
  public int getBackColor();
  public cn.hutool.extra.qrcode.QrConfig setBackColor(int);
  public cn.hutool.extra.qrcode.QrConfig setBackColor(java.awt.Color);
  public java.lang.Integer getMargin();
  public cn.hutool.extra.qrcode.QrConfig setMargin(java.lang.Integer);
  public java.lang.Integer getQrVersion();
  public cn.hutool.extra.qrcode.QrConfig setQrVersion(java.lang.Integer);
  public com.google.zxing.qrcode.decoder.ErrorCorrectionLevel getErrorCorrection();
  public cn.hutool.extra.qrcode.QrConfig setErrorCorrection(com.google.zxing.qrcode.decoder.ErrorCorrectionLevel);
  public java.nio.charset.Charset getCharset();
  public cn.hutool.extra.qrcode.QrConfig setCharset(java.nio.charset.Charset);
  public java.awt.Image getImg();
  public cn.hutool.extra.qrcode.QrConfig setImg(java.lang.String);
  public cn.hutool.extra.qrcode.QrConfig setImg(java.io.File);
  public cn.hutool.extra.qrcode.QrConfig setImg(java.awt.Image);
  public int getRatio();
  public cn.hutool.extra.qrcode.QrConfig setRatio(int);
  public double getRound();
  public cn.hutool.extra.qrcode.QrConfig setRound(double);
  public cn.hutool.extra.qrcode.QrConfig setShapeHint(com.google.zxing.datamatrix.encoder.SymbolShapeHint);
  public java.util.HashMap<com.google.zxing.EncodeHintType, java.lang.Object> toHints();
  public java.util.HashMap<com.google.zxing.EncodeHintType, java.lang.Object> toHints(com.google.zxing.BarcodeFormat);
}
```
