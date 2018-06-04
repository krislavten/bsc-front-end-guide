# vue 相关

[vue 文档地址](https://cn.vuejs.org/v2/guide/index.html)

## vue 原理
### 双向数据绑定
vue 通过 [Object.defineProperty( )](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/defineProperty) 劫持数据的 `get` `set` 并结合发布者-订阅者的方式来实现双向数据绑定

`Object.defineProperty()` demo

  ```
  var Book = {}
  var name = ''
  Object.defineProperty(Book, 'name', {
    set: function (value) {
      name = value
      console.log('你取了一个书名叫做' + value);
    },
    get: function () {
      return '《' + name + '》'
    }
  })
  
  Book.name = '白山云为何如此优秀'
  console.log(Book.name)// 你取了一个书名叫做白山云为何如此优秀
  ```

[动手实现一个 vue](https://github.com/DMQ/mvvm)

## 哪里在用
* `storage-dashboard-vue` 云存储管理平台
