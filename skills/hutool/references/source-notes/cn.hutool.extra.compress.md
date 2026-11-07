# cn.hutool.extra.compress

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.extra.compress.CompressUtil` | `Archiver createArchiver(Charset charset,String archiverName,File file)` | 创建归档器，支持： ArchiveStreamFactory#AR ArchiveStreamFactory#CPIO ArchiveStreamFactory#JAR ArchiveStreamFactory#TAR ArchiveStreamFactory#ZIP ArchiveStreamFactory#SEVEN_Z |
| `cn.hutool.extra.compress.CompressUtil` | `Archiver createArchiver(Charset charset,String archiverName,OutputStream out)` | 创建归档器，支持： ArchiveStreamFactory#AR ArchiveStreamFactory#CPIO ArchiveStreamFactory#JAR ArchiveStreamFactory#TAR ArchiveStreamFactory#ZIP ArchiveStreamFactory#SEVEN_Z |
| `cn.hutool.extra.compress.CompressUtil` | `CompressorInputStream getIn(String compressorName,InputStream in)` | 获取压缩输入流，用于解压缩指定内容，支持的格式例如： {@value CompressorStreamFactory#GZIP} {@value CompressorStreamFactory#BZIP2} {@value CompressorStreamFactory#XZ} {@value CompressorStreamFactory#PACK200} {@value CompressorStreamFactory#SNAPPY_FRAMED} {@value CompressorStreamFactory#LZ4_BLOCK} {@value CompressorStreamFacto… |
| `cn.hutool.extra.compress.CompressUtil` | `CompressorOutputStream getOut(String compressorName,OutputStream out)` | 获取压缩输出流，用于压缩指定内容，支持的格式例如： {@value CompressorStreamFactory#GZIP} {@value CompressorStreamFactory#BZIP2} {@value CompressorStreamFactory#XZ} {@value CompressorStreamFactory#PACK200} {@value CompressorStreamFactory#SNAPPY_FRAMED} {@value CompressorStreamFactory#LZ4_BLOCK} {@value CompressorStreamFactor… |
| `cn.hutool.extra.compress.CompressUtil` | `Extractor createExtractor(Charset charset,File file)` | 创建归档解包器，支持： ArchiveStreamFactory#AR ArchiveStreamFactory#CPIO ArchiveStreamFactory#JAR ArchiveStreamFactory#TAR ArchiveStreamFactory#ZIP ArchiveStreamFactory#SEVEN_Z |
| `cn.hutool.extra.compress.CompressUtil` | `Extractor createExtractor(Charset charset,InputStream in)` | 创建归档解包器，支持： ArchiveStreamFactory#AR ArchiveStreamFactory#CPIO ArchiveStreamFactory#JAR ArchiveStreamFactory#TAR ArchiveStreamFactory#ZIP ArchiveStreamFactory#SEVEN_Z |
| `cn.hutool.extra.compress.CompressUtil` | `Extractor createExtractor(Charset charset,String archiverName,File file)` | 创建归档解包器，支持： ArchiveStreamFactory#AR ArchiveStreamFactory#CPIO ArchiveStreamFactory#JAR ArchiveStreamFactory#TAR ArchiveStreamFactory#ZIP ArchiveStreamFactory#SEVEN_Z |
| `cn.hutool.extra.compress.CompressUtil` | `Extractor createExtractor(Charset charset,String archiverName,InputStream in)` | 创建归档解包器，支持： ArchiveStreamFactory#AR ArchiveStreamFactory#CPIO ArchiveStreamFactory#JAR ArchiveStreamFactory#TAR ArchiveStreamFactory#ZIP ArchiveStreamFactory#SEVEN_Z |
