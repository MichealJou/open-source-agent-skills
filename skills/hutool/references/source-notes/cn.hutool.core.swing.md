# cn.hutool.core.swing

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.swing.DesktopUtil` | `Desktop getDsktop()` | 获得Desktop |
| `cn.hutool.core.swing.DesktopUtil` | `void browse(String url)` | 使用平台默认浏览器打开指定URL地址 |
| `cn.hutool.core.swing.DesktopUtil` | `void browse(URI uri)` | 使用平台默认浏览器打开指定URI地址 |
| `cn.hutool.core.swing.DesktopUtil` | `void edit(File file)` | 启动关联编辑器应用程序并打开用于编辑的文件 |
| `cn.hutool.core.swing.DesktopUtil` | `void mail(String mailAddress)` | 使用平台默认浏览器打开指定URL地址 |
| `cn.hutool.core.swing.DesktopUtil` | `void open(File file)` | 启动关联应用程序来打开文件 |
| `cn.hutool.core.swing.DesktopUtil` | `void print(File file)` | 使用关联应用程序的打印命令, 用本机桌面打印设备来打印文件 |
| `cn.hutool.core.swing.RobotUtil` | `BufferedImage captureScreen()` | 截取全屏 |
| `cn.hutool.core.swing.RobotUtil` | `BufferedImage captureScreen(Rectangle screenRect)` | 截屏 |
| `cn.hutool.core.swing.RobotUtil` | `File captureScreen(File outFile)` | 截取全屏到文件 |
| `cn.hutool.core.swing.RobotUtil` | `File captureScreen(Rectangle screenRect,File outFile)` | 截屏 |
| `cn.hutool.core.swing.RobotUtil` | `Robot getRobot()` | 获取 Robot 单例实例 |
| `cn.hutool.core.swing.RobotUtil` | `int getDelay()` | 获取全局默认的延迟时间 |
| `cn.hutool.core.swing.RobotUtil` | `void click()` | 模拟单击 鼠标单击包括鼠标左键的按下和释放 |
| `cn.hutool.core.swing.RobotUtil` | `void delay()` | 等待指定毫秒数 |
| `cn.hutool.core.swing.RobotUtil` | `void keyClick(int... keyCodes)` | 模拟键盘点击 包括键盘的按下和释放 |
| `cn.hutool.core.swing.RobotUtil` | `void keyPressString(String str)` | 打印输出指定字符串（借助剪贴板） |
| `cn.hutool.core.swing.RobotUtil` | `void keyPressWithAlt(int key)` | alt+ 按键 |
| `cn.hutool.core.swing.RobotUtil` | `void keyPressWithCtrl(int key)` | ctrl+ 按键 |
| `cn.hutool.core.swing.RobotUtil` | `void keyPressWithShift(int key)` | shift+ 按键 |
| `cn.hutool.core.swing.RobotUtil` | `void mouseMove(int x,int y)` | 模拟鼠标移动 |
| `cn.hutool.core.swing.RobotUtil` | `void mouseWheel(int wheelAmt)` | 模拟鼠标滚轮滚动 |
| `cn.hutool.core.swing.RobotUtil` | `void rightClick()` | 模拟右键单击 鼠标单击包括鼠标右键的按下和释放 |
| `cn.hutool.core.swing.RobotUtil` | `void setDelay(int delayMillis)` | 设置默认的延迟时间 当按键执行完后的等待时间，也可以用ThreadUtil.sleep方法代替 |
| `cn.hutool.core.swing.ScreenUtil` | `BufferedImage captureScreen()` | 截取全屏 |
| `cn.hutool.core.swing.ScreenUtil` | `BufferedImage captureScreen(Rectangle screenRect)` | 截屏 |
| `cn.hutool.core.swing.ScreenUtil` | `File captureScreen(File outFile)` | 截取全屏到文件 |
| `cn.hutool.core.swing.ScreenUtil` | `File captureScreen(Rectangle screenRect,File outFile)` | 截屏 |
| `cn.hutool.core.swing.ScreenUtil` | `Rectangle getRectangle()` | 获取屏幕的矩形 |
| `cn.hutool.core.swing.ScreenUtil` | `int getHeight()` | 获取屏幕高度 |
| `cn.hutool.core.swing.ScreenUtil` | `int getWidth()` | 获取屏幕宽度 |
