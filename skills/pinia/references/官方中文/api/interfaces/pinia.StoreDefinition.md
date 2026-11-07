---
sidebar: 'auto'
editLinks: false
sidebarDepth: 3
---

[API 文档](https://pinia.vuejs.org/zh/api/index.md) / [pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md) / StoreDefinition

# 接口：StoreDefinition<Id, S, G, A\> %{#interface-storedefinition-id-s-g-a}%

[pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md).StoreDefinition

## 类型参数 %{#type-parameters}%

| 名称 | 类型                                                                                                |
| :--- | :-------------------------------------------------------------------------------------------------- |
| `Id` | extends `string` = `string`                                                                         |
| `S`  | extends [`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree) = [`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree) |
| `G`  | [`_GettersTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#_getterstree)<`S`\>                                            |
| `A`  | [`_ActionsTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#_actionstree)                                                  |

## Callable %{#callable}%

### StoreDefinition %{#storedefinition}%

▸ **StoreDefinition**(`pinia?`, `hot?`): [`Store`](https://pinia.vuejs.org/zh/api/modules/pinia.md#store)<`Id`, `S`, `G`, `A`\>

返回一个 store，有需要才创建它。

#### 参数

| 名称     | 类型                                               | 描述                                 |
| :------- | :------------------------------------------------- | :----------------------------------- |
| `pinia?` | `null` \| [`Pinia`](https://pinia.vuejs.org/zh/api/interfaces/pinia.Pinia.md)                | Pinia instance to retrieve the store |
| `hot?`   | [`StoreGeneric`](https://pinia.vuejs.org/zh/api/modules/pinia.md#storegeneric) | dev only hot module replacement      |

#### 返回值

[`Store`](https://pinia.vuejs.org/zh/api/modules/pinia.md#store)<`Id`, `S`, `G`, `A`\>

## 属性

### $id %{#id}%

• **$id**: `Id`

store 的 id。供映射辅助函数使用。
