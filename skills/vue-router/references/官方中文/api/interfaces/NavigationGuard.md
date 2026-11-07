---
editLink: false
---

[API 参考](https://router.vuejs.org/zh/api/index.md) / NavigationGuard

# 接口：NavigationGuard %{#interface-navigationguard}%

导航守卫。详情可查阅[导航守卫](https://router.vuejs.org/zh/guide/advanced/navigation-guards.md)。

## 可调用函数 %{#Callable}%

### NavigationGuard %{#Callable-NavigationGuard}%

▸ **NavigationGuard**(`to`, `from`, `next`): `NavigationGuardReturn` \| `Promise`\<`NavigationGuardReturn`\>

#### 参数 %{#Callable-NavigationGuard-Parameters}%

| 名称 | 类型 |
| :------ | :------ |
| `to` | [`RouteLocationNormalized`](https://router.vuejs.org/zh/api/interfaces/RouteLocationNormalized.md) |
| `from` | [`RouteLocationNormalized`](https://router.vuejs.org/zh/api/interfaces/RouteLocationNormalized.md) |
| `next` | [`NavigationGuardNext`](https://router.vuejs.org/zh/api/interfaces/NavigationGuardNext.md) |

#### 返回值 %{#Callable-NavigationGuard-Returns}%

`NavigationGuardReturn` \| `Promise`\<`NavigationGuardReturn`\>
