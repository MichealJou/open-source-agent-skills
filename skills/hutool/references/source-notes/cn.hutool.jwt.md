# cn.hutool.jwt

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.jwt.Claims` | `JSONObject getClaimsJson()` | 获取Claims的JSON字符串形式 |
| `cn.hutool.jwt.Claims` | `Object getClaim(String name)` | 获取指定名称属性 |
| `cn.hutool.jwt.Claims` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.jwt.Claims` | `void parse(String tokenPart,Charset charset)` | 解析JWT JSON |
| `cn.hutool.jwt.JWT` | `JSONObject getHeaders()` | 获取所有头信息 |
| `cn.hutool.jwt.JWT` | `JSONObject getPayloads()` | 获取所有载荷信息 |
| `cn.hutool.jwt.JWT` | `JWT addHeaders(Map<String, ?> headers)` | 增加JWT头信息 |
| `cn.hutool.jwt.JWT` | `JWT addPayloads(Map<String, ?> payloads)` | 增加JWT载荷信息 |
| `cn.hutool.jwt.JWT` | `JWT create()` | 创建空的JWT对象 |
| `cn.hutool.jwt.JWT` | `JWT of(String token)` | 创建并解析JWT对象 |
| `cn.hutool.jwt.JWT` | `JWT parse(String token)` | 解析JWT内容 |
| `cn.hutool.jwt.JWT` | `JWT setCharset(Charset charset)` | 设置编码 |
| `cn.hutool.jwt.JWT` | `JWT setHeader(String name,Object value)` | 设置JWT头信息 |
| `cn.hutool.jwt.JWT` | `JWT setKey(byte[] key)` | 设置密钥，如果头部指定了算法，直接使用，否则默认算法是：HS256(HmacSHA256) |
| `cn.hutool.jwt.JWT` | `JWT setPayload(String name,Object value)` | 设置JWT载荷信息 |
| `cn.hutool.jwt.JWT` | `JWT setSigner(JWTSigner signer)` | 设置签名算法 |
| `cn.hutool.jwt.JWT` | `JWT setSigner(String algorithmId,Key key)` | 设置签名算法 |
| `cn.hutool.jwt.JWT` | `JWT setSigner(String algorithmId,KeyPair keyPair)` | 设置非对称签名算法 |
| `cn.hutool.jwt.JWT` | `JWT setSigner(String algorithmId,byte[] key)` | 设置签名算法 |
| `cn.hutool.jwt.JWT` | `JWTHeader getHeader()` | 获取头 |
| `cn.hutool.jwt.JWT` | `JWTPayload getPayload()` | 获取载荷对象 |
| `cn.hutool.jwt.JWT` | `JWTSigner getSigner()` | 获取JWT算法签名器 |
| `cn.hutool.jwt.JWT` | `Object getHeader(String name)` | 获取头信息 |
| `cn.hutool.jwt.JWT` | `Object getPayload(String name)` | 获取载荷信息 |
| `cn.hutool.jwt.JWT` | `String getAlgorithm()` | 获取算法ID(alg)头信息 |
| `cn.hutool.jwt.JWT` | `String sign()` | 签名生成JWT字符串 |
| `cn.hutool.jwt.JWT` | `String sign(JWTSigner signer)` | 签名生成JWT字符串 |
| `cn.hutool.jwt.JWT` | `String sign(JWTSigner signer,boolean addTypeIfNot)` | 签名生成JWT字符串 |
| `cn.hutool.jwt.JWT` | `String sign(boolean addTypeIfNot)` | 签名生成JWT字符串 |
| `cn.hutool.jwt.JWT` | `boolean validate(long leeway)` | 验证JWT是否有效，验证包括： Token是否正确 JWTPayload#NOT_BEFORE：生效时间不能晚于当前时间 JWTPayload#EXPIRES_AT：失效时间不能早于当前时间 JWTPayload#ISSUED_AT： 签发时间不能晚于当前时间 |
| `cn.hutool.jwt.JWT` | `boolean verify()` | 验证JWT Token是否有效 |
| `cn.hutool.jwt.JWT` | `boolean verify(JWTSigner signer)` | 验证JWT Token是否有效 |
| `cn.hutool.jwt.JWTHeader` | `JWTHeader addHeaders(Map<String, ?> headerClaims)` | 增加自定义JWT认证头 |
| `cn.hutool.jwt.JWTHeader` | `JWTHeader setAlgorithm(final String algorithm)` | 增加“alg”头信息 |
| `cn.hutool.jwt.JWTHeader` | `JWTHeader setContentType(final String contentType)` | 增加“cty”头信息 |
| `cn.hutool.jwt.JWTHeader` | `JWTHeader setKeyId(String keyId)` | 增加“kid”头信息 |
| `cn.hutool.jwt.JWTHeader` | `JWTHeader setType(final String type)` | 增加“typ”头信息 |
| `cn.hutool.jwt.JWTPayload` | `JWTPayload addPayloads(Map<String, ?> payloadClaims)` | 增加自定义JWT认证载荷信息 |
| `cn.hutool.jwt.JWTPayload` | `JWTPayload setPayload(String name,Object value)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.jwt.JWTUtil` | `JWT parseToken(String token)` | 解析JWT Token |
| `cn.hutool.jwt.JWTUtil` | `String createToken(Map<String, Object> headers,Map<String, Object> payload,JWTSigner signer)` | 创建JWT Token |
| `cn.hutool.jwt.JWTUtil` | `String createToken(Map<String, Object> headers,Map<String, Object> payload,byte[] key)` | 创建HS256(HmacSHA256) JWT Token |
| `cn.hutool.jwt.JWTUtil` | `String createToken(Map<String, Object> payload,JWTSigner signer)` | 创建JWT Token |
| `cn.hutool.jwt.JWTUtil` | `String createToken(Map<String, Object> payload,byte[] key)` | 创建HS256(HmacSHA256) JWT Token |
| `cn.hutool.jwt.JWTUtil` | `boolean verify(String token,JWTSigner signer)` | 验证JWT Token有效性 |
| `cn.hutool.jwt.JWTUtil` | `boolean verify(String token,byte[] key)` | 验证JWT Token有效性 |
| `cn.hutool.jwt.JWTValidator` | `JWTValidator of(JWT jwt)` | 创建JWT验证器 |
| `cn.hutool.jwt.JWTValidator` | `JWTValidator of(String token)` | 创建JWT验证器 |
| `cn.hutool.jwt.JWTValidator` | `JWTValidator validateAlgorithm()` | 验证算法，使用JWT对象自带的JWTSigner |
| `cn.hutool.jwt.JWTValidator` | `JWTValidator validateAlgorithm(JWTSigner signer)` | 验证算法，使用自定义的JWTSigner |
| `cn.hutool.jwt.JWTValidator` | `JWTValidator validateDate()` | 检查JWT的以下三两个时间： JWTPayload#NOT_BEFORE：被检查时间必须晚于生效时间 JWTPayload#EXPIRES_AT：被检查时间必须早于失效时间 JWTPayload#ISSUED_AT：签发时间必须早于失效时间 如果某个时间没有设置，则不检查（表示无限制） |
| `cn.hutool.jwt.JWTValidator` | `JWTValidator validateDate(Date dateToCheck)` | 检查JWT的以下三两个时间： JWTPayload#NOT_BEFORE：生效时间不能晚于当前时间 JWTPayload#EXPIRES_AT：失效时间不能早于当前时间 JWTPayload#ISSUED_AT： 签发时间不能晚于当前时间 如果某个时间没有设置，则不检查（表示无限制） |
| `cn.hutool.jwt.JWTValidator` | `JWTValidator validateDate(Date dateToCheck,long leeway)` | 检查JWT的以下三两个时间： JWTPayload#NOT_BEFORE：生效时间不能晚于当前时间 JWTPayload#EXPIRES_AT：失效时间不能早于当前时间 JWTPayload#ISSUED_AT： 签发时间不能晚于当前时间 如果某个时间没有设置，则不检查（表示无限制） |
| `cn.hutool.jwt.RegisteredPayload` | `T setAudience(String... audience)` | 设置接收jwt的一方("aud")的Payload值 |
| `cn.hutool.jwt.RegisteredPayload` | `T setExpiresAt(Date expiresAt)` | 设置jwt的过期时间("exp")的Payload值，这个过期时间必须要大于签发时间 |
| `cn.hutool.jwt.RegisteredPayload` | `T setIssuedAt(Date issuedAt)` | 设置jwt的签发时间("iat") |
| `cn.hutool.jwt.RegisteredPayload` | `T setIssuer(String issuer)` | 设置 jwt签发者("iss")的Payload值 |
| `cn.hutool.jwt.RegisteredPayload` | `T setJWTId(String jwtId)` | 设置jwt的唯一身份标识("jti") |
| `cn.hutool.jwt.RegisteredPayload` | `T setNotBefore(Date notBefore)` | 设置不可用时间点界限("nbf")的Payload值 |
| `cn.hutool.jwt.RegisteredPayload` | `T setPayload(String name,Object value)` | 设置Payload值 |
| `cn.hutool.jwt.RegisteredPayload` | `T setSubject(String subject)` | 设置jwt所面向的用户("sub")的Payload值 |
