# com.feilong.taglib.display.breadcrumb.command

版本 4.5.1。以下为上游源码 Javadoc 的短摘录，按声明签名区分重载；不是经过逐项验证的选型建议。

| 类 | 声明 | 源码说明 |
| --- | --- | --- |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity` | `String getName()` | Gets the name,用于拼接. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity` | `String getPath()` | Gets the 匹配的路径. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity` | `String getTitle()` | 【原文待译】Gets the title. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity` | `T getId()` | 获得 current id, 可以是Number String 或者其他类型. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity` | `T getParentId()` | 获得 parent id ,可以是Number String 或者其他类型. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity` | `void setId(T id)` | 设置 current id, 可以是Number String 或者其他类型. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity` | `void setName(String name)` | Sets the name,用于拼接. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity` | `void setParentId(T parentId)` | 设置 parent id ,可以是Number String 或者其他类型. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity` | `void setPath(String path)` | Sets the 匹配的路径. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbEntity` | `void setTitle(String title)` | 【原文待译】Sets the title. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbParams` | `List<BreadCrumbEntity<T>> getBreadCrumbEntityList()` | 获得 the bread crumb entity list. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbParams` | `String getConnector()` | 获得 the connector. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbParams` | `String getCurrentPath()` | 获得 the current path. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbParams` | `String getUrlPrefix()` | 获得 url前缀, 用来拼接 BreadCrumbEntity#path. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbParams` | `String getVmPath()` | 获得 vm的路径. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbParams` | `void setBreadCrumbEntityList(List<BreadCrumbEntity<T>> breadCrumbEntityList)` | 设置 the bread crumb entity list. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbParams` | `void setConnector(String connector)` | 设置 the connector. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbParams` | `void setCurrentPath(String currentPath)` | 设置 the current path. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbParams` | `void setUrlPrefix(String urlPrefix)` | 设置 url前缀, 用来拼接 BreadCrumbEntity#path. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbParams` | `void setVmPath(String vmPath)` | 设置 vm的路径. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbVMParams` | `List<BreadCrumbEntity<T>> getBreadCrumbEntityList()` | 获得 the bread crumb entity list. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbVMParams` | `String getConnector()` | 获得 the connector. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbVMParams` | `void setBreadCrumbEntityList(List<BreadCrumbEntity<T>> breadCrumbEntityList)` | 设置 the bread crumb entity list. |
| `com.feilong.taglib.display.breadcrumb.command.BreadCrumbVMParams` | `void setConnector(String connector)` | 设置 the connector. |
