---
sidebar: 'auto'
editLinks: false
sidebarDepth: 3
---

[API 文档](https://pinia.vuejs.org/zh/api/index.md) / [pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md) / PiniaPluginContext

# 接口：PiniaPluginContext<Id, S, G, A\> %{#interface-piniaplugincontext-id-s-g-a}%

[pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md).PiniaPluginContext

传递给 Pinia 插件的上下文参数。

## 类型参数 %{#type-parameters}%

| Name | Type                                                                                                |
| :--- | :-------------------------------------------------------------------------------------------------- |
| `Id` | extends `string` = `string`                                                                         |
| `S`  | extends [`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree) = [`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree) |
| `G`  | [`_GettersTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#_getterstree)<`S`\>                                            |
| `A`  | [`_ActionsTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#_actionstree)                                                  |

## 属性

### app %{#app}%

• **app**: `App`<`any`\>

用 `Vue.createApp()`创建的当前应用。

---

### options %{#options}%

• **options**: [`DefineStoreOptionsInPlugin`](https://pinia.vuejs.org/zh/api/interfaces/pinia.DefineStoreOptionsInPlugin.md)<`Id`, `S`, `G`, `A`\>

调用 `defineStore()` 时定义 store 的初始选项。

---

### pinia %{#pinia}%

• **pinia**: [`Pinia`](https://pinia.vuejs.org/zh/api/interfaces/pinia.Pinia.md)

pinia 实例

---

### store %{#store}%

• **store**: [`Store`](https://pinia.vuejs.org/zh/api/modules/pinia.md#store)<`Id`, `S`, `G`, `A`\>

目前正在扩展的 store
