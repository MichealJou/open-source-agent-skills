---
sidebar: 'auto'
editLinks: false
sidebarDepth: 3
---

[API 文档](https://pinia.vuejs.org/zh/api/index.md) / [pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md) / PiniaPlugin

# 接口：PiniaPlugin %{#interface-piniaplugin}%

[pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md).PiniaPlugin

## Callable %{#callable}%

### PiniaPlugin %{#piniaplugin}%

▸ **PiniaPlugin**(`context`): `void` \| `Partial`<[`PiniaCustomProperties`](https://pinia.vuejs.org/zh/api/interfaces/pinia.PiniaCustomProperties.md)<`string`, [`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree), [`_GettersTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#_getterstree)<[`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree)\>, [`_ActionsTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#_actionstree)\> & [`PiniaCustomStateProperties`](https://pinia.vuejs.org/zh/api/interfaces/pinia.PiniaCustomStateProperties.md)<[`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree)\>\>

用于扩展每个 store 的插件。返回一个扩展 store 的对象或
没有返回值。

#### 参数

| 名称      | 类型                                                                                                                                                                                                                                                                | 描述    |
| :-------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | :------ |
| `context` | [`PiniaPluginContext`](https://pinia.vuejs.org/zh/api/interfaces/pinia.PiniaPluginContext.md)<`string`, [`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree), [`_GettersTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#_getterstree)<[`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree)\>, [`_ActionsTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#_actionstree)\> | Context |

#### 返回值

`void` \| `Partial`<[`PiniaCustomProperties`](https://pinia.vuejs.org/zh/api/interfaces/pinia.PiniaCustomProperties.md)<`string`, [`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree), [`_GettersTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#_getterstree)<[`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree)\>, [`_ActionsTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#_actionstree)\> & [`PiniaCustomStateProperties`](https://pinia.vuejs.org/zh/api/interfaces/pinia.PiniaCustomStateProperties.md)<[`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree)\>\>
