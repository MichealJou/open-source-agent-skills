---
sidebar: 'auto'
editLinks: false
sidebarDepth: 3
---

[API 文档](https://pinia.vuejs.org/zh/api/index.md) / [pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md) / PiniaCustomProperties

# 接口：PiniaCustomProperties<Id, S, G, A\> %{#interface-piniacustomproperties-id-s-g-a}%

[pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md).PiniaCustomProperties

当用户通过插件添加属性时，接口可被扩展。

## 类型参数 %{#type-parameters}%

| 名称 | 类型                                                                                                |
| :--- | :-------------------------------------------------------------------------------------------------- |
| `Id` | extends `string` = `string`                                                                         |
| `S`  | extends [`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree) = [`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree) |
| `G`  | [`_GettersTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#_getterstree)<`S`\>                                            |
| `A`  | [`_ActionsTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#_actionstree)                                                  |

## Accessors %{#accessors}%

### route %{#route}%

• `get` **route**(): `RouteLocationNormalized`

#### 返回值

`RouteLocationNormalized`

• `set` **route**(`value`): `void`

#### 参数

| Name    | Type                                                                       |
| :------ | :------------------------------------------------------------------------- |
| `value` | `RouteLocationNormalizedLoaded` \| `Ref`<`RouteLocationNormalizedLoaded`\> |

#### 返回值

`void`
