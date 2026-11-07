# cn.hutool.core.img

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.img.BackgroundRemoval`

```java
public class cn.hutool.core.img.BackgroundRemoval {
  public cn.hutool.core.img.BackgroundRemoval();
  public static boolean backgroundRemoval(java.lang.String, java.lang.String, int);
  public static boolean backgroundRemoval(java.io.File, java.io.File, int);
  public static boolean backgroundRemoval(java.io.File, java.io.File, java.awt.Color, int);
  public static java.awt.image.BufferedImage backgroundRemoval(java.awt.image.BufferedImage, java.awt.Color, int);
  public static java.awt.image.BufferedImage backgroundRemoval(java.io.ByteArrayOutputStream, java.awt.Color, int);
  public static java.awt.Color hexToRgb(java.lang.String);
  public static boolean areColorsWithinTolerance(java.awt.Color, java.awt.Color, int);
  public static boolean areColorsWithinTolerance(java.awt.Color, java.awt.Color, java.awt.Color);
  public static java.lang.String getMainColor(java.lang.String);
  public static java.lang.String getMainColor(java.io.File);
  public static java.lang.String getMainColor(java.awt.image.BufferedImage);
}
```

## `cn.hutool.core.img.ColorUtil`

```java
public class cn.hutool.core.img.ColorUtil {
  public cn.hutool.core.img.ColorUtil();
  public static java.lang.String toHex(java.awt.Color);
  public static java.lang.String toHex(int, int, int);
  public static java.awt.Color getColor(java.lang.String);
  public static java.awt.Color getColor(int);
  public static java.awt.Color hexToColor(java.lang.String);
  public static java.awt.Color add(java.awt.Color, java.awt.Color);
  public static java.awt.Color randomColor(java.awt.Color, int);
  public static java.awt.Color randomColor();
  public static int maxDistance(java.awt.Color);
  public static int computeColorDistance(java.awt.Color, java.awt.Color);
  public static java.awt.Color randomColor(java.util.Random);
  public static java.lang.String getMainColor(java.awt.image.BufferedImage, int[]...);
}
```

## `cn.hutool.core.img.FontUtil`

```java
public class cn.hutool.core.img.FontUtil {
  public cn.hutool.core.img.FontUtil();
  public static java.awt.Font createFont();
  public static java.awt.Font createSansSerifFont(int);
  public static java.awt.Font createFont(java.lang.String, int);
  public static java.awt.Font createFont(java.io.File);
  public static java.awt.Font createFont(java.io.InputStream);
  public static java.awt.Dimension getDimension(java.awt.FontMetrics, java.lang.String);
}
```

## `cn.hutool.core.img.GraphicsUtil`

```java
public class cn.hutool.core.img.GraphicsUtil {
  public cn.hutool.core.img.GraphicsUtil();
  public static java.awt.Graphics2D createGraphics(java.awt.image.BufferedImage, java.awt.Color);
  public static int getCenterY(java.awt.Graphics, int);
  public static java.awt.Graphics drawStringColourful(java.awt.Graphics, java.lang.String, java.awt.Font, int, int);
  public static java.awt.Graphics drawStringColourful(java.awt.Graphics, java.lang.String, java.awt.Font, int, int, java.awt.Color, int);
  public static java.awt.Graphics drawStringColourful(java.awt.Graphics, java.lang.String, java.awt.Font, int, int, java.awt.Color);
  public static java.awt.Graphics drawString(java.awt.Graphics, java.lang.String, java.awt.Font, java.awt.Color, int, int);
  public static java.awt.Graphics drawString(java.awt.Graphics, java.lang.String, java.awt.Font, java.awt.Color, int, int, java.awt.Color, int);
  public static java.awt.Graphics drawString(java.awt.Graphics, java.lang.String, java.awt.Font, java.awt.Color, java.awt.Rectangle);
  public static java.awt.Graphics drawString(java.awt.Graphics, java.lang.String, java.awt.Font, java.awt.Color, java.awt.Point);
  public static java.awt.Graphics drawImg(java.awt.Graphics, java.awt.Image, java.awt.Point);
  public static java.awt.Graphics drawImg(java.awt.Graphics, java.awt.Image, java.awt.Rectangle);
  public static java.awt.Graphics2D setAlpha(java.awt.Graphics2D, float);
}
```

## `cn.hutool.core.img.Img`

```java
public class cn.hutool.core.img.Img implements java.io.Flushable,java.io.Serializable {
  public static cn.hutool.core.img.Img from(java.nio.file.Path);
  public static cn.hutool.core.img.Img from(java.io.File);
  public static cn.hutool.core.img.Img from(cn.hutool.core.io.resource.Resource);
  public static cn.hutool.core.img.Img from(java.io.InputStream);
  public static cn.hutool.core.img.Img from(javax.imageio.stream.ImageInputStream);
  public static cn.hutool.core.img.Img from(java.net.URL);
  public static cn.hutool.core.img.Img from(java.awt.Image);
  public cn.hutool.core.img.Img(java.awt.image.BufferedImage);
  public cn.hutool.core.img.Img(java.awt.image.BufferedImage, java.lang.String);
  public cn.hutool.core.img.Img setTargetImageType(java.lang.String);
  public cn.hutool.core.img.Img setPositionBaseCentre(boolean);
  public cn.hutool.core.img.Img setQuality(double);
  public cn.hutool.core.img.Img setQuality(float);
  public cn.hutool.core.img.Img setBackgroundColor(java.awt.Color);
  public cn.hutool.core.img.Img scale(float);
  public cn.hutool.core.img.Img scale(int, int);
  public cn.hutool.core.img.Img scale(int, int, int);
  public cn.hutool.core.img.Img scale(int, int, java.awt.Color);
  public cn.hutool.core.img.Img cut(java.awt.Rectangle);
  public cn.hutool.core.img.Img cut(int, int);
  public cn.hutool.core.img.Img cut(int, int, int);
  public cn.hutool.core.img.Img round(double);
  public cn.hutool.core.img.Img gray();
  public cn.hutool.core.img.Img binary();
  public cn.hutool.core.img.Img pressText(java.lang.String, java.awt.Color, java.awt.Font, int, int, float);
  public cn.hutool.core.img.Img pressText(java.lang.String, java.awt.Color, java.awt.Font, java.awt.Point, float);
  public cn.hutool.core.img.Img pressTextFull(java.lang.String, java.awt.Color, java.awt.Font, int, int, float);
  public cn.hutool.core.img.Img pressImage(java.awt.Image, int, int, float);
  public cn.hutool.core.img.Img pressImage(java.awt.Image, java.awt.Rectangle, float);
  public cn.hutool.core.img.Img rotate(int);
  public cn.hutool.core.img.Img flip();
  public cn.hutool.core.img.Img stroke(java.awt.Color, float);
  public cn.hutool.core.img.Img stroke(java.awt.Color, java.awt.Stroke);
  public java.awt.Image getImg();
  public boolean write(java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public boolean write(javax.imageio.stream.ImageOutputStream) throws cn.hutool.core.io.IORuntimeException;
  public boolean write(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public void flush();
}
```

## `cn.hutool.core.img.ImgUtil`

```java
public class cn.hutool.core.img.ImgUtil {
  public cn.hutool.core.img.ImgUtil();
  public static void scale(java.io.File, java.io.File, float);
  public static void scale(java.io.InputStream, java.io.OutputStream, float);
  public static void scale(javax.imageio.stream.ImageInputStream, javax.imageio.stream.ImageOutputStream, float);
  public static void scale(java.awt.Image, java.io.File, float) throws cn.hutool.core.io.IORuntimeException;
  public static void scale(java.awt.Image, java.io.OutputStream, float) throws cn.hutool.core.io.IORuntimeException;
  public static void scale(java.awt.Image, javax.imageio.stream.ImageOutputStream, float) throws cn.hutool.core.io.IORuntimeException;
  public static java.awt.Image scale(java.awt.Image, float);
  public static java.awt.Image scale(java.awt.Image, int, int);
  public static void scale(java.io.File, java.io.File, int, int, java.awt.Color) throws cn.hutool.core.io.IORuntimeException;
  public static void scale(java.io.InputStream, java.io.OutputStream, int, int, java.awt.Color) throws cn.hutool.core.io.IORuntimeException;
  public static void scale(javax.imageio.stream.ImageInputStream, javax.imageio.stream.ImageOutputStream, int, int, java.awt.Color) throws cn.hutool.core.io.IORuntimeException;
  public static void scale(java.awt.Image, javax.imageio.stream.ImageOutputStream, int, int, java.awt.Color) throws cn.hutool.core.io.IORuntimeException;
  public static java.awt.Image scale(java.awt.Image, int, int, java.awt.Color);
  public static void cut(java.io.File, java.io.File, java.awt.Rectangle);
  public static void cut(java.io.InputStream, java.io.OutputStream, java.awt.Rectangle);
  public static void cut(javax.imageio.stream.ImageInputStream, javax.imageio.stream.ImageOutputStream, java.awt.Rectangle);
  public static void cut(java.awt.Image, java.io.File, java.awt.Rectangle) throws cn.hutool.core.io.IORuntimeException;
  public static void cut(java.awt.Image, java.io.OutputStream, java.awt.Rectangle) throws cn.hutool.core.io.IORuntimeException;
  public static void cut(java.awt.Image, javax.imageio.stream.ImageOutputStream, java.awt.Rectangle) throws cn.hutool.core.io.IORuntimeException;
  public static java.awt.Image cut(java.awt.Image, java.awt.Rectangle);
  public static java.awt.Image cut(java.awt.Image, int, int);
  public static java.awt.Image cut(java.awt.Image, int, int, int);
  public static void slice(java.io.File, java.io.File, int, int);
  public static void slice(java.awt.Image, java.io.File, int, int);
  public static void sliceByRowsAndCols(java.io.File, java.io.File, int, int);
  public static void sliceByRowsAndCols(java.io.File, java.io.File, java.lang.String, int, int);
  public static void sliceByRowsAndCols(java.awt.Image, java.io.File, int, int);
  public static void sliceByRowsAndCols(java.awt.Image, java.io.File, java.lang.String, int, int);
  public static void convert(java.io.File, java.io.File);
  public static void convert(java.io.InputStream, java.lang.String, java.io.OutputStream);
  public static void convert(java.awt.Image, java.lang.String, javax.imageio.stream.ImageOutputStream);
  public static void convert(java.awt.Image, java.lang.String, javax.imageio.stream.ImageOutputStream, boolean);
  public static void gray(java.io.File, java.io.File);
  public static void gray(java.io.InputStream, java.io.OutputStream);
  public static void gray(javax.imageio.stream.ImageInputStream, javax.imageio.stream.ImageOutputStream);
  public static void gray(java.awt.Image, java.io.File);
  public static void gray(java.awt.Image, java.io.OutputStream);
  public static void gray(java.awt.Image, javax.imageio.stream.ImageOutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static java.awt.Image gray(java.awt.Image);
  public static void binary(java.io.File, java.io.File);
  public static void binary(java.io.InputStream, java.io.OutputStream, java.lang.String);
  public static void binary(javax.imageio.stream.ImageInputStream, javax.imageio.stream.ImageOutputStream, java.lang.String);
  public static void binary(java.awt.Image, java.io.File);
  public static void binary(java.awt.Image, java.io.OutputStream, java.lang.String);
  public static void binary(java.awt.Image, javax.imageio.stream.ImageOutputStream, java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.awt.Image binary(java.awt.Image);
  public static void pressText(java.io.File, java.io.File, java.lang.String, java.awt.Color, java.awt.Font, int, int, float);
  public static void pressText(java.io.InputStream, java.io.OutputStream, java.lang.String, java.awt.Color, java.awt.Font, int, int, float);
  public static void pressText(javax.imageio.stream.ImageInputStream, javax.imageio.stream.ImageOutputStream, java.lang.String, java.awt.Color, java.awt.Font, int, int, float);
  public static void pressText(java.awt.Image, java.io.File, java.lang.String, java.awt.Color, java.awt.Font, int, int, float) throws cn.hutool.core.io.IORuntimeException;
  public static void pressText(java.awt.Image, java.io.OutputStream, java.lang.String, java.awt.Color, java.awt.Font, int, int, float) throws cn.hutool.core.io.IORuntimeException;
  public static void pressText(java.awt.Image, javax.imageio.stream.ImageOutputStream, java.lang.String, java.awt.Color, java.awt.Font, int, int, float) throws cn.hutool.core.io.IORuntimeException;
  public static java.awt.Image pressText(java.awt.Image, java.lang.String, java.awt.Color, java.awt.Font, int, int, float);
  public static void pressImage(java.io.File, java.io.File, java.awt.Image, int, int, float);
  public static void pressImage(java.io.InputStream, java.io.OutputStream, java.awt.Image, int, int, float);
  public static void pressImage(javax.imageio.stream.ImageInputStream, javax.imageio.stream.ImageOutputStream, java.awt.Image, int, int, float) throws cn.hutool.core.io.IORuntimeException;
  public static void pressImage(java.awt.Image, java.io.File, java.awt.Image, int, int, float) throws cn.hutool.core.io.IORuntimeException;
  public static void pressImage(java.awt.Image, java.io.OutputStream, java.awt.Image, int, int, float) throws cn.hutool.core.io.IORuntimeException;
  public static void pressImage(java.awt.Image, javax.imageio.stream.ImageOutputStream, java.awt.Image, int, int, float) throws cn.hutool.core.io.IORuntimeException;
  public static java.awt.Image pressImage(java.awt.Image, java.awt.Image, int, int, float);
  public static java.awt.Image pressImage(java.awt.Image, java.awt.Image, java.awt.Rectangle, float);
  public static void rotate(java.io.File, int, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static void rotate(java.awt.Image, int, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static void rotate(java.awt.Image, int, java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static void rotate(java.awt.Image, int, javax.imageio.stream.ImageOutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static java.awt.Image rotate(java.awt.Image, int);
  public static void flip(java.io.File, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static void flip(java.awt.Image, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static void flip(java.awt.Image, java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static void flip(java.awt.Image, javax.imageio.stream.ImageOutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static java.awt.Image flip(java.awt.Image);
  public static void compress(java.io.File, java.io.File, float) throws cn.hutool.core.io.IORuntimeException;
  public static java.awt.image.RenderedImage toRenderedImage(java.awt.Image);
  public static java.awt.image.BufferedImage toBufferedImage(java.awt.Image);
  public static java.awt.image.RenderedImage castToRenderedImage(java.awt.Image, java.lang.String);
  public static java.awt.image.BufferedImage castToBufferedImage(java.awt.Image, java.lang.String);
  public static java.awt.image.BufferedImage toBufferedImage(java.awt.Image, java.lang.String);
  public static java.awt.image.BufferedImage toBufferedImage(java.awt.Image, java.lang.String, java.awt.Color);
  public static java.awt.image.BufferedImage toBufferedImage(java.awt.Image, int);
  public static java.awt.image.BufferedImage toBufferedImage(java.awt.Image, int, java.awt.Color);
  public static java.awt.image.BufferedImage copyImage(java.awt.Image, int);
  public static java.awt.image.BufferedImage copyImage(java.awt.Image, int, java.awt.Color);
  public static java.awt.image.BufferedImage createCompatibleImage(int, int, int) throws java.awt.HeadlessException;
  public static java.awt.image.BufferedImage toImage(java.lang.String) throws cn.hutool.core.io.IORuntimeException;
  public static java.awt.image.BufferedImage toImage(byte[]) throws cn.hutool.core.io.IORuntimeException;
  public static java.io.ByteArrayInputStream toStream(java.awt.Image, java.lang.String);
  public static java.lang.String toBase64DataUri(java.awt.Image, java.lang.String);
  public static java.lang.String toBase64(java.awt.Image, java.lang.String);
  public static byte[] toBytes(java.awt.Image, java.lang.String);
  public static void createImage(java.lang.String, java.awt.Font, java.awt.Color, java.awt.Color, javax.imageio.stream.ImageOutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static void createTransparentImage(java.lang.String, java.awt.Font, java.awt.Color, javax.imageio.stream.ImageOutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static java.awt.image.BufferedImage createImage(java.lang.String, java.awt.Font, java.awt.Color, java.awt.Color, int) throws cn.hutool.core.io.IORuntimeException;
  public static java.awt.geom.Rectangle2D getRectangle(java.lang.String, java.awt.Font);
  public static java.awt.Font createFont(java.io.File);
  public static java.awt.Font createFont(java.io.InputStream);
  public static java.awt.Graphics2D createGraphics(java.awt.image.BufferedImage, java.awt.Color);
  public static void writeJpg(java.awt.Image, javax.imageio.stream.ImageOutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static void writePng(java.awt.Image, javax.imageio.stream.ImageOutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static void writeJpg(java.awt.Image, java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static void writePng(java.awt.Image, java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static void write(javax.imageio.stream.ImageInputStream, java.lang.String, javax.imageio.stream.ImageOutputStream);
  public static void write(java.awt.Image, java.lang.String, java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static boolean write(java.awt.Image, java.lang.String, javax.imageio.stream.ImageOutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static boolean write(java.awt.Image, java.lang.String, javax.imageio.stream.ImageOutputStream, float) throws cn.hutool.core.io.IORuntimeException;
  public static boolean write(java.awt.Image, java.lang.String, javax.imageio.stream.ImageOutputStream, float, java.awt.Color) throws cn.hutool.core.io.IORuntimeException;
  public static void write(java.awt.Image, java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static boolean write(java.awt.Image, javax.imageio.ImageWriter, javax.imageio.stream.ImageOutputStream, float);
  public static javax.imageio.ImageReader getReader(java.lang.String);
  public static java.awt.image.BufferedImage read(java.lang.String);
  public static java.awt.image.BufferedImage read(java.io.File);
  public static java.awt.Image getImage(java.net.URL);
  public static java.awt.image.BufferedImage read(cn.hutool.core.io.resource.Resource);
  public static java.awt.image.BufferedImage read(java.io.InputStream);
  public static java.awt.image.BufferedImage read(javax.imageio.stream.ImageInputStream);
  public static java.awt.image.BufferedImage read(java.net.URL);
  public static javax.imageio.stream.ImageOutputStream getImageOutputStream(java.io.OutputStream) throws cn.hutool.core.io.IORuntimeException;
  public static javax.imageio.stream.ImageOutputStream getImageOutputStream(java.io.File) throws cn.hutool.core.io.IORuntimeException;
  public static javax.imageio.stream.ImageInputStream getImageInputStream(java.io.InputStream) throws cn.hutool.core.io.IORuntimeException;
  public static javax.imageio.ImageWriter getWriter(java.awt.Image, java.lang.String);
  public static javax.imageio.ImageWriter getWriter(java.lang.String);
  public static java.lang.String toHex(java.awt.Color);
  public static java.lang.String toHex(int, int, int);
  public static java.awt.Color hexToColor(java.lang.String);
  public static java.awt.Color getColor(int);
  public static java.awt.Color getColor(java.lang.String);
  public static java.awt.Color randomColor();
  public static java.awt.Color randomColor(java.awt.Color, int);
  public static java.awt.Color randomColor(java.awt.Color);
  public static java.awt.Color randomColor(java.util.Random);
  public static java.awt.Point getPointBaseCentre(java.awt.Rectangle, int, int);
  public static java.lang.String getMainColor(java.awt.image.BufferedImage, int[]...);
  public static boolean backgroundRemoval(java.lang.String, java.lang.String, int);
  public static boolean backgroundRemoval(java.io.File, java.io.File, int);
  public static boolean backgroundRemoval(java.io.File, java.io.File, java.awt.Color, int);
  public static java.awt.image.BufferedImage backgroundRemoval(java.awt.image.BufferedImage, java.awt.Color, int);
  public static java.awt.image.BufferedImage backgroundRemoval(java.io.ByteArrayOutputStream, java.awt.Color, int);
  public static java.awt.image.BufferedImage colorConvert(java.awt.color.ColorSpace, java.awt.image.BufferedImage);
  public static java.awt.image.BufferedImage transform(java.awt.geom.AffineTransform, java.awt.image.BufferedImage);
  public static java.awt.image.BufferedImage filter(java.awt.image.BufferedImageOp, java.awt.image.BufferedImage);
  public static java.awt.Image filter(java.awt.image.ImageFilter, java.awt.Image);
  public static void flush(java.awt.Image);
}
```

## `cn.hutool.core.img.LabColor`

```java
public class cn.hutool.core.img.LabColor {
  public cn.hutool.core.img.LabColor(java.lang.Integer);
  public cn.hutool.core.img.LabColor(java.awt.Color);
  public double getDistance(cn.hutool.core.img.LabColor);
}
```

## `cn.hutool.core.img.ScaleType`

```java
public final class cn.hutool.core.img.ScaleType extends java.lang.Enum<cn.hutool.core.img.ScaleType> {
  public static cn.hutool.core.img.ScaleType[] values();
  public static cn.hutool.core.img.ScaleType valueOf(java.lang.String);
  public int getValue();
}
```
