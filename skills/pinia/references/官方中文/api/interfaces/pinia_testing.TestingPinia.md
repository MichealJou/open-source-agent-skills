---
sidebar: 'auto'
editLinks: false
sidebarDepth: 3
---

[API 文档](https://pinia.vuejs.org/zh/api/index.md) / [@pinia/testing](https://pinia.vuejs.org/zh/api/modules/pinia_testing.md) / TestingPinia

# 接口：TestingPinia %{#interface-testingpinia}%

[@pinia/testing](https://pinia.vuejs.org/zh/api/modules/pinia_testing.md).TestingPinia

专门为测试设计的 Pinia 实例。
用测试中的特定属性扩展普通的 [Pinia](https://pinia.vuejs.org/zh/api/interfaces/pinia.Pinia.md) 实例。

## 层次结构 %{#hierarchy}%

- [`Pinia`](https://pinia.vuejs.org/zh/api/interfaces/pinia.Pinia.md)

  ↳ **`TestingPinia`**

## 属性

### app %{#app}%

• **app**: `App`<`any`\>

Pinia 使用的应用

---

### 安装 %{#install}%

• **install**: (`app`: `App`<`any`\>) => `void`

#### 类型声明 %{#type-declaration}%

▸ (`app`): `void`

##### 参数

| 名称  | 类型          |
| :---- | :------------ |
| `app` | `App`<`any`\> |

##### 返回值

`void`

#### 继承于

[Pinia](https://pinia.vuejs.org/zh/api/interfaces/pinia.Pinia.md).[install](https://pinia.vuejs.org/zh/api/interfaces/pinia.Pinia.md#install)

---

### state %{#state}%

• **state**: `Ref`<`Record`<`string`, [`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree)\>\>

根 state

#### 继承于

[Pinia](https://pinia.vuejs.org/zh/api/interfaces/pinia.Pinia.md).[state](https://pinia.vuejs.org/zh/api/interfaces/pinia.Pinia.md#state)

## 方法 %{#methods}%

### use %{#use}%

▸ **use**(`plugin`): [`Pinia`](https://pinia.vuejs.org/zh/api/interfaces/pinia.Pinia.md)

增加了一个 store 插件来扩展每个 store

#### 参数

| 名称     | 类型                                  | 描述                |
| :------- | :------------------------------------ | :------------------ |
| `plugin` | [`PiniaPlugin`](https://pinia.vuejs.org/zh/api/interfaces/pinia.PiniaPlugin.md) | store plugin to add |

#### 返回值

[`Pinia`](https://pinia.vuejs.org/zh/api/interfaces/pinia.Pinia.md)

#### 继承于

[Pinia](https://pinia.vuejs.org/zh/api/interfaces/pinia.Pinia.md).[use](https://pinia.vuejs.org/zh/api/interfaces/pinia.Pinia.md#use)
