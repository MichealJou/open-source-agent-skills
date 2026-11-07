# cn.hutool.core.net.url

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.core.net.url.UrlBuilder` | `Charset getCharset()` | 获取编码，用于URLEncode和URLDecode |
| `cn.hutool.core.net.url.UrlBuilder` | `String build()` | 创建URL字符串 |
| `cn.hutool.core.net.url.UrlBuilder` | `String getAuthority()` | 获得authority部分 |
| `cn.hutool.core.net.url.UrlBuilder` | `String getFragment()` | 获取标识符，#后边的部分 |
| `cn.hutool.core.net.url.UrlBuilder` | `String getFragmentEncoded()` | 获取标识符，#后边的部分 |
| `cn.hutool.core.net.url.UrlBuilder` | `String getHost()` | 获取 主机，例如127.0.0.1 |
| `cn.hutool.core.net.url.UrlBuilder` | `String getPathStr()` | 获得路径，例如/aa/bb/cc |
| `cn.hutool.core.net.url.UrlBuilder` | `String getQueryStr()` | 获取查询语句，例如a=1&b=2 |
| `cn.hutool.core.net.url.UrlBuilder` | `String getScheme()` | 获取协议，例如http |
| `cn.hutool.core.net.url.UrlBuilder` | `String getSchemeWithDefault()` | 获取协议，例如http，如果用户未定义协议，使用默认的http协议 |
| `cn.hutool.core.net.url.UrlBuilder` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.url.UrlBuilder` | `URI toURI()` | 转换为URI |
| `cn.hutool.core.net.url.UrlBuilder` | `URL toURL()` | 转换为URL 对象 |
| `cn.hutool.core.net.url.UrlBuilder` | `URL toURL(URLStreamHandler handler)` | 转换为URL 对象 |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder addPath(CharSequence path)` | 增加路径，在现有路径基础上追加路径 |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder addPathSegment(CharSequence segment)` | 增加路径节点，路径节点中的"/"会被转义为"%2F" |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder addQuery(String key,Object value)` | 添加查询项，支持重复键 |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder appendPath(CharSequence path)` | 追加path节点 |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder create()` | 创建空的UrlBuilder |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder of()` | 创建空的UrlBuilder |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder of(String scheme,String host,int port,String path,String query,String fragment,Charset charset)` | 构建UrlBuilder |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder of(String scheme,String host,int port,UrlPath path,UrlQuery query,String fragment,Charset charset)` | 构建UrlBuilder |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder of(String url)` | 使用URL字符串构建UrlBuilder，默认使用UTF-8编码 |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder of(String url,Charset charset)` | 使用URL字符串构建UrlBuilder |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder of(URI uri,Charset charset)` | 使用URI构建UrlBuilder |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder of(URL url,Charset charset)` | 使用URL构建UrlBuilder |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder ofHttp(String httpUrl)` | 使用URL字符串构建UrlBuilder，当传入的URL没有协议时，按照http协议对待，编码默认使用UTF-8 |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder ofHttp(String httpUrl,Charset charset)` | 使用URL字符串构建UrlBuilder，当传入的URL没有协议时，按照http协议对待。 |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder ofHttpWithoutEncode(String httpUrl)` | 使用URL字符串构建UrlBuilder，当传入的URL没有协议时，按照http协议对待 此方法不对URL编码 |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder setCharset(Charset charset)` | 设置编码，用于URLEncode和URLDecode |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder setFragment(String fragment)` | 设置标识符，例如#后边的部分 |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder setHost(String host)` | 设置主机，例如127.0.0.1 |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder setPath(UrlPath path)` | 设置路径，例如/aa/bb/cc，将覆盖之前所有的path相关设置 |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder setPort(int port)` | 设置端口，默认-1 |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder setQuery(UrlQuery query)` | 设置查询语句，例如a=1&b=2，将覆盖之前所有的query相关设置 |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder setScheme(String scheme)` | 设置协议，例如http |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlBuilder setWithEndTag(boolean withEngTag)` | 是否path的末尾加 / |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlPath getPath()` | 获取路径，例如/aa/bb/cc |
| `cn.hutool.core.net.url.UrlBuilder` | `UrlQuery getQuery()` | 获取查询语句，例如a=1&b=2 可能为null |
| `cn.hutool.core.net.url.UrlBuilder` | `int getPort()` | 获取端口，默认-1 |
| `cn.hutool.core.net.url.UrlBuilder` | `int getPortWithDefault()` | 获取端口，如果未自定义返回协议默认端口 |
| `cn.hutool.core.net.url.UrlPath` | `List<String> getSegments()` | 获取path的节点列表 |
| `cn.hutool.core.net.url.UrlPath` | `String build(Charset charset)` | 构建path，前面带'/' |
| `cn.hutool.core.net.url.UrlPath` | `String build(Charset charset,boolean encodePercent)` | 构建path，前面带'/' |
| `cn.hutool.core.net.url.UrlPath` | `String getSegment(int index)` | 获得指定节点 |
| `cn.hutool.core.net.url.UrlPath` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.core.net.url.UrlPath` | `UrlPath add(CharSequence segment)` | 添加到path最后面 |
| `cn.hutool.core.net.url.UrlPath` | `UrlPath addBefore(CharSequence segment)` | 添加到path最前面 |
| `cn.hutool.core.net.url.UrlPath` | `UrlPath of(CharSequence pathStr,Charset charset)` | 构建UrlPath |
| `cn.hutool.core.net.url.UrlPath` | `UrlPath parse(CharSequence path,Charset charset)` | 解析path |
| `cn.hutool.core.net.url.UrlPath` | `UrlPath setWithEndTag(boolean withEngTag)` | 是否path的末尾加 / |
| `cn.hutool.core.net.url.UrlQuery` | `CharSequence get(CharSequence key)` | 获取查询值 |
| `cn.hutool.core.net.url.UrlQuery` | `Map<CharSequence, CharSequence> getQueryMap()` | 获得查询的Map |
| `cn.hutool.core.net.url.UrlQuery` | `String build(Charset charset)` | 构建URL查询字符串，即将key-value键值对转换为key1=v1&key2=v2&key3=v3形式。 对于null处理规则如下： 如果key为null，则这个键值对忽略 如果value为null，只保留key，如key1对应value为null生成类似于key1&key2=v2形式 |
| `cn.hutool.core.net.url.UrlQuery` | `String build(Charset charset,boolean encodePercent)` | 构建URL查询字符串，即将key-value键值对转换为key1=v1&key2=v2&key3=v3形式。 对于null处理规则如下： 如果key为null，则这个键值对忽略 如果value为null，只保留key，如key1对应value为null生成类似于key1&key2=v2形式 |
| `cn.hutool.core.net.url.UrlQuery` | `String build(PercentCodec keyCoder,PercentCodec valueCoder,Charset charset)` | 构建URL查询字符串，即将key-value键值对转换为key1=v1&key2=v2&key3=v3形式。 对于null处理规则如下： 如果key为null，则这个键值对忽略 如果value为null，只保留key，如key1对应value为null生成类似于key1&key2=v2形式 |
| `cn.hutool.core.net.url.UrlQuery` | `String build(PercentCodec keyCoder,PercentCodec valueCoder,Charset charset,boolean encodePercent)` | 构建URL查询字符串，即将key-value键值对转换为key1=v1&key2=v2&key3=v3形式。 对于null处理规则如下： 如果key为null，则这个键值对忽略 如果value为null，只保留key，如key1对应value为null生成类似于key1&key2=v2形式 |
| `cn.hutool.core.net.url.UrlQuery` | `String toString()` | 生成查询字符串，类似于aaa=111&bbb=222 此方法不对任何特殊字符编码，仅用于输出显示 |
| `cn.hutool.core.net.url.UrlQuery` | `UrlQuery add(CharSequence key,Object value)` | 增加键值对 |
| `cn.hutool.core.net.url.UrlQuery` | `UrlQuery addAll(Map<? extends CharSequence, ?> queryMap)` | 批量增加键值对 |
| `cn.hutool.core.net.url.UrlQuery` | `UrlQuery of(Map<? extends CharSequence, ?> queryMap)` | 构建UrlQuery |
| `cn.hutool.core.net.url.UrlQuery` | `UrlQuery of(Map<? extends CharSequence, ?> queryMap,boolean isFormUrlEncoded)` | 构建UrlQuery |
| `cn.hutool.core.net.url.UrlQuery` | `UrlQuery of(String queryStr,Charset charset)` | 构建UrlQuery |
| `cn.hutool.core.net.url.UrlQuery` | `UrlQuery of(String queryStr,Charset charset,boolean autoRemovePath)` | 构建UrlQuery |
| `cn.hutool.core.net.url.UrlQuery` | `UrlQuery of(String queryStr,Charset charset,boolean autoRemovePath,boolean isFormUrlEncoded)` | 构建UrlQuery |
| `cn.hutool.core.net.url.UrlQuery` | `UrlQuery parse(String queryStr,Charset charset)` | 解析URL中的查询字符串 |
| `cn.hutool.core.net.url.UrlQuery` | `UrlQuery parse(String queryStr,Charset charset,boolean autoRemovePath)` | 解析URL中的查询字符串 |
| `cn.hutool.core.net.url.UrlQuery` | `UrlQuery remove(CharSequence key)` | 移除键及对应所有的值 |
| `cn.hutool.core.net.url.UrlQuery` | `UrlQuery setStrict(final boolean strict)` | 设置是否严格模式 |
