# docsify 教程


## 命令行

cd /Users/cnfeat/Documents/GitHub/book.LearnThingsTheHardWay.com

docsify serve docs

http://localhost:3000 

创建  _sidebar.md

docsify简单教程 - Wilson998 - 博客园
https://www.cnblogs.com/CatFish/p/8251044.html


如果你的侧边栏没有出现，一定是没有 .nojekyll 文件，记得在 docs 根目录创建一个  .nojekyll 文件



---

## **开始写文档**

初始化成功后，可以看到 `./docs` 目录下创建的几个文件

  * `index.html` 入口文件
  * `README.md` 会做为主页内容渲染
  * `.nojekyll` 用于阻止 GitHub Pages 会忽略掉下划线开头的文件

直接编辑 `docs/README.md` 就能更新网站内容，也可以[写多个页面](http://link.zhihu.com/?target=https%3A//docsify.js.org/%23/zh-cn/more-pages)。

## **[本地预览网站]**

运行一个本地服务器通过 `docsify serve` 可以方便的预览效果，而且提供 LiveReload 功能，可以让实时的预览。默认访问 [http://localhost:3000](http://link.zhihu.com/?target=http%3A//localhost%3A3000/) 。
    
    docsify serve docs 

## **[Loading提示]**

初始化时会显示 Loading…内容，也可自定义

index.html

## **loadNavbar**

  * 类型：`Boolean|String`
  * 默认值: `false`

加载自定义导航栏，参考[定制导航栏](http://link.zhihu.com/?target=https%3A//docsify.js.org/%23/zh-cn/custom-navbar) 了解用法。设置为 `true` 后会加载 `_navbar.md` 文件，也可以自定义加载的文件名。
    
    window.$docsify = { // 加载 _navbar.md loadNavbar: true, // 加载 nav.md loadNavbar: 'nav.md' }; 

## **loadSidebar**

  * 类型：`Boolean|String`
  * 默认值: `false`

加载自定义侧边栏，参考[多页文档](http://link.zhihu.com/?target=https%3A//docsify.js.org/%23/zh-cn/more-pages)。设置为 `true` 后会加载 `_sidebar.md` 文件，也可以自定义加载的文件名。
    
    window.$docsify = { // 加载 _sidebar.md loadSidebar: true, // 加载 summary.md loadSidebar: 'summary.md' }; 

## **[subMaxLevel]**

  * 类型：`Number`
  * 默认值: `0`

自定义侧边栏后默认不会再生成目录，你也可以通过设置生成目录的最大层级开启这个功能。
    
    window.$docsify = { subMaxLevel: 2 }; 

## **[封面作为首页]**

通常封面和首页是同时出现的，当然你也是当封面独立出来通过设置[onlyCover 选项](http://link.zhihu.com/?target=https%3A//docsify.js.org/%23/zh-cn/configuration%3Fid%3Donlycover)。

## **[多个封面]**

如果文档网站是多语言的，或设置多个封面。

例如文档目录结构如下
    
    . └── docs ├── README.md ├── python.md ├── _coverpage.md └── django ├── README.md └── django.md └── _coverpage.md 

可以配置



## 参考

https://github.com/Snipaste/feedback
http://card.learnwritingthehardway.cn/

docsify，文档生成利器！ - 掘金

https://juejin.im/post/5afe93ab6fb9a07aa83efab7

Snipaste

https://docs.snipaste.com/


