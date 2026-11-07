---
sidebar: 'auto'
editLinks: false
sidebarDepth: 3
---

[API 文档](https://pinia.vuejs.org/zh/api/index.md) / [pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md) / SubscriptionCallbackMutationPatchObject

# 接口：SubscriptionCallbackMutationPatchObject<S\> %{#interface-subscriptioncallbackmutationpatchobject-s}%

[pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md).SubscriptionCallbackMutationPatchObject

当 `store.$patch()` 与一个对象一起被调用时，
传递给订阅回调的上下文。

## 类型参数 %{#type-parameters}%

| 名称 |
| :--- |
| `S`  |

## 层次结构 %{#hierarchy}%

- [`_SubscriptionCallbackMutationBase`](https://pinia.vuejs.org/zh/api/interfaces/pinia._SubscriptionCallbackMutationBase.md)

  ↳ **`SubscriptionCallbackMutationPatchObject`**

## 属性

### 事件 %{#events}%

• **events**: `DebuggerEvent`[]

仅限 DEV， patch 调用的数组。

---

### payload %{#payload}%

• **payload**: [`_DeepPartial`](https://pinia.vuejs.org/zh/api/modules/pinia.md#_deeppartial)<`S`\>

传递给 `store.$patch()` 的对象

---

### storeId %{#storeid}%

• **storeId**: `string`

执行 mutation 的 store 的 `id`

#### 继承于

[\_SubscriptionCallbackMutationBase](https://pinia.vuejs.org/zh/api/interfaces/pinia._SubscriptionCallbackMutationBase.md).[storeId](https://pinia.vuejs.org/zh/api/interfaces/pinia._SubscriptionCallbackMutationBase.md#storeid)

---

### 类型 %{#type}%

• **type**: [`patchObject`](https://pinia.vuejs.org/zh/api/enums/pinia.MutationType.md#patchobject)

mutation 的类型

#### 重写 %{#overrides}%

[\_SubscriptionCallbackMutationBase](https://pinia.vuejs.org/zh/api/interfaces/pinia._SubscriptionCallbackMutationBase.md).[type](https://pinia.vuejs.org/zh/api/interfaces/pinia._SubscriptionCallbackMutationBase.md#type)
