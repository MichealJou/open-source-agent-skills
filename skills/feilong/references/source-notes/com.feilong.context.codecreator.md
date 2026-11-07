# com.feilong.context.codecreator

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.context.codecreator.CodeCreatorHelper` | `String debugLength(StringBuilder sb,boolean isDebug)` | 显示长度. |
| `com.feilong.context.codecreator.CodeCreatorHelper` | `String debugSeparator(boolean isDebug)` | 【原文待译】Debug. |
| `com.feilong.context.codecreator.CodeCreatorHelper` | `String formatLastValue(Long value,int lastLength)` | 格式化值. |
| `com.feilong.context.codecreator.DefaultGuestShoppingcartLineIdCreator` | `long create()` | 创建 id. 游客的购物车行id 仅仅用于增删修改等操作,不会存储到DB |
| `com.feilong.context.codecreator.GuestShoppingcartLineIdCreator` | `long create()` | 创建. |
| `com.feilong.context.codecreator.MultiSellerOrderCodeCreator` | `String create(Long buyerId,Long sellerId)` | 创建订单号. |
| `com.feilong.context.codecreator.SequenceTypeOrderCodeCreator` | `String create(long sequence,int maxLength)` | 创建code. |
| `com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreator` | `String create(Long buyerId,Long sellerId)` | 创建订单号. |
| `com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreator` | `void setSimpleMultiSellerOrderCodeCreatorConfig(SimpleMultiSellerOrderCodeCreatorConfig simpleMultiSellerOrderCodeCreatorConfig)` | 【原文待译】Sets the simple multi seller order code creator config. |
| `com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreatorConfig` | `String getPrefix()` | 获得 前缀, 以示区分, 比如,1 表示退单号, 4代表订单号;后期视业务需要可以将 b店 和C店 也区分出来. |
| `com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreatorConfig` | `boolean getIsDebug()` | 获得 是否开启debug模式. |
| `com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreatorConfig` | `int getBuyerIdLastLength()` | 获得 截取用户id 后面位数. |
| `com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreatorConfig` | `int getRandomNumberLength()` | 获得 随机数位数. |
| `com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreatorConfig` | `int getShopIdLastLength()` | 获得 截取shop id 后面位数. |
| `com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreatorConfig` | `void setBuyerIdLastLength(int buyerIdLastLength)` | 设置 截取用户id 后面位数. |
| `com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreatorConfig` | `void setIsDebug(boolean isDebug)` | 设置 是否开启debug模式. |
| `com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreatorConfig` | `void setPrefix(String prefix)` | 设置 前缀, 以示区分, 比如,1 表示退单号, 4代表订单号;后期视业务需要可以将 b店 和C店 也区分出来. |
| `com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreatorConfig` | `void setRandomNumberLength(int randomNumberLength)` | 设置 随机数位数. |
| `com.feilong.context.codecreator.SimpleMultiSellerOrderCodeCreatorConfig` | `void setShopIdLastLength(int shopIdLastLength)` | 设置 截取shop id 后面位数. |
| `com.feilong.context.codecreator.SimpleSequenceTypeOrderCodeCreator` | `String create(long sequence,int maxLength)` | 创建. |
| `com.feilong.context.codecreator.SimpleSequenceTypeOrderCodeCreator` | `void setIsDebug(boolean isDebug)` | 【原文待译】Sets the checks if is debug. |
