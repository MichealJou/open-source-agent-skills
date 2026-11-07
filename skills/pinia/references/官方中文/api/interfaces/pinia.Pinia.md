---
sidebar: 'auto'
editLinks: false
sidebarDepth: 3
---

[API 文档](https://pinia.vuejs.org/zh/api/index.md) / [pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md) / Pinia

# 接口：Pinia %{#interface-pinia}%

[pinia](https://pinia.vuejs.org/zh/api/modules/pinia.md).Pinia

Every application must own its own pinia to be able to create stores

## 层次结构 %{#hierarchy}%

- **`Pinia`**

  ↳ [`TestingPinia`](https://pinia.vuejs.org/zh/api/interfaces/pinia_testing.TestingPinia.md)

## 属性

### 安装 %{#install}%

• **install**: (`app`: `App`<`any`\>) => `void`

#### 类型声明 %{#type-declaration}%

▸ (`app`): `void`

##### 参数

| Name  | Type          |
| :---- | :------------ |
| `app` | `App`<`any`\> |

##### 返回值

`void`

---

### state %{#state}%

• **state**: `Ref`<`Record`<`string`, [`StateTree`](https://pinia.vuejs.org/zh/api/modules/pinia.md#statetree)\>\>

根 state

## 方法 %{#methods}%

### use %{#use}%

▸ **use**(`plugin`): [`Pinia`](https://pinia.vuejs.org/zh/api/interfaces/pinia.Pinia.md)

添加 store 插件来扩展每一个 store

#### 参数 %{#parameters}%

| Name     | Type                                  | Description         |
| :------- | :------------------------------------ | :------------------ |
| `plugin` | [`PiniaPlugin`](https://pinia.vuejs.org/zh/api/interfaces/pinia.PiniaPlugin.md) | store plugin to add |

#### 返回值

[`Pinia`](https://pinia.vuejs.org/zh/api/interfaces/pinia.Pinia.md)
