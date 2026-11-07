# com.feilong.accessor.cookie

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.accessor.cookie.CookieAccessor` | `CookieEntity getCookieEntity()` | 获得 cookie entity. |
| `com.feilong.accessor.cookie.CookieAccessor` | `String get(HttpServletRequest request)` | 获得寄存器中保存的内容. |
| `com.feilong.accessor.cookie.CookieAccessor` | `boolean getIsValueEncoding()` | 获得 是否将值进行encode操作. |
| `com.feilong.accessor.cookie.CookieAccessor` | `void remove(HttpServletResponse response)` | 删除寄存器保存的内容. |
| `com.feilong.accessor.cookie.CookieAccessor` | `void save(String value,HttpServletResponse response)` | 将 value 保存到cookie中. |
| `com.feilong.accessor.cookie.CookieAccessor` | `void setCookieEntity(CookieEntity cookieEntity)` | 设置 cookie entity. |
| `com.feilong.accessor.cookie.CookieAccessor` | `void setIsValueEncoding(boolean isValueEncoding)` | 设置 是否将值进行encode操作. |
