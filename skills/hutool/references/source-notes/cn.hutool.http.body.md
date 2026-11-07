# cn.hutool.http.body

版本 5.8.46。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `cn.hutool.http.body.BytesBody` | `BytesBody create(byte[] content)` | 创建 Http request body |
| `cn.hutool.http.body.BytesBody` | `void write(OutputStream out)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.body.FormUrlEncodedBody` | `FormUrlEncodedBody create(Map<String, Object> form,Charset charset)` | 创建 Http request body |
| `cn.hutool.http.body.FormUrlEncodedBody` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.body.MultipartBody` | `MultipartBody create(Map<String, Object> form,Charset charset)` | 根据已有表单内容，构建MultipartBody |
| `cn.hutool.http.body.MultipartBody` | `String getContentType()` | 获取Multipart的Content-Type类型 |
| `cn.hutool.http.body.MultipartBody` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.body.MultipartBody` | `void write(OutputStream out)` | 写出Multiparty数据，不关闭流 |
| `cn.hutool.http.body.RequestBody` | `void write(OutputStream out)` | 写出数据，不关闭流 |
| `cn.hutool.http.body.RequestBody` | `void writeClose(OutputStream out)` | 写出并关闭OutputStream |
| `cn.hutool.http.body.ResourceBody` | `ResourceBody create(Resource resource)` | 创建 Http request body |
| `cn.hutool.http.body.ResourceBody` | `String toString()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `cn.hutool.http.body.ResourceBody` | `void write(OutputStream out)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
