---
editLink: false
---

[API 参考](https://router.vuejs.org/zh/api/index.md) / NavigationGuardWithThis

# 接口：NavigationGuardWithThis\<T\> %{#interface-navigationguardwiththis-t}%

导航守卫。详情可查阅[导航守卫](https://router.vuejs.org/zh/guide/advanced/navigation-guards.md)。

## 类型参数 %{#Type-parameters}%

| Name |
| :------ |
| `T` |

## 可调用函数 %{#Callable}%

### NavigationGuardWithThis %{#Callable-NavigationGuardWithThis}%

▸ **NavigationGuardWithThis**(`this`, `to`, `from`, `next`): `NavigationGuardReturn` \| `Promise`\<`NavigationGuardReturn`\>

#### 参数 %{#Callable-NavigationGuardWithThis-Parameters}%

| 名称 | 类型 |
| :------ | :------ |
| `this` | `T` |
| `to` | [`RouteLocationNormalized`](https://router.vuejs.org/zh/api/interfaces/RouteLocationNormalized.md) |
| `from` | [`RouteLocationNormalized`](https://router.vuejs.org/zh/api/interfaces/RouteLocationNormalized.md) |
| `next` | [`NavigationGuardNext`](https://router.vuejs.org/zh/api/interfaces/NavigationGuardNext.md) |

#### 返回值 %{#Callable-NavigationGuardWithThis-Returns}%

`NavigationGuardReturn` \| `Promise`\<`NavigationGuardReturn`\>
