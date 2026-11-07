# com.feilong.taglib.display.pager.command

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.taglib.display.pager.command.Pager` | `Integer getCount()` | Gets the 总共数据数,不同的数据库返回的类型不一样. |
| `com.feilong.taglib.display.pager.command.Pager` | `Integer getCurrentPageNo()` | Gets the 当前页码. |
| `com.feilong.taglib.display.pager.command.Pager` | `Integer getMaxShowPageNo()` | 显示最大的页码数,(-1或者不设置,默认显示所有页数). 比如淘宝,不管搜索东西多少,最多显示100页 这是一种折中的处理方式, 空间换时间 . 数据查询越往后翻,对服务器的压力越大,速度越低,而且从业务上来讲商品质量也越差,所以就没有必要给太多了. 新浪微博的时间轴也只给出了10页,同样的折中处理. |
| `com.feilong.taglib.display.pager.command.Pager` | `Integer getPageSize()` | Gets the 每页显示数量,默认10,传入该参数 可以计算分页数量. |
| `com.feilong.taglib.display.pager.command.Pager` | `List<T> getItemList()` | 获得 存放的数据集合. |
| `com.feilong.taglib.display.pager.command.Pager` | `int getAllPageNo()` | 总页数(#maxShowPageNo 参与装饰). 如果要获得原始的真正的总页数,请使用 #getOriginatingAllPageNo() |
| `com.feilong.taglib.display.pager.command.Pager` | `int getNextPageNo()` | 下一页页码. |
| `com.feilong.taglib.display.pager.command.Pager` | `int getOriginatingAllPageNo()` | 获得原始的总页数(不经过 #maxShowPageNo)修饰过的. 通过这个值可以实现一些特殊的功能,一般用不到 |
| `com.feilong.taglib.display.pager.command.Pager` | `int getOriginatingNextPageNo()` | 在原始的总页数基础上进行解析的下一页页码. 通过这个值可以实现一些特殊的功能,一般用不到 |
| `com.feilong.taglib.display.pager.command.Pager` | `int getPrePageNo()` | 上一页页码. |
| `com.feilong.taglib.display.pager.command.Pager` | `void setCount(Integer count)` | Sets the 总共数据数,不同的数据库返回的类型不一样. |
| `com.feilong.taglib.display.pager.command.Pager` | `void setCurrentPageNo(Integer currentPageNo)` | Sets the 当前页码. |
| `com.feilong.taglib.display.pager.command.Pager` | `void setItemList(List<T> itemList)` | 设置 存放的数据集合. |
| `com.feilong.taglib.display.pager.command.Pager` | `void setMaxShowPageNo(Integer maxShowPageNo)` | 显示最大的页码数,(-1或者不设置,默认显示所有页数). 比如淘宝,不管搜索东西多少,最多显示100页 这是一种折中的处理方式, 空间换时间 . 数据查询越往后翻,对服务器的压力越大,速度越低,而且从业务上来讲商品质量也越差,所以就没有必要给太多了. 新浪微博的时间轴也只给出了10页,同样的折中处理. |
| `com.feilong.taglib.display.pager.command.Pager` | `void setPageSize(Integer pageSize)` | Sets the 每页显示数量,默认10,传入该参数 可以计算分页数量. |
| `com.feilong.taglib.display.pager.command.PagerAndContent` | `Pager<T> getPager()` | 获得 分页数据(包含数据集). |
| `com.feilong.taglib.display.pager.command.PagerAndContent` | `String getContent()` | 获得 渲染出来的分页html代码. |
| `com.feilong.taglib.display.pager.command.PagerAndContent` | `void setContent(String content)` | 设置 渲染出来的分页html代码. |
| `com.feilong.taglib.display.pager.command.PagerAndContent` | `void setPager(Pager<T> pager)` | 设置 分页数据(包含数据集). |
| `com.feilong.taglib.display.pager.command.PagerParams` | `Integer getCurrentPageNo()` | 获得 当前第几页. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `Integer getMaxShowPageNo()` | 显示最大的页码数,(-1或者不设置,默认显示所有页数). 比如淘宝,不管搜索东西多少,最多显示100页 这是一种折中的处理方式, 空间换时间 . 数据查询越往后翻,对服务器的压力越大,速度越低,而且从业务上来讲商品质量也越差,所以就没有必要给太多了. 新浪微博的时间轴也只给出了10页,同样的折中处理. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `Integer getPageSize()` | 获得 每页显示多少条. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `Integer getTotalCount()` | 获得 总数据条数. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `Locale getLocale()` | 获得 获得此 Java 虚拟机实例的当前默认语言环境值. Java 虚拟机根据主机的环境在启动期间设置默认语言环境.如果没有明确地指定语言环境,则很多语言环境敏感的方法都使用该方法.可使用 setDefault 方法更改该值.. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `PagerType getPagerType()` | 获得 the pager type. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `String getCharsetType()` | 获得 编码集. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `String getDynamicNavigationPageNumberConfig()` | 动态显示导航页码数量(默认是 PagerConstants#DEFAULT_DYNAMIC_NAVIGATION_PAGE_NUMBER_CONFIG). |
| `com.feilong.taglib.display.pager.command.PagerParams` | `String getPageParamName()` | 获得 分页参数名称. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `String getPageUrl()` | 获得 分页的 基础 url. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `String getSkin()` | 获得 皮肤:可选. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `String getVmPath()` | 获得 vm的路径. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `boolean equals(Object obj)` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.display.pager.command.PagerParams` | `boolean getDebugIsNotParseVM()` | 获得 debug 模式. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `int hashCode()` | 【无源码摘要】需查对应源码、继承文档或上游 API。 |
| `com.feilong.taglib.display.pager.command.PagerParams` | `void setCharsetType(String charsetType)` | 设置 编码集. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `void setCurrentPageNo(Integer currentPageNo)` | 设置 当前第几页. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `void setDebugIsNotParseVM(boolean debugIsNotParseVM)` | 设置 debug 模式. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `void setDynamicNavigationPageNumberConfig(String dynamicNavigationPageNumberConfig)` | 动态显示导航页码数量(默认是 PagerConstants#DEFAULT_DYNAMIC_NAVIGATION_PAGE_NUMBER_CONFIG). |
| `com.feilong.taglib.display.pager.command.PagerParams` | `void setLocale(Locale locale)` | 设置 获得此 Java 虚拟机实例的当前默认语言环境值. Java 虚拟机根据主机的环境在启动期间设置默认语言环境.如果没有明确地指定语言环境,则很多语言环境敏感的方法都使用该方法.可使用 setDefault 方法更改该值.. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `void setMaxShowPageNo(Integer maxShowPageNo)` | 显示最大的页码数,(-1或者不设置,默认显示所有页数). 比如淘宝,不管搜索东西多少,最多显示100页 这是一种折中的处理方式, 空间换时间 . 数据查询越往后翻,对服务器的压力越大,速度越低,而且从业务上来讲商品质量也越差,所以就没有必要给太多了. 新浪微博的时间轴也只给出了10页,同样的折中处理. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `void setPageParamName(String pageParamName)` | 设置 分页参数名称. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `void setPageSize(Integer pageSize)` | 设置 每页显示多少条. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `void setPageUrl(String pageUrl)` | 设置 分页的 基础 url. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `void setPagerType(PagerType pagerType)` | 设置 the pager type. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `void setSkin(String skin)` | 设置 皮肤:可选. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `void setTotalCount(Integer totalCount)` | 设置 总数据条数. |
| `com.feilong.taglib.display.pager.command.PagerParams` | `void setVmPath(String vmPath)` | 设置 vm的路径. |
| `com.feilong.taglib.display.pager.command.PagerUrlTemplate` | `Integer getTemplateValue()` | 获得 模板链接里面的分页号码. |
| `com.feilong.taglib.display.pager.command.PagerUrlTemplate` | `String getHref()` | 获得 链接的模板,以便前端js 替换. |
| `com.feilong.taglib.display.pager.command.PagerUrlTemplate` | `void setHref(String href)` | 设置 链接的模板,以便前端js 替换. |
| `com.feilong.taglib.display.pager.command.PagerUrlTemplate` | `void setTemplateValue(Integer templateValue)` | 设置 模板链接里面的分页号码. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `Integer getAllPageNo()` | Gets the 总页数. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `Integer getCurrentPageNo()` | Gets the 当前页码. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `Integer getEndIteratorIndex()` | Gets the 结束迭代索引编号. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `Integer getMaxShowPageNo()` | 显示最大的页码数,(-1或者不设置,默认显示所有页数). 比如淘宝,不管搜索东西多少,最多显示100页 这是一种折中的处理方式, 空间换时间 . 数据查询越往后翻,对服务器的压力越大,速度越低,而且从业务上来讲商品质量也越差,所以就没有必要给太多了. 新浪微博的时间轴也只给出了10页,同样的折中处理. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `Integer getNextPageNo()` | 获得 下一页页码. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `Integer getPrePageNo()` | 获得 上一页页码. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `Integer getStartIteratorIndex()` | Gets the 开始迭代索引编号. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `Integer getTotalCount()` | Gets the 总行数,总结果数. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `Map<Integer, String> getIteratorIndexMap()` | 获得 循环迭代索引map,key是编号,value是页面链接. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `PagerType getPagerType()` | 获得 the pager type. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `PagerUrlTemplate getPagerUrlTemplate()` | 【原文待译】Gets the pager url template. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `String getFirstUrl()` | Gets the 第一页的链接. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `String getLastUrl()` | Gets the 最后一页的链接. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `String getNextUrl()` | Gets the 下一页链接. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `String getPageParamName()` | 获得 参数. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `String getPreUrl()` | Gets the 上一页链接. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `String getSkin()` | Gets the 设置的皮肤. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setAllPageNo(Integer allPageNo)` | Sets the 总页数. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setCurrentPageNo(Integer currentPageNo)` | Sets the 当前页码. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setEndIteratorIndex(Integer endIteratorIndex)` | Sets the 结束迭代索引编号. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setFirstUrl(String firstUrl)` | Sets the 第一页的链接. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setIteratorIndexMap(Map<Integer, String> iteratorIndexMap)` | 设置 循环迭代索引map,key是编号,value是页面链接. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setLastUrl(String lastUrl)` | Sets the 最后一页的链接. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setMaxShowPageNo(Integer maxShowPageNo)` | 显示最大的页码数,(-1或者不设置,默认显示所有页数). 比如淘宝,不管搜索东西多少,最多显示100页 这是一种折中的处理方式, 空间换时间 . 数据查询越往后翻,对服务器的压力越大,速度越低,而且从业务上来讲商品质量也越差,所以就没有必要给太多了. 新浪微博的时间轴也只给出了10页,同样的折中处理. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setNextPageNo(Integer nextPageNo)` | 设置 下一页页码. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setNextUrl(String nextUrl)` | Sets the 下一页链接. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setPageParamName(String pageParamName)` | 设置 参数. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setPagerType(PagerType pagerType)` | 设置 the pager type. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setPagerUrlTemplate(PagerUrlTemplate pagerUrlTemplate)` | 【原文待译】Sets the pager url template. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setPrePageNo(Integer prePageNo)` | 设置 上一页页码. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setPreUrl(String preUrl)` | Sets the 上一页链接. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setSkin(String skin)` | Sets the 设置的皮肤. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setStartIteratorIndex(Integer startIteratorIndex)` | Sets the 开始迭代索引编号. |
| `com.feilong.taglib.display.pager.command.PagerVMParam` | `void setTotalCount(Integer totalCount)` | Sets the 总行数,总结果数. |
