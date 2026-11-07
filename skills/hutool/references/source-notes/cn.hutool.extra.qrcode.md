# cn.hutool.extra.qrcode

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.qrcode.BufferedImageLuminanceSource` | `LuminanceSource crop(int left,int top,int width,int height)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.qrcode.BufferedImageLuminanceSource` | `LuminanceSource rotateCounterClockwise()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.qrcode.BufferedImageLuminanceSource` | `boolean isCropSupported()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.qrcode.BufferedImageLuminanceSource` | `boolean isRotateSupported()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.qrcode.BufferedImageLuminanceSource` | `byte[] getMatrix()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.qrcode.BufferedImageLuminanceSource` | `byte[] getRow(int y,byte[] row)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `BitMatrix encode(String content,BarcodeFormat format,QrConfig config)` | 将文本内容编码为条形码或二维码 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `BitMatrix encode(String content,BarcodeFormat format,int width,int height)` | 将文本内容编码为条形码或二维码 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `BitMatrix encode(String content,QrConfig config)` | 将文本内容编码为二维码 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `BitMatrix encode(String content,int width,int height)` | 将文本内容编码为二维码 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `BufferedImage generate(String content,BarcodeFormat format,QrConfig config)` | 生成二维码或条形码图片 只有二维码时QrConfig中的图片才有效 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `BufferedImage generate(String content,BarcodeFormat format,int width,int height)` | 生成二维码或条形码图片 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `BufferedImage generate(String content,QrConfig config)` | 生成二维码图片 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `BufferedImage generate(String content,int width,int height)` | 生成二维码图片 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `BufferedImage toImage(BitMatrix matrix,int foreColor,Integer backColor)` | BitMatrix转BufferedImage |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `File generate(String content,QrConfig config,File targetFile)` | 生成二维码到文件，二维码图片格式取决于文件的扩展名 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `File generate(String content,int width,int height,File targetFile)` | 生成二维码到文件，二维码图片格式取决于文件的扩展名 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String decode(File qrCodeFile)` | 解码二维码或条形码图片为文本 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String decode(Image image)` | 将二维码或条形码图片解码为文本 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String decode(Image image,Map<DecodeHintType, Object> hints)` | 将二维码或条形码图片解码为文本 此方法会尝试使用HybridBinarizer和GlobalHistogramBinarizer两种模式解析 需要注意部分二维码如果不带logo，使用PureBarcode模式会解析失败，此时须设置此选项为false。 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String decode(Image image,boolean isTryHarder,boolean isPureBarcode)` | 将二维码或条形码图片解码为文本 此方法会尝试使用HybridBinarizer和GlobalHistogramBinarizer两种模式解析 需要注意部分二维码如果不带logo，使用PureBarcode模式会解析失败，此时须设置此选项为false。 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String decode(InputStream qrCodeInputStream)` | 解码二维码或条形码图片为文本 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String generateAsAsciiArt(String content)` | 生成ASCII Art字符画形式的二维码 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String generateAsAsciiArt(String content,QrConfig qrConfig)` | 生成ASCII Art字符画形式的二维码 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String generateAsAsciiArt(String content,int width,int height,int margin)` | @param content 内容 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String generateAsBase64(String content,QrConfig qrConfig,String targetType)` | 生成 Base64 编码格式的二维码，以 String 形式表示 输出格式为: data:image/[type];base64,[data] |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String generateAsBase64(String content,QrConfig qrConfig,String targetType,Image logo)` | 生成代 logo 图片的 Base64 编码格式的二维码，以 String 形式表示 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String generateAsBase64(String content,QrConfig qrConfig,String targetType,String logoBase64)` | 生成代 logo 图片的 Base64 编码格式的二维码，以 String 形式表示 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String generateAsBase64(String content,QrConfig qrConfig,String targetType,byte[] logo)` | 生成代 logo 图片的 Base64 编码格式的二维码，以 String 形式表示 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String generateAsSvg(String content,QrConfig qrConfig)` | @param content 内容 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String toAsciiArt(BitMatrix bitMatrix,QrConfig qrConfig)` | BitMatrix转ASCII Art字符画形式的二维码 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String toSVG(BitMatrix matrix,Integer foreColor,Integer backColor,Image logoImg,int ratio)` | BitMatrix转SVG(字符串) |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `String toSVG(BitMatrix matrix,QrConfig qrConfig)` | BitMatrix转SVG(字符串) |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `byte[] generatePng(String content,QrConfig config)` | 生成PNG格式的二维码图片，以byte[]形式表示 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `byte[] generatePng(String content,int width,int height)` | 生成PNG格式的二维码图片，以byte[]形式表示 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `void generate(String content,QrConfig config,String targetType,OutputStream out)` | 生成二维码到输出流 |
| `cn.hutool.extra.qrcode.QrCodeUtil` | `void generate(String content,int width,int height,String targetType,OutputStream out)` | 生成二维码到输出流 |
| `cn.hutool.extra.qrcode.QrConfig` | `Charset getCharset()` | 获取编码 |
| `cn.hutool.extra.qrcode.QrConfig` | `ErrorCorrectionLevel getErrorCorrection()` | 获取纠错级别 |
| `cn.hutool.extra.qrcode.QrConfig` | `HashMap<EncodeHintType, Object> toHints()` | 转换为Zxing的二维码配置 |
| `cn.hutool.extra.qrcode.QrConfig` | `HashMap<EncodeHintType, Object> toHints(BarcodeFormat format)` | 转换为Zxing的二维码配置 |
| `cn.hutool.extra.qrcode.QrConfig` | `Image getImg()` | 获取二维码中的Logo |
| `cn.hutool.extra.qrcode.QrConfig` | `Integer getMargin()` | 获取边距 |
| `cn.hutool.extra.qrcode.QrConfig` | `Integer getQrVersion()` | 设置二维码中的信息量，可设置0-40的整数，二维码图片也会根据qrVersion而变化，0表示根据传入信息自动变化 |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig create()` | 创建QrConfig |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setBackColor(Color backColor)` | 设置背景色，例如：Color.BLUE |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setBackColor(int backColor)` | 设置背景色，例如：Color.BLUE.getRGB() |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setCharset(Charset charset)` | 设置编码 |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setErrorCorrection(ErrorCorrectionLevel errorCorrection)` | 设置纠错级别 |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setForeColor(Color foreColor)` | 设置前景色，例如：Color.BLUE.getRGB() |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setForeColor(int foreColor)` | 设置前景色，例如：Color.BLUE.getRGB() |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setHeight(int height)` | 设置高度 |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setImg(File imgFile)` | 设置二维码中的Logo文件 |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setImg(Image img)` | 设置二维码中的Logo |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setImg(String imgPath)` | 设置二维码中的Logo文件 |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setMargin(Integer margin)` | 设置边距 |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setQrVersion(Integer qrVersion)` | 设置二维码中的信息量，可设置0-40的整数，二维码图片也会根据qrVersion而变化，0表示根据传入信息自动变化 |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setRatio(int ratio)` | 设置二维码中的Logo缩放的比例系数，如5表示长宽最小值的1/5 |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setRound(double round)` | 设置二维码中的Logo圆角弧度 |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setShapeHint(SymbolShapeHint shapeHint)` | 设置DATA_MATRIX的符号形状 |
| `cn.hutool.extra.qrcode.QrConfig` | `QrConfig setWidth(int width)` | 设置宽度 |
| `cn.hutool.extra.qrcode.QrConfig` | `double getRound()` | 获取二维码中的Logo圆角弧度 |
| `cn.hutool.extra.qrcode.QrConfig` | `int getBackColor()` | 获取背景色 |
| `cn.hutool.extra.qrcode.QrConfig` | `int getForeColor()` | 获取前景色 |
| `cn.hutool.extra.qrcode.QrConfig` | `int getHeight()` | 获取高度 |
| `cn.hutool.extra.qrcode.QrConfig` | `int getRatio()` | 获取二维码中的Logo缩放的比例系数，如5表示长宽最小值的1/5 |
| `cn.hutool.extra.qrcode.QrConfig` | `int getWidth()` | 获取宽度 |
