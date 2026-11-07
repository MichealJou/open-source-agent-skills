---
editLink: false
---

<!-- TODO: translation -->

[API Documentation](https://router.vuejs.org/zh/api/index.md) / RouteRecordMultipleViewsWithChildren

# Interface: RouteRecordMultipleViewsWithChildren

Route Record defining multiple named components with the `components` option and children.

## Hierarchy

- [`_RouteRecordBase`](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md)

  ↳ **`RouteRecordMultipleViewsWithChildren`**

## Properties

### alias

• `Optional` **alias**: `string` \| `string`[]

Aliases for the record. Allows defining extra paths that will behave like a
copy of the record. Allows having paths shorthands like `/users/:id` and
`/u/:id`. All `alias` and `path` values must share the same params.

#### Inherited from

[_RouteRecordBase](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md).[alias](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md#alias)

___

### beforeEnter

• `Optional` **beforeEnter**: [`NavigationGuardWithThis`](https://router.vuejs.org/zh/api/interfaces/NavigationGuardWithThis.md)\<`undefined`\> \| [`NavigationGuardWithThis`](https://router.vuejs.org/zh/api/interfaces/NavigationGuardWithThis.md)\<`undefined`\>[]

Before Enter guard specific to this record. Note `beforeEnter` has no
effect if the record has a `redirect` property.

#### Inherited from

[_RouteRecordBase](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md).[beforeEnter](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md#beforeEnter)

___

### children

• **children**: [`RouteRecordRaw`](https://router.vuejs.org/zh/api/index.md#RouteRecordRaw)[]

Array of nested routes.

#### Overrides

[_RouteRecordBase](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md).[children](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md#children)

___

### component

• `Optional` **component**: `undefined`

___

### components

• `Optional` **components**: ``null`` \| `Record`\<`string`, `RawRouteComponent`\>

Components to display when the URL matches this route. Allow using named views.

___

### end

• `Optional` **end**: `boolean`

Should the RegExp match until the end by appending a `$` to it.

**`Default Value`**

`true`

#### Inherited from

[_RouteRecordBase](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md).[end](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md#end)

___

### meta

• `Optional` **meta**: [`RouteMeta`](https://router.vuejs.org/zh/api/interfaces/RouteMeta.md)

Arbitrary data attached to the record.

#### Inherited from

[_RouteRecordBase](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md).[meta](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md#meta)

___

### name

• `Optional` **name**: [`RouteRecordName`](https://router.vuejs.org/zh/api/index.md#RouteRecordName)

Name for the route record. Must be unique.

#### Inherited from

[_RouteRecordBase](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md).[name](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md#name)

___

### path

• **path**: `string`

Path of the record. Should start with `/` unless the record is the child of
another record.

**`Example`**

```ts
`/users/:id` matches `/users/1` as well as `/users/posva`.
```

#### Inherited from

[_RouteRecordBase](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md).[path](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md#path)

___

### props

• `Optional` **props**: `boolean` \| `Record`\<`string`, `_RouteRecordProps`\>

Allow passing down params as props to the component rendered by
`router-view`. Should be an object with the same keys as `components` or a
boolean to be applied to every component.

#### Overrides

[_RouteRecordBase](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md).[props](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md#props)

___

### redirect

• `Optional` **redirect**: `RouteRecordRedirectOption`

Where to redirect if the route is directly matched. The redirection happens
before any navigation guard and triggers a new navigation with the new
target location.

#### Inherited from

[_RouteRecordBase](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md).[redirect](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md#redirect)

___

### sensitive

• `Optional` **sensitive**: `boolean`

Makes the RegExp case-sensitive.

**`Default Value`**

`false`

#### Inherited from

[_RouteRecordBase](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md).[sensitive](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md#sensitive)

___

### strict

• `Optional` **strict**: `boolean`

Whether to disallow a trailing slash or not.

**`Default Value`**

`false`

#### Inherited from

[_RouteRecordBase](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md).[strict](https://router.vuejs.org/zh/api/interfaces/RouteRecordBase.md#strict)
