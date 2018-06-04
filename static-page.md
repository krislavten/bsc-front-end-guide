# 静态页面开发相关
## html 
* [圣杯布局(非等高)](http://www.cnblogs.com/lyzg/p/5160570.html) [圣杯布局 & 双飞翼布局(等高)](http://www.cnblogs.com/lyzg/p/5164593.html) 在常规情况下，使用 `flexbox` 布局最方便

## css tips
* [flexbox](http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html)  适合局部布局，推荐替代盒子模型
* [grid 指南 ](http://www.css88.com/archives/8510)  多用于大页面布局，ps: 目前兼容性较差，Chrome 47 版本以前不支持
* rem / em / px   `rem`取决于页根元素的字体大小，`em`取决于当前使用 em 单位的元素的字体大小，`px`浏览器像素
* 垂直居中的方法有哪些
  * 不知道自己高度和父容器高度的情况下
  ```
    parentElement{
      position:relative;
    }

    childElement{
      position: absolute;
      top: 50%;
      transform: translateY(-50%);
    }
  ```
  * 若父容器下只有一个元素，且父元素设置了高度，则只需要使用相对定位即可
  ```
    parentElement{
      height:xxx;
    }

    .childElement {
      position: relative;
      top: 50%;
      transform: translateY(-50%);
    }
  ```
  * flex box 一劳永逸法 
  ``` 
    parentElement{
      display:flex;/*Flex布局*/
      align-items:center;/*指定垂直居中*/
    }
  ```
* `object-fit`  定义内容块在不同宽高下的表现，常用于 `img` `video` 等带有  `object-positon`的标签
  * `object-fit:cover` `background-image:cover` 在 img 和 div:background-images 下的表现一致

## js tips

## jekyll
