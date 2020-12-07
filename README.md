# vue3-notes
## 开发实践方面：
- 为了支持TreeShaking，只打包入必要的API，一些API改成引入函数的形式
- ref一般用于基本类型，reactive用于对象类型
- getCurrentInstance 获取Vue当前实例，ctx 属性获取当前上下文` const { ctx } = getCurrentInstance();console.log(ctx.$router.currentRoute.value)`
- 监听属性watch & watchEffect
- props是响应式的，不能使用 ES6 解构，因为它会消除prop的响应性,如果需要解构prop，可以通过使用 setup 函数中的toRefs来安全地完成此操作`const { title } = toRefs(props)`
- context暴露三个组件的 property{ attrs, slots, emit }
- teleport
## 内部优化
- 性能优化：虚拟dom、编译模板、Proxy数据监听、更小的打包文件
- Composition API
- 对TypeScript支持更好，去掉this操作，更强大的类型推导
## vue-router
- $route.params.pathMatch
- https://github.com/pillarjs/path-to-regexp/tree/v1.7.0
## vuex
## vite
Vite 是面向现代浏览器，基于原生模块系统 ESModule 实现了按需编译的 Web 开发构建工具。在生产环境下基于 Rollup 打包。
- 快速冷启动服务器
- 即时热模块更换（HMR）
- 真正的按需编译
- node >= 10.16.0
## axios
## ant-design-vue
## vant
- https://vant-contrib.gitee.io/vant/next/#/zh-CN
## vue-cli
## https://www.nuxtjs.cn/
## https://github.com/ConsoleTVs/vswr
