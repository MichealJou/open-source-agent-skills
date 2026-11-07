# cn.hutool.core.img.gif

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.img.gif.AnimatedGifEncoder` | `boolean addFrame(BufferedImage im)` | 【原文待译】Adds next GIF frame. The frame is not written immediately, but is actually deferred until the next frame is received so that timing data can be inserted. Invoking finish() flushes all frames. If setSize was not invoked, the size of the first image is used for all subsequent frames. |
| `cn.hutool.core.img.gif.AnimatedGifEncoder` | `boolean finish()` | 【原文待译】Flushes any pending data and closes output file. If writing to an OutputStream, the stream is not closed. |
| `cn.hutool.core.img.gif.AnimatedGifEncoder` | `boolean isStarted()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.img.gif.AnimatedGifEncoder` | `boolean start(OutputStream os)` | 【原文待译】Initiates GIF file creation on the given stream. The stream is not closed automatically. |
| `cn.hutool.core.img.gif.AnimatedGifEncoder` | `boolean start(String file)` | 【原文待译】Initiates writing of a GIF file with the specified name. |
| `cn.hutool.core.img.gif.AnimatedGifEncoder` | `void setBackground(Color c)` | 【原文待译】Sets the background color for the last added frame and any subsequent frames. Since all colors are subject to modification in the quantization process, the color in the final palette for each frame closest to the given color becomes the background color for that frame. May be set to null to indicate… |
| `cn.hutool.core.img.gif.AnimatedGifEncoder` | `void setDelay(int ms)` | 设置每一帧的间隔时间 Sets the delay time between each frame, or changes it for subsequent frames (applies to last frame added). |
| `cn.hutool.core.img.gif.AnimatedGifEncoder` | `void setDispose(int code)` | 【原文待译】Sets the GIF frame disposal code for the last added frame and any subsequent frames. Default is 0 if no transparent color has been set, otherwise 2. |
| `cn.hutool.core.img.gif.AnimatedGifEncoder` | `void setFrameRate(float fps)` | 【原文待译】Sets frame rate in frames per second. Equivalent to setDelay(1000/fps). |
| `cn.hutool.core.img.gif.AnimatedGifEncoder` | `void setQuality(int quality)` | 【原文待译】Sets quality of color quantization (conversion of images to the maximum 256 colors allowed by the GIF specification). Lower values (minimum = 1) produce better colors, but slow processing significantly. 10 is the default, and produces good color mapping at reasonable speeds. Values greater than 20 d… |
| `cn.hutool.core.img.gif.AnimatedGifEncoder` | `void setRepeat(int iter)` | 【原文待译】Sets the number of times the set of GIF frames should be played. Default is 1; 0 means play indefinitely. Must be invoked before the first image is added. |
| `cn.hutool.core.img.gif.AnimatedGifEncoder` | `void setSize(int w,int h)` | 【原文待译】Sets the GIF frame size. The default size is the size of the first frame added if this method is not invoked. |
| `cn.hutool.core.img.gif.AnimatedGifEncoder` | `void setTransparent(Color c)` | 【原文待译】Sets the transparent color for the last added frame and any subsequent frames. Since all colors are subject to modification in the quantization process, the color in the final palette for each frame closest to the given color becomes the transparent color for that frame. May be set to null to indica… |
| `cn.hutool.core.img.gif.AnimatedGifEncoder` | `void setTransparent(Color c,boolean exactMatch)` | 【原文待译】Sets the transparent color for the last added frame and any subsequent frames. Since all colors are subject to modification in the quantization process, the color in the final palette for each frame closest to the given color becomes the transparent color for that frame. If exactMatch is set to true… |
| `cn.hutool.core.img.gif.GifDecoder` | `BufferedImage getFrame(int n)` | 【原文待译】Gets the image contents of frame n. |
| `cn.hutool.core.img.gif.GifDecoder` | `BufferedImage getImage()` | 【原文待译】Gets the first (or only) image read. |
| `cn.hutool.core.img.gif.GifDecoder` | `Dimension getFrameSize()` | 【原文待译】Gets image size. |
| `cn.hutool.core.img.gif.GifDecoder` | `int getDelay(int n)` | 【原文待译】Gets display duration for specified frame. |
| `cn.hutool.core.img.gif.GifDecoder` | `int getFrameCount()` | 【原文待译】Gets the number of frames read from file. |
| `cn.hutool.core.img.gif.GifDecoder` | `int getLoopCount()` | 【原文待译】Gets the "Netscape" iteration count, if any. A count of 0 means repeat indefinitiely. |
| `cn.hutool.core.img.gif.GifDecoder` | `int read(BufferedInputStream is)` | 【原文待译】Reads GIF image from stream |
| `cn.hutool.core.img.gif.GifDecoder` | `int read(InputStream is)` | 【原文待译】Reads GIF image from stream |
| `cn.hutool.core.img.gif.GifDecoder` | `int read(String name)` | 【原文待译】Reads GIF file from specified file/URL source (URL assumed if name contains ":/" or "file:") |
| `cn.hutool.core.img.gif.NeuQuant` | `byte[] colorMap()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.img.gif.NeuQuant` | `byte[] process()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.img.gif.NeuQuant` | `int map(int b,int g,int r)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.img.gif.NeuQuant` | `void inxbuild()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.img.gif.NeuQuant` | `void learn()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.img.gif.NeuQuant` | `void unbiasnet()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
