---
title: “hexo 设置摘要信息
date: 2018-06-27 12:04:36
tags:
---



# [如何在静态博客hexo中只显示摘要信息](https://www.cnblogs.com/pcy0/p/how-to-show-less-in-home-page-of-hexo.html)

1. 在文章中使用`< !--more-->` 手动进行截断
    这种方法可以根据文章的内容，自己在合适的位置添加 `< !--more-->` 标签，使用灵活，也是Hexo推荐的方法。

   

2. 在文章中的`front-matter`中添加description，并提供文章摘录
    这种方式只会在首页列表中显示文章的摘要内容，进入文章详情后不会再显示。

   

   

3. 自动形成摘要，在**主题配置文件**中添加
    默认截取的长度为 150 字符，可以根据需要自行设定

```
auto_excerpt:
  enable: true
  length: 150
```

**建议使用 < !-- more -->（即第一种方式），除了可以精确控制需要显示的摘录内容以外， 这种方式也可以让 Hexo 中的插件更好的识别**

 



参考：

https://www.jianshu.com/p/78c218f9d1e7

 

 

 

 