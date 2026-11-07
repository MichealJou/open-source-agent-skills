# cn.hutool.core.img

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.img.BackgroundRemoval` | `BufferedImage backgroundRemoval(BufferedImage bufferedImage,Color override,int tolerance)` | 背景移除 图片去底工具 将 "纯色背景的图片" 还原成 "透明背景的图片" 将纯色背景的图片转成矢量图 取图片边缘的像素点和获取到的图片主题色作为要替换的背景色 再加入一定的容差值,然后将所有像素点与该颜色进行比较 发现相同则将颜色不透明度设置为0,使颜色完全透明. |
| `cn.hutool.core.img.BackgroundRemoval` | `BufferedImage backgroundRemoval(ByteArrayOutputStream outputStream,Color override,int tolerance)` | 背景移除 图片去底工具 将 "纯色背景的图片" 还原成 "透明背景的图片" 将纯色背景的图片转成矢量图 取图片边缘的像素点和获取到的图片主题色作为要替换的背景色 再加入一定的容差值,然后将所有像素点与该颜色进行比较 发现相同则将颜色不透明度设置为0,使颜色完全透明. |
| `cn.hutool.core.img.BackgroundRemoval` | `Color hexToRgb(String hex)` | 十六进制颜色码转RGB颜色值 |
| `cn.hutool.core.img.BackgroundRemoval` | `String getMainColor(BufferedImage bufferedImage)` | 获取图片大概的主题色 循环所有的像素点,取出出现次数最多的一个像素点的RGB值 |
| `cn.hutool.core.img.BackgroundRemoval` | `String getMainColor(File input)` | 获取图片大概的主题色 循环所有的像素点,取出出现次数最多的一个像素点的RGB值 |
| `cn.hutool.core.img.BackgroundRemoval` | `String getMainColor(String input)` | 获取图片大概的主题色 循环所有的像素点,取出出现次数最多的一个像素点的RGB值 |
| `cn.hutool.core.img.BackgroundRemoval` | `boolean areColorsWithinTolerance(Color color1,Color color2,Color tolerance)` | 判断颜色是否在容差范围内 对比两个颜色的相似度，判断这个相似度是否小于 tolerance 容差值 |
| `cn.hutool.core.img.BackgroundRemoval` | `boolean areColorsWithinTolerance(Color color1,Color color2,int tolerance)` | 判断颜色是否在容差范围内 对比两个颜色的相似度，判断这个相似度是否小于 tolerance 容差值 |
| `cn.hutool.core.img.BackgroundRemoval` | `boolean backgroundRemoval(File input,File output,Color override,int tolerance)` | 背景移除 图片去底工具 将 "纯色背景的图片" 还原成 "透明背景的图片" 将纯色背景的图片转成矢量图 取图片边缘的像素点和获取到的图片主题色作为要替换的背景色 再加入一定的容差值,然后将所有像素点与该颜色进行比较 发现相同则将颜色不透明度设置为0,使颜色完全透明. |
| `cn.hutool.core.img.BackgroundRemoval` | `boolean backgroundRemoval(File input,File output,int tolerance)` | 背景移除 图片去底工具 将 "纯色背景的图片" 还原成 "透明背景的图片" 将纯色背景的图片转成矢量图 取图片边缘的像素点和获取到的图片主题色作为要替换的背景色 再加入一定的容差值,然后将所有像素点与该颜色进行比较 发现相同则将颜色不透明度设置为0,使颜色完全透明. |
| `cn.hutool.core.img.BackgroundRemoval` | `boolean backgroundRemoval(String inputPath,String outputPath,int tolerance)` | 背景移除 图片去底工具 将 "纯色背景的图片" 还原成 "透明背景的图片" 将纯色背景的图片转成矢量图 取图片边缘的像素点和获取到的图片主题色作为要替换的背景色 再加入一定的容差值,然后将所有像素点与该颜色进行比较 发现相同则将颜色不透明度设置为0,使颜色完全透明. |
| `cn.hutool.core.img.ColorUtil` | `Color add(Color color1,Color color2)` | 叠加颜色 |
| `cn.hutool.core.img.ColorUtil` | `Color getColor(String colorName)` | 将颜色值转换成具体的颜色类型 汇集了常用的颜色集，支持以下几种形式： |
| `cn.hutool.core.img.ColorUtil` | `Color getColor(int rgb)` | 获取一个RGB值对应的颜色 |
| `cn.hutool.core.img.ColorUtil` | `Color hexToColor(String hex)` | 16进制的颜色值转换为Color对象，例如#fcf6d6 |
| `cn.hutool.core.img.ColorUtil` | `Color randomColor()` | 生成随机颜色 |
| `cn.hutool.core.img.ColorUtil` | `Color randomColor(Color compareColor,int minDistance)` | 生成随机颜色，与指定颜色有一定的区分度 |
| `cn.hutool.core.img.ColorUtil` | `Color randomColor(Random random)` | 生成随机颜色 |
| `cn.hutool.core.img.ColorUtil` | `String getMainColor(BufferedImage image,int[]... rgbFilters)` | 获取给定图片的主色调，背景填充用 |
| `cn.hutool.core.img.ColorUtil` | `String toHex(Color color)` | Color对象转16进制表示，例如#fcf6d6 |
| `cn.hutool.core.img.ColorUtil` | `String toHex(int r,int g,int b)` | RGB颜色值转换成十六进制颜色码 |
| `cn.hutool.core.img.ColorUtil` | `int computeColorDistance(Color color1,Color color2)` | 计算两个颜色之间的色差，按三维坐标距离计算 |
| `cn.hutool.core.img.ColorUtil` | `int maxDistance(final Color color)` | 计算给定点与其他点之间的最大可能距离。 |
| `cn.hutool.core.img.FontUtil` | `Dimension getDimension(FontMetrics metrics,String str)` | 获得字体对应字符串的长宽信息 |
| `cn.hutool.core.img.FontUtil` | `Font createFont()` | 创建默认字体 |
| `cn.hutool.core.img.FontUtil` | `Font createFont(File fontFile)` | 根据文件创建字体 首先尝试创建Font#TRUETYPE_FONT字体，此类字体无效则创建Font#TYPE1_FONT |
| `cn.hutool.core.img.FontUtil` | `Font createFont(InputStream fontStream)` | 根据文件创建字体 首先尝试创建Font#TRUETYPE_FONT字体，此类字体无效则创建Font#TYPE1_FONT |
| `cn.hutool.core.img.FontUtil` | `Font createFont(String name,int size)` | 创建指定名称的字体 |
| `cn.hutool.core.img.FontUtil` | `Font createSansSerifFont(int size)` | 创建SansSerif字体 |
| `cn.hutool.core.img.GraphicsUtil` | `Graphics drawImg(Graphics g,Image img,Point point)` | 绘制图片 |
| `cn.hutool.core.img.GraphicsUtil` | `Graphics drawImg(Graphics g,Image img,Rectangle rectangle)` | 绘制图片 |
| `cn.hutool.core.img.GraphicsUtil` | `Graphics drawString(Graphics g,String str,Font font,Color color,Point point)` | 绘制字符串，默认抗锯齿 |
| `cn.hutool.core.img.GraphicsUtil` | `Graphics drawString(Graphics g,String str,Font font,Color color,Rectangle rectangle)` | 绘制字符串，默认抗锯齿。 此方法定义一个矩形区域和坐标，文字基于这个区域中间偏移x,y绘制。 |
| `cn.hutool.core.img.GraphicsUtil` | `Graphics drawString(Graphics g,String str,Font font,Color color,int width,int height)` | 绘制字符串，默认抗锯齿 |
| `cn.hutool.core.img.GraphicsUtil` | `Graphics drawString(Graphics g,String str,Font font,Color color,int width,int height,Color compareColor,int minColorDistance)` | 绘制字符串，默认抗锯齿 |
| `cn.hutool.core.img.GraphicsUtil` | `Graphics drawStringColourful(Graphics g,String str,Font font,int width,int height)` | 绘制字符串，使用随机颜色，默认抗锯齿 |
| `cn.hutool.core.img.GraphicsUtil` | `Graphics drawStringColourful(Graphics g,String str,Font font,int width,int height,Color backgroundColor)` | 绘制字符串，使用随机颜色，并且与背景颜色保持一定色差，默认抗锯齿 |
| `cn.hutool.core.img.GraphicsUtil` | `Graphics drawStringColourful(Graphics g,String str,Font font,int width,int height,Color compareColor,int minColorDistance)` | 绘制字符串，使用随机颜色，默认抗锯齿 |
| `cn.hutool.core.img.GraphicsUtil` | `Graphics2D createGraphics(BufferedImage image,Color color)` | 创建Graphics2D |
| `cn.hutool.core.img.GraphicsUtil` | `Graphics2D setAlpha(Graphics2D g,float alpha)` | 设置画笔透明度 |
| `cn.hutool.core.img.GraphicsUtil` | `int getCenterY(Graphics g,int backgroundHeight)` | 获取文字居中高度的Y坐标（距离上边距距离） 此方法依赖FontMetrics，如果获取失败，默认为背景高度的1/3 |
| `cn.hutool.core.img.Img` | `Image getImg()` | 获取处理过的图片 |
| `cn.hutool.core.img.Img` | `Img binary()` | 彩色转为黑白二值化图片 |
| `cn.hutool.core.img.Img` | `Img cut(Rectangle rectangle)` | 图像切割(按指定起点坐标和宽高切割) |
| `cn.hutool.core.img.Img` | `Img cut(int x,int y)` | 图像切割为圆形(按指定起点坐标和半径切割)，填充满整个图片（直径取长宽最小值） |
| `cn.hutool.core.img.Img` | `Img cut(int x,int y,int radius)` | 图像切割为圆形(按指定起点坐标和半径切割) |
| `cn.hutool.core.img.Img` | `Img flip()` | 水平翻转图像 |
| `cn.hutool.core.img.Img` | `Img from(File imageFile)` | 从文件读取图片并开始处理 |
| `cn.hutool.core.img.Img` | `Img from(Image image)` | 从Image取图片并开始处理 |
| `cn.hutool.core.img.Img` | `Img from(ImageInputStream imageStream)` | 从ImageInputStream取图片并开始处理 |
| `cn.hutool.core.img.Img` | `Img from(InputStream in)` | 从流读取图片并开始处理 |
| `cn.hutool.core.img.Img` | `Img from(Path imagePath)` | 从Path读取图片并开始处理 |
| `cn.hutool.core.img.Img` | `Img from(Resource resource)` | 从资源对象中读取图片并开始处理 |
| `cn.hutool.core.img.Img` | `Img from(URL imageUrl)` | 从URL取图片并开始处理 |
| `cn.hutool.core.img.Img` | `Img gray()` | 彩色转为灰度 |
| `cn.hutool.core.img.Img` | `Img pressImage(Image pressImg,Rectangle rectangle,float alpha)` | 给图片添加图片水印 |
| `cn.hutool.core.img.Img` | `Img pressImage(Image pressImg,int x,int y,float alpha)` | 给图片添加图片水印 |
| `cn.hutool.core.img.Img` | `Img pressText(String pressText,Color color,Font font,Point point,float alpha)` | 给图片添加文字水印 此方法只在给定位置写出一个水印字符串 |
| `cn.hutool.core.img.Img` | `Img pressText(String pressText,Color color,Font font,int x,int y,float alpha)` | 给图片添加文字水印 此方法只在给定位置写出一个水印字符串 |
| `cn.hutool.core.img.Img` | `Img pressTextFull(String pressText,Color color,Font font,int lineHeight,int degree,float alpha)` | 给图片添加全屏文字水印 |
| `cn.hutool.core.img.Img` | `Img rotate(int degree)` | 旋转图片为指定角度 来自：http://blog.51cto.com/cping1982/130066 |
| `cn.hutool.core.img.Img` | `Img round(double arc)` | 图片圆角处理 |
| `cn.hutool.core.img.Img` | `Img scale(float scale)` | 缩放图像（按比例缩放） |
| `cn.hutool.core.img.Img` | `Img scale(int width,int height)` | 缩放图像（按长宽缩放） 注意：目标长宽与原图不成比例会变形 |
| `cn.hutool.core.img.Img` | `Img scale(int width,int height,Color fixedColor)` | 等比缩放图像，此方法按照按照给定的长宽等比缩放图片，按照长宽缩放比最多的一边等比缩放，空白部分填充背景色 缩放后默认为jpeg格式 |
| `cn.hutool.core.img.Img` | `Img scale(int width,int height,int scaleType)` | 缩放图像（按长宽缩放） 注意：目标长宽与原图不成比例会变形 |
| `cn.hutool.core.img.Img` | `Img setBackgroundColor(Color backgroundColor)` | 设置图片的背景色 |
| `cn.hutool.core.img.Img` | `Img setPositionBaseCentre(boolean positionBaseCentre)` | 计算x,y坐标的时候是否从中心做为原始坐标开始计算 |
| `cn.hutool.core.img.Img` | `Img setQuality(double quality)` | 设置图片输出质量，数字为0~1（不包括0和1）表示质量压缩比，除此数字外设置表示不压缩 |
| `cn.hutool.core.img.Img` | `Img setQuality(float quality)` | 设置图片输出质量，数字为0~1（不包括0和1）表示质量压缩比，除此数字外设置表示不压缩 |
| `cn.hutool.core.img.Img` | `Img setTargetImageType(String imgType)` | 设置目标图片文件格式，用于写出 |
| `cn.hutool.core.img.Img` | `Img stroke(Color color,Stroke stroke)` | 描边，此方法为向内描边，会覆盖图片相应的位置 |
| `cn.hutool.core.img.Img` | `Img stroke(Color color,float width)` | 描边，此方法为向内描边，会覆盖图片相应的位置 |
| `cn.hutool.core.img.Img` | `boolean write(File targetFile)` | 写出图像为目标文件扩展名对应的格式 |
| `cn.hutool.core.img.Img` | `boolean write(ImageOutputStream targetImageStream)` | 写出图像为结果设置格式 结果类型设定见#setTargetImageType(String) |
| `cn.hutool.core.img.Img` | `boolean write(OutputStream out)` | 写出图像为结果设置格式 结果类型设定见#setTargetImageType(String) |
| `cn.hutool.core.img.Img` | `void flush()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage backgroundRemoval(BufferedImage bufferedImage,Color override,int tolerance)` | 背景移除 图片去底工具 将 "纯色背景的图片" 还原成 "透明背景的图片" 将纯色背景的图片转成矢量图 取图片边缘的像素点和获取到的图片主题色作为要替换的背景色 再加入一定的容差值,然后将所有像素点与该颜色进行比较 发现相同则将颜色不透明度设置为0,使颜色完全透明. |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage backgroundRemoval(ByteArrayOutputStream outputStream,Color override,int tolerance)` | 背景移除 图片去底工具 将 "纯色背景的图片" 还原成 "透明背景的图片" 将纯色背景的图片转成矢量图 取图片边缘的像素点和获取到的图片主题色作为要替换的背景色 再加入一定的容差值,然后将所有像素点与该颜色进行比较 发现相同则将颜色不透明度设置为0,使颜色完全透明. |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage castToBufferedImage(final Image img,final String imageType)` | Image 转 BufferedImage 首先尝试强转，否则新建一个BufferedImage后重新绘制，使用 imageType 模式 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage colorConvert(ColorSpace colorSpace,BufferedImage image)` | 图片颜色转换 可以使用灰度 (gray)等 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage copyImage(Image img,int imageType)` | 将已有Image复制新的一份出来 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage copyImage(Image img,int imageType,Color backgroundColor)` | 将已有Image复制新的一份出来 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage createCompatibleImage(int width,int height,int transparency)` | 创建与当前设备颜色模式兼容的 BufferedImage |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage createImage(String str,Font font,Color backgroundColor,Color fontColor,int imageType)` | 根据文字创建图片 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage filter(BufferedImageOp op,BufferedImage image)` | 图片过滤转换 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage read(File imageFile)` | 从文件中读取图片 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage read(ImageInputStream imageStream)` | 从图片流中读取图片 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage read(InputStream imageStream)` | 从流中读取图片 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage read(Resource resource)` | 从Resource中读取图片 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage read(String imageFilePath)` | 从文件中读取图片，请使用绝对路径，使用相对路径会相对于ClassPath |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage read(URL imageUrl)` | 从URL中读取图片 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage toBufferedImage(Image image,String imageType)` | Image 转 BufferedImage 如果源图片的RGB模式与目标模式一致，则直接转换，否则重新绘制 默认的，png图片使用 BufferedImage#TYPE_INT_ARGB模式，其它使用 BufferedImage#TYPE_INT_RGB 模式 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage toBufferedImage(Image image,String imageType,Color backgroundColor)` | Image 转 BufferedImage 如果源图片的RGB模式与目标模式一致，则直接转换，否则重新绘制 默认的，png图片使用 BufferedImage#TYPE_INT_ARGB模式，其它使用 BufferedImage#TYPE_INT_RGB 模式 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage toBufferedImage(Image image,int imageType)` | Image 转 BufferedImage 如果源图片的RGB模式与目标模式一致，则直接转换，否则重新绘制 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage toBufferedImage(Image image,int imageType,Color backgroundColor)` | Image 转 BufferedImage 如果源图片的RGB模式与目标模式一致，则直接转换，否则重新绘制 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage toBufferedImage(Image img)` | Image 转 BufferedImage 首先尝试强转，否则新建一个BufferedImage后重新绘制，使用 BufferedImage#TYPE_INT_RGB 模式 |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage toImage(String base64)` | 将Base64编码的图像信息转为 BufferedImage |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage toImage(byte[] imageBytes)` | 将的图像bytes转为 BufferedImage |
| `cn.hutool.core.img.ImgUtil` | `BufferedImage transform(AffineTransform xform,BufferedImage image)` | 转换图片 可以使用一系列平移 (translation)、缩放 (scale)、翻转 (flip)、旋转 (rotation) 和错切 (shear) 来构造仿射变换。 |
| `cn.hutool.core.img.ImgUtil` | `ByteArrayInputStream toStream(Image image,String imageType)` | 将图片对象转换为InputStream形式 |
| `cn.hutool.core.img.ImgUtil` | `Color getColor(String colorName)` | 将颜色值转换成具体的颜色类型 汇集了常用的颜色集，支持以下几种形式： |
| `cn.hutool.core.img.ImgUtil` | `Color getColor(int rgb)` | 获取一个RGB值对应的颜色 |
| `cn.hutool.core.img.ImgUtil` | `Color hexToColor(String hex)` | 16进制的颜色值转换为Color对象，例如#fcf6d6 |
| `cn.hutool.core.img.ImgUtil` | `Color randomColor()` | 生成随机颜色 |
| `cn.hutool.core.img.ImgUtil` | `Color randomColor(Color compareColor)` | 生成随机颜色，与指定颜色有一定的区分度 |
| `cn.hutool.core.img.ImgUtil` | `Color randomColor(Color compareColor,int minDistance)` | 生成随机颜色，与指定颜色有一定的区分度 |
| `cn.hutool.core.img.ImgUtil` | `Color randomColor(Random random)` | 生成随机颜色 |
| `cn.hutool.core.img.ImgUtil` | `Font createFont(File fontFile)` | 根据文件创建字体 首先尝试创建Font#TRUETYPE_FONT字体，此类字体无效则创建Font#TYPE1_FONT |
| `cn.hutool.core.img.ImgUtil` | `Font createFont(InputStream fontStream)` | 根据文件创建字体 首先尝试创建Font#TRUETYPE_FONT字体，此类字体无效则创建Font#TYPE1_FONT |
| `cn.hutool.core.img.ImgUtil` | `Graphics2D createGraphics(BufferedImage image,Color color)` | 创建Graphics2D |
| `cn.hutool.core.img.ImgUtil` | `Image binary(Image srcImage)` | 彩色转为黑白二值化图片 |
| `cn.hutool.core.img.ImgUtil` | `Image cut(Image srcImage,Rectangle rectangle)` | 图像切割(按指定起点坐标和宽高切割) |
| `cn.hutool.core.img.ImgUtil` | `Image cut(Image srcImage,int x,int y)` | 图像切割(按指定起点坐标和宽高切割)，填充满整个图片（直径取长宽最小值） |
| `cn.hutool.core.img.ImgUtil` | `Image cut(Image srcImage,int x,int y,int radius)` | 图像切割(按指定起点坐标和宽高切割) |
| `cn.hutool.core.img.ImgUtil` | `Image filter(ImageFilter filter,Image image)` | 图片滤镜，借助 ImageFilter实现，实现不同的图片滤镜 |
| `cn.hutool.core.img.ImgUtil` | `Image flip(Image image)` | 水平翻转图像 |
| `cn.hutool.core.img.ImgUtil` | `Image getImage(URL url)` | 从URL中获取或读取图片对象 |
| `cn.hutool.core.img.ImgUtil` | `Image gray(Image srcImage)` | 彩色转为黑白 |
| `cn.hutool.core.img.ImgUtil` | `Image pressImage(Image srcImage,Image pressImg,Rectangle rectangle,float alpha)` | 给图片添加图片水印 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `Image pressImage(Image srcImage,Image pressImg,int x,int y,float alpha)` | 给图片添加图片水印 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `Image pressText(Image srcImage,String pressText,Color color,Font font,int x,int y,float alpha)` | 给图片添加文字水印 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `Image rotate(Image image,int degree)` | 旋转图片为指定角度 来自： http://blog.51cto.com/cping1982/130066 |
| `cn.hutool.core.img.ImgUtil` | `Image scale(Image srcImage,int width,int height,Color fixedColor)` | 缩放图像（按高度和宽度缩放） 缩放后默认为jpeg格式 |
| `cn.hutool.core.img.ImgUtil` | `Image scale(Image srcImg,float scale)` | 缩放图像（按比例缩放） |
| `cn.hutool.core.img.ImgUtil` | `Image scale(Image srcImg,int width,int height)` | 缩放图像（按长宽缩放） 注意：目标长宽与原图不成比例会变形 |
| `cn.hutool.core.img.ImgUtil` | `ImageInputStream getImageInputStream(InputStream in)` | 获取ImageInputStream |
| `cn.hutool.core.img.ImgUtil` | `ImageOutputStream getImageOutputStream(File outFile)` | 获取ImageOutputStream |
| `cn.hutool.core.img.ImgUtil` | `ImageOutputStream getImageOutputStream(OutputStream out)` | 获取ImageOutputStream |
| `cn.hutool.core.img.ImgUtil` | `ImageReader getReader(String type)` | 获得ImageReader |
| `cn.hutool.core.img.ImgUtil` | `ImageWriter getWriter(Image img,String formatName)` | 根据给定的Image对象和格式获取对应的ImageWriter，如果未找到合适的Writer，返回null |
| `cn.hutool.core.img.ImgUtil` | `ImageWriter getWriter(String formatName)` | 根据给定的图片格式或者扩展名获取ImageWriter，如果未找到合适的Writer，返回null |
| `cn.hutool.core.img.ImgUtil` | `Point getPointBaseCentre(Rectangle rectangle,int backgroundWidth,int backgroundHeight)` | 获得修正后的矩形坐标位置，变为以背景中心为基准坐标（即x,y == 0,0时，处于背景正中） |
| `cn.hutool.core.img.ImgUtil` | `Rectangle2D getRectangle(String str,Font font)` | 获取font的样式应用在str上的整个矩形 |
| `cn.hutool.core.img.ImgUtil` | `RenderedImage castToRenderedImage(final Image img,final String imageType)` | Image 转 RenderedImage 首先尝试强转，否则新建一个BufferedImage后重新绘制，使用 BufferedImage#TYPE_INT_RGB 模式。 |
| `cn.hutool.core.img.ImgUtil` | `RenderedImage toRenderedImage(Image img)` | Image 转 RenderedImage 首先尝试强转，否则新建一个BufferedImage后重新绘制，使用 BufferedImage#TYPE_INT_RGB 模式。 |
| `cn.hutool.core.img.ImgUtil` | `String getMainColor(BufferedImage image,int[]... rgbFilters)` | 获取给定图片的主色调，背景填充用 |
| `cn.hutool.core.img.ImgUtil` | `String toBase64(Image image,String imageType)` | 将图片对象转换为Base64形式 |
| `cn.hutool.core.img.ImgUtil` | `String toBase64DataUri(Image image,String imageType)` | 将图片对象转换为Base64的Data URI形式，格式为：data:image/[imageType];base64,[data] |
| `cn.hutool.core.img.ImgUtil` | `String toHex(Color color)` | Color对象转16进制表示，例如#fcf6d6 |
| `cn.hutool.core.img.ImgUtil` | `String toHex(int r,int g,int b)` | RGB颜色值转换成十六进制颜色码 |
| `cn.hutool.core.img.ImgUtil` | `boolean backgroundRemoval(File input,File output,Color override,int tolerance)` | 背景移除 图片去底工具 将 "纯色背景的图片" 还原成 "透明背景的图片" 将纯色背景的图片转成矢量图 取图片边缘的像素点和获取到的图片主题色作为要替换的背景色 再加入一定的容差值,然后将所有像素点与该颜色进行比较 发现相同则将颜色不透明度设置为0,使颜色完全透明. |
| `cn.hutool.core.img.ImgUtil` | `boolean backgroundRemoval(File input,File output,int tolerance)` | 背景移除 图片去底工具 将 "纯色背景的图片" 还原成 "透明背景的图片" 将纯色背景的图片转成矢量图 取图片边缘的像素点和获取到的图片主题色作为要替换的背景色 再加入一定的容差值,然后将所有像素点与该颜色进行比较 发现相同则将颜色不透明度设置为0,使颜色完全透明. |
| `cn.hutool.core.img.ImgUtil` | `boolean backgroundRemoval(String inputPath,String outputPath,int tolerance)` | 背景移除 图片去底工具 将 "纯色背景的图片" 还原成 "透明背景的图片" 将纯色背景的图片转成矢量图 取图片边缘的像素点和获取到的图片主题色作为要替换的背景色 再加入一定的容差值,然后将所有像素点与该颜色进行比较 发现相同则将颜色不透明度设置为0,使颜色完全透明. |
| `cn.hutool.core.img.ImgUtil` | `boolean write(Image image,ImageWriter writer,ImageOutputStream output,float quality)` | 通过ImageWriter写出图片到输出流 |
| `cn.hutool.core.img.ImgUtil` | `boolean write(Image image,String imageType,ImageOutputStream destImageStream)` | 写出图像为指定格式：GIF=》JPG、GIF=》PNG、PNG=》JPG、PNG=》GIF(X)、BMP=》PNG 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `boolean write(Image image,String imageType,ImageOutputStream destImageStream,float quality)` | 写出图像为指定格式 |
| `cn.hutool.core.img.ImgUtil` | `boolean write(Image image,String imageType,ImageOutputStream destImageStream,float quality,Color backgroundColor)` | 写出图像为指定格式 |
| `cn.hutool.core.img.ImgUtil` | `byte[] toBytes(Image image,String imageType)` | 将图片对象转换为bytes形式 |
| `cn.hutool.core.img.ImgUtil` | `void binary(File srcImageFile,File destImageFile)` | 彩色转为黑白二值化图片，根据目标文件扩展名确定转换后的格式 |
| `cn.hutool.core.img.ImgUtil` | `void binary(Image srcImage,File outFile)` | 彩色转为黑白二值化图片，根据目标文件扩展名确定转换后的格式 |
| `cn.hutool.core.img.ImgUtil` | `void binary(Image srcImage,ImageOutputStream destImageStream,String imageType)` | 彩色转为黑白二值化图片 此方法并不关闭流，输出JPG格式 |
| `cn.hutool.core.img.ImgUtil` | `void binary(Image srcImage,OutputStream out,String imageType)` | 彩色转为黑白二值化图片 此方法并不关闭流，输出JPG格式 |
| `cn.hutool.core.img.ImgUtil` | `void binary(ImageInputStream srcStream,ImageOutputStream destStream,String imageType)` | 彩色转为黑白黑白二值化图片 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void binary(InputStream srcStream,OutputStream destStream,String imageType)` | 彩色转为黑白二值化图片 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void compress(File imageFile,File outFile,float quality)` | 压缩图像，输出图像只支持jpg文件 |
| `cn.hutool.core.img.ImgUtil` | `void convert(File srcImageFile,File destImageFile)` | 图像类型转换：GIF=》JPG、GIF=》PNG、PNG=》JPG、PNG=》GIF(X)、BMP=》PNG |
| `cn.hutool.core.img.ImgUtil` | `void convert(Image srcImage,String formatName,ImageOutputStream destImageStream)` | 图像类型转换：GIF=》JPG、GIF=》PNG、PNG=》JPG、PNG=》GIF(X)、BMP=》PNG 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void convert(Image srcImage,String formatName,ImageOutputStream destImageStream,boolean isSrcPng)` | 图像类型转换：GIF=》JPG、GIF=》PNG、PNG=》JPG、PNG=》GIF(X)、BMP=》PNG 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void convert(InputStream srcStream,String formatName,OutputStream destStream)` | 图像类型转换：GIF=》JPG、GIF=》PNG、PNG=》JPG、PNG=》GIF(X)、BMP=》PNG 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void createImage(String str,Font font,Color backgroundColor,Color fontColor,ImageOutputStream out)` | 根据文字创建PNG图片 |
| `cn.hutool.core.img.ImgUtil` | `void createTransparentImage(String str,Font font,Color fontColor,ImageOutputStream out)` | 根据文字创建透明背景的PNG图片 |
| `cn.hutool.core.img.ImgUtil` | `void cut(File srcImgFile,File destImgFile,Rectangle rectangle)` | 图像切割(按指定起点坐标和宽高切割) |
| `cn.hutool.core.img.ImgUtil` | `void cut(Image srcImage,File destFile,Rectangle rectangle)` | 图像切割(按指定起点坐标和宽高切割)，此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void cut(Image srcImage,ImageOutputStream destImageStream,Rectangle rectangle)` | 图像切割(按指定起点坐标和宽高切割)，此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void cut(Image srcImage,OutputStream out,Rectangle rectangle)` | 图像切割(按指定起点坐标和宽高切割)，此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void cut(ImageInputStream srcStream,ImageOutputStream destStream,Rectangle rectangle)` | 图像切割(按指定起点坐标和宽高切割)，此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void cut(InputStream srcStream,OutputStream destStream,Rectangle rectangle)` | 图像切割(按指定起点坐标和宽高切割)，此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void flip(File imageFile,File outFile)` | 水平翻转图像 |
| `cn.hutool.core.img.ImgUtil` | `void flip(Image image,File outFile)` | 水平翻转图像 |
| `cn.hutool.core.img.ImgUtil` | `void flip(Image image,ImageOutputStream out)` | 水平翻转图像，写出格式为JPG |
| `cn.hutool.core.img.ImgUtil` | `void flip(Image image,OutputStream out)` | 水平翻转图像 |
| `cn.hutool.core.img.ImgUtil` | `void flush(Image image)` | 刷新和释放Image 资源 |
| `cn.hutool.core.img.ImgUtil` | `void gray(File srcImageFile,File destImageFile)` | 彩色转为黑白 |
| `cn.hutool.core.img.ImgUtil` | `void gray(Image srcImage,File outFile)` | 彩色转为黑白 |
| `cn.hutool.core.img.ImgUtil` | `void gray(Image srcImage,ImageOutputStream destImageStream)` | 彩色转为黑白 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void gray(Image srcImage,OutputStream out)` | 彩色转为黑白 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void gray(ImageInputStream srcStream,ImageOutputStream destStream)` | 彩色转为黑白 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void gray(InputStream srcStream,OutputStream destStream)` | 彩色转为黑白 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void pressImage(File srcImageFile,File destImageFile,Image pressImg,int x,int y,float alpha)` | 给图片添加图片水印 |
| `cn.hutool.core.img.ImgUtil` | `void pressImage(Image srcImage,File outFile,Image pressImg,int x,int y,float alpha)` | 给图片添加图片水印 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void pressImage(Image srcImage,ImageOutputStream destImageStream,Image pressImg,int x,int y,float alpha)` | 给图片添加图片水印 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void pressImage(Image srcImage,OutputStream out,Image pressImg,int x,int y,float alpha)` | 给图片添加图片水印 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void pressImage(ImageInputStream srcStream,ImageOutputStream destStream,Image pressImg,int x,int y,float alpha)` | 给图片添加图片水印 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void pressImage(InputStream srcStream,OutputStream destStream,Image pressImg,int x,int y,float alpha)` | 给图片添加图片水印 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void pressText(File imageFile,File destFile,String pressText,Color color,Font font,int x,int y,float alpha)` | 给图片添加文字水印 |
| `cn.hutool.core.img.ImgUtil` | `void pressText(Image srcImage,File destFile,String pressText,Color color,Font font,int x,int y,float alpha)` | 给图片添加文字水印 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void pressText(Image srcImage,ImageOutputStream destImageStream,String pressText,Color color,Font font,int x,int y,float alpha)` | 给图片添加文字水印 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void pressText(Image srcImage,OutputStream to,String pressText,Color color,Font font,int x,int y,float alpha)` | 给图片添加文字水印 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void pressText(ImageInputStream srcStream,ImageOutputStream destStream,String pressText,Color color,Font font,int x,int y,float alpha)` | 给图片添加文字水印 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void pressText(InputStream srcStream,OutputStream destStream,String pressText,Color color,Font font,int x,int y,float alpha)` | 给图片添加文字水印 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void rotate(File imageFile,int degree,File outFile)` | 旋转图片为指定角度 此方法不会关闭输出流 |
| `cn.hutool.core.img.ImgUtil` | `void rotate(Image image,int degree,File outFile)` | 旋转图片为指定角度 此方法不会关闭输出流 |
| `cn.hutool.core.img.ImgUtil` | `void rotate(Image image,int degree,ImageOutputStream out)` | 旋转图片为指定角度 此方法不会关闭输出流，输出格式为JPG |
| `cn.hutool.core.img.ImgUtil` | `void rotate(Image image,int degree,OutputStream out)` | 旋转图片为指定角度 此方法不会关闭输出流 |
| `cn.hutool.core.img.ImgUtil` | `void scale(File srcImageFile,File destImageFile,float scale)` | 缩放图像（按比例缩放），目标文件的扩展名决定目标文件类型 |
| `cn.hutool.core.img.ImgUtil` | `void scale(File srcImageFile,File destImageFile,int width,int height,Color fixedColor)` | 缩放图像（按高度和宽度缩放） 缩放后默认格式与源图片相同，无法识别原图片默认JPG |
| `cn.hutool.core.img.ImgUtil` | `void scale(Image srcImage,ImageOutputStream destImageStream,int width,int height,Color fixedColor)` | 缩放图像（按高度和宽度缩放） 缩放后默认为jpeg格式，此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void scale(Image srcImg,File destFile,float scale)` | 缩放图像（按比例缩放） 缩放后默认为jpeg格式，此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void scale(Image srcImg,ImageOutputStream destImageStream,float scale)` | 缩放图像（按比例缩放） 缩放后默认为jpeg格式，此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void scale(Image srcImg,OutputStream out,float scale)` | 缩放图像（按比例缩放） 缩放后默认为jpeg格式，此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void scale(ImageInputStream srcStream,ImageOutputStream destStream,float scale)` | 缩放图像（按比例缩放） 缩放后默认为jpeg格式，此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void scale(ImageInputStream srcStream,ImageOutputStream destStream,int width,int height,Color fixedColor)` | 缩放图像（按高度和宽度缩放） 缩放后默认为jpeg格式，此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void scale(InputStream srcStream,OutputStream destStream,float scale)` | 缩放图像（按比例缩放） 缩放后默认为jpeg格式，此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void scale(InputStream srcStream,OutputStream destStream,int width,int height,Color fixedColor)` | 缩放图像（按高度和宽度缩放） 缩放后默认为jpeg格式，此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void slice(File srcImageFile,File descDir,int destWidth,int destHeight)` | 图像切片（指定切片的宽度和高度） |
| `cn.hutool.core.img.ImgUtil` | `void slice(Image srcImage,File descDir,int destWidth,int destHeight)` | 图像切片（指定切片的宽度和高度） |
| `cn.hutool.core.img.ImgUtil` | `void sliceByRowsAndCols(File srcImageFile,File destDir,String format,int rows,int cols)` | 图像切割（指定切片的行数和列数） |
| `cn.hutool.core.img.ImgUtil` | `void sliceByRowsAndCols(File srcImageFile,File destDir,int rows,int cols)` | 图像切割（指定切片的行数和列数） |
| `cn.hutool.core.img.ImgUtil` | `void sliceByRowsAndCols(Image srcImage,File destDir,String format,int rows,int cols)` | 图像切割（指定切片的行数和列数），默认RGB模式 |
| `cn.hutool.core.img.ImgUtil` | `void sliceByRowsAndCols(Image srcImage,File destDir,int rows,int cols)` | 图像切割（指定切片的行数和列数），默认RGB模式 |
| `cn.hutool.core.img.ImgUtil` | `void write(Image image,File targetFile)` | 写出图像为目标文件扩展名对应的格式 |
| `cn.hutool.core.img.ImgUtil` | `void write(Image image,String imageType,OutputStream out)` | 写出图像：GIF=》JPG、GIF=》PNG、PNG=》JPG、PNG=》GIF(X)、BMP=》PNG 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void write(ImageInputStream srcStream,String formatName,ImageOutputStream destStream)` | 按照目标格式写出图像：GIF=》JPG、GIF=》PNG、PNG=》JPG、PNG=》GIF(X)、BMP=》PNG 此方法并不关闭流 |
| `cn.hutool.core.img.ImgUtil` | `void writeJpg(Image image,ImageOutputStream destImageStream)` | 写出图像为JPG格式 |
| `cn.hutool.core.img.ImgUtil` | `void writeJpg(Image image,OutputStream out)` | 写出图像为JPG格式 |
| `cn.hutool.core.img.ImgUtil` | `void writePng(Image image,ImageOutputStream destImageStream)` | 写出图像为PNG格式 |
| `cn.hutool.core.img.ImgUtil` | `void writePng(Image image,OutputStream out)` | 写出图像为PNG格式 |
| `cn.hutool.core.img.LabColor` | `double getDistance(LabColor other)` | 获取颜色差 |
| `cn.hutool.core.img.ScaleType` | `int getValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
