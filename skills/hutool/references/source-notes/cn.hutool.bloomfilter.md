# cn.hutool.bloomfilter

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.bloomfilter.BitMapBloomFilter` | `boolean add(String str)` | 增加字符串到Filter映射中 |
| `cn.hutool.bloomfilter.BitMapBloomFilter` | `boolean contains(String str)` | 是否可能包含此字符串，此处存在误判 |
| `cn.hutool.bloomfilter.BitSetBloomFilter` | `boolean add(String str)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.bloomfilter.BitSetBloomFilter` | `boolean contains(String str)` | 判定是否包含指定字符串 |
| `cn.hutool.bloomfilter.BitSetBloomFilter` | `double getFalsePositiveProbability()` | @return 得到当前过滤器的错误率. |
| `cn.hutool.bloomfilter.BitSetBloomFilter` | `int hash(String str,int k)` | 计算Hash值 |
| `cn.hutool.bloomfilter.BitSetBloomFilter` | `int[] createHashes(String str,int hashNumber)` | 将字符串的字节表示进行多哈希编码. |
| `cn.hutool.bloomfilter.BitSetBloomFilter` | `void init(String path,Charset charset)` | 通过文件初始化过滤器. |
| `cn.hutool.bloomfilter.BitSetBloomFilter` | `void init(String path,String charsetName)` | 通过文件初始化过滤器. |
| `cn.hutool.bloomfilter.BloomFilter` | `boolean add(String str)` | 在boolean的bitMap中增加一个字符串 如果存在就返回false .如果不存在.先增加这个字符串.再返回true |
| `cn.hutool.bloomfilter.BloomFilter` | `boolean contains(String str)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.bloomfilter.BloomFilterUtil` | `BitMapBloomFilter createBitMap(int m)` | 创建BitMap实现的布隆过滤器 |
| `cn.hutool.bloomfilter.BloomFilterUtil` | `BitSetBloomFilter createBitSet(int c,int n,int k)` | 创建一个BitSet实现的布隆过滤器，过滤器的容量为c * k 个bit. |
