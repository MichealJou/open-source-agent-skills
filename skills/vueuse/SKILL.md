---
name: vueuse
description: 在 Vue 项目选择或审查 VueUse 组合式函数，复用响应式、计时和浏览器能力。
---

# VueUse

先核对项目实际版本、已有组件和 composable，再查对应函数的官方文档与类型；不要复制或再包装已有功能。

- 确认输入与返回值的 ref/reactive 语义、实例共享范围，以及组件销毁时的监听器和定时器清理。
- 涉及网络、浏览器 API 或 SSR 时核对可用环境、并发请求、取消和旧结果覆盖；保留现有权限、状态和 API 原值类型。
- 项目已有实时更新机制时沿用其设计，不因工具存在就新增轮询、全局状态或依赖。
- 对交互与状态变化使用项目现有测试和必要页面验证。

官方：[VueUse](https://vueuse.org/)；官网默认最新版本，实际使用以项目锁文件及源码为准。

## 什么时候用，怎么用

先查项目已有 composable 和锁文件。以下以 14.3.0 为核验基线，官网最新版可能不同。

| 场景 | 选择 | 注意 |
| --- | --- | --- |
| 组件内周期执行 | `useIntervalFn` | 确认何时启动、暂停和销毁；异步任务重叠和旧结果覆盖需自行处理。 |
| 组件内注册浏览器事件 | `useEventListener` | 确认目标对象生命周期；SSR 环境避免在服务端直接读取 `window`。 |
| 防抖或节流 | 查对应版本的 `useDebounceFn` / `useThrottleFn` | 明确首尾触发和取消行为，勿改变提交或请求语义。 |

```ts
import { useIntervalFn } from '@vueuse/core'

const { pause, resume } = useIntervalFn(refresh, 5000, { immediate: false })
// 在确实需要开始时调用 resume()，不需要时调用 pause()。
```

`refresh` 由调用方提供；计时器不能代替请求取消、并发控制或错误处理。已有推送和刷新机制时沿用现有方案，不额外引入轮询。

## 方法用途与优先级

按场景读取 [方法用途与选择](references/selection-guide.md) 和 [常用方法中文说明](references/usage-extended.md)，先核对已有项目能力、业务语义和当前依赖版本。未覆盖的方法继续查版本索引、源码与官方文档，不根据名称猜测。

## 查找全部方法

查看本技能的 [公开 API 索引](references/API-INDEX.md)，按包或名称定位方法与重载；调用前再查官方文档和项目实际版本。索引记录声明，不等于逐项解释、使用建议或兼容性保证；注意继承方法与索引范围。

## 上游参考

按需查阅 [上游技能原文](references/upstream/UPSTREAM.md)；其版本和默认建议以当前项目依赖、用户要求及本技能既有规则为准。来源和许可证见 [上游来源说明](references/上游来源说明.md)。

## 中文与英文资料

先查 [中文使用指南](references/中文指南.md) 中的场景、选择顺序与边界；英文原文见指南中的对应链接。用户和项目规则、项目实际依赖版本优先。

按需查阅 [社区中文文档索引](references/vueuse-cn/README.md)；该来源不是项目当前 VueUse 版本，必须对照安装版本核实。
