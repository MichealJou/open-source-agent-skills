# com.feilong.taglib.display.pager

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.taglib.display.pager.PagerBuilder` | `PagerAndContent<T> buildPagerAndContent(PagerParams pagerParams,List<T> itemList)` | 通常用于ajax分页. |
| `com.feilong.taglib.display.pager.PagerBuilder` | `String buildContent(PagerParams pagerParams)` | 解析VM模板,生成分页HTML代码. |
| `com.feilong.taglib.display.pager.PagerCacheContentBuilder` | `String build(PagerParams pagerParams)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.display.pager.PagerHelper` | `Integer getCurrentPageNo(HttpServletRequest request,String pageParamName)` | 获得当前分页数字,不带这个参数或者转换异常 返回1. |
| `com.feilong.taglib.display.pager.PagerTag` | `String buildContent(HttpServletRequest request)` | 【原文待译】Write content. |
| `com.feilong.taglib.display.pager.PagerTag` | `void setCharsetType(String charsetType)` | Sets the url编码. |
| `com.feilong.taglib.display.pager.PagerTag` | `void setCount(Integer count)` | Sets the 数据总数. |
| `com.feilong.taglib.display.pager.PagerTag` | `void setDynamicNavigationPageNumberConfig(String dynamicNavigationPageNumberConfig)` | 动态显示导航页码数量(默认是 PagerConstants#DEFAULT_DYNAMIC_NAVIGATION_PAGE_NUMBER_CONFIG). |
| `com.feilong.taglib.display.pager.PagerTag` | `void setLocale(Object locale)` | 设置Locale 环境, 支持 java.util.Locale 或 String 类型的实例 . |
| `com.feilong.taglib.display.pager.PagerTag` | `void setMaxShowPageNo(Integer maxShowPageNo)` | 显示最大的页码数,(-1或者不设置,默认显示所有页数). 比如淘宝,不管搜索东西多少,最多显示100页 这是一种折中的处理方式, 空间换时间 . 数据查询越往后翻,对服务器的压力越大,速度越低,而且从业务上来讲商品质量也越差,所以就没有必要给太多了. 新浪微博的时间轴也只给出了10页,同样的折中处理. |
| `com.feilong.taglib.display.pager.PagerTag` | `void setPageParamName(String pageParamName)` | Sets the url页码参数,默认 pageNo. |
| `com.feilong.taglib.display.pager.PagerTag` | `void setPageSize(Integer pageSize)` | Sets the 每页显示多少行,默认20. |
| `com.feilong.taglib.display.pager.PagerTag` | `void setPagerHtmlAttributeName(String pagerHtmlAttributeName)` | vm被解析出来的文本,会被存在在这个变量中,作用域为pageContext,以便重复使用. 比如某些页面,上面下面都要显示同样的分页,方便用户操作. 此外,此变量名称允许变更,以便实现同一页页面不同功能的的分页. |
| `com.feilong.taglib.display.pager.PagerTag` | `void setSkin(String skin)` | Sets the 皮肤 默认digg. |
| `com.feilong.taglib.display.pager.PagerTag` | `void setVmPath(String vmPath)` | 基于classpath 下面的velocity模版文件路径. |
| `com.feilong.taglib.display.pager.PagerTagExtraInfo` | `ValidationMessage[] validate(TagData tagData)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.display.pager.PagerTagExtraInfo` | `VariableInfo[] getVariableInfo(TagData tagData)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
