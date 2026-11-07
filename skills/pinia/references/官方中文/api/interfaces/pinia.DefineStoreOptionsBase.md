---
sidebar: 'auto'
editLinks: false
sidebarDepth: 3
---

[API 文档](https://pinia.vuejs.org/zh/api/index.md) / [pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md) / DefineStoreOptionsBase

# 接口：DefineStoreOptionsBase<S, Store\> %{#interface-definestoreoptionsbase-s-store}%

[pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md).DefineStoreOptionsBase

传递给 `defineStore()` 的选项，在 option store 和 setup store 之间是通用的。
如果你想为这两种 store 添加自定义的选项，
请扩展这个接口。

## 类型参数 %{#type-parameters}%

| Name    | Type                                                 |
| :------ | :--------------------------------------------------- |
| `S`     | extends [`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree) |
| `Store` | `Store`                                              |

## 层次结构 %{#hierarchy}%

- **`DefineStoreOptionsBase`**

  ↳ [`DefineStoreOptions`](https://pinia.vuejs.org/zh/api/interfaces/pinia.DefineStoreOptions.md)

  ↳ [`DefineSetupStoreOptions`](https://pinia.vuejs.org/zh/api/interfaces/pinia.DefineSetupStoreOptions.md)
