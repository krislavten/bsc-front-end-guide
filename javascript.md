# javascript 

## 基础语法
* [面向对象 / 原型链 / 深拷贝](http://www.ruanyifeng.com/blog/2010/05/object-oriented_javascript_encapsulation.html)
* [Event Loop](http://www.ruanyifeng.com/blog/2014/10/event-loop.html)
* [Execution Context & Stack](https://github.com/muwoo/blogs/issues/20)

## 通用组件解析
* [单页应用路由实现原理](https://github.com/happylindz/blog/issues/4)
  * `hash` 基于改变 url 中的 hash 参数页面不会发生改变这个特性，监听 hash 的修改并做相应处理
  * `history` 使用 HTML5 规范中提供的 history.pushState || history.replaceState 来进行路由控制
  * [造轮子----动手实现一个数据驱动的 router](https://zhuanlan.zhihu.com/p/37730038)
* [状态管理原理解析](https://cn.vuejs.org/v2/guide/state-management.html)
  * `vuex` `redux` `dva` 等类 flux 状态管理组件是提供一个全局对象并为保持数据流动过程透明和可持续实现的一套管理方法的集合
  * `react 16.3` 的 `context api` 方法提供了一种通过 `生产者-消费者` 的模式来进行状态的共享