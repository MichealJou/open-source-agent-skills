# cn.hutool.core.img.gif

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.img.gif.AnimatedGifEncoder`

```java
public class cn.hutool.core.img.gif.AnimatedGifEncoder {
  public cn.hutool.core.img.gif.AnimatedGifEncoder();
  public void setDelay(int);
  public void setDispose(int);
  public void setRepeat(int);
  public void setTransparent(java.awt.Color);
  public void setTransparent(java.awt.Color, boolean);
  public void setBackground(java.awt.Color);
  public boolean addFrame(java.awt.image.BufferedImage);
  public boolean finish();
  public void setFrameRate(float);
  public void setQuality(int);
  public void setSize(int, int);
  public boolean start(java.io.OutputStream);
  public boolean start(java.lang.String);
  public boolean isStarted();
}
```

## `cn.hutool.core.img.gif.GifDecoder`

```java
public class cn.hutool.core.img.gif.GifDecoder {
  public cn.hutool.core.img.gif.GifDecoder();
  public int getDelay(int);
  public int getFrameCount();
  public java.awt.image.BufferedImage getImage();
  public int getLoopCount();
  public java.awt.image.BufferedImage getFrame(int);
  public java.awt.Dimension getFrameSize();
  public int read(java.io.BufferedInputStream);
  public int read(java.io.InputStream);
  public int read(java.lang.String);
}
```

## `cn.hutool.core.img.gif.NeuQuant`

```java
public class cn.hutool.core.img.gif.NeuQuant {
  public cn.hutool.core.img.gif.NeuQuant(byte[], int, int);
  public byte[] colorMap();
  public void inxbuild();
  public void learn();
  public int map(int, int, int);
  public byte[] process();
  public void unbiasnet();
}
```
