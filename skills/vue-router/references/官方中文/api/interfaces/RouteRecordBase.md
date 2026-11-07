---
editLink: false
---

<!-- TODO: translation -->

[API Documentation](https://router.vuejs.org/zh/api/index.md) / \_RouteRecordBase

# Interface: \_RouteRecordBase

Internal type for common properties among all kind of [RouteRecordRaw](https://router.vuejs.org/zh/api/index.md#RouteRecordRaw).

## Hierarchy

- [`PathParserOptions`](https://router.vuejs.org/zh/api/index.md#PathParserOptions)

  ↳ **`_RouteRecordBase`**

  ↳↳ [`RouteRecordSingleView`](https://router.vuejs.org/zh/api/interfaces/RouteRecordSingleView.md)

  ↳↳ [`RouteRecordSingleViewWithChildren`](https://router.vuejs.org/zh/api/interfaces/RouteRecordSingleViewWithChildren.md)

  ↳↳ [`RouteRecordMultipleViews`](https://router.vuejs.org/zh/api/interfaces/RouteRecordMultipleViews.md)

  ↳↳ [`RouteRecordMultipleViewsWithChildren`](https://router.vuejs.org/zh/api/interfaces/RouteRecordMultipleViewsWithChildren.md)

  ↳↳ [`RouteRecordRedirect`](https://router.vuejs.org/zh/api/interfaces/RouteRecordRedirect.md)

## Properties

### alias

• `Optional` **alias**: `string` \| `string`[]

Aliases for the record. Allows defining extra paths that will behave like a
copy of the record. Allows having paths shorthands like `/users/:id` and
`/u/:id`. All `alias` and `path` values must share the same params.

___

### beforeEnter

• `Optional` **beforeEnter**: [`NavigationGuardWithThis`](https://router.vuejs.org/zh/api/interfaces/NavigationGuardWithThis.md)\<`undefined`\> \| [`NavigationGuardWithThis`](https://router.vuejs.org/zh/api/interfaces/NavigationGuardWithThis.md)\<`undefined`\>[]

Before Enter guard specific to this record. Note `beforeEnter` has no
effect if the record has a `redirect` property.

___

### children

• `Optional` **children**: [`RouteRecordRaw`](https://router.vuejs.org/zh/api/index.md#RouteRecordRaw)[]

Array of nested routes.

___

### end

• `Optional` **end**: `boolean`

Should the RegExp match until the end by appending a `$` to it.

**`Default Value`**

`true`

#### Inherited from

PathParserOptions.end

___

### meta

• `Optional` **meta**: [`RouteMeta`](https://router.vuejs.org/zh/api/interfaces/RouteMeta.md)

Arbitrary data attached to the record.

___

### name

• `Optional` **name**: [`RouteRecordName`](https://router.vuejs.org/zh/api/index.md#RouteRecordName)

Name for the route record. Must be unique.

___

### path

• **path**: `string`

Path of the record. Should start with `/` unless the record is the child of
another record.

**`Example`**

```ts
`/users/:id` matches `/users/1` as well as `/users/posva`.
```

___

### props

• `Optional` **props**: `_RouteRecordProps` \| `Record`\<`string`, `_RouteRecordProps`\>

Allow passing down params as props to the component rendered by `router-view`.

___

### redirect

• `Optional` **redirect**: `RouteRecordRedirectOption`

Where to redirect if the route is directly matched. The redirection happens
before any navigation guard and triggers a new navigation with the new
target location.

___

### sensitive

• `Optional` **sensitive**: `boolean`

Makes the RegExp case-sensitive.

**`Default Value`**

`false`

#### Inherited from

PathParserOptions.sensitive

___

### strict

• `Optional` **strict**: `boolean`

Whether to disallow a trailing slash or not.

**`Default Value`**

`false`

#### Inherited from

PathParserOptions.strict
