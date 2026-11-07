# cn.hutool.core.swing

版本：5.8.46。由本地已安装二进制的公开声明生成；包含构造方法和重载，不展开继承方法。

## `cn.hutool.core.swing.DesktopUtil`

```java
public class cn.hutool.core.swing.DesktopUtil {
  public cn.hutool.core.swing.DesktopUtil();
  public static java.awt.Desktop getDsktop();
  public static void browse(java.lang.String);
  public static void browse(java.net.URI);
  public static void open(java.io.File);
  public static void edit(java.io.File);
  public static void print(java.io.File);
  public static void mail(java.lang.String);
}
```

## `cn.hutool.core.swing.RobotUtil`

```java
public class cn.hutool.core.swing.RobotUtil {
  public cn.hutool.core.swing.RobotUtil();
  public static java.awt.Robot getRobot();
  public static void setDelay(int);
  public static int getDelay();
  public static void mouseMove(int, int);
  public static void click();
  public static void rightClick();
  public static void mouseWheel(int);
  public static void keyClick(int...);
  public static void keyPressString(java.lang.String);
  public static void keyPressWithShift(int);
  public static void keyPressWithCtrl(int);
  public static void keyPressWithAlt(int);
  public static java.awt.image.BufferedImage captureScreen();
  public static java.io.File captureScreen(java.io.File);
  public static java.awt.image.BufferedImage captureScreen(java.awt.Rectangle);
  public static java.io.File captureScreen(java.awt.Rectangle, java.io.File);
  public static void delay();
}
```

## `cn.hutool.core.swing.ScreenUtil`

```java
public class cn.hutool.core.swing.ScreenUtil {
  public cn.hutool.core.swing.ScreenUtil();
  public static int getWidth();
  public static int getHeight();
  public static java.awt.Rectangle getRectangle();
  public static java.awt.image.BufferedImage captureScreen();
  public static java.io.File captureScreen(java.io.File);
  public static java.awt.image.BufferedImage captureScreen(java.awt.Rectangle);
  public static java.io.File captureScreen(java.awt.Rectangle, java.io.File);
}
```
