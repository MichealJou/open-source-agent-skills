# com.feilong.validator

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.validator.ValidatorUtil` | `boolean isEmail(String email)` | 判断给定的email 字符串是不是邮箱. |
| `com.feilong.validator.ValidatorUtil` | `boolean isMatches(String pattern,String input)` | 编译给定正则表达式 regexPattern ,并尝试将给定输入 input 与其匹配. |
| `com.feilong.validator.ValidatorUtil` | `boolean isMobile(String mobile)` | 判断字符串是否是手机号码. |
| `com.feilong.validator.ValidatorUtil` | `boolean isTelephone(String telephone)` | 判断字符串是否是大陆的电话号码. |
| `com.feilong.validator.ValidatorUtil` | `boolean isTelephoneMustAreacode(String telephoneMustAreacode)` | 判断字符串是否是大陆的电话号码(必须要有区号). |
| `com.feilong.validator.ValidatorUtil` | `boolean isZipcode(String zipcode)` | 判断字符串是否是邮编. |
