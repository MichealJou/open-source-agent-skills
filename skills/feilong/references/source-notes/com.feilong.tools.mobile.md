# com.feilong.tools.mobile

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.tools.mobile.MobileUtil` | `String getMobileNumberHided(String mobileNo,int count)` | 输入 11位手机号码,返回 中间4位或者n位数字为星(*)的号码. |
| `com.feilong.tools.mobile.MobileUtil` | `String getMobileNumberHided(String mobileNumber)` | 输入11位手机号码,返回 中间4位或者n位数字为星(*)的号码,默认4个星星. Examples: |
| `com.feilong.tools.mobile.MobileUtil` | `String getMobileNumberSegment(String mobileNumber)` | 获得手机的号码段. |
