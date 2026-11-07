# cn.hutool.captcha

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.captcha.AbstractCaptcha` | `BufferedImage getImage()` | 获取验证码图 |
| `cn.hutool.captcha.AbstractCaptcha` | `CodeGenerator getGenerator()` | 获取验证码生成器 |
| `cn.hutool.captcha.AbstractCaptcha` | `String getCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.captcha.AbstractCaptcha` | `String getImageBase64()` | 获得图片的Base64形式 |
| `cn.hutool.captcha.AbstractCaptcha` | `String getImageBase64Data()` | 获取图片带文件格式的 Base64 |
| `cn.hutool.captcha.AbstractCaptcha` | `boolean verify(String userInputCode)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.captcha.AbstractCaptcha` | `byte[] getImageBytes()` | 获取图形验证码图片bytes |
| `cn.hutool.captcha.AbstractCaptcha` | `void createCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.captcha.AbstractCaptcha` | `void setBackground(Color background)` | 设置背景色 |
| `cn.hutool.captcha.AbstractCaptcha` | `void setFont(Font font)` | 自定义字体 |
| `cn.hutool.captcha.AbstractCaptcha` | `void setGenerator(CodeGenerator generator)` | 设置验证码生成器 |
| `cn.hutool.captcha.AbstractCaptcha` | `void setStroke(Stroke stroke)` | 设置画笔线条特征，如线条宽度等 |
| `cn.hutool.captcha.AbstractCaptcha` | `void setTextAlpha(float textAlpha)` | 设置文字透明度 |
| `cn.hutool.captcha.AbstractCaptcha` | `void write(File file)` | 验证码写出到文件 |
| `cn.hutool.captcha.AbstractCaptcha` | `void write(OutputStream out)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.captcha.AbstractCaptcha` | `void write(String path)` | 验证码写出到文件 |
| `cn.hutool.captcha.CaptchaUtil` | `CircleCaptcha createCircleCaptcha(int width,int height)` | 创建圆圈干扰的验证码，默认5位验证码，15个干扰圈 |
| `cn.hutool.captcha.CaptchaUtil` | `CircleCaptcha createCircleCaptcha(int width,int height,CodeGenerator generator,int circleCount)` | 创建圆圈干扰的验证码 |
| `cn.hutool.captcha.CaptchaUtil` | `CircleCaptcha createCircleCaptcha(int width,int height,int codeCount,int circleCount)` | 创建圆圈干扰的验证码 |
| `cn.hutool.captcha.CaptchaUtil` | `CircleCaptcha createCircleCaptcha(int width,int height,int codeCount,int circleCount,float size)` | 创建圆圈干扰的验证码 |
| `cn.hutool.captcha.CaptchaUtil` | `GifCaptcha createGifCaptcha(int width,int height)` | 创建GIF验证码 |
| `cn.hutool.captcha.CaptchaUtil` | `GifCaptcha createGifCaptcha(int width,int height,CodeGenerator generator,int thickness)` | 创建GIF验证码 |
| `cn.hutool.captcha.CaptchaUtil` | `GifCaptcha createGifCaptcha(int width,int height,int codeCount)` | 创建GIF验证码 |
| `cn.hutool.captcha.CaptchaUtil` | `GifCaptcha createGifCaptcha(int width,int height,int codeCount,int thickness,float size)` | 创建圆圈干扰的验证码 |
| `cn.hutool.captcha.CaptchaUtil` | `LineCaptcha createLineCaptcha(int width,int height)` | 创建线干扰的验证码，默认5位验证码，150条干扰线 |
| `cn.hutool.captcha.CaptchaUtil` | `LineCaptcha createLineCaptcha(int width,int height,CodeGenerator generator,int lineCount)` | 创建线干扰的验证码 |
| `cn.hutool.captcha.CaptchaUtil` | `LineCaptcha createLineCaptcha(int width,int height,int codeCount,int lineCount)` | 创建线干扰的验证码 |
| `cn.hutool.captcha.CaptchaUtil` | `LineCaptcha createLineCaptcha(int width,int height,int codeCount,int lineCount,float size)` | 创建线干扰的验证码 |
| `cn.hutool.captcha.CaptchaUtil` | `ShearCaptcha createShearCaptcha(int width,int height)` | 创建扭曲干扰的验证码，默认5位验证码 |
| `cn.hutool.captcha.CaptchaUtil` | `ShearCaptcha createShearCaptcha(int width,int height,CodeGenerator generator,int thickness)` | 创建扭曲干扰的验证码，默认5位验证码 |
| `cn.hutool.captcha.CaptchaUtil` | `ShearCaptcha createShearCaptcha(int width,int height,int codeCount,int thickness)` | 创建扭曲干扰的验证码，默认5位验证码 |
| `cn.hutool.captcha.CaptchaUtil` | `ShearCaptcha createShearCaptcha(int width,int height,int codeCount,int thickness,float size)` | 创建扭曲干扰的验证码，默认5位验证码 |
| `cn.hutool.captcha.CircleCaptcha` | `Image createImage(String code)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.captcha.GifCaptcha` | `GifCaptcha setMaxColor(int maxColor)` | 设置验证码字符颜色 |
| `cn.hutool.captcha.GifCaptcha` | `GifCaptcha setMinColor(int minColor)` | 设置验证码字符颜色 |
| `cn.hutool.captcha.GifCaptcha` | `GifCaptcha setQuality(int quality)` | 设置图像的颜色量化(转换质量 由GIF规范允许的最大256种颜色)。 低的值(最小值= 1)产生更好的颜色,但处理显著缓慢。 10是默认,并产生良好的颜色而且有以合理的速度。 值更大(大于20)不产生显著的改善速度 |
| `cn.hutool.captcha.GifCaptcha` | `GifCaptcha setRepeat(int repeat)` | 设置GIF帧应该播放的次数。 默认是 0; 0意味着无限循环。 必须在添加的第一个图像之前被调用。 |
| `cn.hutool.captcha.GifCaptcha` | `void createCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.captcha.ICaptcha` | `String getCode()` | 获取验证码的文字内容 |
| `cn.hutool.captcha.ICaptcha` | `boolean verify(String userInputCode)` | 验证验证码是否正确，建议忽略大小写 |
| `cn.hutool.captcha.ICaptcha` | `void createCode()` | 创建验证码，实现类需同时生成随机验证码字符串和验证码图片 |
| `cn.hutool.captcha.ICaptcha` | `void write(OutputStream out)` | 将验证码写出到目标流中 |
| `cn.hutool.captcha.LineCaptcha` | `Image createImage(String code)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.captcha.ShearCaptcha` | `Image createImage(String code)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
