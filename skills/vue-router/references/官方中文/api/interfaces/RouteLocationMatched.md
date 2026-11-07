---
editLink: false
---

[API 参考](https://router.vuejs.org/zh/api/index.md) / RouteLocationMatched

# 接口：RouteLocationMatched

一条[路由记录](https://router.vuejs.org/zh/api/index.md#routerecord)的规范化版本。

## 继承关系 %{#Hierarchy}%

- [`RouteRecordNormalized`](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md)

  ↳ **`RouteLocationMatched`**

## 属性 %{#Properties}%

### aliasOf %{#Properties-aliasOf}%

• **aliasOf**: `undefined` \| [`RouteRecordNormalized`](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md)

定义了是否这条记录是另一条的别名。如果记录是原始记录，则该属性为 `undefined`。

#### 继承自 %{#Properties-aliasOf-Inherited-from}%

[RouteRecordNormalized](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md).[aliasOf](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md#aliasof)

___

### beforeEnter %{#Properties-beforeEnter}%

• **beforeEnter**: `undefined` \| [`NavigationGuardWithThis`](https://router.vuejs.org/zh/api/interfaces/NavigationGuardWithThis.md)\<`undefined`\> \| [`NavigationGuardWithThis`](https://router.vuejs.org/zh/api/interfaces/NavigationGuardWithThis.md)\<`undefined`\>[]

被注册的 beforeEnter 守卫

#### 继承自 %{#Properties-beforeEnter-Inherited-from}%

[RouteRecordNormalized](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md).[beforeEnter](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md#beforeenter)

___

### children %{#Properties-children}%

• **children**: [`RouteRecordRaw`](https://router.vuejs.org/zh/api/index.md#routerecordraw)[]

嵌套的路由记录。

#### 继承自 %{#Properties-children-Inherited-from}%

[RouteRecordNormalized](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md).[children](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md#children)

___

### components %{#Properties-components}%

• **components**: `undefined` \| ``null`` \| `Record`\<`string`, [`RouteComponent`](https://router.vuejs.org/zh/api/index.md#routecomponent)\>

{@inheritDoc RouteRecordMultipleViews.components}

#### Override %{#Properties-components-Overrides}%

[RouteRecordNormalized](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md).[components](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md#components)

___

### instances %{#Properties-instances}%

• **instances**: `Record`\<`string`, `undefined` \| ``null`` \| `ComponentPublicInstance`\>

<!-- TODO: translation -->

Mounted route component instance。 Having the instances on the record mean beforeRouteUpdate and beforeRouteLeave guards can only be invoked with the latest mounted app instance if there are multiple application instances rendering the same view, basically duplicating the content on the page, which shouldn't happen in practice. It will work if multiple apps are rendering different named views.

#### 继承自 %{#Properties-instances-Inherited-from}%

[RouteRecordNormalized](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md).[instances](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md#instances)

___

### meta %{#Properties-meta}%

• **meta**: [`RouteMeta`](https://router.vuejs.org/zh/api/interfaces/RouteMeta.md)

<!-- TODO: translation -->

Arbitrary data attached to the record.

#### 继承自 %{#Properties-meta-Inherited-from}%

[RouteRecordNormalized](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md).[meta](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md#meta)

___

### name %{#Properties-name}%

• **name**: `undefined` \| [`RouteRecordName`](https://router.vuejs.org/zh/api/index.md#routerecordname)

<!-- TODO: translation -->

Name for the route record. Must be unique.

#### 继承自 %{#Properties-name-Inherited-from}%

[RouteRecordNormalized](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md).[name](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md#name)

___

### path %{#Properties-path}%

• **path**: `string`

<!-- TODO: translation -->

Path of the record. Should start with `/` unless the record is the child of another record.

#### 继承自 %{#Properties-path-Inherited-from}%

[RouteRecordNormalized](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md).[path](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md#path)

___

### props %{#Properties-props}%

• **props**: `Record`\<`string`, `_RouteRecordProps`\>

<!-- TODO: translation -->

Allow passing down params as props to the component rendered by `router-view`. Should be an object with the same keys as `components` or a boolean to be applied to every component.

#### 继承自 %{#Properties-props-Inherited-from}%

[RouteRecordNormalized](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md).[props](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md#props)

___

### redirect %{#Properties-redirect}%

• **redirect**: `undefined` \| `RouteRecordRedirectOption`

<!-- TODO: translation -->

Where to redirect if the route is directly matched. The redirection happens before any navigation guard and triggers a new navigation with the new target location.

#### 继承自 %{#Properties-redirect-Inherited-from}%

[RouteRecordNormalized](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md).[redirect](https://router.vuejs.org/zh/api/interfaces/RouteRecordNormalized.md#redirect)
