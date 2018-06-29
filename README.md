# Vue.js 技术揭秘

> 本文Fork自黄轶大佬的[项目](https://github.com/ustbhuangyi/vue-analysis)，另外加上了一些本人自己的注释

[电子书](https://ustbhuangyi.github.io/vue-analysis/)

目前社区有很多 Vue.js 的源码解析文章，但是质量层次不齐，不够系统和全面，这本电子书的目标是全方位细致深度解析 Vue.js 的实现原理，让同学们可以彻底掌握 Vue.js。目前分析的版本是 Vue.js 的最新版本 Vue.js 2.5.17-beta.0，并且之后会随着版本升级而做相应的更新，充分发挥电子书的优势。

这本电子书是作为 [《Vue.js 源码揭秘》](http://coding.imooc.com/class/228.html)视频课程的辅助教材。电子书是开源的，同学们可以免费阅读，视频是收费的，25+小时纯干货课程，如果有需要的同学可以购买来学习，**但请务必支持正版，请尊重作者的劳动成果**。

## 章节目录

为了把 Vue.js 的源码讲明白，课程设计成由浅入深，分为核心、编译、扩展、生态四个方面去讲，并拆成了八个章节，如下图：

<img src="https://ustbhuangyi.github.io/vue-analysis/assets/mind.png">

**第一章：准备工作**

介绍了 Flow、Vue.js 的源码目录设计、Vue.js 的源码构建方式，以及从入口开始分析了 Vue.js 的初始化过程。

**第二章：数据驱动**

详细讲解了模板数据到 DOM 渲染的过程，从 `new Vue` 开始，分析了 `mount`、`render`、`update`、`patch` 等流程。

**第三章：组件化**

分析了组件化的实现原理，并且分析了组件周边的原理实现，包括合并配置、生命周期、组件注册、异步组件。

**第四章：深入响应式原理**

详细讲解了数据的变化如何驱动视图的变化，分析了响应式对象的创建，依赖收集、派发更新的实现过程，一些特殊情况的处理，并对比了计算属性和侦听属性的实现，最后分析了组件更新的过程。

**第五章：编译**

从编译的入口函数开始，分析了编译的三个核心流程的实现：`parse` -> `optimize` -> `codegen`。

**第六章：扩展**

详细讲解了 `event`、`v-model`、`slot`、`keep-alive`、`transition`、`transition-group` 等常用功能的原理实现，该章节作为一个可扩展章节，未来会分析更多 Vue 提供的特性。

**第七章：Vue-Router**

分析了 Vue-Router 的实现原理，从路由注册开始，分析了路由对象、`matcher`，并深入分析了整个路径切换的实现过程和细节。

**第八章：Vuex**

分析了 Vuex 的实现原理，深入分析了它的初始化过程，常用 API 以及插件部分的实现。


