# com.feilong.taglib.display.breadcrumb

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.taglib.display.breadcrumb.BreadCrumbTag` | `String getConnector()` | 获得 连接符,默认>. |
| `com.feilong.taglib.display.breadcrumb.BreadCrumbTag` | `String getUrlPrefix()` | 获得 url前缀, 用来拼接 BreadCrumbEntity#getPath(),可以不设置,那么原样输出BreadCrumbEntity#getPath(). |
| `com.feilong.taglib.display.breadcrumb.BreadCrumbTag` | `String getVmPath()` | 获得 vm的路径. |
| `com.feilong.taglib.display.breadcrumb.BreadCrumbTag` | `void setBreadCrumbEntityList(List<BreadCrumbEntity<Object>> breadCrumbEntityList)` | 设置 siteMapEntityList,用户所有可以访问的菜单url List. |
| `com.feilong.taglib.display.breadcrumb.BreadCrumbTag` | `void setConnector(String connector)` | 设置 连接符,默认>. |
| `com.feilong.taglib.display.breadcrumb.BreadCrumbTag` | `void setUrlPrefix(String urlPrefix)` | url前缀, 用来拼接 BreadCrumbEntity#getPath(),可以不设置,那么原样输出BreadCrumbEntity#getPath(). |
| `com.feilong.taglib.display.breadcrumb.BreadCrumbTag` | `void setVmPath(String vmPath)` | 设置 vm的路径. |
| `com.feilong.taglib.display.breadcrumb.BreadCrumbUtil` | `String getBreadCrumbContent(BreadCrumbParams breadCrumbParams)` | 获得 bread crumb content. |
