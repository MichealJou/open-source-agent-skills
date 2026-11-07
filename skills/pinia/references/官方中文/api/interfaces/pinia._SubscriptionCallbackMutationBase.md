---
sidebar: 'auto'
editLinks: false
sidebarDepth: 3
---

[API 文档](https://pinia.vuejs.org/zh/api/index.md) / [pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md) / \_SubscriptionCallbackMutationBase

# 接口：\_SubscriptionCallbackMutationBase %{#interface-subscriptioncallbackmutationbase}%

[pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md).\_SubscriptionCallbackMutationBase

传递给订阅回调的上下文的基本类型。内部类型。

## 层次结构 %{#hierarchy}%

- **`_SubscriptionCallbackMutationBase`**

  ↳ [`SubscriptionCallbackMutationDirect`](https://pinia.vuejs.org/zh/api/interfaces/pinia.SubscriptionCallbackMutationDirect.md)

  ↳ [`SubscriptionCallbackMutationPatchFunction`](https://pinia.vuejs.org/zh/api/interfaces/pinia.SubscriptionCallbackMutationPatchFunction.md)

  ↳ [`SubscriptionCallbackMutationPatchObject`](https://pinia.vuejs.org/zh/api/interfaces/pinia.SubscriptionCallbackMutationPatchObject.md)

## 属性

### storeId %{#storeid}%

• **storeId**: `string`

执行 mutation 的 store 的`id`。

---

### 类型 %{#type}%

• **type**: [`MutationType`](https://pinia.vuejs.org/zh/api/enums/pinia.MutationType.md)

mutation 的类型
