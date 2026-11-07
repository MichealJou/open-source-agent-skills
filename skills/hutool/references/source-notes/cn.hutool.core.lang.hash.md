# cn.hutool.core.lang.hash

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.lang.hash.CityHash` | `Number128 hash128(byte[] data)` | 计算128位City Hash值 |
| `cn.hutool.core.lang.hash.CityHash` | `Number128 hash128(byte[] data,Number128 seed)` | 计算128位City Hash值 |
| `cn.hutool.core.lang.hash.CityHash` | `int hash32(byte[] data)` | 计算32位City Hash值 |
| `cn.hutool.core.lang.hash.CityHash` | `long hash64(byte[] data)` | 计算64位City Hash值 |
| `cn.hutool.core.lang.hash.CityHash` | `long hash64(byte[] data,long seed)` | 计算64位City Hash值，种子1使用默认的#k2 |
| `cn.hutool.core.lang.hash.CityHash` | `long hash64(byte[] data,long seed0,long seed1)` | 计算64位City Hash值 |
| `cn.hutool.core.lang.hash.Hash` | `Number hash(T t)` | 计算Hash值 |
| `cn.hutool.core.lang.hash.Hash128` | `Number hash(T t)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.Hash128` | `Number128 hash128(T t)` | 计算Hash值 |
| `cn.hutool.core.lang.hash.Hash32` | `Number hash(T t)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.Hash32` | `int hash32(T t)` | 计算Hash值 |
| `cn.hutool.core.lang.hash.Hash64` | `Number hash(T t)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.Hash64` | `long hash64(T t)` | 计算Hash值 |
| `cn.hutool.core.lang.hash.KetamaHash` | `Number hash(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.KetamaHash` | `int hash32(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.KetamaHash` | `long hash64(String key)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.MetroHash` | `Number128 hash128(byte[] data)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.MetroHash` | `Number128 hash128(byte[] data,long seed)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.MetroHash` | `long hash64(byte[] data)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.MetroHash` | `long hash64(byte[] data,long seed)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.MurmurHash` | `int hash32(CharSequence data)` | Murmur3 32-bit Hash值计算 |
| `cn.hutool.core.lang.hash.MurmurHash` | `int hash32(byte[] data)` | Murmur3 32-bit Hash值计算 |
| `cn.hutool.core.lang.hash.MurmurHash` | `int hash32(byte[] data,int length,int seed)` | Murmur3 32-bit Hash值计算 |
| `cn.hutool.core.lang.hash.MurmurHash` | `int hash32(byte[] data,int offset,int length,int seed)` | Murmur3 32-bit Hash值计算 |
| `cn.hutool.core.lang.hash.MurmurHash` | `long hash64(CharSequence data)` | Murmur3 64-bit Hash值计算 |
| `cn.hutool.core.lang.hash.MurmurHash` | `long hash64(byte[] data)` | Murmur3 64-bit 算法 This is essentially MSB 8 bytes of Murmur3 128-bit variant. |
| `cn.hutool.core.lang.hash.MurmurHash` | `long hash64(byte[] data,int length,int seed)` | 类Murmur3 64-bit 算法 This is essentially MSB 8 bytes of Murmur3 128-bit variant. |
| `cn.hutool.core.lang.hash.MurmurHash` | `long[] hash128(CharSequence data)` | Murmur3 128-bit Hash值计算 |
| `cn.hutool.core.lang.hash.MurmurHash` | `long[] hash128(byte[] data)` | Murmur3 128-bit 算法. |
| `cn.hutool.core.lang.hash.MurmurHash` | `long[] hash128(byte[] data,int length,int seed)` | 【原文待译】Murmur3 128-bit variant. |
| `cn.hutool.core.lang.hash.MurmurHash` | `long[] hash128(byte[] data,int offset,int length,int seed)` | 【原文待译】Murmur3 128-bit variant. |
| `cn.hutool.core.lang.hash.Number128` | `boolean equals(final Object o)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.Number128` | `double doubleValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.Number128` | `float floatValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.Number128` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.Number128` | `int intValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.Number128` | `long getHighValue()` | 获取高位值 |
| `cn.hutool.core.lang.hash.Number128` | `long getLowValue()` | 获取低位值 |
| `cn.hutool.core.lang.hash.Number128` | `long longValue()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.lang.hash.Number128` | `long[] getLongArray()` | 获取高低位数组，long[0]：低位，long[1]：高位 |
| `cn.hutool.core.lang.hash.Number128` | `void setHighValue(long hiValue)` | 设置高位值 |
| `cn.hutool.core.lang.hash.Number128` | `void setLowValue(long lowValue)` | 设置低位值 |
