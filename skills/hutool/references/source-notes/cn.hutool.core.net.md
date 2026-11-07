# cn.hutool.core.net

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.net.DefaultTrustManager` | `X509Certificate[] getAcceptedIssuers()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.DefaultTrustManager` | `void checkClientTrusted(X509Certificate[] chain,String authType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.DefaultTrustManager` | `void checkClientTrusted(X509Certificate[] x509Certificates,String s,SSLEngine sslEngine)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.DefaultTrustManager` | `void checkClientTrusted(X509Certificate[] x509Certificates,String s,Socket socket)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.DefaultTrustManager` | `void checkServerTrusted(X509Certificate[] chain,String authType)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.DefaultTrustManager` | `void checkServerTrusted(X509Certificate[] x509Certificates,String s,SSLEngine sslEngine)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.DefaultTrustManager` | `void checkServerTrusted(X509Certificate[] x509Certificates,String s,Socket socket)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.Ipv4Util` | `List<String> list(String ip,int maskBit,boolean isAll)` | 根据IP地址、子网掩码获取IP地址区间 |
| `cn.hutool.core.net.Ipv4Util` | `List<String> list(String ipFrom,String ipTo)` | 得到IP地址区间 |
| `cn.hutool.core.net.Ipv4Util` | `List<String> list(String ipRange,boolean isAll)` | 智能转换IP地址集合 |
| `cn.hutool.core.net.Ipv4Util` | `Long getBeginIpLong(String ip,int maskBit)` | 根据 ip/掩码位 计算IP段的起始IP（Long型） |
| `cn.hutool.core.net.Ipv4Util` | `Long getEndIpLong(String ip,int maskBit)` | 根据 ip/掩码位 计算IP段的终止IP（Long型） 注：此接口返回负数，请使用转成字符串后再转Long型 |
| `cn.hutool.core.net.Ipv4Util` | `String formatIpBlock(String ip,String mask)` | 格式化IP段 |
| `cn.hutool.core.net.Ipv4Util` | `String getBeginIpStr(String ip,int maskBit)` | 根据 ip/掩码位 计算IP段的起始IP（字符串型） 方法别名：inet_ntoa |
| `cn.hutool.core.net.Ipv4Util` | `String getEndIpStr(String ip,int maskBit)` | 根据 ip/掩码位 计算IP段的终止IP（字符串型） |
| `cn.hutool.core.net.Ipv4Util` | `String getMaskByIpRange(String fromIp,String toIp)` | 根据开始IP与结束IP计算掩码 |
| `cn.hutool.core.net.Ipv4Util` | `String getMaskByMaskBit(int maskBit)` | 根据掩码位获取掩码 |
| `cn.hutool.core.net.Ipv4Util` | `String longToIpv4(long longIP)` | 根据long值获取ip v4地址：xx.xx.xx.xx |
| `cn.hutool.core.net.Ipv4Util` | `boolean isInnerIP(String ipAddress)` | 判定是否为内网IPv4 私有IP： |
| `cn.hutool.core.net.Ipv4Util` | `boolean isMaskBitValid(int maskBit)` | 判断掩码位是否合法 |
| `cn.hutool.core.net.Ipv4Util` | `boolean isMaskValid(String mask)` | 判断掩码是否合法 |
| `cn.hutool.core.net.Ipv4Util` | `boolean matches(String wildcard,String ipAddress)` | 检测指定 IP 地址是否匹配通配符 wildcard |
| `cn.hutool.core.net.Ipv4Util` | `int countByIpRange(String fromIp,String toIp)` | 计算IP区间有多少个IP |
| `cn.hutool.core.net.Ipv4Util` | `int countByMaskBit(int maskBit,boolean isAll)` | 计算子网大小 |
| `cn.hutool.core.net.Ipv4Util` | `int getMaskBitByMask(String mask)` | 根据子网掩码转换为掩码位 |
| `cn.hutool.core.net.Ipv4Util` | `long ipv4ToLong(String strIP)` | 根据ip地址(xxx.xxx.xxx.xxx)计算出long型的数据 方法别名：inet_aton |
| `cn.hutool.core.net.Ipv4Util` | `long ipv4ToLong(String strIP,long defaultValue)` | 根据ip地址(xxx.xxx.xxx.xxx)计算出long型的数据, 如果格式不正确返回 defaultValue |
| `cn.hutool.core.net.LocalPortGenerater` | `int generate()` | 生成一个本地端口，用于远程端口映射 |
| `cn.hutool.core.net.MaskBit` | `Integer getMaskBit(String mask)` | 根据掩码获取掩码位 |
| `cn.hutool.core.net.MaskBit` | `String get(int maskBit)` | 根据掩码位获取掩码 |
| `cn.hutool.core.net.NetUtil` | `BigInteger ipv6ToBigInteger(String ipv6Str)` | 将IPv6地址字符串转为大整数 |
| `cn.hutool.core.net.NetUtil` | `BigInteger ipv6ToBitInteger(String ipv6Str)` | 将IPv6地址字符串转为大整数 |
| `cn.hutool.core.net.NetUtil` | `Collection<NetworkInterface> getNetworkInterfaces()` | 获取本机所有网卡 |
| `cn.hutool.core.net.NetUtil` | `InetAddress getLocalhost()` | 获取本机网卡IP地址，规则如下： |
| `cn.hutool.core.net.NetUtil` | `InetSocketAddress buildInetSocketAddress(String host,int defaultPort)` | 构建InetSocketAddress 当host中包含端口时（用“：”隔开），使用host中的端口，否则使用默认端口 给定host为空时使用本地host（127.0.0.1） |
| `cn.hutool.core.net.NetUtil` | `InetSocketAddress createAddress(String host,int port)` | 创建 InetSocketAddress |
| `cn.hutool.core.net.NetUtil` | `LinkedHashSet<InetAddress> localAddressList(Filter<InetAddress> addressFilter)` | 获取所有满足过滤条件的本地IP地址对象 |
| `cn.hutool.core.net.NetUtil` | `LinkedHashSet<InetAddress> localAddressList(Filter<NetworkInterface> networkInterfaceFilter,Filter<InetAddress> addressFilter)` | 获取所有满足过滤条件的本地IP地址对象 |
| `cn.hutool.core.net.NetUtil` | `LinkedHashSet<String> localIps()` | 获得本机的IP地址列表（包括Ipv4和Ipv6） 返回的IP列表有序，按照系统设备顺序 |
| `cn.hutool.core.net.NetUtil` | `LinkedHashSet<String> localIpv4s()` | 获得本机的IPv4地址列表 返回的IP列表有序，按照系统设备顺序 |
| `cn.hutool.core.net.NetUtil` | `LinkedHashSet<String> localIpv6s()` | 获得本机的IPv6地址列表 返回的IP列表有序，按照系统设备顺序 |
| `cn.hutool.core.net.NetUtil` | `LinkedHashSet<String> toIpList(Set<InetAddress> addressList)` | 地址列表转换为IP地址列表 |
| `cn.hutool.core.net.NetUtil` | `List<HttpCookie> parseCookies(String cookieStr)` | 解析Cookie信息 |
| `cn.hutool.core.net.NetUtil` | `List<String> getDnsInfo(String hostName,String... attrNames)` | 获取DNS信息，如TXT信息： |
| `cn.hutool.core.net.NetUtil` | `NetworkInterface getNetworkInterface(String name)` | 获取指定名称的网卡信息 |
| `cn.hutool.core.net.NetUtil` | `String bigIntegerToIPv6(BigInteger bigInteger)` | 将大整数转换成ipv6字符串 |
| `cn.hutool.core.net.NetUtil` | `String getIpByHost(String hostName)` | 通过域名得到IP |
| `cn.hutool.core.net.NetUtil` | `String getLocalHostName()` | 获取主机名称，一次获取会缓存名称 注意此方法会触发反向DNS解析，导致阻塞，阻塞时间取决于网络！ |
| `cn.hutool.core.net.NetUtil` | `String getLocalMacAddress()` | 获得本机MAC地址 |
| `cn.hutool.core.net.NetUtil` | `String getLocalhostStr()` | 获取本机网卡IP地址，这个地址为所有网卡中非回路地址的第一个 如果获取失败调用 InetAddress#getLocalHost()方法获取。 此方法不会抛出异常，获取失败将返回null 参考：http://stackoverflow.com/questions/9481865/getting-the-ip-address-of-the-current-machine-using-java |
| `cn.hutool.core.net.NetUtil` | `String getMacAddress(InetAddress inetAddress)` | 获得指定地址信息中的MAC地址，使用分隔符“-” |
| `cn.hutool.core.net.NetUtil` | `String getMacAddress(InetAddress inetAddress,String separator)` | 获得指定地址信息中的MAC地址 |
| `cn.hutool.core.net.NetUtil` | `String getMultistageReverseProxyIp(String ip)` | 从多级反向代理中获得第一个非unknown IP地址 |
| `cn.hutool.core.net.NetUtil` | `String hideIpPart(String ip)` | 隐藏掉IP地址的最后一部分为 * 代替 |
| `cn.hutool.core.net.NetUtil` | `String hideIpPart(long ip)` | 隐藏掉IP地址的最后一部分为 * 代替 |
| `cn.hutool.core.net.NetUtil` | `String idnToASCII(String unicode)` | Unicode域名转puny code |
| `cn.hutool.core.net.NetUtil` | `String longToIpv4(long longIP)` | 根据long值获取ip v4地址 |
| `cn.hutool.core.net.NetUtil` | `String toAbsoluteUrl(String absoluteBasePath,String relativePath)` | 相对URL转换为绝对URL |
| `cn.hutool.core.net.NetUtil` | `TreeSet<Integer> getUsableLocalPorts(int numRequested,int minPort,int maxPort)` | 获取多个本地可用端口 来自org.springframework.util.SocketUtils |
| `cn.hutool.core.net.NetUtil` | `boolean isInRange(String ip,String cidr)` | 是否在CIDR规则配置范围内 方法来自：【成都】小邓 |
| `cn.hutool.core.net.NetUtil` | `boolean isInnerIP(String ipAddress)` | 判定是否为内网IPv4 私有IP： |
| `cn.hutool.core.net.NetUtil` | `boolean isOpen(InetSocketAddress address,int timeout)` | 检查远程端口是否开启 |
| `cn.hutool.core.net.NetUtil` | `boolean isUnknown(String checkString)` | 检测给定字符串是否为未知，多用于检测HTTP请求相关 |
| `cn.hutool.core.net.NetUtil` | `boolean isUsableLocalPort(int port)` | 检测本地端口可用性 来自org.springframework.util.SocketUtils |
| `cn.hutool.core.net.NetUtil` | `boolean isValidPort(int port)` | 是否为有效的端口 此方法并不检查端口是否被占用 |
| `cn.hutool.core.net.NetUtil` | `boolean ping(String ip)` | 检测IP地址是否能ping通 |
| `cn.hutool.core.net.NetUtil` | `boolean ping(String ip,int timeout)` | 检测IP地址是否能ping通 |
| `cn.hutool.core.net.NetUtil` | `byte[] getHardwareAddress(InetAddress inetAddress)` | 获得指定地址信息中的硬件地址 |
| `cn.hutool.core.net.NetUtil` | `byte[] getLocalHardwareAddress()` | 获得本机物理地址 |
| `cn.hutool.core.net.NetUtil` | `int getUsableLocalPort()` | 查找1024~65535范围内的可用端口 此方法只检测给定范围内的随机一个端口，检测65535-1024次 来自org.springframework.util.SocketUtils |
| `cn.hutool.core.net.NetUtil` | `int getUsableLocalPort(int minPort)` | 查找指定范围内的可用端口，最大值为65535 此方法只检测给定范围内的随机一个端口，检测65535-minPort次 来自org.springframework.util.SocketUtils |
| `cn.hutool.core.net.NetUtil` | `int getUsableLocalPort(int minPort,int maxPort)` | 查找指定范围内的可用端口 此方法只检测给定范围内的随机一个端口，检测maxPort-minPort次 来自org.springframework.util.SocketUtils |
| `cn.hutool.core.net.NetUtil` | `long ipv4ToLong(String strIP)` | 根据ip地址计算出long型的数据 |
| `cn.hutool.core.net.NetUtil` | `void netCat(String host,int port,boolean isBlock,ByteBuffer data)` | 简易的使用Socket发送数据 |
| `cn.hutool.core.net.NetUtil` | `void netCat(String host,int port,byte[] data)` | 使用普通Socket发送数据 |
| `cn.hutool.core.net.NetUtil` | `void setGlobalAuthenticator(Authenticator authenticator)` | 设置全局验证 |
| `cn.hutool.core.net.NetUtil` | `void setGlobalAuthenticator(String user,char[] pass)` | 设置全局验证 |
| `cn.hutool.core.net.PassAuth` | `PassAuth of(String user,char[] pass)` | 创建账号密码形式的Authenticator 实现。 |
| `cn.hutool.core.net.ProxySocketFactory` | `ProxySocketFactory of(final Proxy proxy)` | 创建代理SocketFactory |
| `cn.hutool.core.net.ProxySocketFactory` | `Socket createSocket()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.ProxySocketFactory` | `Socket createSocket(final InetAddress address,final int port)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.ProxySocketFactory` | `Socket createSocket(final InetAddress address,final int port,final InetAddress localAddr,final int localPort)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.ProxySocketFactory` | `Socket createSocket(final String host,final int port)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.ProxySocketFactory` | `Socket createSocket(final String host,final int port,final InetAddress localAddr,final int localPort)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.SSLContextBuilder` | `SSLContext build()` | 构建SSLContext |
| `cn.hutool.core.net.SSLContextBuilder` | `SSLContext buildChecked()` | 构建SSLContext需要处理异常 |
| `cn.hutool.core.net.SSLContextBuilder` | `SSLContext buildQuietly()` | 构建SSLContext |
| `cn.hutool.core.net.SSLContextBuilder` | `SSLContextBuilder create()` | 创建 SSLContextBuilder |
| `cn.hutool.core.net.SSLContextBuilder` | `SSLContextBuilder setKeyManagers(KeyManager... keyManagers)` | 设置 JSSE key managers |
| `cn.hutool.core.net.SSLContextBuilder` | `SSLContextBuilder setProtocol(String protocol)` | 设置协议。例如TLS等 |
| `cn.hutool.core.net.SSLContextBuilder` | `SSLContextBuilder setSecureRandom(SecureRandom secureRandom)` | 设置 SecureRandom |
| `cn.hutool.core.net.SSLContextBuilder` | `SSLContextBuilder setTrustManagers(TrustManager... trustManagers)` | 设置信任信息 |
| `cn.hutool.core.net.SSLUtil` | `SSLContext createSSLContext(String protocol)` | 创建SSLContext，默认信任全部 |
| `cn.hutool.core.net.SSLUtil` | `SSLContext createSSLContext(String protocol,KeyManager keyManager,TrustManager trustManager)` | 创建SSLContext |
| `cn.hutool.core.net.SSLUtil` | `SSLContext createSSLContext(String protocol,KeyManager[] keyManagers,TrustManager[] trustManagers)` | 创建和初始化SSLContext |
| `cn.hutool.core.net.URLDecoder` | `String decode(String str,Charset charset)` | 解码 规则见：https://url.spec.whatwg.org/#urlencoded-parsing |
| `cn.hutool.core.net.URLDecoder` | `String decode(String str,Charset charset,boolean isPlusToSpace)` | 解码 |
| `cn.hutool.core.net.URLDecoder` | `String decodeForPath(String str,Charset charset)` | 解码，不对+解码 将%20转换为空格 将 "%xy"转换为文本形式,xy是两位16进制的数值 跳过不符合规范的%形式，直接输出 |
| `cn.hutool.core.net.URLDecoder` | `byte[] decode(byte[] bytes)` | 解码 |
| `cn.hutool.core.net.URLDecoder` | `byte[] decode(byte[] bytes,boolean isPlusToSpace)` | 解码 |
| `cn.hutool.core.net.URLEncodeUtil` | `String encode(String url)` | 编码URL，默认使用UTF-8编码 将需要转换的内容（ASCII码形式之外的内容），用十六进制表示法转换出来，并在之前加上%开头。 此方法用于URL自动编码，类似于浏览器中键入地址自动编码，对于像类似于“/”的字符不再编码 |
| `cn.hutool.core.net.URLEncodeUtil` | `String encode(String url,Charset charset)` | 编码字符为 application/x-www-form-urlencoded 将需要转换的内容（ASCII码形式之外的内容），用十六进制表示法转换出来，并在之前加上%开头。 此方法用于URL自动编码，类似于浏览器中键入地址自动编码，对于像类似于“/”的字符不再编码 |
| `cn.hutool.core.net.URLEncodeUtil` | `String encodeAll(String url)` | 编码URL，默认使用UTF-8编码 将需要转换的内容（ASCII码形式之外的内容），用十六进制表示法转换出来，并在之前加上%开头。 |
| `cn.hutool.core.net.URLEncodeUtil` | `String encodeAll(String url,Charset charset)` | 编码URL 将需要转换的内容（ASCII码形式之外的内容），用十六进制表示法转换出来，并在之前加上%开头。 |
| `cn.hutool.core.net.URLEncodeUtil` | `String encodeFragment(String url)` | 编码URL，默认使用UTF-8编码 URL的Fragment URLEncoder 默认的编码器针对Fragment，定义如下： |
| `cn.hutool.core.net.URLEncodeUtil` | `String encodeFragment(String url,Charset charset)` | URL的Fragment URLEncoder 默认的编码器针对Fragment，定义如下： |
| `cn.hutool.core.net.URLEncodeUtil` | `String encodePathSegment(String url)` | 编码URL，默认使用UTF-8编码 将需要转换的内容（ASCII码形式之外的内容），用十六进制表示法转换出来，并在之前加上%开头。 此方法用于URL的Segment中自动编码，转义大部分特殊字符 |
| `cn.hutool.core.net.URLEncodeUtil` | `String encodePathSegment(String url,Charset charset)` | 编码字符为URL中查询语句 将需要转换的内容（ASCII码形式之外的内容），用十六进制表示法转换出来，并在之前加上%开头。 此方法用于URL的Segment中自动编码，转义大部分特殊字符 |
| `cn.hutool.core.net.URLEncodeUtil` | `String encodeQuery(String url)` | 编码URL，默认使用UTF-8编码 将需要转换的内容（ASCII码形式之外的内容），用十六进制表示法转换出来，并在之前加上%开头。 此方法用于POST请求中的请求体自动编码，转义大部分特殊字符 |
| `cn.hutool.core.net.URLEncodeUtil` | `String encodeQuery(String url,Charset charset)` | 编码字符为URL中查询语句 将需要转换的内容（ASCII码形式之外的内容），用十六进制表示法转换出来，并在之前加上%开头。 此方法用于POST请求中的请求体自动编码，转义大部分特殊字符 |
| `cn.hutool.core.net.URLEncoder` | `String encode(String path,Charset charset)` | 将URL中的字符串编码为%形式 |
| `cn.hutool.core.net.URLEncoder` | `URLEncoder createAll()` | 创建URLEncoder 编码器针对URI路径编码，定义如下： |
| `cn.hutool.core.net.URLEncoder` | `URLEncoder createDefault()` | 创建默认URLEncoder 默认的编码器针对URI路径编码，定义如下： |
| `cn.hutool.core.net.URLEncoder` | `URLEncoder createFragment()` | URL的Fragment URLEncoder 默认的编码器针对Fragment，定义如下： |
| `cn.hutool.core.net.URLEncoder` | `URLEncoder createPathSegment()` | URL的Path的每一个Segment URLEncoder 默认的编码器针对URI路径的每一段编码，定义如下： |
| `cn.hutool.core.net.URLEncoder` | `URLEncoder createQuery()` | 创建用于查询语句的URLEncoder 编码器针对URI路径编码，定义如下： |
| `cn.hutool.core.net.URLEncoder` | `void addSafeCharacter(char c)` | 增加安全字符 安全字符不被编码 |
| `cn.hutool.core.net.URLEncoder` | `void removeSafeCharacter(char c)` | 移除安全字符 安全字符不被编码 |
| `cn.hutool.core.net.URLEncoder` | `void setEncodeSpaceAsPlus(boolean encodeSpaceAsPlus)` | 是否将空格编码为+ |
